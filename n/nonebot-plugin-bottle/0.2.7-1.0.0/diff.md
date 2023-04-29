# Comparing `tmp/nonebot_plugin_bottle-0.2.7-py3-none-any.whl.zip` & `tmp/nonebot_plugin_bottle-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 24375 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat    13254 b- defN 23-Feb-25 13:32 nonebot_plugin_bottle/__init__.py
--rw-rw-rw-  2.0 fat      484 b- defN 23-Feb-24 13:16 nonebot_plugin_bottle/config.py
--rw-rw-rw-  2.0 fat    14830 b- defN 23-Feb-25 13:23 nonebot_plugin_bottle/data_source.py
--rw-rw-rw-  2.0 fat    35821 b- defN 23-Feb-25 13:35 nonebot_plugin_bottle-0.2.7.dist-info/LICENCE
--rw-rw-rw-  2.0 fat     7224 b- defN 23-Feb-25 13:35 nonebot_plugin_bottle-0.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-25 13:35 nonebot_plugin_bottle-0.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Feb-25 13:35 nonebot_plugin_bottle-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      729 b- defN 23-Feb-25 13:35 nonebot_plugin_bottle-0.2.7.dist-info/RECORD
-8 files, 72456 bytes uncompressed, 23087 bytes compressed:  68.1%
+Zip file size: 26837 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    17111 b- defN 23-Apr-29 06:02 nonebot_plugin_bottle/__init__.py
+-rw-rw-rw-  2.0 fat      636 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/config.py
+-rw-rw-rw-  2.0 fat    17498 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/data_source.py
+-rw-rw-rw-  2.0 fat     1426 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/model.py
+-rw-rw-rw-  2.0 fat    35821 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/LICENCE
+-rw-rw-rw-  2.0 fat     8238 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      816 b- defN 23-Apr-29 06:06 nonebot_plugin_bottle-1.0.0.dist-info/RECORD
+9 files, 81660 bytes uncompressed, 25413 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: nonebot_plugin_bottle/config.py
 Comment: 
 
 Filename: nonebot_plugin_bottle/data_source.py
 Comment: 
 
-Filename: nonebot_plugin_bottle-0.2.7.dist-info/LICENCE
+Filename: nonebot_plugin_bottle/model.py
 Comment: 
 
-Filename: nonebot_plugin_bottle-0.2.7.dist-info/METADATA
+Filename: nonebot_plugin_bottle-1.0.0.dist-info/LICENCE
 Comment: 
 
-Filename: nonebot_plugin_bottle-0.2.7.dist-info/WHEEL
+Filename: nonebot_plugin_bottle-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: nonebot_plugin_bottle-0.2.7.dist-info/top_level.txt
+Filename: nonebot_plugin_bottle-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: nonebot_plugin_bottle-0.2.7.dist-info/RECORD
+Filename: nonebot_plugin_bottle-1.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: nonebot_plugin_bottle-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nonebot_plugin_bottle/__init__.py

```diff
@@ -1,15 +1,38 @@
-import asyncio
 import random
-from nonebot.plugin import PluginMetadata
-from nonebot import on_command
+import asyncio
+
+from nonebot.matcher import Matcher
+from nonebot import require, on_command
 from nonebot.permission import SUPERUSER
-from nonebot.adapters.onebot.v11 import Bot, MessageEvent, GroupMessageEvent, GROUP, Message
-from .data_source import bottle,text_audit,ba
+from nonebot.plugin import PluginMetadata
+from nonebot.params import Depends, CommandArg
+
+require("nonebot_plugin_datastore")
+from nonebot_plugin_datastore import get_session
+from sqlalchemy.ext.asyncio.session import AsyncSession
+from nonebot.adapters.onebot.v11 import (
+    GROUP,
+    Bot,
+    Message,
+    ActionFailed,
+    MessageEvent,
+    MessageSegment,
+    GroupMessageEvent,
+)
+
+from .model import Bottle
 from .config import Config
+from .data_source import (
+    ba,
+    text_audit,
+    bottle_manager,
+    serialize_message,
+    deserialize_message,
+)
 
 __plugin_meta__ = PluginMetadata(
     name="漂流瓶",
     description="群与群互通的漂流瓶插件",
     config=Config,
     usage=f"""
 指令：
@@ -28,274 +51,431 @@
     漂流瓶黑名单 [QQ / 群聊] [QQ号 / 群号]
     漂流瓶详情 [漂流瓶编号]
 """.strip(),
     extra={
         "unique_name": "nonebot_plugin_bottle",
         "example": "扔漂流瓶\n寄漂流瓶\n捡漂流瓶\n评论漂流瓶\n举报漂流瓶\n查看漂流瓶\n删除漂流瓶",
         "author": "Todysheep",
-        "version": "0.2.7",
+        "version": "1.0.0,
     },
 )
 
-throw = on_command("扔漂流瓶 ", aliases=set(["寄漂流瓶 ","丢漂流瓶 "]),permission=GROUP, priority=100, block=True)
+throw = on_command(
+    "扔漂流瓶", aliases=set(["寄漂流瓶", "丢漂流瓶"]), permission=GROUP, priority=100, block=True
+)
 get = on_command("捡漂流瓶", priority=100, block=True)
-report = on_command("举报漂流瓶 ", priority=100, block=True)
-comment = on_command("评论漂流瓶 ", priority=100, block=True)
-check_bottle = on_command("查看漂流瓶 ", priority=100, block=True)
-remove = on_command("删除漂流瓶 ", priority=100, block=True)
+report = on_command("举报漂流瓶", priority=100, block=True)
+comment = on_command("评论漂流瓶", priority=100, block=True)
+check_bottle = on_command("查看漂流瓶", priority=100, block=True)
+remove = on_command("删除漂流瓶", priority=100, block=True)
 
-resume = on_command("恢复漂流瓶 ", permission=SUPERUSER, priority=100, block=True)
+resume = on_command("恢复漂流瓶", permission=SUPERUSER, priority=100, block=True)
 clear = on_command("清空漂流瓶", permission=SUPERUSER, priority=100, block=True)
-comrem = on_command("删除漂流瓶评论",permission=SUPERUSER, priority=100, block=True)
-listqq = on_command("漂流瓶详情",permission=SUPERUSER, priority=100, block=True)
-ban = on_command("漂流瓶黑名单",aliases=set(["banbottle",'漂流瓶封禁']),permission=SUPERUSER, priority=100, block=True)
-white = on_command("漂流瓶白名单",aliases=set(["whitebottle"]),permission=SUPERUSER, priority=100, block=True)
+comrem = on_command("删除漂流瓶评论", permission=SUPERUSER, priority=100, block=True)
+listqq = on_command("漂流瓶详情", permission=SUPERUSER, priority=100, block=True)
+ban = on_command(
+    "漂流瓶黑名单",
+    aliases=set(["banbottle", "漂流瓶封禁"]),
+    permission=SUPERUSER,
+    priority=100,
+    block=True,
+)
+white = on_command(
+    "漂流瓶白名单",
+    aliases=set(["whitebottle"]),
+    permission=SUPERUSER,
+    priority=100,
+    block=True,
+)
+
+
+async def get_bottle(
+    index: str, matcher: Matcher, session: AsyncSession, include_del=False
+) -> Bottle:
+    if not index.isdigit():
+        await matcher.finish("漂流瓶编号必须为正整数！")
+    bottle = await bottle_manager.get_bottle(
+        index=int(index), session=session, include_del=include_del
+    )
+    if not bottle:
+        await matcher.finish("该漂流瓶不存在或已被删除！")
+    return bottle
+
+
+async def verify(matcher: Matcher, event: GroupMessageEvent) -> None:
+    if not ba.verify(event.user_id, event.group_id):
+        await matcher.finish(ba.bannedMessage)
+
 
 @throw.handle()
-async def thr(bot: Bot, event: GroupMessageEvent):
-    if not ba.verify(event.user_id,event.group_id):
-        await throw.finish(ba.bannedMessage)
+async def _(
+    bot: Bot,
+    matcher: Matcher,
+    event: GroupMessageEvent,
+    args: Message = CommandArg(),
+    session: AsyncSession = Depends(get_session),
+):
+    await verify(matcher=matcher, event=event)
 
-    try:
-        message = str(event.message).split(maxsplit=1)[1]
-    except:
+    if not args:
         await throw.finish("想说些什么话呢？在指令后边写上吧！")
-    
-    try:
-        message_text = event.message.extract_plain_text().split(maxsplit=1)[1]
-    except:
-        message_text = ""
+
+    message_text = args.extract_plain_text().strip()
 
     audit = await text_audit(text=message_text)
-    if not audit == 'pass':
-        if audit == 'Error': 
-            await throw.finish("文字审核未通过！原因：调用审核API失败，请检查违禁词词表是否存在，或token是否正确设置！" )
-        elif audit['conclusion'] == '不合规':
-            await throw.finish("文字审核未通过！原因：" + audit['data'][0]['msg'])
-
-    group_name = await bot.get_group_info(group_id=event.group_id)
-    group_name = group_name['group_name']
-    user_name = await bot.get_group_member_info(group_id=event.group_id,user_id=event.user_id)
-    user_name = user_name['nickname']
+    if not audit == "pass":
+        if audit == "Error":
+            await throw.finish("文字审核未通过！原因：调用审核API失败，请检查违禁词词表是否存在，或token是否正确设置！")
+        elif audit["conclusion"] == "不合规":
+            await throw.finish("文字审核未通过！原因：" + audit["data"][0]["msg"])
 
-    add_index = bottle.add(bot=bot,user=event.user_id, group=event.group_id, text=message, user_name=user_name, group_name=group_name)
+    try:
+        group_info = await bot.get_group_info(group_id=event.group_id)
+        group_name = group_info["group_name"]
+    except:
+        group_name = "Unknown"
+    user_info = await bot.get_group_member_info(
+        group_id=event.group_id, user_id=event.user_id
+    )
+    user_name = user_info.get("card") or user_info.get("nickname")
+
+    add_index = await bottle_manager.add_bottle(
+        user_id=event.user_id,
+        group_id=event.group_id,
+        content=await serialize_message(message=args),
+        user_name=user_name,
+        group_name=group_name,
+        session=session,
+    )
+    await session.commit()
     if add_index:
         # 添加个人冷却
-        ba.add('cooldown',event.user_id)
+        ba.add("cooldown", event.user_id)
         await asyncio.sleep(2)
-        await throw.finish(f'你将编号No.{add_index}的漂流瓶以时速{random.randint(0,2**16)}km/h的速度扔出去，谁会捡到这个瓶子呢...')
+        await throw.send(
+            f"你将编号No.{add_index}的漂流瓶以时速{random.randint(0,2**16)}km/h的速度扔出去，谁会捡到这个瓶子呢..."
+        )
     else:
         await asyncio.sleep(2)
-        await throw.finish("你的瓶子以奇怪的方式消失掉了！")
+        await throw.send("你的瓶子以奇怪的方式消失掉了！")
+
 
 @get.handle()
-async def g(bot: Bot, event: GroupMessageEvent):
-    if not ba.verify(event.user_id,event.group_id):
-        await throw.finish(ba.bannedMessage)
+async def _(
+    bot: Bot,
+    matcher: Matcher,
+    event: GroupMessageEvent,
+    session: AsyncSession = Depends(get_session),
+):
+    await verify(matcher=matcher, event=event)
 
-    if not bottle.select():
+    bottle = await bottle_manager.select(session=session)
+    if not bottle:
         await get.finish("好像一个瓶子也没有呢..要不要扔一个？")
-    else:
-        bott = bottle.select()
-        data = bott[1]
-        try:
-            user = await bot.get_group_member_info(group_id=data['group'], user_id=data['user'])
-            user = user["nickname"]
-        except:
-            user = data['user_name']
-        try:    
-            group = await bot.get_group_info(group_id=data['group'])
-            group = group["group_name"]
-        except:
-            group = data['group_name']
-
-        comment_list = bottle.check_comment(bott[0])
-        comment:str = ""
-        for i in comment_list[-3:]:
-            comment += i+"\n"
-        ba.add('cooldown',event.user_id)
-        await get.finish(f'【漂流瓶No.{bott[0]}|被捡到{data["picked"]}次】来自【{group}】的 {user} ！\n'+Message(data['text']) + (f"\n★评论共 {len(comment_list)} 条★\n{comment.strip()}" if comment else ""))
+    try:
+        user_info = await bot.get_group_member_info(
+            group_id=event.group_id, user_id=event.user_id
+        )
+        user_name = user_info.get("card") or user_info.get("nickname")
+    except ActionFailed:
+        user_name = bottle.user_name
+    try:
+        group_info = await bot.get_group_info(group_id=bottle.group_id)
+        group_name = group_info["group_name"]
+    except ActionFailed:
+        group_name = bottle.group_name
+
+    comments = await bottle_manager.get_comment(bottle=bottle, session=session)
+    comment_str = "\n".join(
+        [f"{comment.user_name}：{comment.content}" for comment in comments]
+    )
+    ba.add("cooldown", event.user_id)
+    await get.send(
+        f"【漂流瓶No.{bottle.id}|被捡到{bottle.picked}次】来自【{group_name}】的 {user_name} ！\n"
+        + deserialize_message(bottle.content)
+        + (f"\n★前 {len(comments)} 条评论★\n{comment_str}" if comment_str else "")
+    )
+    await session.commit()
 
-@report.handle()
-async def rep(bot: Bot, event: GroupMessageEvent):
-    if (not ba.verify(event.user_id,event.group_id)) or (not ba.verifyReport(event.user_id)):
-        await throw.finish(ba.bannedMessage)
 
-    index = int(str(event.message).split(maxsplit=1)[1])
-    result = bottle.report(index,event.user_id)
+@report.handle()
+async def _(
+    bot: Bot,
+    matcher: Matcher,
+    event: GroupMessageEvent,
+    args: Message = CommandArg(),
+    session: AsyncSession = Depends(get_session),
+):
+    await verify(matcher=matcher, event=event)
+    if not ba.verifyReport(event.user_id):
+        await report.finish(ba.bannedMessage)
+
+    index = args.extract_plain_text().strip()
+    bottle = await get_bottle(index=index, matcher=matcher, session=session)
+    result = await bottle_manager.report(
+        bottle=bottle, user_id=event.user_id, session=session
+    )
     if result == 0:
-        await report.finish("举报失败！")
-    if result == 1:
-        ba.add('cooldown',event.user_id)
-        await report.finish(f"举报成功！关于此漂流瓶已经有 {bottle.check_report(index)} 次举报")
-    if result == 2:
-        # 获取漂流瓶详情
-        data = bottle.check_bottle(int(index))
-        mes = f"有一漂流瓶遭到封禁！\n编号：{index}\n用户QQ：{data['user']}\n来源群组：{data['group']}\n"
-        mes += Message(data['text'])
-        commentList = ""
-        for i in data['comment']:
-            commentList += f"【{i[0]}】{i[1]}\n"
+        await report.send("举报失败！")
+    elif result == 1:
+        ba.add("cooldown", event.user_id)
+        await report.send(f"举报成功！关于此漂流瓶已经有 {bottle.report} 次举报")
+        await session.commit()
+    elif result == 2:
+        mes = f"有一漂流瓶遭到封禁！\n编号：{bottle.id}\n用户QQ：{bottle.user_id}\n来源群组：{bottle.group_id}\n"
+        mes += deserialize_message(bottle.content)
+        comments = await bottle_manager.get_comment(
+            bottle=bottle, session=session, limit=None
+        )
+        comment_str = "\n".join(
+            [
+                f"【{comment.user_id}】{comment.user_name}：{comment.content}"
+                for comment in comments
+            ]
+        )
+        await session.commit()
 
         # 私聊发送被删除的漂流瓶详情
         for i in list(bot.config.superusers):
-            await bot.send_private_msg(user_id = i,message=mes)
-            await bot.send_private_msg(user_id = i,message=commentList)
+            await bot.send_private_msg(user_id=i, message=mes)
+            await bot.send_private_msg(user_id=i, message=comment_str)
             await asyncio.sleep(0.5)
-        await report.finish("举报成功！已经进行删除该漂流瓶处理！")
-    if result == 3:
-        await report.finish("该漂流瓶已经被删除！")
+        await report.send("举报成功！已经进行删除该漂流瓶处理！")
+    elif result == 3:
+        await report.send("该漂流瓶已经被删除！")
+
 
 @comment.handle()
-async def com(bot: Bot, event: GroupMessageEvent):
-    if not ba.verify(event.user_id,event.group_id):
-        await throw.finish(ba.bannedMessage)
-        
-    mes = str(event.message.extract_plain_text()).split(maxsplit=2)
-    index = int(mes[1])
-    data = bottle.check_bottle(index)
-    if not data or data['del']:
-        await check_bottle.finish("该漂流瓶不存在或已被删除！")
-    user = await bot.get_group_member_info(group_id=event.group_id, user_id=event.user_id)
-    try:
-        commen = f"{user['nickname']}：{mes[2]}"
-    except:
+async def _(
+    bot: Bot,
+    matcher: Matcher,
+    event: GroupMessageEvent,
+    args: Message = CommandArg(),
+    session: AsyncSession = Depends(get_session),
+):
+    await verify(matcher=matcher, event=event)
+
+    command = args.extract_plain_text().strip().split()
+    if not command:
+        await comment.finish(f"请在指令后接 漂流瓶id 评论")
+    if len(command) == 1:
         await comment.finish("想评论什么呀，在后边写上吧！")
-    
+    bottle = await get_bottle(index=command[0], matcher=matcher, session=session)
+    user_info = await bot.get_group_member_info(
+        group_id=event.group_id, user_id=event.user_id
+    )
+    user_name = user_info.get("card") or user_info["nickname"]
+    command[1] = command[1].strip()
+
     # 进行文字审核
-    audit = await text_audit(text=commen)
-    if not audit == 'pass':
-        if audit == 'Error': 
-            await comment.finish("文字审核未通过！原因：调用审核API失败，请检查违禁词词表格式是否正确，或token是否正确设置！" )
-        elif audit['conclusion'] == '不合规':
-            await comment.finish("文字审核未通过！原因：" + audit['data'][0]['msg'])
+    audit = await text_audit(text=command[1])
+    if not audit == "pass":
+        if audit == "Error":
+            await comment.finish("文字审核未通过！原因：调用审核API失败，请检查违禁词词表格式是否正确，或token是否正确设置！")
+        elif audit["conclusion"] == "不合规":
+            await comment.finish("文字审核未通过！原因：" + audit["data"][0]["msg"])
 
     # 审核通过
-    bottle.comment(index,event.user_id, commen)
+    bottle_manager.comment(
+        bottle=bottle,
+        user_id=event.user_id,
+        user_name=user_name,
+        content=command[1],
+        session=session,
+    )
     try:
-        await bot.send_msg(group_id=bottle.check_bottle(index)['group'], message=Message(f"[CQ:at,qq={bottle.check_bottle(index)['user']}] 你的{index}号漂流瓶被评论啦！\n{commen}"))
+        await bot.send_group_msg(
+            group_id=bottle.group_id,
+            message=Message(
+                MessageSegment.at(bottle.user_id)
+                + f" 你的{bottle.id}号漂流瓶被评论啦！\n{command[1]}"
+            ),
+        )
         await asyncio.sleep(2)
     finally:
-        ba.add('cooldown',event.user_id)
-        await comment.finish("回复成功！")
+        ba.add("cooldown", event.user_id)
+        await comment.send("回复成功！")
+    await session.commit()
+
 
 @check_bottle.handle()
-async def che(bot: Bot, event: MessageEvent):
-    index = int(str(event.message).split(maxsplit=1)[1])
-    comment_list = bottle.check_comment(index)
-    data = bottle.check_bottle(index)
+async def _(
+    bot: Bot,
+    event: MessageEvent,
+    matcher: Matcher,
+    args: Message = CommandArg(),
+    session: AsyncSession = Depends(get_session),
+):
+    index = args.extract_plain_text().strip()
+    bottle = await get_bottle(index=index, matcher=matcher, session=session)
 
-    if data['del'] == 1:
-        await check_bottle.finish("该漂流瓶不存在或已被删除！")
     try:
-        user = await bot.get_group_member_info(group_id=data['group'], user_id=data['user'])
-        user = user["nickname"]
-    except:
-        user = data['user_name']
-    try:    
-        group = await bot.get_group_info(group_id=data['group'])
-        group = group["group_name"]
-    except:
-        group = data['group_name']
-    if not comment_list:
-        await check_bottle.finish(f"这个编号的漂流瓶还没有评论,不能给你看里面的东西！\n【该#{index} 漂流瓶来自【{group}】的 {user}，被捡到{data['picked']}次，于{data['time']}扔出】")
-    comment = ""
-    for i in comment_list:
-        comment += i+"\n"
-    ba.add('cooldown',event.user_id)
-    await check_bottle.finish(f"来自【{group}】的 {user} 的第{index}号漂流瓶：\n" + Message(data['text']) + f"\n★评论共 {len(comment_list)} 条★\n{comment}【被捡到{data['picked']}次，于{data['time']}扔出】")
+        user_info = await bot.get_group_member_info(
+            group_id=event.group_id, user_id=event.user_id
+        )
+        user_name = user_info.get("card") or user_info.get("nickname")
+    except ActionFailed:
+        user_name = bottle.user_name
+    try:
+        group_info = await bot.get_group_info(group_id=bottle.group_id)
+        group_name = group_info["group_name"]
+    except ActionFailed:
+        group_name = bottle.group_name
+    comments = await bottle_manager.get_comment(bottle=bottle, session=session)
+    if not comments:
+        await check_bottle.finish(
+            f"这个编号的漂流瓶还没有评论,不能给你看里面的东西！\n【该#{index} 漂流瓶来自【{group_name}】的 {user_name}，被捡到{bottle.picked}次，于{bottle.time.strftime('%Y-%m-%d %H:%M:%S')}扔出】"
+        )
+    comment_str = "\n".join(
+        [f"{comment.user_name}：{comment.content}" for comment in comments]
+    )
+    ba.add("cooldown", event.user_id)
+    await check_bottle.finish(
+        f"来自【{group_name}】的 {user_name} 的第{index}号漂流瓶：\n"
+        + deserialize_message(bottle.content)
+        + f"\n★前 {len(comments)} 条评论★\n{comment_str}\n【被捡到{bottle.picked}次，于{bottle.time.strftime('%Y-%m-%d %H:%M:%S')}扔出】"
+    )
+
 
 @remove.handle()
-async def rem(bot:Bot, event: GroupMessageEvent):
-    index = int(str(event.message).split()[1])
-    if str(event.user_id) in list(bot.config.superusers) or bottle.check_bottle(index)['user'] == event.user_id:
-        if bottle.remove(index):
-            await remove.finish(f"成功删除 {index} 号漂流瓶！")
-        else:
-            await remove.finish('删除失败！请检查编号')
+async def rem(
+    bot: Bot,
+    matcher: Matcher,
+    event: GroupMessageEvent,
+    arg: Message = CommandArg(),
+    session: AsyncSession = Depends(get_session),
+):
+    index = arg.extract_plain_text().strip()
+    bottle = await get_bottle(index=index, matcher=matcher, session=session)
+    if (
+        str(event.user_id) in list(bot.config.superusers)
+        or bottle.user_id == event.user_id
+    ):
+        bottle.is_del = True
+        await session.commit()
+        await remove.finish(f"成功删除 {index} 号漂流瓶！")
     else:
-        await remove.finish('删除失败！你没有相关的权限！')
+        await remove.finish("删除失败！你没有相关的权限！")
+
 
 ###### SUPERUSER命令 ######
 
+
 @resume.handle()
-async def res(bot: Bot, event: MessageEvent):
-    index = int(str(event.message).split()[1])
-    if bottle.resume(index):
-        await resume.finish(f"成功恢复 {index} 号漂流瓶！")
-    else:
-        await resume.finish('恢复失败！请检查编号')
+async def _(
+    matcher: Matcher,
+    arg: Message = CommandArg(),
+    session: AsyncSession = Depends(get_session),
+):
+    index = arg.extract_plain_text().strip()
+    bottle = await get_bottle(
+        index=index, matcher=matcher, session=session, include_del=True
+    )
+    bottle.is_del = False
+    await session.commit()
+    await resume.finish(f"成功恢复 {index} 号漂流瓶！")
+
 
 @clear.handle()
-async def cle(bot: Bot, event: MessageEvent):
-    bottle.clear()
+async def _(session: AsyncSession = Depends(get_session)):
+    await bottle_manager.clear(session)
+    await session.commit()
     await clear.finish("所有漂流瓶清空成功！")
 
+
 @listqq.handle()
-async def lis(bot: Bot, event: MessageEvent):
-    command = str(event.message).split(" ")[1]
-    data = bottle.check_bottle(int(command))
-    if data:
-        mes = f"漂流瓶编号：{command}\n用户QQ：{data['user']}\n来源群组：{data['group']}\n发送时间：{data['time']}\n"
-        mes += Message(data['text'])
-        await listqq.send(mes)
-        
-        commentList = ""
-        for i in data['comment']:
-            commentList += f"【{i[0]}】{i[1]}\n"
-        if commentList :
-            await listqq.finish(commentList)
-        else:
-            await listqq.finish("漂流瓶暂无回复")
+async def _(
+    matcher: Matcher,
+    args: Message = CommandArg(),
+    session: AsyncSession = Depends(get_session),
+):
+    index = args.extract_plain_text().strip()
+    bottle = await get_bottle(
+        index=index, matcher=matcher, session=session, include_del=True
+    )
+    mes = f"漂流瓶编号：{index}\n用户QQ：{bottle.user_id}\n来源群组：{bottle.group_id}\n发送时间：{bottle.time.strftime('%Y-%m-%d %H:%M:%S')}\n"
+    await listqq.send(mes + deserialize_message(bottle.content))
+
+    comments = await bottle_manager.get_comment(
+        bottle=bottle, session=session, limit=None
+    )
+    comment_str = "\n".join(
+        [
+            f"【{comment.user_id}】{comment.user_name}：{comment.content}"
+            for comment in comments
+        ]
+    )
+    if comment_str:
+        await listqq.send(comment_str)
+    else:
+        await listqq.send("漂流瓶暂无回复")
 
 
 @ban.handle()
-async def li(bot:Bot, event: MessageEvent):
-    command = str(event.message).split(" ")[1:]
-    if command[0] in ['group','群聊','群号']:
-        if ba.add('group',command[1]):
+async def _(
+    args: Message = CommandArg(),
+):
+    command = args.extract_plain_text().strip().split(" ")
+    if command[0] in ["group", "群聊", "群号"]:
+        if ba.add("group", command[1]):
             await ban.finish(f"成功封禁{command[0]}：{command[1]}")
         else:
-            ba.remove('group',command[1])
+            ba.remove("group", command[1])
             await ban.finish(f"成功解封{command[0]}：{command[1]}")
 
-    if command[0] in ['qq','QQ','user','用户','qq号','QQ号']:
-        if ba.add('user',command[1]):
+    if command[0] in ["qq", "QQ", "user", "用户", "qq号", "QQ号"]:
+        if ba.add("user", command[1]):
             await ban.finish(f"成功封禁{command[0]}：{command[1]}")
         else:
-            ba.remove('user',command[1])
+            ba.remove("user", command[1])
             await ban.finish(f"成功解封{command[0]}：{command[1]}")
-    
-    if command[0] in ['report','举报']:
+
+    if command[0] in ["report", "举报"]:
         result = ba.banreport(command[1])
         if result == 1:
             await ban.finish(f"成功取消{command[0]}权限：{command[1]}")
         elif result == 0:
             await ban.finish(f"成功赋予{command[0]}权限：{command[1]}")
         else:
             await ban.finish(result)
 
+
 @white.handle()
-async def wh(bot:Bot, event: MessageEvent):
-    command = str(event.message).split(" ")[1:]
-    if command[0] in ['group','群聊','群号']:
-        if ba.add('whiteGroup',command[1]):
+async def _(
+    args: Message = CommandArg(),
+):
+    command = args.extract_plain_text().strip().split(" ")
+    if command[0] in ["group", "群聊", "群号"]:
+        if ba.add("whiteGroup", command[1]):
             await ban.finish(f"成功设置白名单{command[0]}：{command[1]}")
         else:
-            ba.remove('whiteGroup',command[1])
+            ba.remove("whiteGroup", command[1])
             await ban.finish(f"成功移除白名单{command[0]}：{command[1]}")
 
-    if command[0] in ['qq','QQ','user','用户','qq号','QQ号']:
-        if ba.add('whiteUser',command[1]):
+    if command[0] in ["qq", "QQ", "user", "用户", "qq号", "QQ号"]:
+        if ba.add("whiteUser", command[1]):
             await ban.finish(f"成功设置白名单{command[0]}：{command[1]}")
         else:
-            ba.remove('whiteUser',command[1])
+            ba.remove("whiteUser", command[1])
             await ban.finish(f"成功移除白名单{command[0]}：{command[1]}")
 
 
 @comrem.handle()
-async def cr(bot:Bot,event: MessageEvent):
-    command = str(event.message).split(" ")[1:]
-    if bottle.remove_comment(int(command[0]),int(command[1])):
-        await comrem.finish("删除成功！")
-    else:
-        await comrem.finish("删除失败，请检查编号！")
+async def _(
+    matcher: Matcher,
+    args: Message = CommandArg(),
+    session: AsyncSession = Depends(get_session),
+):
+    command = args.extract_plain_text().strip().split()
+    if len(command) != 2:
+        await comrem.finish("请检查参数")
+    bottle = await get_bottle(
+        index=command[0], matcher=matcher, session=session, include_del=True
+    )
+    command[1] = command[1].strip()
+    if not command[1].isdigit():
+        await comrem.finish("用户id必须为数字！")
+    await bottle_manager.del_comment(
+        bottle=bottle, user_id=int(command[1]), session=session
+    )
+    await session.commit()
+    await comrem.finish("删除成功！")
```

## nonebot_plugin_bottle/config.py

```diff
@@ -1,14 +1,17 @@
-from pydantic import BaseModel, Extra
 from nonebot import get_driver
+from pydantic import Extra, BaseModel
 
 
 class Config(BaseModel, extra=Extra.ignore):
     # 百度智能云文字审核API
     # 申请网址：https://cloud.baidu.com/doc/ANTIPORN/s/dkk6wyt3z
     nonebot_plugin_bottle_api_key: str = ""
     nonebot_plugin_bottle_secret_key: str = ""
+    # 是否将图片保存在本地
+    nonebot_plugin_bottle_local_storage: bool = True
 
 
 config = Config.parse_obj(get_driver().config.dict())
 api_key = config.nonebot_plugin_bottle_api_key
 secret_key = config.nonebot_plugin_bottle_secret_key
+local_storage = config.nonebot_plugin_bottle_local_storage
```

## nonebot_plugin_bottle/data_source.py

```diff
@@ -1,471 +1,547 @@
-import json
-import random
-import httpx
+try:
+    import ujson as json
+except:
+    import json
+
 import time
+import hashlib
 from pathlib import Path
-from typing import List
+from datetime import datetime
+from typing import Any, Dict, List, Optional, Sequence
+
+import httpx
+import asyncio
+import aiofiles
 from nonebot.log import logger
-from nonebot.adapters.onebot.v11 import Bot
-from .config import api_key,secret_key
+from pydantic import parse_obj_as
+from sqlalchemy import func, text, select
+from sqlalchemy.ext.asyncio.session import AsyncSession
+from nonebot.adapters.onebot.v11 import Message, MessageSegment
+from nonebot_plugin_datastore.db import get_engine, post_db_init, create_session
+
+from .model import Bottle, Report, Comment
+from .config import api_key, secret_key, local_storage
+
+data_dir = Path("data/bottle")
+if local_storage:
+    cache_dir = data_dir / "cache"
+    cache_dir.mkdir(parents=True, exist_ok=True)
+data_dir.mkdir(parents=True, exist_ok=True)
 
-class Bottle(object):
-    def __init__(self) -> None:
-        self.data_path = Path("data/bottle/data.json").absolute()
-        self.data_dir = Path("data/bottle").absolute()
-        self.data_dir.mkdir(parents=True, exist_ok=True)
-        self.__data: List[dict] = []
-        self.__load()
 
-    def __load(self):
-        if self.data_path.exists() and self.data_path.is_file():
-            with self.data_path.open("r", encoding="utf-8") as f:
-                data: List[dict] = json.load(f)
+# https://github.com/noneplugin/nonebot-plugin-chatrecorder
+async def cache_file(msg: Message):
+    async with httpx.AsyncClient() as client:
+        await asyncio.gather(
+            *[cache_image_url(seg, client) for seg in msg if seg.type == "image"]
+        )
+
 
-            for i in data:
+async def cache_image_url(seg: MessageSegment, client: httpx.AsyncClient):
+    if url := seg.data.get("url"):
+        try:
+            r = await client.get(url)
+            data = r.content
+        except httpx.TimeoutException:
+            return
+        seg.type = "cached_image"
+        seg.data.clear()
+    else:
+        return
+    hash = hashlib.md5(data).hexdigest()
+    filename = f"{hash}.cache"
+    cache_file_path = cache_dir / filename
+    cache_files = [f.name for f in cache_dir.iterdir() if f.is_file()]
+    if filename not in cache_files:
+        async with aiofiles.open(cache_file_path, "wb") as f:
+            await f.write(data)
+    seg.data = {"file": filename}
+
+
+async def serialize_message(message: Message) -> List[Dict[str, Any]]:
+    if local_storage:
+        await cache_file(message)
+    return [seg.__dict__ for seg in message]
+
+
+def deserialize_message(message: List[Dict[str, Any]]) -> Message:
+    for seg in message:
+        if seg["type"] == "cached_image":
+            seg["type"] = "image"
+            seg["data"]["file"] = (cache_dir / seg["data"]["file"]).resolve().as_uri()
+    return parse_obj_as(Message, message)
+
+
+@post_db_init
+async def _():
+    old_data = data_dir / "data.json"
+    if old_data.exists():
+        logger.info("开始迁移旧漂流瓶数据")
+        with open(old_data, "r", encoding="utf-8") as f:
+            data = json.load(f)
+        async with create_session() as session:
+            offset = (await session.scalar(func.max(Bottle.id))) or 0 + 1
+            for idx, i in enumerate(data):
                 # 旧版json兼容 - 评论
                 isOldVersion = False
                 commentnew = []
-                for index, value in enumerate(i['comment']):
-                    if isinstance(value,str):
+                for index, value in enumerate(i["comment"]):
+                    if isinstance(value, str):
                         isOldVersion = True
-                        commentnew.append([0,value])
+                        commentnew.append([0, value])
                 if isOldVersion:
-                    i['comment'] = commentnew
+                    i["comment"] = commentnew
 
                 # 旧版json兼容 - 时间time、举报者
-                i.setdefault('time','0000-00-00 00:00:00')
-                i.setdefault('reported',[])
-                try:
-                    self.__data.append({
-                        'del': i['del'],
-                        "user": i["user"],
-                        "group": i['group'],
-                        "user_name": i['user_name'],
-                        "group_name": i["group_name"],
-                        "text": i['text'],
-                        "report": i['report'],
-                        "reported": i['reported'],
-                        "picked": i['picked'],
-                        "comment": i['comment'],
-                        "time": i['time']
-                    })
-                except:
-                    self.__data.append({})
-        else:
-            self.__data = 'E'
-            with self.data_path.open('w+', encoding='utf-8') as f:
-                f.write("[]")
-            logger.success(f"在 {self.data_path} 成功创建漂流瓶数据库")
-            self.__load()
+                i.setdefault("time", "0000-00-00 00:00:00")
+                i.setdefault("reported", [])
+                bottle = Bottle(
+                    user_id=i["user"],
+                    group_id=i["group"],
+                    user_name=i["user_name"],
+                    group_name=i["group_name"],
+                    content=await serialize_message(Message(i["text"])),
+                    report=i["report"],
+                    picked=i["picked"],
+                    is_del=i["del"],
+                    time=datetime.strptime(i["time"], "%Y-%m-%d %H:%M:%S"),
+                )
+                session.add(bottle)
+                for comment in i.get("comment", []):
+                    new_comment = Comment(
+                        user_id=comment[0],
+                        user_name=comment[1].split(":")[0],
+                        content=comment[1].split(":")[1],
+                        bottle_id=idx + offset,
+                    )
+                    session.add(new_comment)
+                for report in i.get("reported", []):
+                    new_report = Report(user_id=report, bottle_id=idx + offset)
+                    session.add(new_report)
+            await session.commit()
+            old_data.rename(data_dir / "data.json.old")
+            logger.info("旧漂流瓶数据迁移完成")
 
-    def __save(self) -> None:
-        with self.data_path.open('w+', encoding='utf-8') as f:
-            json.dump(self.__data, f, ensure_ascii=False, indent=4)
 
-    def print_all(self):
-        '''
-        打印读取`data文件`
-        '''
-        with self.data_path.open('r', encoding='utf-8') as f:
-            logger.info(f.read())
-
-    def check(self, key) -> bool:
-        '''
-        检查是否存在重复内容
-        '''
-        if not self.__data:
-            return False
-        for i in self.__data:
-            if key == i:
-                return True
-        return False
+class BottleManager:
+    def __init__(self) -> None:
+        pass
 
-    def add(self,bot:Bot, user: str, group: str, text,user_name,group_name) -> int:
-        '''
-        新增一个漂流瓶  
-        `user`: 用户QQ  
-        `group`: 群号  
-        `text`: 漂流瓶内容
-        '''
-        temp = {
-            'user': user,
-            'group': group,
-            'user_name': user_name,
-            'group_name': group_name,
-            'text': text,
-            'report': 0,
-            'reported': [],
-            'picked': 0,
-            'del': 0,
-            'comment': [],
-            'time': time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()),
-        }
-        if not self.check(temp):
-            self.__data.append(temp)
-            self.__save()
-            return self.__data.index(temp)
+    async def get_bottle(
+        self, index: int, session: AsyncSession, include_del: bool = False
+    ) -> Optional["Bottle"]:
+        """获取一个瓶子
+
+        Args:
+            index (int): 瓶子序号
+            session (AsyncSession): 会话
+            include_del (bool) : 是否包括被删除的瓶子
+        """
+        if not include_del:
+            return await session.scalar(
+                select(Bottle).where(Bottle.id == index, Bottle.is_del == False)
+            )
         else:
-            logger.warning("添加失败！")
-            return 0
+            return await session.scalar(select(Bottle).where(Bottle.id == index))
 
-    def select(self,time = 0):
-        '''
-        抽取漂流瓶
-        '''
-        if time >= 100:
-            return []
-        elif self.__data:
-            print(time)
-            index = random.randint(0, len(self.__data)-1)
-            if self.__data[index]['del']:
-                return self.select(time + 1)
-            self.__data[index]['picked'] += 1
-            self.__save()
-            return [index, self.__data[index]]
-            
+    async def add_bottle(
+        self,
+        user_id: int,
+        group_id: int,
+        content: List[Dict[str, Any]],
+        user_name: str,
+        group_name: str,
+        session: AsyncSession,
+    ) -> int:
+        """添加漂流瓶
+
+        Args:
+            user_id (int): 用户id
+            group_id (int): 群id
+            content (str): 内容
+            user_name (str): 用户名
+            group_name (str): 群名
+            session (AsyncSession): 会话
+
+        Returns:
+            int: 漂流瓶id
+        """
+        bottles = await session.scalars(
+            select(Bottle).where(Bottle.user_id == user_id, Bottle.group_id == group_id)
+        )
+        for bottle in bottles:
+            if bottle.content == content:
+                logger.warning("添加失败！")
+                return 0
+        else:
+            bottle = Bottle(
+                user_id=user_id,
+                group_id=group_id,
+                content=content,
+                user_name=user_name,
+                group_name=group_name,
+            )
+            session.add(bottle)
+            await session.commit()
+            await session.refresh(bottle)
+            return bottle.id
+
+    async def select(self, session: AsyncSession) -> Optional[Bottle]:
+        """随机选择一个漂流瓶
+
+        Args:
+            session (AsyncSession): 会话
+
+        Returns:
+            Optional[Bottle]: 随机一个瓶子
+        """
+        bottle = await session.scalar(
+            select(Bottle)
+            .where(Bottle.is_del == False)
+            .order_by(func.random())
+            .limit(1)
+        )
+        if bottle:
+            bottle.picked += 1
+        return bottle
+
+    async def clear(self, session: AsyncSession) -> None:
+        """清空漂流瓶
+
+        Args:
+            session (AsyncSession): 会话
+        """
+        engine = get_engine()
+        for table in [
+            "nonebot_plugin_bottle_bottle",
+            "nonebot_plugin_bottle_comment",
+            "nonebot_plugin_bottle_report",
+        ]:
+            if engine.name == "sqlite":
+                await session.execute(text(f"DELETE FROM {table}"))
+            else:
+                await session.execute(text(f"TRUNCATE TABLE {table}"))
 
-    def clear(self):
-        '''
-        清空漂流瓶
-        '''
-        self.__data = []
-        self.__save()
-
-    def report(self, index: int,user_id, timesMax: int = 5) -> int:
-        '''
-        举报漂流瓶  
+    async def report(
+        self, bottle: Bottle, user_id: int, session: AsyncSession, times_max: int = 5
+    ) -> int:
+        """
+        举报漂流瓶
         `index`: 漂流瓶编号
         `timesMax`: 到达此数值自动处理
 
-        返回  
+        返回
         0 举报失败
         1 举报成功
         2 举报成功并且已经自动处理
         3 已经删除
-        '''
-        if index > len(self.__data)-1 or index < 0:
+        """
+        if await session.scalar(
+            select(Report).where(
+                Report.user_id == user_id, Report.bottle_id == bottle.id
+            )
+        ):
             return 0
-        if user_id in self.__data[index]['reported']:
-            return 0
-        
-        try:
-            self.__data[index]['report'] += 1
-        except:
-            self.__data[index]['report'] = 1
-
-        if self.__data[index]['del'] == 1:
+        if bottle.is_del:
             return 3
-
-        if self.__data[index]['report'] >= timesMax:
-            try:
-                self.remove(index)
-                self.__save()
-                return 2
-            except:
-                return 0
+        bottle.report += 1
+        if bottle.report >= times_max:
+            bottle.is_del = True
+            return 2
         else:
-            self.__data[index]['reported'].append(user_id)
-            self.__save()
+            new_report = Report(user_id=user_id, bottle_id=bottle.id)
+            session.add(new_report)
             return 1
 
-    def check_report(self, index: int) -> int:
-        '''
-        返回漂流瓶被举报次数
-        `index`: 漂流瓶编号
-        '''
-        return self.__data[index]['report']
+    def comment(
+        self,
+        bottle: Bottle,
+        user_id: int,
+        user_name: str,
+        content: str,
+        session: AsyncSession,
+    ) -> None:
+        """评论漂流瓶
+
+        Args:
+            bottle (Bottle): 瓶子
+            user_id (int): 用户id
+            user_name (str): 用户名
+            content (str): 内容
+            session (AsyncSession): 会话
+        """
+        new_comment = Comment(
+            user_id=user_id, user_name=user_name, content=content, bottle_id=bottle.id
+        )
+        session.add(new_comment)
+
+    async def get_comment(
+        self,
+        bottle: Bottle,
+        session: AsyncSession,
+        limit: Optional[int] = 3,
+    ) -> Sequence[Comment]:
+        """获取评论
+
+        Args:
+            bottle (Bottle): 瓶子
+            session (AsyncSession): 会话
+            limit (Optional[int], optional): 评论个数. Defaults to 3.
+
+        Returns:
+            Sequence[Comment]: 评论们
+        """
+        return (
+            await session.scalars(
+                statement=select(Comment)
+                .where(Comment.bottle_id == bottle.id)
+                .order_by(Comment.time.desc())
+                .limit(limit)
+            )
+        ).all()
+
+    async def del_comment(self, bottle: Bottle, user_id: int, session: AsyncSession):
+        """删除瓶子中用户id的所有评论
+
+        Args:
+            bottle (Bottle): 瓶子
+            user_id (int): 用户id
+            session (AsyncSession): 会话
+        """
+        comments = await session.scalars(
+            statement=select(Comment).where(
+                Comment.bottle_id == bottle.id, Comment.user_id == user_id
+            )
+        )
+        for comment in comments:
+            await session.delete(comment)
 
-    def comment(self, index: int,user:str, com):
-        '''
-        评论漂流瓶
-        `index`: 漂流瓶编号  
-        `user`: QQ号  
-        `com`: 评论内容
-        '''
-        com = [user,com]
-        try:
-            if not com in self.__data[index]['comment']:
-                self.__data[index]['comment'].append(com)
-        except:
-            self.__data[index]['comment'] = [com]
-        self.__save()
 
-    def check_comment(self, index: int):
-        '''
-        查看评论
-        `index`: 漂流瓶编号
-        '''
-        try:
-            return [value[1] for value in self.__data[index]['comment']]
-        except:
-            try:
-                self.__data[index]['comment'] = []
-            except:
-                pass
-            return []
-
-    def remove_comment(self,index: int,user: int):
-        '''
-        删除指定漂流瓶里某人的所有评论
-        `index`: 漂流瓶编号  
-        `user`: QQ号  
-        '''
-        user = int(user)
-        self.__data[index]['comment'] = [i for i in self.__data[index]['comment'] if i[0] != user]
-        self.__save()
-        return True
+bottle_manager = BottleManager()
 
-    def check_bottle(self,index:int):
-        '''
-        获取漂流瓶信息
-        `index`: 漂流瓶编号
-        '''
-        if 0<=index<len(self.__data):
-            return self.__data[index]
-        else:
-            return {}
-
-    def remove(self,index:int):
-        '''
-        直接移除漂流瓶
-        `index`: 漂流瓶编号
-        '''
-        try:
-            self.__data[index]['del'] = 1
-            self.__save()
-            return True
-        except:
-            logger.warning('删除错误！')
-            return False
-        
-    def resume(self,index:int):
-        '''
-        恢复漂流瓶
-        `index`: 漂流瓶编号
-        '''
-        try:
-            self.__data[index]['del'] = 0
-            self.__save()
-            return True
-        except:
-            logger.warning('恢复错误！')
-            return False
-        
-bottle = Bottle()
 
 class Audit(object):
-    bannedMessage = ''
+    bannedMessage = ""
+
     def __init__(self) -> None:
         self.data_path = Path("data/bottle/permissionsList.json").absolute()
         self.data_dir = Path("data/bottle").absolute()
         self.data_dir.mkdir(parents=True, exist_ok=True)
         self.__data = {
-            'enableCooldown': True,
-            'cooldownTime': 30,
-            'bannedMessage': '',
-            'user': [],
-            'group':[],
-            'cooldown':{},
-            'disreportable':[],
-            'whiteUser':[],
-            'whiteGroup': [],
+            "enableCooldown": True,
+            "cooldownTime": 30,
+            "bannedMessage": "",
+            "user": [],
+            "group": [],
+            "cooldown": {},
+            "disreportable": [],
+            "whiteUser": [],
+            "whiteGroup": [],
         }
         self.__load()
 
     def __load(self):
         try:
             with self.data_path.open("r+", encoding="utf-8") as f:
                 data = json.load(f)
         except Exception as e:
-            with self.data_path.open('w+', encoding='utf-8') as f:
+            with self.data_path.open("w+", encoding="utf-8") as f:
                 json.dump(self.__data, f)
             logger.success(f"在 {self.data_path} 成功创建漂流瓶黑名单数据库")
         else:
             self.__data.update(data)
-            self.bannedMessage = self.__data['bannedMessage']
-            
+            self.bannedMessage = self.__data["bannedMessage"]
 
     def __save(self) -> None:
-        with self.data_path.open('w+', encoding='utf-8') as f:
+        with self.data_path.open("w+", encoding="utf-8") as f:
             f.write(json.dumps(self.__data, ensure_ascii=False, indent=4))
 
-    def add(self,mode,num):
-        '''
-        添加权限  
-        `mode`:  
+    def add(self, mode, num):
+        """
+        添加权限
+        `mode`:
             `group`: 群号
             `user`: QQ号
-            `cooldown`: 暂时冷却QQ号  
-            `whiteUser`: 白名单QQ号  
-            `whiteGroup`: 白名单群号  
+            `cooldown`: 暂时冷却QQ号
+            `whiteUser`: 白名单QQ号
+            `whiteGroup`: 白名单群号
         `num`: QQ/QQ群号
-        '''
+        """
         num = str(num)
         try:
-            if mode != 'cooldown' and num not in self.__data[mode]:
+            if mode != "cooldown" and num not in self.__data[mode]:
                 self.__data[mode].append(num)
-            elif not (self.checkWhite('whiteUser',num) or self.check('whiteGroup',num)) and self.__data['enableCooldown'] and mode == 'cooldown':
-                self.__data['cooldown'][num] = int(time.time()) + self.__data['cooldownTime']
+            elif (
+                not (self.checkWhite("whiteUser", num) or self.check("whiteGroup", num))
+                and self.__data["enableCooldown"]
+                and mode == "cooldown"
+            ):
+                self.__data["cooldown"][num] = (
+                    int(time.time()) + self.__data["cooldownTime"]
+                )
             else:
                 return False
             self.__save()
             return True
         except Exception as e:
-            print(e)
+            logger.warning(e)
             return False
-        
-    def remove(self,mode,num):
-        '''
-        移除黑名单  
-        `mode`:  
+
+    def remove(self, mode, num):
+        """
+        移除黑名单
+        `mode`:
             `group`: 群号
             `user`: QQ号
-            `whiteUser`: 白名单QQ号  
-            `whiteGroup`: 白名单群号  
+            `whiteUser`: 白名单QQ号
+            `whiteGroup`: 白名单群号
         `num`: QQ/QQ群号
-        '''
+        """
         num = str(num)
         try:
             self.__data[mode].remove(num)
             self.__save()
             return True
         except:
             return False
-    
-    def verify(self,user,group):
-        '''
-        返回是否通过验证(白名单优先)  
+
+    def verify(self, user, group):
+        """
+        返回是否通过验证(白名单优先)
         `user`: QQ号
         `group`: 群号
 
-        返回：  
-            `True`: 通过  
-            `False`: 未通过  
-        '''
-        if not (self.checkWhite('whiteUser',user) or self.checkWhite('whiteGroup',group)):
-            if self.check('user',user) or self.check('group',group) or self.check('cooldown',user):
+        返回：
+            `True`: 通过
+            `False`: 未通过
+        """
+        if not (
+            self.checkWhite("whiteUser", user) or self.checkWhite("whiteGroup", group)
+        ):
+            if (
+                self.check("user", user)
+                or self.check("group", group)
+                or self.check("cooldown", user)
+            ):
                 return False
         return True
-    
-    def verifyReport(self,qq):
-        '''
-        检查是否有举报权限  
-
-        返回：  
-            `True`: 具有权限  
-            `False`： 不具有权限  
-        '''
-        if str(qq) in self.__data['disreportable']:
+
+    def verifyReport(self, qq):
+        """
+        检查是否有举报权限
+
+        返回：
+            `True`: 具有权限
+            `False`： 不具有权限
+        """
+        if str(qq) in self.__data["disreportable"]:
             return False
         else:
             return True
 
-    def check(self,mode,num):
-        
-        '''
+    def check(self, mode, num):
+        """
         查找是否处于黑名单
-        `mode`:  
+        `mode`:
             `group`: 群号
             `user`: QQ号
-            `cooldown`: 暂时冷却QQ号  
+            `cooldown`: 暂时冷却QQ号
         `num`: QQ/QQ群号
-        '''
+        """
         num = str(num)
-        if mode in ['group','user']:
+        if mode in ["group", "user"]:
             if num in self.__data[mode]:
                 return True
         else:
             if num in self.__data[mode]:
                 if time.time() <= self.__data[mode][num]:
                     return True
         return False
-    
-    def checkWhite(self,mode,num:str):
-        '''
-        检查是否为白名单  
-        `mode`:  
-            `whiteUser`: 白名单QQ号  
-            `whiteGroup`: 白名单群号  
+
+    def checkWhite(self, mode, num: str):
+        """
+        检查是否为白名单
+        `mode`:
+            `whiteUser`: 白名单QQ号
+            `whiteGroup`: 白名单群号
         `num`: QQ/QQ群号
-        '''
+        """
         num = str(num)
-        if mode == 'whiteUser' and num in self.__data['whiteUser']:
+        if mode == "whiteUser" and num in self.__data["whiteUser"]:
             return True
-        elif mode == 'whiteGroup' and num in self.__data['whiteGroup']:
+        elif mode == "whiteGroup" and num in self.__data["whiteGroup"]:
             return True
         else:
             return False
-        
-    def banreport(self,qq):
-        '''
-        删除/恢复某人的举报权限  
-        `qq`: QQ号  
+
+    def banreport(self, qq):
+        """
+        删除/恢复某人的举报权限
+        `qq`: QQ号
         返回:
-            `0`: 成功解封  
+            `0`: 成功解封
             `1`: 成功封禁
             `e`: 错误信息
-        '''
+        """
         try:
-            if qq not in self.__data['disreportable']:
-                self.__data['disreportable'].append(qq)
+            if qq not in self.__data["disreportable"]:
+                self.__data["disreportable"].append(qq)
                 self.__save()
                 return 1
             else:
-                self.__data['disreportable'].remove(qq)
+                self.__data["disreportable"].remove(qq)
                 self.__save()
                 return 0
         except Exception as e:
             return e
 
+
 ba = Audit()
 
 cursepath = Path("data/bottle/curse.json").absolute()
-async def text_audit(text:str,ak = api_key,sk = secret_key):
-    '''
-    文本审核(百度智能云)  
+
+
+async def text_audit(text: str, ak=api_key, sk=secret_key):
+    """
+    文本审核(百度智能云)
     `text`: 待审核文本
     `ak`: api_key
     `sk`: secret_key
-    '''
+    """
     if (not api_key) or (not secret_key):
         # 未配置key 进行简单违禁词审核
-        try: 
-            with cursepath.open('r',encoding='utf-8') as f:
-                for i in json.load(f):
+        try:
+            async with aiofiles.open(cursepath, "r", encoding="utf-8") as f:
+                for i in json.loads(await f.read()):
                     if i in text:
-                        return {
-                            'conclusion': '不合规',
-                            'data': [
-                                {
-                                    'msg': f'触发违禁词 {i}'
-                                }
-                            ]
-                        }
-                return 'pass'
+                        return {"conclusion": "不合规", "data": [{"msg": f"触发违禁词 {i}"}]}
+                return "pass"
         except:
             if not cursepath.exists():
-                with cursepath.open('w+',encoding='utf-8') as f:
+                with cursepath.open("w+", encoding="utf-8") as f:
                     f.write("[]")
-                return 'pass'
+                return "pass"
             else:
-                return 'Error'
+                return "Error"
     # access_token 获取
-    host = f'https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id={ak}&client_secret={sk}'
+    host = f"https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id={ak}&client_secret={sk}"
     async with httpx.AsyncClient() as client:
         response = await client.get(host)
         if response:
-            access_token = response.json()['access_token']
+            access_token = response.json()["access_token"]
         else:
             # 未返回access_token 返回错误
-            return 'Error'
-    
-        request_url = "https://aip.baidubce.com/rest/2.0/solution/v1/text_censor/v2/user_defined"
-        params = {"text":text}
+            return "Error"
+
+        request_url = (
+            "https://aip.baidubce.com/rest/2.0/solution/v1/text_censor/v2/user_defined"
+        )
+        params = {"text": text}
         request_url = request_url + "?access_token=" + access_token
-        headers = {'content-type': 'application/x-www-form-urlencoded'}
+        headers = {"content-type": "application/x-www-form-urlencoded"}
         response = await client.post(request_url, data=params, headers=headers)
         if response:
             return response.json()
         else:
             # 调用审核API失败
-            return 'Error'
+            return "Error"
```

## Comparing `nonebot_plugin_bottle-0.2.7.dist-info/LICENCE` & `nonebot_plugin_bottle-1.0.0.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `nonebot_plugin_bottle-0.2.7.dist-info/METADATA` & `nonebot_plugin_bottle-1.0.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 0.2.7
+Version: 1.0.0
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 Author: Todysheep
 Author-email: todysheep@163.com
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: nonebot2 (>=2.0.0-beta.2)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0b1)
 Requires-Dist: nonebot-adapter-onebot
+Requires-Dist: aiofiles (>=0.8.0)
+Requires-Dist: nonebot-plugin-datastore (>=0.6.0)
 Requires-Dist: httpx
 
 # Nonebot 漂流瓶插件
 * 安装
     -
     - 使用 `pip install nonebot_plugin_bottle`
     - 使用 `nb plugin install nonebot_plugin_bottle`
@@ -73,33 +75,46 @@
         - 格式：  
             ```
             ["屏蔽词1","屏蔽词2"]
             ```
         - 屏蔽词推荐（需要手动更改）：[防嘴臭插件](https://github.com/tkgs0/nonebot-plugin-antiinsult/blob/main/nonebot_plugin_antiinsult/curse.json)
         - 若为空列表则不进行审核
 
-* 已知bug
+* 配置文件（.env.*）
     -
-    - 第一次加载该插件时无法正常使用（重启后恢复）
+    | 配置项 | 配置名 | 变量类型 |  默认值 |
+    |:--------|:----------|:-------------:|------:|
+    | API KEY | nonebot_plugin_bottle_api_key | str | "" |
+    | SECRET KEY | nonebot_plugin_bottle_secret_key | str | "" |
+    | 是否缓存图片 | nonebot_plugin_bottle_local_storage | bool | True |
+
 
 * 更新日志
+    -  
+    - ***重构版本*** 1.0.0 [2023-3-10] [#32](https://github.com/Todysheep/nonebot_plugin_bottle/issues/32) [@LambdaYH](https://github.com/LambdaYH)
+        - 使用`nonebot_plugin_datastore`重构
+        - 异步读取违禁词文件
+        - 异步读取违禁词文件
+        - 启动时将旧json数据迁移
+        - 优化图片缓存
+        - 调整require位置
     - 0.2.7 [2023-2-25]
         - `举报漂流瓶`现在可以禁止某人使用了（`漂流瓶黑名单 举报 [qq号]`）
         - 新增`恢复漂流瓶`指令，可以恢复被删除的漂流瓶
     - 0.2.6 [2023-2-24]
         - `举报漂流瓶`修复了单人可以举报多次的问题
         - [ ] 格式化漂流瓶输出
-    - 0.2.5 [2023-2-24]
-        - 更改`requests`请求方式为`httpx` #29
-        - 适配`metadata` #29
-        - 💥破坏性更新 `api_key`与`secret_key`将在`.env.*`中填写（详见上方） #29
 
     <details>
         <summary>更多更新</summary>
 
+        - 0.2.5 [2023-2-24]
+            - 更改`requests`请求方式为`httpx` [#29](https://github.com/Todysheep/nonebot_plugin_bottle/issues/29)
+            - 适配`metadata` #29
+            - 💥破坏性更新 `api_key`与`secret_key`将在`.env.*`中填写（详见上方） [#29](https://github.com/Todysheep/nonebot_plugin_bottle/issues/29)
         - 0.2.4
             - 现在开始记录扔漂流瓶的时间，旧版本的漂流瓶时间为`0000-00-00 00:00:00`,使用`查看漂流瓶可以查看具体时间`
         - 0.2.3
             - `删除漂流瓶`现在所有人可用，并进行了一些权限限制
             - `捡漂流瓶`函数更新了递归上限防止无限递归
             - 要求后续内容输入的所有指令现需要空格隔开
         - 0.2.2
@@ -122,21 +137,18 @@
             - 新增配置项`api_key`,'secret_key'，用于文本审核
             - 新增配置项`black_group`，用于屏蔽特定群聊
 
     </details>
 
 * 特别感谢
     -
-    - @a563696823 适配commit，更改config填写，适配httpx
-    - @MTmin 多机器人版本
-    - @Sevenyine 发了~~114514条~~issue
+    - **[@LambdaYH](https://github.com/LambdaYH)** PR了~~一个现有作者根本看不懂的~~重构版本 (1.0.0)
+    - [@a563696823](https://github.com/a563696823) 适配commit，更改config填写，适配httpx
+    - [@MTmin](https://github.com/MTmin) 多机器人版本
+    - [@Sevenyine](https://github.com/Sevenyine) 发了~~114514条~~issue
 
 * 效果展示
     -
     ![image](https://user-images.githubusercontent.com/97968466/191049794-1b409436-fd70-43d9-8dcb-3575e82fd69b.png)  
     ![image](https://user-images.githubusercontent.com/97968466/213113862-e6c7568b-8686-4e97-8f83-7354ff1cb704.png)  
     ![image](https://user-images.githubusercontent.com/97968466/191052704-1b5ec89d-7a49-40d6-a5d9-b0a0171c730e.png)  
     ![image](https://user-images.githubusercontent.com/97968466/191049649-2e8d8555-f285-470f-9f7b-f5a0994341ee.png)  
-
-* ~~TODO~~
-    -
-    - [ ] ~~我迟早要把你这个史山代码重构了~~
```

## Comparing `nonebot_plugin_bottle-0.2.7.dist-info/RECORD` & `nonebot_plugin_bottle-1.0.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-nonebot_plugin_bottle/__init__.py,sha256=akC0ZKJ-GBXGYMRfs6UlWrEJHnSkb8AXkTPY91G9C-I,13254
-nonebot_plugin_bottle/config.py,sha256=PANDyTJF-KATE5-K4mpuxVwmUqChnCQNAvl2peaoQ1k,484
-nonebot_plugin_bottle/data_source.py,sha256=npsCD9WuR2ZTTg1Qwqfq_pPau-IKu_2u5-nUNg4UDmM,14830
-nonebot_plugin_bottle-0.2.7.dist-info/LICENCE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
-nonebot_plugin_bottle-0.2.7.dist-info/METADATA,sha256=lyagjjb8kQwmztprFkRKOGQGe3f7KKt60nDKesMIDtQ,7224
-nonebot_plugin_bottle-0.2.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-nonebot_plugin_bottle-0.2.7.dist-info/top_level.txt,sha256=Q9vMfveUHJFO9CzFuJmg1yJ0jzwBs0034WbzsgQrcfw,22
-nonebot_plugin_bottle-0.2.7.dist-info/RECORD,,
+nonebot_plugin_bottle/__init__.py,sha256=IRsRQKTwGJZdkGzbUDVLliBIEUwng58g_veLYsbcYyA,17111
+nonebot_plugin_bottle/config.py,sha256=ZR5r0jPivngaixOdWe8Zq51GdVNH2eGMB2mY6g8BJb4,636
+nonebot_plugin_bottle/data_source.py,sha256=abz1ePDi3wvAKfDAv6L4kF2Wrf4UPNyddKLU5vxVRZQ,17498
+nonebot_plugin_bottle/model.py,sha256=KOSnuuBvJJJtWPKnrvo8hvZACX1l1K4ahYLuyrXQb6A,1426
+nonebot_plugin_bottle-1.0.0.dist-info/LICENCE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
+nonebot_plugin_bottle-1.0.0.dist-info/METADATA,sha256=sXYvfm61yO0EBrsTRDKEGKEGzstL7JhoGlpKm7xks_4,8238
+nonebot_plugin_bottle-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+nonebot_plugin_bottle-1.0.0.dist-info/top_level.txt,sha256=Q9vMfveUHJFO9CzFuJmg1yJ0jzwBs0034WbzsgQrcfw,22
+nonebot_plugin_bottle-1.0.0.dist-info/RECORD,,
```

