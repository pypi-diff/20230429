# Comparing `tmp/meme_generator-0.0.8.tar.gz` & `tmp/meme_generator-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meme_generator-0.0.8.tar", max compression
+gzip compressed data, was "meme_generator-0.0.9.tar", max compression
```

## Comparing `meme_generator-0.0.8.tar` & `meme_generator-0.0.9.tar`

### file list

```diff
@@ -1,169 +1,174 @@
--rw-r--r--   0        0        0     1063 2023-03-28 16:27:36.599649 meme_generator-0.0.8/LICENSE
--rw-r--r--   0        0        0     9549 2023-03-28 16:27:36.599649 meme_generator-0.0.8/README.md
--rw-r--r--   0        0        0      998 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/__init__.py
--rw-r--r--   0        0        0     7005 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/app.py
--rw-r--r--   0        0        0     6529 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/cli.py
--rw-r--r--   0        0        0     1363 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/config.py
--rw-r--r--   0        0        0     8303 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/dirs.py
--rw-r--r--   0        0        0     2272 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/download.py
--rw-r--r--   0        0        0     3446 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/exception.py
--rw-r--r--   0        0        0      131 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/log.py
--rw-r--r--   0        0        0     2777 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/manager.py
--rw-r--r--   0        0        0     5616 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/meme.py
--rw-r--r--   0        0        0     5138 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/memes/5000choyen/__init__.py
--rw-r--r--   0        0        0     1025 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/memes/addiction/__init__.py
--rw-r--r--   0        0        0      775 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/memes/alike/__init__.py
--rw-r--r--   0        0        0     3505 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/memes/always/__init__.py
--rw-r--r--   0        0        0     2768 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/memes/always_like/__init__.py
--rw-r--r--   0        0        0      503 2023-03-28 16:27:36.939654 meme_generator-0.0.8/meme_generator/memes/anti_kidnap/__init__.py
--rw-r--r--   0        0        0     1166 2023-03-28 16:27:36.947654 meme_generator-0.0.8/meme_generator/memes/anya_suki/__init__.py
--rw-r--r--   0        0        0      859 2023-03-28 16:27:36.947654 meme_generator-0.0.8/meme_generator/memes/applaud/__init__.py
--rw-r--r--   0        0        0      845 2023-03-28 16:27:36.947654 meme_generator-0.0.8/meme_generator/memes/ascension/__init__.py
--rw-r--r--   0        0        0     2570 2023-03-28 16:27:36.951654 meme_generator-0.0.8/meme_generator/memes/ask/__init__.py
--rw-r--r--   0        0        0      587 2023-03-28 16:27:36.951654 meme_generator-0.0.8/meme_generator/memes/back_to_work/__init__.py
--rw-r--r--   0        0        0      888 2023-03-28 16:27:36.951654 meme_generator-0.0.8/meme_generator/memes/bad_news/__init__.py
--rw-r--r--   0        0        0     1252 2023-03-28 16:27:36.955654 meme_generator-0.0.8/meme_generator/memes/beat_head/__init__.py
--rw-r--r--   0        0        0      966 2023-03-28 16:27:36.955654 meme_generator-0.0.8/meme_generator/memes/bite/__init__.py
--rw-r--r--   0        0        0      640 2023-03-28 16:27:36.959654 meme_generator-0.0.8/meme_generator/memes/blood_pressure/__init__.py
--rw-r--r--   0        0        0     1611 2023-03-28 16:27:36.963654 meme_generator-0.0.8/meme_generator/memes/bocchi_draft/__init__.py
--rw-r--r--   0        0        0      795 2023-03-28 16:27:36.987655 meme_generator-0.0.8/meme_generator/memes/bronya_holdsign/__init__.py
--rw-r--r--   0        0        0     1678 2023-03-28 16:27:36.991654 meme_generator-0.0.8/meme_generator/memes/bubble_tea/__init__.py
--rw-r--r--   0        0        0      679 2023-03-28 16:27:36.991654 meme_generator-0.0.8/meme_generator/memes/call_110/__init__.py
--rw-r--r--   0        0        0      857 2023-03-28 16:27:36.991654 meme_generator-0.0.8/meme_generator/memes/capoo_rub/__init__.py
--rw-r--r--   0        0        0     1465 2023-03-28 16:27:36.991654 meme_generator-0.0.8/meme_generator/memes/capoo_say/__init__.py
--rw-r--r--   0        0        0     1371 2023-03-28 16:27:36.991654 meme_generator-0.0.8/meme_generator/memes/capoo_strike/__init__.py
--rw-r--r--   0        0        0      871 2023-03-28 16:27:36.991654 meme_generator-0.0.8/meme_generator/memes/captain/__init__.py
--rw-r--r--   0        0        0     1211 2023-03-28 16:27:36.995655 meme_generator-0.0.8/meme_generator/memes/charpic/__init__.py
--rw-r--r--   0        0        0     3233 2023-03-28 16:27:36.995655 meme_generator-0.0.8/meme_generator/memes/chase_train/__init__.py
--rw-r--r--   0        0        0      487 2023-03-28 16:27:37.003655 meme_generator-0.0.8/meme_generator/memes/china_flag/__init__.py
--rw-r--r--   0        0        0      973 2023-03-28 16:27:37.007655 meme_generator-0.0.8/meme_generator/memes/confuse/__init__.py
--rw-r--r--   0        0        0     1188 2023-03-28 16:27:37.015655 meme_generator-0.0.8/meme_generator/memes/coupon/__init__.py
--rw-r--r--   0        0        0      567 2023-03-28 16:27:37.015655 meme_generator-0.0.8/meme_generator/memes/cover_face/__init__.py
--rw-r--r--   0        0        0     1000 2023-03-28 16:27:37.015655 meme_generator-0.0.8/meme_generator/memes/crawl/__init__.py
--rw-r--r--   0        0        0      749 2023-03-28 16:27:37.059656 meme_generator-0.0.8/meme_generator/memes/cyan/__init__.py
--rw-r--r--   0        0        0      508 2023-03-28 16:27:37.059656 meme_generator-0.0.8/meme_generator/memes/decent_kiss/__init__.py
--rw-r--r--   0        0        0     1710 2023-03-28 16:27:37.059656 meme_generator-0.0.8/meme_generator/memes/dianzhongdian/__init__.py
--rw-r--r--   0        0        0      634 2023-03-28 16:27:37.059656 meme_generator-0.0.8/meme_generator/memes/dinosaur/__init__.py
--rw-r--r--   0        0        0      700 2023-03-28 16:27:37.063655 meme_generator-0.0.8/meme_generator/memes/distracted/__init__.py
--rw-r--r--   0        0        0      500 2023-03-28 16:27:37.063655 meme_generator-0.0.8/meme_generator/memes/divorce/__init__.py
--rw-r--r--   0        0        0      632 2023-03-28 16:27:37.067656 meme_generator-0.0.8/meme_generator/memes/dont_touch/__init__.py
--rw-r--r--   0        0        0     2342 2023-03-28 16:27:37.067656 meme_generator-0.0.8/meme_generator/memes/douyin/__init__.py
--rw-r--r--   0        0        0      595 2023-03-28 16:27:37.067656 meme_generator-0.0.8/meme_generator/memes/eat/__init__.py
--rw-r--r--   0        0        0      776 2023-03-28 16:27:37.067656 meme_generator-0.0.8/meme_generator/memes/fanatic/__init__.py
--rw-r--r--   0        0        0     1273 2023-03-28 16:27:37.067656 meme_generator-0.0.8/meme_generator/memes/fencing/__init__.py
--rw-r--r--   0        0        0     1101 2023-03-28 16:27:37.071656 meme_generator-0.0.8/meme_generator/memes/find_chips/__init__.py
--rw-r--r--   0        0        0     1269 2023-03-28 16:27:37.071656 meme_generator-0.0.8/meme_generator/memes/follow/__init__.py
--rw-r--r--   0        0        0      829 2023-03-28 16:27:37.071656 meme_generator-0.0.8/meme_generator/memes/funny_mirror/__init__.py
--rw-r--r--   0        0        0      903 2023-03-28 16:27:37.071656 meme_generator-0.0.8/meme_generator/memes/garbage/__init__.py
--rw-r--r--   0        0        0     4141 2023-03-28 16:27:37.079656 meme_generator-0.0.8/meme_generator/memes/gif_subtitle/__init__.py
--rw-r--r--   0        0        0      901 2023-03-28 16:27:37.131657 meme_generator-0.0.8/meme_generator/memes/good_news/__init__.py
--rw-r--r--   0        0        0      697 2023-03-28 16:27:37.135657 meme_generator-0.0.8/meme_generator/memes/google/__init__.py
--rw-r--r--   0        0        0     1631 2023-03-28 16:27:37.135657 meme_generator-0.0.8/meme_generator/memes/gun/__init__.py
--rw-r--r--   0        0        0      886 2023-03-28 16:27:37.135657 meme_generator-0.0.8/meme_generator/memes/hammer/__init__.py
--rw-r--r--   0        0        0     1094 2023-03-28 16:27:37.135657 meme_generator-0.0.8/meme_generator/memes/high_EQ/__init__.py
--rw-r--r--   0        0        0     1950 2023-03-28 16:27:37.135657 meme_generator-0.0.8/meme_generator/memes/hit_screen/__init__.py
--rw-r--r--   0        0        0     1050 2023-03-28 16:27:37.139657 meme_generator-0.0.8/meme_generator/memes/hold_grudge/__init__.py
--rw-r--r--   0        0        0      499 2023-03-28 16:27:37.139657 meme_generator-0.0.8/meme_generator/memes/hold_tight/__init__.py
--rw-r--r--   0        0        0      862 2023-03-28 16:27:37.139657 meme_generator-0.0.8/meme_generator/memes/hug_leg/__init__.py
--rw-r--r--   0        0        0      766 2023-03-28 16:27:37.143657 meme_generator-0.0.8/meme_generator/memes/hutao_bite/__init__.py
--rw-r--r--   0        0        0      753 2023-03-28 16:27:37.143657 meme_generator-0.0.8/meme_generator/memes/imprison/__init__.py
--rw-r--r--   0        0        0     1192 2023-03-28 16:27:37.143657 meme_generator-0.0.8/meme_generator/memes/incivilization/__init__.py
--rw-r--r--   0        0        0     1285 2023-03-28 16:27:37.147657 meme_generator-0.0.8/meme_generator/memes/interview/__init__.py
--rw-r--r--   0        0        0     2926 2023-03-28 16:27:37.147657 meme_generator-0.0.8/meme_generator/memes/jiji_king/__init__.py
--rw-r--r--   0        0        0      652 2023-03-28 16:27:37.147657 meme_generator-0.0.8/meme_generator/memes/jiujiu/__init__.py
--rw-r--r--   0        0        0     1769 2023-03-28 16:27:37.147657 meme_generator-0.0.8/meme_generator/memes/kaleidoscope/__init__.py
--rw-r--r--   0        0        0      512 2023-03-28 16:27:37.147657 meme_generator-0.0.8/meme_generator/memes/karyl_point/__init__.py
--rw-r--r--   0        0        0     1353 2023-03-28 16:27:37.151657 meme_generator-0.0.8/meme_generator/memes/keep_away/__init__.py
--rw-r--r--   0        0        0      910 2023-03-28 16:27:37.151657 meme_generator-0.0.8/meme_generator/memes/kick_ball/__init__.py
--rw-r--r--   0        0        0     1995 2023-03-28 16:27:37.155657 meme_generator-0.0.8/meme_generator/memes/kirby_hammer/__init__.py
--rw-r--r--   0        0        0     1179 2023-03-28 16:27:37.187657 meme_generator-0.0.8/meme_generator/memes/kiss/__init__.py
--rw-r--r--   0        0        0     1089 2023-03-28 16:27:37.191657 meme_generator-0.0.8/meme_generator/memes/klee_eat/__init__.py
--rw-r--r--   0        0        0      894 2023-03-28 16:27:37.195657 meme_generator-0.0.8/meme_generator/memes/knock/__init__.py
--rw-r--r--   0        0        0     1099 2023-03-28 16:27:37.203657 meme_generator-0.0.8/meme_generator/memes/learn/__init__.py
--rw-r--r--   0        0        0     1268 2023-03-28 16:27:37.203657 meme_generator-0.0.8/meme_generator/memes/lim_x_0/__init__.py
--rw-r--r--   0        0        0      724 2023-03-28 16:27:37.207658 meme_generator-0.0.8/meme_generator/memes/listen_music/__init__.py
--rw-r--r--   0        0        0     1599 2023-03-28 16:27:37.207658 meme_generator-0.0.8/meme_generator/memes/little_angel/__init__.py
--rw-r--r--   0        0        0     1262 2023-03-28 16:27:37.207658 meme_generator-0.0.8/meme_generator/memes/loading/__init__.py
--rw-r--r--   0        0        0     1599 2023-03-28 16:27:37.207658 meme_generator-0.0.8/meme_generator/memes/look_flat/__init__.py
--rw-r--r--   0        0        0     1176 2023-03-28 16:27:37.207658 meme_generator-0.0.8/meme_generator/memes/look_this_icon/__init__.py
--rw-r--r--   0        0        0      823 2023-03-28 16:27:37.207658 meme_generator-0.0.8/meme_generator/memes/love_you/__init__.py
--rw-r--r--   0        0        0     1072 2023-03-28 16:27:37.207658 meme_generator-0.0.8/meme_generator/memes/luoyonghao_say/__init__.py
--rw-r--r--   0        0        0      912 2023-03-28 16:27:37.211658 meme_generator-0.0.8/meme_generator/memes/luxun_say/__init__.py
--rw-r--r--   0        0        0     1384 2023-03-28 16:27:37.211658 meme_generator-0.0.8/meme_generator/memes/make_friend/__init__.py
--rw-r--r--   0        0        0      804 2023-03-28 16:27:37.211658 meme_generator-0.0.8/meme_generator/memes/marriage/__init__.py
--rw-r--r--   0        0        0      738 2023-03-28 16:27:37.211658 meme_generator-0.0.8/meme_generator/memes/meteor/__init__.py
--rw-r--r--   0        0        0      715 2023-03-28 16:27:37.215658 meme_generator-0.0.8/meme_generator/memes/murmur/__init__.py
--rw-r--r--   0        0        0     2816 2023-03-28 16:27:37.215658 meme_generator-0.0.8/meme_generator/memes/my_friend/__init__.py
--rw-r--r--   0        0        0     1452 2023-03-28 16:27:37.215658 meme_generator-0.0.8/meme_generator/memes/my_wife/__init__.py
--rw-r--r--   0        0        0     3379 2023-03-28 16:27:37.215658 meme_generator-0.0.8/meme_generator/memes/name_generator/__init__.py
--rw-r--r--   0        0        0      620 2023-03-28 16:27:37.215658 meme_generator-0.0.8/meme_generator/memes/need/__init__.py
--rw-r--r--   0        0        0      504 2023-03-28 16:27:37.215658 meme_generator-0.0.8/meme_generator/memes/no_response/__init__.py
--rw-r--r--   0        0        0     1069 2023-03-28 16:27:37.219658 meme_generator-0.0.8/meme_generator/memes/nokia/__init__.py
--rw-r--r--   0        0        0      762 2023-03-28 16:27:37.219658 meme_generator-0.0.8/meme_generator/memes/not_call_me/__init__.py
--rw-r--r--   0        0        0      518 2023-03-28 16:27:37.219658 meme_generator-0.0.8/meme_generator/memes/overtime/__init__.py
--rw-r--r--   0        0        0      512 2023-03-28 16:27:37.223658 meme_generator-0.0.8/meme_generator/memes/paint/__init__.py
--rw-r--r--   0        0        0      527 2023-03-28 16:27:37.223658 meme_generator-0.0.8/meme_generator/memes/painter/__init__.py
--rw-r--r--   0        0        0      916 2023-03-28 16:27:37.223658 meme_generator-0.0.8/meme_generator/memes/pat/__init__.py
--rw-r--r--   0        0        0      502 2023-03-28 16:27:37.223658 meme_generator-0.0.8/meme_generator/memes/perfect/__init__.py
--rw-r--r--   0        0        0     1431 2023-03-28 16:27:37.227658 meme_generator-0.0.8/meme_generator/memes/petpet/__init__.py
--rw-r--r--   0        0        0     1405 2023-03-28 16:27:37.227658 meme_generator-0.0.8/meme_generator/memes/play/__init__.py
--rw-r--r--   0        0        0     1281 2023-03-28 16:27:37.231658 meme_generator-0.0.8/meme_generator/memes/play_game/__init__.py
--rw-r--r--   0        0        0      866 2023-03-28 16:27:37.235658 meme_generator-0.0.8/meme_generator/memes/police/__init__.py
--rw-r--r--   0        0        0     1085 2023-03-28 16:27:37.235658 meme_generator-0.0.8/meme_generator/memes/pornhub/__init__.py
--rw-r--r--   0        0        0      489 2023-03-28 16:27:37.235658 meme_generator-0.0.8/meme_generator/memes/potato/__init__.py
--rw-r--r--   0        0        0      904 2023-03-28 16:27:37.239658 meme_generator-0.0.8/meme_generator/memes/pound/__init__.py
--rw-r--r--   0        0        0      806 2023-03-28 16:27:37.239658 meme_generator-0.0.8/meme_generator/memes/printing/__init__.py
--rw-r--r--   0        0        0      733 2023-03-28 16:27:37.247658 meme_generator-0.0.8/meme_generator/memes/prpr/__init__.py
--rw-r--r--   0        0        0     2676 2023-03-28 16:27:37.251658 meme_generator-0.0.8/meme_generator/memes/psyduck/__init__.py
--rw-r--r--   0        0        0      959 2023-03-28 16:27:37.251658 meme_generator-0.0.8/meme_generator/memes/punch/__init__.py
--rw-r--r--   0        0        0     1053 2023-03-28 16:27:37.255658 meme_generator-0.0.8/meme_generator/memes/raise_sign/__init__.py
--rw-r--r--   0        0        0     1840 2023-03-28 16:27:37.255658 meme_generator-0.0.8/meme_generator/memes/read_book/__init__.py
--rw-r--r--   0        0        0     2387 2023-03-28 16:27:37.263658 meme_generator-0.0.8/meme_generator/memes/repeat/__init__.py
--rw-r--r--   0        0        0      919 2023-03-28 16:27:37.263658 meme_generator-0.0.8/meme_generator/memes/rip/__init__.py
--rw-r--r--   0        0        0      586 2023-03-28 16:27:37.271659 meme_generator-0.0.8/meme_generator/memes/rip_angrily/__init__.py
--rw-r--r--   0        0        0     1188 2023-03-28 16:27:37.271659 meme_generator-0.0.8/meme_generator/memes/rise_dead/__init__.py
--rw-r--r--   0        0        0      866 2023-03-28 16:27:37.279659 meme_generator-0.0.8/meme_generator/memes/roll/__init__.py
--rw-r--r--   0        0        0     1271 2023-03-28 16:27:37.279659 meme_generator-0.0.8/meme_generator/memes/rub/__init__.py
--rw-r--r--   0        0        0      845 2023-03-28 16:27:37.279659 meme_generator-0.0.8/meme_generator/memes/run/__init__.py
--rw-r--r--   0        0        0     1213 2023-03-28 16:27:37.279659 meme_generator-0.0.8/meme_generator/memes/safe_sense/__init__.py
--rw-r--r--   0        0        0      876 2023-03-28 16:27:37.283659 meme_generator-0.0.8/meme_generator/memes/scratch_head/__init__.py
--rw-r--r--   0        0        0      890 2023-03-28 16:27:37.283659 meme_generator-0.0.8/meme_generator/memes/scratchcard/__init__.py
--rw-r--r--   0        0        0     1882 2023-03-28 16:27:37.283659 meme_generator-0.0.8/meme_generator/memes/scroll/__init__.py
--rw-r--r--   0        0        0      636 2023-03-28 16:27:37.283659 meme_generator-0.0.8/meme_generator/memes/shock/__init__.py
--rw-r--r--   0        0        0      741 2023-03-28 16:27:37.283659 meme_generator-0.0.8/meme_generator/memes/shutup/__init__.py
--rw-r--r--   0        0        0     1058 2023-03-28 16:27:37.283659 meme_generator-0.0.8/meme_generator/memes/sit_still/__init__.py
--rw-r--r--   0        0        0      671 2023-03-28 16:27:37.283659 meme_generator-0.0.8/meme_generator/memes/slap/__init__.py
--rw-r--r--   0        0        0     1096 2023-03-28 16:27:37.283659 meme_generator-0.0.8/meme_generator/memes/slogan/__init__.py
--rw-r--r--   0        0        0      722 2023-03-28 16:27:37.287659 meme_generator-0.0.8/meme_generator/memes/smash/__init__.py
--rw-r--r--   0        0        0      915 2023-03-28 16:27:37.287659 meme_generator-0.0.8/meme_generator/memes/step_on/__init__.py
--rw-r--r--   0        0        0     1061 2023-03-28 16:27:37.287659 meme_generator-0.0.8/meme_generator/memes/suck/__init__.py
--rw-r--r--   0        0        0      513 2023-03-28 16:27:37.287659 meme_generator-0.0.8/meme_generator/memes/support/__init__.py
--rw-r--r--   0        0        0     3094 2023-03-28 16:27:37.291659 meme_generator-0.0.8/meme_generator/memes/symmetric/__init__.py
--rw-r--r--   0        0        0     1770 2023-03-28 16:27:37.291659 meme_generator-0.0.8/meme_generator/memes/tankuku_raisesign/__init__.py
--rw-r--r--   0        0        0     1169 2023-03-28 16:27:37.307659 meme_generator-0.0.8/meme_generator/memes/teach/__init__.py
--rw-r--r--   0        0        0      628 2023-03-28 16:27:37.311659 meme_generator-0.0.8/meme_generator/memes/think_what/__init__.py
--rw-r--r--   0        0        0      576 2023-03-28 16:27:37.315659 meme_generator-0.0.8/meme_generator/memes/throw/__init__.py
--rw-r--r--   0        0        0      962 2023-03-28 16:27:37.315659 meme_generator-0.0.8/meme_generator/memes/throw_gif/__init__.py
--rw-r--r--   0        0        0      790 2023-03-28 16:27:37.319659 meme_generator-0.0.8/meme_generator/memes/thump/__init__.py
--rw-r--r--   0        0        0     1214 2023-03-28 16:27:37.319659 meme_generator-0.0.8/meme_generator/memes/tightly/__init__.py
--rw-r--r--   0        0        0      985 2023-03-28 16:27:37.327659 meme_generator-0.0.8/meme_generator/memes/together/__init__.py
--rw-r--r--   0        0        0      728 2023-03-28 16:27:37.327659 meme_generator-0.0.8/meme_generator/memes/trance/__init__.py
--rw-r--r--   0        0        0      661 2023-03-28 16:27:37.327659 meme_generator-0.0.8/meme_generator/memes/turn/__init__.py
--rw-r--r--   0        0        0      831 2023-03-28 16:27:37.327659 meme_generator-0.0.8/meme_generator/memes/twist/__init__.py
--rw-r--r--   0        0        0     1172 2023-03-28 16:27:37.327659 meme_generator-0.0.8/meme_generator/memes/universal/__init__.py
--rw-r--r--   0        0        0      788 2023-03-28 16:27:37.327659 meme_generator-0.0.8/meme_generator/memes/wakeup/__init__.py
--rw-r--r--   0        0        0      768 2023-03-28 16:27:37.327659 meme_generator-0.0.8/meme_generator/memes/wallpaper/__init__.py
--rw-r--r--   0        0        0      632 2023-03-28 16:27:37.343659 meme_generator-0.0.8/meme_generator/memes/walnut_pad/__init__.py
--rw-r--r--   0        0        0     1180 2023-03-28 16:27:37.347660 meme_generator-0.0.8/meme_generator/memes/walnut_zoom/__init__.py
--rw-r--r--   0        0        0     1427 2023-03-28 16:27:37.363660 meme_generator-0.0.8/meme_generator/memes/wave/__init__.py
--rw-r--r--   0        0        0      501 2023-03-28 16:27:37.363660 meme_generator-0.0.8/meme_generator/memes/why_at_me/__init__.py
--rw-r--r--   0        0        0      977 2023-03-28 16:27:37.367660 meme_generator-0.0.8/meme_generator/memes/windmill_turn/__init__.py
--rw-r--r--   0        0        0      747 2023-03-28 16:27:37.367660 meme_generator-0.0.8/meme_generator/memes/wish_fail/__init__.py
--rw-r--r--   0        0        0      573 2023-03-28 16:27:37.367660 meme_generator-0.0.8/meme_generator/memes/wooden_fish/__init__.py
--rw-r--r--   0        0        0      752 2023-03-28 16:27:37.399660 meme_generator-0.0.8/meme_generator/memes/worship/__init__.py
--rw-r--r--   0        0        0     1457 2023-03-28 16:27:37.399660 meme_generator-0.0.8/meme_generator/memes/wujing/__init__.py
--rw-r--r--   0        0        0     1971 2023-03-28 16:27:37.399660 meme_generator-0.0.8/meme_generator/memes/youtube/__init__.py
--rw-r--r--   0        0        0    13448 2023-03-28 16:27:37.399660 meme_generator-0.0.8/meme_generator/utils.py
--rw-r--r--   0        0        0       22 2023-03-28 16:27:37.399660 meme_generator-0.0.8/meme_generator/version.py
--rw-r--r--   0        0        0      957 2023-03-28 16:27:37.399660 meme_generator-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    10614 1970-01-01 00:00:00.000000 meme_generator-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-31 05:46:15.609802 meme_generator-0.0.9/LICENSE
+-rw-r--r--   0        0        0    10129 2023-03-31 05:46:15.609802 meme_generator-0.0.9/README.md
+-rw-r--r--   0        0        0      998 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/__init__.py
+-rw-r--r--   0        0        0     7005 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/app.py
+-rw-r--r--   0        0        0     6529 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/cli.py
+-rw-r--r--   0        0        0     1363 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/config.py
+-rw-r--r--   0        0        0     8303 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/dirs.py
+-rw-r--r--   0        0        0     2272 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/download.py
+-rw-r--r--   0        0        0     3446 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/exception.py
+-rw-r--r--   0        0        0      131 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/log.py
+-rw-r--r--   0        0        0     2777 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/manager.py
+-rw-r--r--   0        0        0     5616 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/meme.py
+-rw-r--r--   0        0        0     5138 2023-03-31 05:46:15.981804 meme_generator-0.0.9/meme_generator/memes/5000choyen/__init__.py
+-rw-r--r--   0        0        0     1127 2023-03-31 05:46:15.985804 meme_generator-0.0.9/meme_generator/memes/acg_entrance/__init__.py
+-rw-r--r--   0        0        0     1025 2023-03-31 05:46:15.985804 meme_generator-0.0.9/meme_generator/memes/addiction/__init__.py
+-rw-r--r--   0        0        0      775 2023-03-31 05:46:15.985804 meme_generator-0.0.9/meme_generator/memes/alike/__init__.py
+-rw-r--r--   0        0        0     3505 2023-03-31 05:46:15.985804 meme_generator-0.0.9/meme_generator/memes/always/__init__.py
+-rw-r--r--   0        0        0     2768 2023-03-31 05:46:15.985804 meme_generator-0.0.9/meme_generator/memes/always_like/__init__.py
+-rw-r--r--   0        0        0      503 2023-03-31 05:46:15.985804 meme_generator-0.0.9/meme_generator/memes/anti_kidnap/__init__.py
+-rw-r--r--   0        0        0     1166 2023-03-31 05:46:15.993805 meme_generator-0.0.9/meme_generator/memes/anya_suki/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 05:46:15.993805 meme_generator-0.0.9/meme_generator/memes/applaud/__init__.py
+-rw-r--r--   0        0        0      845 2023-03-31 05:46:15.993805 meme_generator-0.0.9/meme_generator/memes/ascension/__init__.py
+-rw-r--r--   0        0        0     2570 2023-03-31 05:46:15.997804 meme_generator-0.0.9/meme_generator/memes/ask/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-31 05:46:15.997804 meme_generator-0.0.9/meme_generator/memes/back_to_work/__init__.py
+-rw-r--r--   0        0        0      888 2023-03-31 05:46:16.001805 meme_generator-0.0.9/meme_generator/memes/bad_news/__init__.py
+-rw-r--r--   0        0        0     1252 2023-03-31 05:46:16.001805 meme_generator-0.0.9/meme_generator/memes/beat_head/__init__.py
+-rw-r--r--   0        0        0      966 2023-03-31 05:46:16.001805 meme_generator-0.0.9/meme_generator/memes/bite/__init__.py
+-rw-r--r--   0        0        0      640 2023-03-31 05:46:16.005805 meme_generator-0.0.9/meme_generator/memes/blood_pressure/__init__.py
+-rw-r--r--   0        0        0     1611 2023-03-31 05:46:16.009805 meme_generator-0.0.9/meme_generator/memes/bocchi_draft/__init__.py
+-rw-r--r--   0        0        0      851 2023-03-31 05:46:16.037805 meme_generator-0.0.9/meme_generator/memes/bronya_holdsign/__init__.py
+-rw-r--r--   0        0        0     1678 2023-03-31 05:46:16.037805 meme_generator-0.0.9/meme_generator/memes/bubble_tea/__init__.py
+-rw-r--r--   0        0        0      679 2023-03-31 05:46:16.041805 meme_generator-0.0.9/meme_generator/memes/call_110/__init__.py
+-rw-r--r--   0        0        0     1258 2023-03-31 05:46:16.041805 meme_generator-0.0.9/meme_generator/memes/capoo_draw/__init__.py
+-rw-r--r--   0        0        0      857 2023-03-31 05:46:16.041805 meme_generator-0.0.9/meme_generator/memes/capoo_rub/__init__.py
+-rw-r--r--   0        0        0     1614 2023-03-31 05:46:16.041805 meme_generator-0.0.9/meme_generator/memes/capoo_say/__init__.py
+-rw-r--r--   0        0        0     1371 2023-03-31 05:46:16.041805 meme_generator-0.0.9/meme_generator/memes/capoo_strike/__init__.py
+-rw-r--r--   0        0        0      871 2023-03-31 05:46:16.045805 meme_generator-0.0.9/meme_generator/memes/captain/__init__.py
+-rw-r--r--   0        0        0     1211 2023-03-31 05:46:16.045805 meme_generator-0.0.9/meme_generator/memes/charpic/__init__.py
+-rw-r--r--   0        0        0     3233 2023-03-31 05:46:16.045805 meme_generator-0.0.9/meme_generator/memes/chase_train/__init__.py
+-rw-r--r--   0        0        0      487 2023-03-31 05:46:16.061805 meme_generator-0.0.9/meme_generator/memes/china_flag/__init__.py
+-rw-r--r--   0        0        0      973 2023-03-31 05:46:16.061805 meme_generator-0.0.9/meme_generator/memes/confuse/__init__.py
+-rw-r--r--   0        0        0     1188 2023-03-31 05:46:16.073805 meme_generator-0.0.9/meme_generator/memes/coupon/__init__.py
+-rw-r--r--   0        0        0      567 2023-03-31 05:46:16.073805 meme_generator-0.0.9/meme_generator/memes/cover_face/__init__.py
+-rw-r--r--   0        0        0     1000 2023-03-31 05:46:16.073805 meme_generator-0.0.9/meme_generator/memes/crawl/__init__.py
+-rw-r--r--   0        0        0      749 2023-03-31 05:46:16.125805 meme_generator-0.0.9/meme_generator/memes/cyan/__init__.py
+-rw-r--r--   0        0        0      508 2023-03-31 05:46:16.125805 meme_generator-0.0.9/meme_generator/memes/decent_kiss/__init__.py
+-rw-r--r--   0        0        0     1710 2023-03-31 05:46:16.129805 meme_generator-0.0.9/meme_generator/memes/dianzhongdian/__init__.py
+-rw-r--r--   0        0        0      634 2023-03-31 05:46:16.129805 meme_generator-0.0.9/meme_generator/memes/dinosaur/__init__.py
+-rw-r--r--   0        0        0      700 2023-03-31 05:46:16.133806 meme_generator-0.0.9/meme_generator/memes/distracted/__init__.py
+-rw-r--r--   0        0        0      500 2023-03-31 05:46:16.133806 meme_generator-0.0.9/meme_generator/memes/divorce/__init__.py
+-rw-r--r--   0        0        0      632 2023-03-31 05:46:16.137806 meme_generator-0.0.9/meme_generator/memes/dont_touch/__init__.py
+-rw-r--r--   0        0        0     2342 2023-03-31 05:46:16.137806 meme_generator-0.0.9/meme_generator/memes/douyin/__init__.py
+-rw-r--r--   0        0        0      595 2023-03-31 05:46:16.137806 meme_generator-0.0.9/meme_generator/memes/eat/__init__.py
+-rw-r--r--   0        0        0      776 2023-03-31 05:46:16.137806 meme_generator-0.0.9/meme_generator/memes/fanatic/__init__.py
+-rw-r--r--   0        0        0     1273 2023-03-31 05:46:16.141806 meme_generator-0.0.9/meme_generator/memes/fencing/__init__.py
+-rw-r--r--   0        0        0     1101 2023-03-31 05:46:16.141806 meme_generator-0.0.9/meme_generator/memes/find_chips/__init__.py
+-rw-r--r--   0        0        0     1269 2023-03-31 05:46:16.141806 meme_generator-0.0.9/meme_generator/memes/follow/__init__.py
+-rw-r--r--   0        0        0      829 2023-03-31 05:46:16.141806 meme_generator-0.0.9/meme_generator/memes/funny_mirror/__init__.py
+-rw-r--r--   0        0        0      903 2023-03-31 05:46:16.141806 meme_generator-0.0.9/meme_generator/memes/garbage/__init__.py
+-rw-r--r--   0        0        0     4141 2023-03-31 05:46:16.153806 meme_generator-0.0.9/meme_generator/memes/gif_subtitle/__init__.py
+-rw-r--r--   0        0        0      901 2023-03-31 05:46:16.213806 meme_generator-0.0.9/meme_generator/memes/good_news/__init__.py
+-rw-r--r--   0        0        0      697 2023-03-31 05:46:16.213806 meme_generator-0.0.9/meme_generator/memes/google/__init__.py
+-rw-r--r--   0        0        0     1631 2023-03-31 05:46:16.213806 meme_generator-0.0.9/meme_generator/memes/gun/__init__.py
+-rw-r--r--   0        0        0      886 2023-03-31 05:46:16.213806 meme_generator-0.0.9/meme_generator/memes/hammer/__init__.py
+-rw-r--r--   0        0        0     1094 2023-03-31 05:46:16.213806 meme_generator-0.0.9/meme_generator/memes/high_EQ/__init__.py
+-rw-r--r--   0        0        0     1950 2023-03-31 05:46:16.213806 meme_generator-0.0.9/meme_generator/memes/hit_screen/__init__.py
+-rw-r--r--   0        0        0     1050 2023-03-31 05:46:16.221806 meme_generator-0.0.9/meme_generator/memes/hold_grudge/__init__.py
+-rw-r--r--   0        0        0      499 2023-03-31 05:46:16.221806 meme_generator-0.0.9/meme_generator/memes/hold_tight/__init__.py
+-rw-r--r--   0        0        0      862 2023-03-31 05:46:16.221806 meme_generator-0.0.9/meme_generator/memes/hug_leg/__init__.py
+-rw-r--r--   0        0        0      766 2023-03-31 05:46:16.225806 meme_generator-0.0.9/meme_generator/memes/hutao_bite/__init__.py
+-rw-r--r--   0        0        0      753 2023-03-31 05:46:16.225806 meme_generator-0.0.9/meme_generator/memes/imprison/__init__.py
+-rw-r--r--   0        0        0     1192 2023-03-31 05:46:16.225806 meme_generator-0.0.9/meme_generator/memes/incivilization/__init__.py
+-rw-r--r--   0        0        0     1285 2023-03-31 05:46:16.229806 meme_generator-0.0.9/meme_generator/memes/interview/__init__.py
+-rw-r--r--   0        0        0     2926 2023-03-31 05:46:16.229806 meme_generator-0.0.9/meme_generator/memes/jiji_king/__init__.py
+-rw-r--r--   0        0        0      652 2023-03-31 05:46:16.229806 meme_generator-0.0.9/meme_generator/memes/jiujiu/__init__.py
+-rw-r--r--   0        0        0     1769 2023-03-31 05:46:16.229806 meme_generator-0.0.9/meme_generator/memes/kaleidoscope/__init__.py
+-rw-r--r--   0        0        0      512 2023-03-31 05:46:16.229806 meme_generator-0.0.9/meme_generator/memes/karyl_point/__init__.py
+-rw-r--r--   0        0        0     1353 2023-03-31 05:46:16.233806 meme_generator-0.0.9/meme_generator/memes/keep_away/__init__.py
+-rw-r--r--   0        0        0      910 2023-03-31 05:46:16.233806 meme_generator-0.0.9/meme_generator/memes/kick_ball/__init__.py
+-rw-r--r--   0        0        0     1995 2023-03-31 05:46:16.237806 meme_generator-0.0.9/meme_generator/memes/kirby_hammer/__init__.py
+-rw-r--r--   0        0        0     1179 2023-03-31 05:46:16.277807 meme_generator-0.0.9/meme_generator/memes/kiss/__init__.py
+-rw-r--r--   0        0        0     1089 2023-03-31 05:46:16.277807 meme_generator-0.0.9/meme_generator/memes/klee_eat/__init__.py
+-rw-r--r--   0        0        0      894 2023-03-31 05:46:16.281807 meme_generator-0.0.9/meme_generator/memes/knock/__init__.py
+-rw-r--r--   0        0        0     1099 2023-03-31 05:46:16.289807 meme_generator-0.0.9/meme_generator/memes/learn/__init__.py
+-rw-r--r--   0        0        0     1268 2023-03-31 05:46:16.293807 meme_generator-0.0.9/meme_generator/memes/lim_x_0/__init__.py
+-rw-r--r--   0        0        0      724 2023-03-31 05:46:16.293807 meme_generator-0.0.9/meme_generator/memes/listen_music/__init__.py
+-rw-r--r--   0        0        0     1599 2023-03-31 05:46:16.293807 meme_generator-0.0.9/meme_generator/memes/little_angel/__init__.py
+-rw-r--r--   0        0        0     1262 2023-03-31 05:46:16.293807 meme_generator-0.0.9/meme_generator/memes/loading/__init__.py
+-rw-r--r--   0        0        0     1599 2023-03-31 05:46:16.293807 meme_generator-0.0.9/meme_generator/memes/look_flat/__init__.py
+-rw-r--r--   0        0        0     1176 2023-03-31 05:46:16.293807 meme_generator-0.0.9/meme_generator/memes/look_this_icon/__init__.py
+-rw-r--r--   0        0        0      823 2023-03-31 05:46:16.297807 meme_generator-0.0.9/meme_generator/memes/love_you/__init__.py
+-rw-r--r--   0        0        0     1072 2023-03-31 05:46:16.297807 meme_generator-0.0.9/meme_generator/memes/luoyonghao_say/__init__.py
+-rw-r--r--   0        0        0      912 2023-03-31 05:46:16.297807 meme_generator-0.0.9/meme_generator/memes/luxun_say/__init__.py
+-rw-r--r--   0        0        0     1384 2023-03-31 05:46:16.297807 meme_generator-0.0.9/meme_generator/memes/make_friend/__init__.py
+-rw-r--r--   0        0        0      804 2023-03-31 05:46:16.297807 meme_generator-0.0.9/meme_generator/memes/marriage/__init__.py
+-rw-r--r--   0        0        0      738 2023-03-31 05:46:16.301807 meme_generator-0.0.9/meme_generator/memes/meteor/__init__.py
+-rw-r--r--   0        0        0      715 2023-03-31 05:46:16.301807 meme_generator-0.0.9/meme_generator/memes/murmur/__init__.py
+-rw-r--r--   0        0        0     2816 2023-03-31 05:46:16.301807 meme_generator-0.0.9/meme_generator/memes/my_friend/__init__.py
+-rw-r--r--   0        0        0     1452 2023-03-31 05:46:16.301807 meme_generator-0.0.9/meme_generator/memes/my_wife/__init__.py
+-rw-r--r--   0        0        0     3379 2023-03-31 05:46:16.305807 meme_generator-0.0.9/meme_generator/memes/name_generator/__init__.py
+-rw-r--r--   0        0        0      620 2023-03-31 05:46:16.305807 meme_generator-0.0.9/meme_generator/memes/need/__init__.py
+-rw-r--r--   0        0        0      884 2023-03-31 05:46:16.305807 meme_generator-0.0.9/meme_generator/memes/nekoha_holdsign/__init__.py
+-rw-r--r--   0        0        0      504 2023-03-31 05:46:16.305807 meme_generator-0.0.9/meme_generator/memes/no_response/__init__.py
+-rw-r--r--   0        0        0     1069 2023-03-31 05:46:16.309807 meme_generator-0.0.9/meme_generator/memes/nokia/__init__.py
+-rw-r--r--   0        0        0      762 2023-03-31 05:46:16.309807 meme_generator-0.0.9/meme_generator/memes/not_call_me/__init__.py
+-rw-r--r--   0        0        0      518 2023-03-31 05:46:16.309807 meme_generator-0.0.9/meme_generator/memes/overtime/__init__.py
+-rw-r--r--   0        0        0      512 2023-03-31 05:46:16.313807 meme_generator-0.0.9/meme_generator/memes/paint/__init__.py
+-rw-r--r--   0        0        0      527 2023-03-31 05:46:16.313807 meme_generator-0.0.9/meme_generator/memes/painter/__init__.py
+-rw-r--r--   0        0        0     1194 2023-03-31 05:46:16.313807 meme_generator-0.0.9/meme_generator/memes/pass_the_buck/__init__.py
+-rw-r--r--   0        0        0      916 2023-03-31 05:46:16.313807 meme_generator-0.0.9/meme_generator/memes/pat/__init__.py
+-rw-r--r--   0        0        0      502 2023-03-31 05:46:16.317807 meme_generator-0.0.9/meme_generator/memes/perfect/__init__.py
+-rw-r--r--   0        0        0     1431 2023-03-31 05:46:16.317807 meme_generator-0.0.9/meme_generator/memes/petpet/__init__.py
+-rw-r--r--   0        0        0     1405 2023-03-31 05:46:16.317807 meme_generator-0.0.9/meme_generator/memes/play/__init__.py
+-rw-r--r--   0        0        0     1281 2023-03-31 05:46:16.325807 meme_generator-0.0.9/meme_generator/memes/play_game/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-31 05:46:16.325807 meme_generator-0.0.9/meme_generator/memes/police/__init__.py
+-rw-r--r--   0        0        0     1085 2023-03-31 05:46:16.329807 meme_generator-0.0.9/meme_generator/memes/pornhub/__init__.py
+-rw-r--r--   0        0        0      489 2023-03-31 05:46:16.329807 meme_generator-0.0.9/meme_generator/memes/potato/__init__.py
+-rw-r--r--   0        0        0      904 2023-03-31 05:46:16.329807 meme_generator-0.0.9/meme_generator/memes/pound/__init__.py
+-rw-r--r--   0        0        0      806 2023-03-31 05:46:16.329807 meme_generator-0.0.9/meme_generator/memes/printing/__init__.py
+-rw-r--r--   0        0        0      733 2023-03-31 05:46:16.341807 meme_generator-0.0.9/meme_generator/memes/prpr/__init__.py
+-rw-r--r--   0        0        0     2676 2023-03-31 05:46:16.341807 meme_generator-0.0.9/meme_generator/memes/psyduck/__init__.py
+-rw-r--r--   0        0        0      959 2023-03-31 05:46:16.345807 meme_generator-0.0.9/meme_generator/memes/punch/__init__.py
+-rw-r--r--   0        0        0     1053 2023-03-31 05:46:16.349807 meme_generator-0.0.9/meme_generator/memes/raise_sign/__init__.py
+-rw-r--r--   0        0        0     1840 2023-03-31 05:46:16.349807 meme_generator-0.0.9/meme_generator/memes/read_book/__init__.py
+-rw-r--r--   0        0        0     2387 2023-03-31 05:46:16.357807 meme_generator-0.0.9/meme_generator/memes/repeat/__init__.py
+-rw-r--r--   0        0        0      919 2023-03-31 05:46:16.357807 meme_generator-0.0.9/meme_generator/memes/rip/__init__.py
+-rw-r--r--   0        0        0      586 2023-03-31 05:46:16.365807 meme_generator-0.0.9/meme_generator/memes/rip_angrily/__init__.py
+-rw-r--r--   0        0        0     1188 2023-03-31 05:46:16.365807 meme_generator-0.0.9/meme_generator/memes/rise_dead/__init__.py
+-rw-r--r--   0        0        0      866 2023-03-31 05:46:16.373807 meme_generator-0.0.9/meme_generator/memes/roll/__init__.py
+-rw-r--r--   0        0        0     1271 2023-03-31 05:46:16.373807 meme_generator-0.0.9/meme_generator/memes/rub/__init__.py
+-rw-r--r--   0        0        0      845 2023-03-31 05:46:16.373807 meme_generator-0.0.9/meme_generator/memes/run/__init__.py
+-rw-r--r--   0        0        0     1213 2023-03-31 05:46:16.377807 meme_generator-0.0.9/meme_generator/memes/safe_sense/__init__.py
+-rw-r--r--   0        0        0      876 2023-03-31 05:46:16.377807 meme_generator-0.0.9/meme_generator/memes/scratch_head/__init__.py
+-rw-r--r--   0        0        0      890 2023-03-31 05:46:16.377807 meme_generator-0.0.9/meme_generator/memes/scratchcard/__init__.py
+-rw-r--r--   0        0        0     1882 2023-03-31 05:46:16.377807 meme_generator-0.0.9/meme_generator/memes/scroll/__init__.py
+-rw-r--r--   0        0        0      636 2023-03-31 05:46:16.377807 meme_generator-0.0.9/meme_generator/memes/shock/__init__.py
+-rw-r--r--   0        0        0      741 2023-03-31 05:46:16.377807 meme_generator-0.0.9/meme_generator/memes/shutup/__init__.py
+-rw-r--r--   0        0        0     1058 2023-03-31 05:46:16.377807 meme_generator-0.0.9/meme_generator/memes/sit_still/__init__.py
+-rw-r--r--   0        0        0      671 2023-03-31 05:46:16.381807 meme_generator-0.0.9/meme_generator/memes/slap/__init__.py
+-rw-r--r--   0        0        0     1096 2023-03-31 05:46:16.381807 meme_generator-0.0.9/meme_generator/memes/slogan/__init__.py
+-rw-r--r--   0        0        0      722 2023-03-31 05:46:16.381807 meme_generator-0.0.9/meme_generator/memes/smash/__init__.py
+-rw-r--r--   0        0        0      915 2023-03-31 05:46:16.381807 meme_generator-0.0.9/meme_generator/memes/step_on/__init__.py
+-rw-r--r--   0        0        0     1061 2023-03-31 05:46:16.385807 meme_generator-0.0.9/meme_generator/memes/suck/__init__.py
+-rw-r--r--   0        0        0      513 2023-03-31 05:46:16.385807 meme_generator-0.0.9/meme_generator/memes/support/__init__.py
+-rw-r--r--   0        0        0     3094 2023-03-31 05:46:16.389807 meme_generator-0.0.9/meme_generator/memes/symmetric/__init__.py
+-rw-r--r--   0        0        0     1770 2023-03-31 05:46:16.389807 meme_generator-0.0.9/meme_generator/memes/tankuku_raisesign/__init__.py
+-rw-r--r--   0        0        0     1169 2023-03-31 05:46:16.405808 meme_generator-0.0.9/meme_generator/memes/teach/__init__.py
+-rw-r--r--   0        0        0      628 2023-03-31 05:46:16.409808 meme_generator-0.0.9/meme_generator/memes/think_what/__init__.py
+-rw-r--r--   0        0        0      576 2023-03-31 05:46:16.413807 meme_generator-0.0.9/meme_generator/memes/throw/__init__.py
+-rw-r--r--   0        0        0      962 2023-03-31 05:46:16.413807 meme_generator-0.0.9/meme_generator/memes/throw_gif/__init__.py
+-rw-r--r--   0        0        0      790 2023-03-31 05:46:16.417808 meme_generator-0.0.9/meme_generator/memes/thump/__init__.py
+-rw-r--r--   0        0        0      795 2023-03-31 05:46:16.417808 meme_generator-0.0.9/meme_generator/memes/thump_wildly/__init__.py
+-rw-r--r--   0        0        0     1214 2023-03-31 05:46:16.425808 meme_generator-0.0.9/meme_generator/memes/tightly/__init__.py
+-rw-r--r--   0        0        0     1156 2023-03-31 05:46:16.433808 meme_generator-0.0.9/meme_generator/memes/together/__init__.py
+-rw-r--r--   0        0        0      728 2023-03-31 05:46:16.433808 meme_generator-0.0.9/meme_generator/memes/trance/__init__.py
+-rw-r--r--   0        0        0      661 2023-03-31 05:46:16.433808 meme_generator-0.0.9/meme_generator/memes/turn/__init__.py
+-rw-r--r--   0        0        0      831 2023-03-31 05:46:16.433808 meme_generator-0.0.9/meme_generator/memes/twist/__init__.py
+-rw-r--r--   0        0        0     1172 2023-03-31 05:46:16.433808 meme_generator-0.0.9/meme_generator/memes/universal/__init__.py
+-rw-r--r--   0        0        0      788 2023-03-31 05:46:16.433808 meme_generator-0.0.9/meme_generator/memes/wakeup/__init__.py
+-rw-r--r--   0        0        0      768 2023-03-31 05:46:16.433808 meme_generator-0.0.9/meme_generator/memes/wallpaper/__init__.py
+-rw-r--r--   0        0        0      632 2023-03-31 05:46:16.453808 meme_generator-0.0.9/meme_generator/memes/walnut_pad/__init__.py
+-rw-r--r--   0        0        0     1180 2023-03-31 05:46:16.453808 meme_generator-0.0.9/meme_generator/memes/walnut_zoom/__init__.py
+-rw-r--r--   0        0        0     1427 2023-03-31 05:46:16.477808 meme_generator-0.0.9/meme_generator/memes/wave/__init__.py
+-rw-r--r--   0        0        0      501 2023-03-31 05:46:16.477808 meme_generator-0.0.9/meme_generator/memes/why_at_me/__init__.py
+-rw-r--r--   0        0        0      977 2023-03-31 05:46:16.477808 meme_generator-0.0.9/meme_generator/memes/windmill_turn/__init__.py
+-rw-r--r--   0        0        0      747 2023-03-31 05:46:16.477808 meme_generator-0.0.9/meme_generator/memes/wish_fail/__init__.py
+-rw-r--r--   0        0        0      573 2023-03-31 05:46:16.477808 meme_generator-0.0.9/meme_generator/memes/wooden_fish/__init__.py
+-rw-r--r--   0        0        0      752 2023-03-31 05:46:16.513808 meme_generator-0.0.9/meme_generator/memes/worship/__init__.py
+-rw-r--r--   0        0        0     1457 2023-03-31 05:46:16.517808 meme_generator-0.0.9/meme_generator/memes/wujing/__init__.py
+-rw-r--r--   0        0        0     1971 2023-03-31 05:46:16.517808 meme_generator-0.0.9/meme_generator/memes/youtube/__init__.py
+-rw-r--r--   0        0        0    13448 2023-03-31 05:46:16.517808 meme_generator-0.0.9/meme_generator/utils.py
+-rw-r--r--   0        0        0       22 2023-03-31 05:46:16.517808 meme_generator-0.0.9/meme_generator/version.py
+-rw-r--r--   0        0        0      957 2023-03-31 05:46:16.517808 meme_generator-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11194 1970-01-01 00:00:00.000000 meme_generator-0.0.9/PKG-INFO
```

### Comparing `meme_generator-0.0.8/LICENSE` & `meme_generator-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/README.md` & `meme_generator-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 也可以调用 `meme_generator/download.py` 中的 `check_resources` 函数进行下载
 
 
 ### 字体安装
 
 为确保表情包中的文字生成正常，需要自行安装字体
 
+> **Note**
+>
 > 字体安装后若文字仍显示不正常，可删掉 `matplotlib` 字体缓存文件重新运行程序
 >
 > 缓存文件位置：
 > - Windows: `C:\Users\<username>\.matplotlib\fontlist-xxx.json`
 > - Linux: `~/.cache/matplotlib/fontlist-xxx.json`
 > - Mac: `~/Library/Caches/matplotlib/fontlist-xxx.json`
 
@@ -103,14 +105,15 @@
 某些表情包需要用到一些额外字体，存放于仓库中 [resources/fonts](https://github.com/MeetWq/meme-generator/tree/main/resources/fonts)，需要自行下载安装
 
 具体字体及对应的表情如下：
 
 | 字体名 | 字体文件名 | 用到该字体的表情 | 备注 |
 | --- | --- | --- | --- |
 | [Consolas](https://learn.microsoft.com/zh-cn/typography/font-list/consolas) | [consola.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/consola.ttf) | `charpic` |  |
+| [FZKaTong-M19S](https://www.foundertype.com/index.php/FontInfo/index/id/136) | [FZKATJW.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZKATJW.ttf) | `capoo_say` | 方正卡通 |
 | [FZXS14](https://www.foundertype.com/index.php/FontInfo/index/id/208) | [FZXS14.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZXS14.ttf) | `nokia` | 方正像素14 |
 | [FZSJ-QINGCRJ](https://www.foundertype.com/index.php/FontInfo/index/id/5178) | [FZSJ-QINGCRJ.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZSJ-QINGCRJ.ttf) | `psyduck` | 方正手迹-青春日记 |
 | [FZShaoEr-M11S](https://www.foundertype.com/index.php/FontInfo/index/id/149) | [FZSEJW.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZSEJW.ttf) | `raise_sign` | 方正少儿 |
 | [NotoSansSC](https://fonts.google.com/noto/specimen/Noto+Sans+SC) | [NotoSansSC-Regular.otf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/NotoSansSC-Regular.otf) | `5000choyen` |  |
 | [NotoSerifSC](https://fonts.google.com/noto/specimen/Noto+Serif+SC) | [NotoSerifSC-Regular.otf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/NotoSerifSC-Regular.otf) | `5000choyen` |  |
 
 
@@ -179,14 +182,22 @@
 
 默认配置文件位置：
 
 - Windows: `C:\Users\<username>\AppData\Roaming\meme_generator\config.toml`
 - Linux: `~/.config/meme_generator/config.toml`
 - Mac: `~/Library/Application Support/meme_generator/config.toml`
 
+> **Warning**
+>
+> 从 v0.0.6 版本开始，不再生成默认配置文件；修改配置时需在对应的文件位置自行创建配置文件
+>
+> 由于 v0.0.6 版本更改了资源链接的拼接方式，如果装过之前的版本，需要修改配置中的 `resource_url`
+>
+> 建议将配置文件中不需要更改的选项删除，以使用默认配置
+
 默认配置：
 ```toml
 [meme]
 load_builtin_memes = true  # 是否加载内置表情包
 meme_dirs = []  # 加载其他位置的表情包，填写文件夹路径
 meme_disabled_list = []  # 禁用的表情包列表，填写表情的 `key`
```

#### html2text {}

```diff
@@ -5,19 +5,19 @@
 <--](docs/memes.md) æ¥ç ## å®è£ ä½¿ç¨ pip å®è£ ```bash pip install
 meme_generator ``` ### å¾çä¸è½½ ç±äºè¡¨æåå¾çä½ç§¯è¾å¤§ï¼`meme-
 generator`
 åå«çè¡¨æä¸­çå¾çå¹¶ä¸éä»£ç ä¸èµ·æåï¼éè¦å¨å®è£åæå¨æ§è¡ä¸è½½å½ä»¤ï¼
 ``` meme download ``` ä¹å¯ä»¥è°ç¨ `meme_generator/download.py` ä¸­ç
 `check_resources` å½æ°è¿è¡ä¸è½½ ### å­ä½å®è£
 ä¸ºç¡®ä¿è¡¨æåä¸­çæå­çææ­£å¸¸ï¼éè¦èªè¡å®è£å­ä½ >
-å­ä½å®è£åè¥æå­ä»æ¾ç¤ºä¸æ­£å¸¸ï¼å¯å æ `matplotlib`
-å­ä½ç¼å­æä»¶éæ°è¿è¡ç¨åº > > ç¼å­æä»¶ä½ç½®ï¼ > - Windows: `C:
-\Users\\.matplotlib\fontlist-xxx.json` > - Linux: `~/.cache/matplotlib/
-fontlist-xxx.json` > - Mac: `~/Library/Caches/matplotlib/fontlist-xxx.json`
-#### ä¸­æå­ä½ å emojiå­ä½ å®è£
+**Note** > > å­ä½å®è£åè¥æå­ä»æ¾ç¤ºä¸æ­£å¸¸ï¼å¯å æ
+`matplotlib` å­ä½ç¼å­æä»¶éæ°è¿è¡ç¨åº > > ç¼å­æä»¶ä½ç½®ï¼ > -
+Windows: `C:\Users\\.matplotlib\fontlist-xxx.json` > - Linux: `~/.cache/
+matplotlib/fontlist-xxx.json` > - Mac: `~/Library/Caches/matplotlib/fontlist-
+xxx.json` #### ä¸­æå­ä½ å emojiå­ä½ å®è£
 æ ¹æ®ç³»ç»çä¸åï¼æ¨èå®è£çå­ä½å¦ä¸ï¼ - Windows: å¤§é¨å
 Windows ç³»ç»èªå¸¦ [å¾®è½¯éé»](https://learn.microsoft.com/zh-cn/
 typography/font-list/microsoft-yahei) ä¸­æå­ä½ å [Segoe UI Emoji](https:/
 /learn.microsoft.com/zh-cn/typography/font-list/segoe-ui-emoji) emoji
 å­ä½ï¼ä¸è¬æåµä¸æ éé¢å¤å®è£ - Linux: é¨åç³»ç»å¯è½èªå¸¦
 [ææ³é©¿å¾®ç±³é»](http://wenq.org/wqy2/index.cgi?MicroHei) ä¸­æå­ä½ï¼
 å¯¹äº Ubuntu ç³»ç»ï¼æ¨èå®è£ Noto Sans CJK å Noto Color Emojiï¼
@@ -35,31 +35,33 @@
 "Apple Color Emoji" emoji å­ä½ #### å¶ä»å­ä½å®è£
 æäºè¡¨æåéè¦ç¨å°ä¸äºé¢å¤å­ä½ï¼å­æ¾äºä»åºä¸­ [resources/
 fonts](https://github.com/MeetWq/meme-generator/tree/main/resources/
 fonts)ï¼éè¦èªè¡ä¸è½½å®è£ å·ä½å­ä½åå¯¹åºçè¡¨æå¦ä¸ï¼ |
 å­ä½å | å­ä½æä»¶å | ç¨å°è¯¥å­ä½çè¡¨æ | å¤æ³¨ | | --- | --- |
 --- | --- | | [Consolas](https://learn.microsoft.com/zh-cn/typography/font-
 list/consolas) | [consola.ttf](https://github.com/MeetWq/meme-generator/blob/
-main/resources/fonts/consola.ttf) | `charpic` | | | [FZXS14](https://
-www.foundertype.com/index.php/FontInfo/index/id/208) | [FZXS14.ttf](https://
-github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZXS14.ttf) |
-`nokia` | æ¹æ­£åç´ 14 | | [FZSJ-QINGCRJ](https://www.foundertype.com/
-index.php/FontInfo/index/id/5178) | [FZSJ-QINGCRJ.ttf](https://github.com/
-MeetWq/meme-generator/blob/main/resources/fonts/FZSJ-QINGCRJ.ttf) | `psyduck` |
-æ¹æ­£æè¿¹-éæ¥æ¥è®° | | [FZShaoEr-M11S](https://www.foundertype.com/
-index.php/FontInfo/index/id/149) | [FZSEJW.ttf](https://github.com/MeetWq/meme-
-generator/blob/main/resources/fonts/FZSEJW.ttf) | `raise_sign` | æ¹æ­£å°å¿ |
-| [NotoSansSC](https://fonts.google.com/noto/specimen/Noto+Sans+SC) |
-[NotoSansSC-Regular.otf](https://github.com/MeetWq/meme-generator/blob/main/
-resources/fonts/NotoSansSC-Regular.otf) | `5000choyen` | | | [NotoSerifSC]
-(https://fonts.google.com/noto/specimen/Noto+Serif+SC) | [NotoSerifSC-
-Regular.otf](https://github.com/MeetWq/meme-generator/blob/main/resources/
-fonts/NotoSerifSC-Regular.otf) | `5000choyen` | | #### å­ä½å®è£æ¹å¼
-ä¸åç³»ç»çå­ä½å®è£æ¹å¼ï¼ - Windows: -
-åå»éè¿å­ä½æ¥çå¨å®è£ - å¤å¶å°å­ä½æä»¶å¤¹ï¼`C:
+main/resources/fonts/consola.ttf) | `charpic` | | | [FZKaTong-M19S](https://
+www.foundertype.com/index.php/FontInfo/index/id/136) | [FZKATJW.ttf](https://
+github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZKATJW.ttf) |
+`capoo_say` | æ¹æ­£å¡é | | [FZXS14](https://www.foundertype.com/index.php/
+FontInfo/index/id/208) | [FZXS14.ttf](https://github.com/MeetWq/meme-generator/
+blob/main/resources/fonts/FZXS14.ttf) | `nokia` | æ¹æ­£åç´ 14 | | [FZSJ-
+QINGCRJ](https://www.foundertype.com/index.php/FontInfo/index/id/5178) | [FZSJ-
+QINGCRJ.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/
+fonts/FZSJ-QINGCRJ.ttf) | `psyduck` | æ¹æ­£æè¿¹-éæ¥æ¥è®° | | [FZShaoEr-
+M11S](https://www.foundertype.com/index.php/FontInfo/index/id/149) |
+[FZSEJW.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/
+fonts/FZSEJW.ttf) | `raise_sign` | æ¹æ­£å°å¿ | | [NotoSansSC](https://
+fonts.google.com/noto/specimen/Noto+Sans+SC) | [NotoSansSC-Regular.otf](https:/
+/github.com/MeetWq/meme-generator/blob/main/resources/fonts/NotoSansSC-
+Regular.otf) | `5000choyen` | | | [NotoSerifSC](https://fonts.google.com/noto/
+specimen/Noto+Serif+SC) | [NotoSerifSC-Regular.otf](https://github.com/MeetWq/
+meme-generator/blob/main/resources/fonts/NotoSerifSC-Regular.otf) |
+`5000choyen` | | #### å­ä½å®è£æ¹å¼ ä¸åç³»ç»çå­ä½å®è£æ¹å¼ï¼ -
+Windows: - åå»éè¿å­ä½æ¥çå¨å®è£ - å¤å¶å°å­ä½æä»¶å¤¹ï¼`C:
 \Windows\Fonts` - Linux: å¨ `/usr/share/fonts` ç®å½ä¸æ°å»ºæä»¶å¤¹ï¼å¦
 `myfonts`ï¼å°å­ä½æä»¶å¤å¶å°è¯¥è·¯å¾ä¸ï¼
 è¿è¡å¦ä¸å½ä»¤å»ºç«å­ä½ç¼å­ï¼ ```bash fc-cache -fv ``` - Mac:
 ä½¿ç¨å­ä½åæå¼å­ä½æä»¶å®è£ ## ä½¿ç¨ ### éè¿ python
 ç¨åºè°ç¨ åè [docs/examples/test_meme.py](https://github.com/MeetWq/
 meme-generator/tree/main/docs/examples/test_meme.py) ### éè¿å½ä»¤è¡ä½¿ç¨
 ```bash meme -h/--help ``` - `meme list (ls)` ååºææå·²å è½½çè¡¨æ -
@@ -81,16 +83,22 @@
 è¡¨æåå¶ä½æä»¶ - [noneplugin/nonebot-plugin-memes-api](https://
 github.com/noneplugin/nonebot-plugin-memes-api) nonebot-plugin-memes è°ç¨ api
 çæ¬ - Yunzai - [ikechan8370/yunzai-meme](https://github.com/ikechan8370/
 yunzai-meme) Yunzaiæºå¨äººçè¡¨æåæä»¶ ## éç½®
 é»è®¤éç½®æä»¶ä½ç½®ï¼ - Windows: `C:
 \Users\\AppData\Roaming\meme_generator\config.toml` - Linux: `~/.config/
 meme_generator/config.toml` - Mac: `~/Library/Application Support/
-meme_generator/config.toml` é»è®¤éç½®ï¼ ```toml [meme] load_builtin_memes =
-true # æ¯å¦å è½½åç½®è¡¨æå meme_dirs = [] #
+meme_generator/config.toml` > **Warning** > > ä» v0.0.6
+çæ¬å¼å§ï¼ä¸åçæé»è®¤éç½®æä»¶ï¼ä¿®æ¹éç½®æ¶éå¨å¯¹åºçæä»¶ä½ç½®èªè¡åå»ºéç½®æä»¶
+> > ç±äº v0.0.6
+çæ¬æ´æ¹äºèµæºé¾æ¥çæ¼æ¥æ¹å¼ï¼å¦æè£è¿ä¹åççæ¬ï¼éè¦ä¿®æ¹éç½®ä¸­ç
+`resource_url` > >
+å»ºè®®å°éç½®æä»¶ä¸­ä¸éè¦æ´æ¹çéé¡¹å é¤ï¼ä»¥ä½¿ç¨é»è®¤éç½®
+é»è®¤éç½®ï¼ ```toml [meme] load_builtin_memes = true #
+æ¯å¦å è½½åç½®è¡¨æå meme_dirs = [] #
 å è½½å¶ä»ä½ç½®çè¡¨æåï¼å¡«åæä»¶å¤¹è·¯å¾ meme_disabled_list = []
 # ç¦ç¨çè¡¨æååè¡¨ï¼å¡«åè¡¨æç `key` [resource] resource_url =
 "https://ghproxy.com/https://raw.githubusercontent.com/MeetWq/meme-generator" #
 ä¸è½½åç½®è¡¨æåå¾çæ¶çèµæºé¾æ¥ [gif] gif_max_size = 10.0 #
 éå¶çæç gif æä»¶å¤§å°ï¼åä½ä¸º Mb gif_max_frames = 100 #
 éå¶çæç gif æä»¶å¸§æ° [translate] baidu_trans_appid = "" #
 ç¾åº¦ç¿»è¯apiç¸å³ï¼è¡¨æå `dianzhongdian` éè¦ä½¿ç¨
```

### Comparing `meme_generator-0.0.8/meme_generator/__init__.py` & `meme_generator-0.0.9/meme_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/app.py` & `meme_generator-0.0.9/meme_generator/app.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/cli.py` & `meme_generator-0.0.9/meme_generator/cli.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/config.py` & `meme_generator-0.0.9/meme_generator/config.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/dirs.py` & `meme_generator-0.0.9/meme_generator/dirs.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/download.py` & `meme_generator-0.0.9/meme_generator/download.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/exception.py` & `meme_generator-0.0.9/meme_generator/exception.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/manager.py` & `meme_generator-0.0.9/meme_generator/manager.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/meme.py` & `meme_generator-0.0.9/meme_generator/meme.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/5000choyen/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/5000choyen/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/addiction/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/addiction/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/alike/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/alike/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/always/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/always/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/always_like/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/always_like/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/anya_suki/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/anya_suki/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/applaud/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/applaud/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/ascension/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/ascension/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/ask/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/ask/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/back_to_work/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/back_to_work/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/bad_news/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/bad_news/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/beat_head/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/beat_head/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/bite/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/bite/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/blood_pressure/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/blood_pressure/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/bocchi_draft/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/bocchi_draft/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/bronya_holdsign/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/shutup/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 
 from meme_generator import add_meme
 from meme_generator.exception import TextOverLength
 
 img_dir = Path(__file__).parent / "images"
 
 
-def bronya_holdsign(images, texts: List[str], args):
+def shutup(images, texts: List[str], args):
     text = texts[0]
     frame = BuildImage.open(img_dir / "0.jpg")
     try:
         frame.draw_text(
-            (190, 675, 640, 930),
+            (10, 180, 230, 230),
             text,
-            fill=(111, 95, 95),
             allow_wrap=True,
-            max_fontsize=60,
-            min_fontsize=25,
+            max_fontsize=40,
+            min_fontsize=15,
         )
     except ValueError:
         raise TextOverLength(text)
     return frame.save_jpg()
 
 
 add_meme(
-    "bronya_holdsign",
-    bronya_holdsign,
+    "shutup",
+    shutup,
     min_texts=1,
     max_texts=1,
-    default_texts=["V我50"],
-    keywords=["大鸭鸭举牌"],
+    default_texts=["你不要再说了"],
+    keywords=["别说了"],
 )
```

### Comparing `meme_generator-0.0.8/meme_generator/memes/bubble_tea/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/bubble_tea/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/call_110/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/call_110/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/capoo_rub/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/capoo_rub/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/capoo_say/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/capoo_say/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,56 +7,61 @@
 from meme_generator import add_meme
 from meme_generator.exception import TextOverLength
 from meme_generator.utils import save_gif
 
 img_dir = Path(__file__).parent / "images"
 
 
-def capoo_say(images, texts: List[str], args):
-    text = texts[0]
+def capoo_say_one_loop(text: str) -> List[IMG]:
     text_frame = BuildImage.new("RGBA", (80, 80))
     try:
         text_frame.draw_text(
             (0, 0, 80, 80),
             text,
             max_fontsize=80,
-            min_fontsize=30,
+            min_fontsize=20,
             allow_wrap=True,
             fontname="FZKaTong-M19S",
+            lines_align="center",
         )
     except ValueError:
         raise TextOverLength(text)
 
     params = [
-        (80, 80, 43, 30, 0),
-        (78, 78, 44, 30, 0),
-        (78, 78, 44, 29, 0),
-        None,
         None,
         None,
         None,
         (45, 45, 74, 112, 25),
         (73, 73, 41, 42, 17),
         (80, 80, 43, 36, 0),
+        (80, 80, 43, 30, 0),
+        (78, 78, 44, 30, 0),
+        (78, 78, 44, 29, 0),
+        None,
     ]
 
     frames: List[IMG] = []
     for i in range(10):
         frame = BuildImage.open(img_dir / f"{i}.png")
         param = params[i]
         if param:
             x, y, w, h, angle = param
             frame.paste(
                 text_frame.resize((x, y)).rotate(angle, expand=True), (w, h), alpha=True
             )
         frames.append(frame.image)
-    return save_gif(frames, 0.11)
+    return frames
+
+
+def capoo_say(images, texts: List[str], args):
+    frames = sum([capoo_say_one_loop(text) for text in texts], [])
+    return save_gif(frames, 0.1)
 
 
 add_meme(
     "capoo_say",
     capoo_say,
     min_texts=1,
-    max_texts=1,
+    max_texts=10,
     default_texts=["寄"],
     keywords=["咖波说"],
 )
```

### Comparing `meme_generator-0.0.8/meme_generator/memes/capoo_strike/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/capoo_strike/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/captain/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/captain/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/charpic/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/charpic/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/chase_train/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/chase_train/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/confuse/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/confuse/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/coupon/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/coupon/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/cover_face/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/cover_face/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/crawl/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/crawl/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/cyan/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/cyan/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/dianzhongdian/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/dianzhongdian/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/dinosaur/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/dinosaur/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/distracted/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/distracted/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/dont_touch/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/dont_touch/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/douyin/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/douyin/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/eat/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/eat/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/fanatic/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/fanatic/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/fencing/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/fencing/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/find_chips/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/find_chips/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/follow/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/follow/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/funny_mirror/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/funny_mirror/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/garbage/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/garbage/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/gif_subtitle/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/gif_subtitle/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/good_news/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/good_news/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/google/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/google/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/gun/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/gun/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/hammer/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/hammer/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/high_EQ/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/high_EQ/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/hit_screen/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/hit_screen/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/hold_grudge/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/hold_grudge/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/hug_leg/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/hug_leg/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/hutao_bite/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/hutao_bite/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/imprison/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/imprison/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/incivilization/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/incivilization/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/interview/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/interview/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/jiji_king/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/jiji_king/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/jiujiu/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/jiujiu/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/kaleidoscope/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/kaleidoscope/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/karyl_point/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/karyl_point/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/keep_away/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/keep_away/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/kick_ball/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/kick_ball/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/kirby_hammer/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/kirby_hammer/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/kiss/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/kiss/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/klee_eat/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/klee_eat/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/knock/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/knock/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/learn/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/learn/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/lim_x_0/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/lim_x_0/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/listen_music/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/listen_music/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/little_angel/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/little_angel/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/loading/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/loading/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/look_flat/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/look_flat/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/look_this_icon/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/look_this_icon/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/love_you/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/love_you/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/luoyonghao_say/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/luoyonghao_say/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/luxun_say/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/luxun_say/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/make_friend/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/make_friend/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/marriage/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/marriage/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/meteor/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/meteor/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/murmur/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/murmur/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/my_friend/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/my_friend/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/my_wife/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/my_wife/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/name_generator/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/name_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/need/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/need/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/nokia/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/nokia/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/not_call_me/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/not_call_me/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/overtime/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/overtime/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/paint/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/paint/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/painter/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/painter/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/pat/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/pat/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/petpet/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/petpet/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/play/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/play/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/play_game/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/play_game/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/police/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/police/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/pornhub/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/pornhub/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/pound/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/pound/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/printing/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/printing/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/prpr/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/prpr/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/psyduck/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/psyduck/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/punch/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/punch/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/raise_sign/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/raise_sign/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/read_book/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/read_book/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/repeat/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/repeat/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/rip/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/rip/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/rip_angrily/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/rip_angrily/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/rise_dead/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/rise_dead/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/roll/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/roll/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/rub/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/rub/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/run/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/run/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/safe_sense/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/safe_sense/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/scratch_head/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/scratch_head/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/scratchcard/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/scratchcard/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/scroll/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/scroll/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/shock/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/shock/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/shutup/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/wakeup/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,31 +5,29 @@
 
 from meme_generator import add_meme
 from meme_generator.exception import TextOverLength
 
 img_dir = Path(__file__).parent / "images"
 
 
-def shutup(images, texts: List[str], args):
+def wakeup(images, texts: List[str], args):
     text = texts[0]
     frame = BuildImage.open(img_dir / "0.jpg")
     try:
-        frame.draw_text(
-            (10, 180, 230, 230),
-            text,
-            allow_wrap=True,
-            max_fontsize=40,
-            min_fontsize=15,
-        )
+        frame.draw_text((310, 270, 460, 380), text, max_fontsize=90, min_fontsize=50)
     except ValueError:
         raise TextOverLength(text)
+    frame.draw_text(
+        (50, 610, 670, 720), f"{text}起来了", max_fontsize=110, min_fontsize=70
+    )
     return frame.save_jpg()
 
 
 add_meme(
-    "shutup",
-    shutup,
+    "wakeup",
+    wakeup,
     min_texts=1,
     max_texts=1,
-    default_texts=["你不要再说了"],
-    keywords=["别说了"],
+    default_texts=["好"],
+    keywords=["xx起来了"],
+    patterns=[r"(.*?)\s+起来了"],
 )
```

### Comparing `meme_generator-0.0.8/meme_generator/memes/sit_still/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/sit_still/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/slap/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/slap/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/slogan/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/slogan/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/smash/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/smash/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/step_on/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/step_on/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/suck/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/suck/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/support/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/support/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/symmetric/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/symmetric/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/tankuku_raisesign/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/tankuku_raisesign/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/teach/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/teach/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/think_what/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/think_what/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/throw/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/throw/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/throw_gif/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/throw_gif/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/thump/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/thump/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/tightly/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/tightly/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/together/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/together/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 from pathlib import Path
 from typing import List
 
 from pil_utils import BuildImage
 
 from meme_generator import MemeArgsModel, add_meme
 from meme_generator.exception import TextOverLength
+from meme_generator.utils import make_jpg_or_gif
 
 img_dir = Path(__file__).parent / "images"
 
 
 def together(images: List[BuildImage], texts: List[str], args: MemeArgsModel):
     frame = BuildImage.open(img_dir / "0.png")
-    frame.paste(images[0].convert("RGBA").resize((63, 63)), (132, 36))
     name = args.user_infos[0].name if args.user_infos else ""
     text = texts[0] if texts else f"一起玩{name}吧！"
     try:
         frame.draw_text(
             (10, 140, 190, 190),
             text,
             weight="bold",
             max_fontsize=50,
             min_fontsize=10,
             allow_wrap=True,
         )
     except ValueError:
         raise TextOverLength(text)
-    return frame.save_jpg()
+
+    def make(img: BuildImage) -> BuildImage:
+        img = img.convert("RGBA").resize((63, 63), keep_ratio=True)
+        return frame.copy().paste(img, (132, 36), alpha=True)
+
+    return make_jpg_or_gif(images[0], make)
 
 
 add_meme(
     "together",
     together,
     min_images=1,
     max_images=1,
```

### Comparing `meme_generator-0.0.8/meme_generator/memes/trance/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/trance/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/turn/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/turn/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/twist/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/twist/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/universal/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/universal/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/wallpaper/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/wallpaper/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/walnut_pad/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/walnut_pad/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/walnut_zoom/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/walnut_zoom/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/wave/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/wave/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/windmill_turn/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/windmill_turn/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/wish_fail/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/wish_fail/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/wooden_fish/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/wooden_fish/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/worship/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/worship/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/wujing/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/wujing/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/memes/youtube/__init__.py` & `meme_generator-0.0.9/meme_generator/memes/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/meme_generator/utils.py` & `meme_generator-0.0.9/meme_generator/utils.py`

 * *Files identical despite different names*

### Comparing `meme_generator-0.0.8/pyproject.toml` & `meme_generator-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meme-generator"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python package for making fun pictures"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MeetWq/meme-generator"
 repository = "https://github.com/MeetWq/meme-generator"
 exclude = [
```

### Comparing `meme_generator-0.0.8/PKG-INFO` & `meme_generator-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meme-generator
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for making fun pictures
 Home-page: https://github.com/MeetWq/meme-generator
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -73,14 +73,16 @@
 也可以调用 `meme_generator/download.py` 中的 `check_resources` 函数进行下载
 
 
 ### 字体安装
 
 为确保表情包中的文字生成正常，需要自行安装字体
 
+> **Note**
+>
 > 字体安装后若文字仍显示不正常，可删掉 `matplotlib` 字体缓存文件重新运行程序
 >
 > 缓存文件位置：
 > - Windows: `C:\Users\<username>\.matplotlib\fontlist-xxx.json`
 > - Linux: `~/.cache/matplotlib/fontlist-xxx.json`
 > - Mac: `~/Library/Caches/matplotlib/fontlist-xxx.json`
 
@@ -131,14 +133,15 @@
 某些表情包需要用到一些额外字体，存放于仓库中 [resources/fonts](https://github.com/MeetWq/meme-generator/tree/main/resources/fonts)，需要自行下载安装
 
 具体字体及对应的表情如下：
 
 | 字体名 | 字体文件名 | 用到该字体的表情 | 备注 |
 | --- | --- | --- | --- |
 | [Consolas](https://learn.microsoft.com/zh-cn/typography/font-list/consolas) | [consola.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/consola.ttf) | `charpic` |  |
+| [FZKaTong-M19S](https://www.foundertype.com/index.php/FontInfo/index/id/136) | [FZKATJW.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZKATJW.ttf) | `capoo_say` | 方正卡通 |
 | [FZXS14](https://www.foundertype.com/index.php/FontInfo/index/id/208) | [FZXS14.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZXS14.ttf) | `nokia` | 方正像素14 |
 | [FZSJ-QINGCRJ](https://www.foundertype.com/index.php/FontInfo/index/id/5178) | [FZSJ-QINGCRJ.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZSJ-QINGCRJ.ttf) | `psyduck` | 方正手迹-青春日记 |
 | [FZShaoEr-M11S](https://www.foundertype.com/index.php/FontInfo/index/id/149) | [FZSEJW.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZSEJW.ttf) | `raise_sign` | 方正少儿 |
 | [NotoSansSC](https://fonts.google.com/noto/specimen/Noto+Sans+SC) | [NotoSansSC-Regular.otf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/NotoSansSC-Regular.otf) | `5000choyen` |  |
 | [NotoSerifSC](https://fonts.google.com/noto/specimen/Noto+Serif+SC) | [NotoSerifSC-Regular.otf](https://github.com/MeetWq/meme-generator/blob/main/resources/fonts/NotoSerifSC-Regular.otf) | `5000choyen` |  |
 
 
@@ -207,14 +210,22 @@
 
 默认配置文件位置：
 
 - Windows: `C:\Users\<username>\AppData\Roaming\meme_generator\config.toml`
 - Linux: `~/.config/meme_generator/config.toml`
 - Mac: `~/Library/Application Support/meme_generator/config.toml`
 
+> **Warning**
+>
+> 从 v0.0.6 版本开始，不再生成默认配置文件；修改配置时需在对应的文件位置自行创建配置文件
+>
+> 由于 v0.0.6 版本更改了资源链接的拼接方式，如果装过之前的版本，需要修改配置中的 `resource_url`
+>
+> 建议将配置文件中不需要更改的选项删除，以使用默认配置
+
 默认配置：
 ```toml
 [meme]
 load_builtin_memes = true  # 是否加载内置表情包
 meme_dirs = []  # 加载其他位置的表情包，填写文件夹路径
 meme_disabled_list = []  # 禁用的表情包列表，填写表情的 `key`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meme-generator Version: 0.0.8 Summary: Python
+Metadata-Version: 2.1 Name: meme-generator Version: 0.0.9 Summary: Python
 package for making fun pictures Home-page: https://github.com/MeetWq/meme-
 generator License: MIT Author: meetwq Author-email: meetwq@gmail.com Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: fastapi (>=0.87.0,<1.0.0) Requires-
@@ -20,19 +20,19 @@
 <--](docs/memes.md) æ¥ç ## å®è£ ä½¿ç¨ pip å®è£ ```bash pip install
 meme_generator ``` ### å¾çä¸è½½ ç±äºè¡¨æåå¾çä½ç§¯è¾å¤§ï¼`meme-
 generator`
 åå«çè¡¨æä¸­çå¾çå¹¶ä¸éä»£ç ä¸èµ·æåï¼éè¦å¨å®è£åæå¨æ§è¡ä¸è½½å½ä»¤ï¼
 ``` meme download ``` ä¹å¯ä»¥è°ç¨ `meme_generator/download.py` ä¸­ç
 `check_resources` å½æ°è¿è¡ä¸è½½ ### å­ä½å®è£
 ä¸ºç¡®ä¿è¡¨æåä¸­çæå­çææ­£å¸¸ï¼éè¦èªè¡å®è£å­ä½ >
-å­ä½å®è£åè¥æå­ä»æ¾ç¤ºä¸æ­£å¸¸ï¼å¯å æ `matplotlib`
-å­ä½ç¼å­æä»¶éæ°è¿è¡ç¨åº > > ç¼å­æä»¶ä½ç½®ï¼ > - Windows: `C:
-\Users\\.matplotlib\fontlist-xxx.json` > - Linux: `~/.cache/matplotlib/
-fontlist-xxx.json` > - Mac: `~/Library/Caches/matplotlib/fontlist-xxx.json`
-#### ä¸­æå­ä½ å emojiå­ä½ å®è£
+**Note** > > å­ä½å®è£åè¥æå­ä»æ¾ç¤ºä¸æ­£å¸¸ï¼å¯å æ
+`matplotlib` å­ä½ç¼å­æä»¶éæ°è¿è¡ç¨åº > > ç¼å­æä»¶ä½ç½®ï¼ > -
+Windows: `C:\Users\\.matplotlib\fontlist-xxx.json` > - Linux: `~/.cache/
+matplotlib/fontlist-xxx.json` > - Mac: `~/Library/Caches/matplotlib/fontlist-
+xxx.json` #### ä¸­æå­ä½ å emojiå­ä½ å®è£
 æ ¹æ®ç³»ç»çä¸åï¼æ¨èå®è£çå­ä½å¦ä¸ï¼ - Windows: å¤§é¨å
 Windows ç³»ç»èªå¸¦ [å¾®è½¯éé»](https://learn.microsoft.com/zh-cn/
 typography/font-list/microsoft-yahei) ä¸­æå­ä½ å [Segoe UI Emoji](https:/
 /learn.microsoft.com/zh-cn/typography/font-list/segoe-ui-emoji) emoji
 å­ä½ï¼ä¸è¬æåµä¸æ éé¢å¤å®è£ - Linux: é¨åç³»ç»å¯è½èªå¸¦
 [ææ³é©¿å¾®ç±³é»](http://wenq.org/wqy2/index.cgi?MicroHei) ä¸­æå­ä½ï¼
 å¯¹äº Ubuntu ç³»ç»ï¼æ¨èå®è£ Noto Sans CJK å Noto Color Emojiï¼
@@ -50,31 +50,33 @@
 "Apple Color Emoji" emoji å­ä½ #### å¶ä»å­ä½å®è£
 æäºè¡¨æåéè¦ç¨å°ä¸äºé¢å¤å­ä½ï¼å­æ¾äºä»åºä¸­ [resources/
 fonts](https://github.com/MeetWq/meme-generator/tree/main/resources/
 fonts)ï¼éè¦èªè¡ä¸è½½å®è£ å·ä½å­ä½åå¯¹åºçè¡¨æå¦ä¸ï¼ |
 å­ä½å | å­ä½æä»¶å | ç¨å°è¯¥å­ä½çè¡¨æ | å¤æ³¨ | | --- | --- |
 --- | --- | | [Consolas](https://learn.microsoft.com/zh-cn/typography/font-
 list/consolas) | [consola.ttf](https://github.com/MeetWq/meme-generator/blob/
-main/resources/fonts/consola.ttf) | `charpic` | | | [FZXS14](https://
-www.foundertype.com/index.php/FontInfo/index/id/208) | [FZXS14.ttf](https://
-github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZXS14.ttf) |
-`nokia` | æ¹æ­£åç´ 14 | | [FZSJ-QINGCRJ](https://www.foundertype.com/
-index.php/FontInfo/index/id/5178) | [FZSJ-QINGCRJ.ttf](https://github.com/
-MeetWq/meme-generator/blob/main/resources/fonts/FZSJ-QINGCRJ.ttf) | `psyduck` |
-æ¹æ­£æè¿¹-éæ¥æ¥è®° | | [FZShaoEr-M11S](https://www.foundertype.com/
-index.php/FontInfo/index/id/149) | [FZSEJW.ttf](https://github.com/MeetWq/meme-
-generator/blob/main/resources/fonts/FZSEJW.ttf) | `raise_sign` | æ¹æ­£å°å¿ |
-| [NotoSansSC](https://fonts.google.com/noto/specimen/Noto+Sans+SC) |
-[NotoSansSC-Regular.otf](https://github.com/MeetWq/meme-generator/blob/main/
-resources/fonts/NotoSansSC-Regular.otf) | `5000choyen` | | | [NotoSerifSC]
-(https://fonts.google.com/noto/specimen/Noto+Serif+SC) | [NotoSerifSC-
-Regular.otf](https://github.com/MeetWq/meme-generator/blob/main/resources/
-fonts/NotoSerifSC-Regular.otf) | `5000choyen` | | #### å­ä½å®è£æ¹å¼
-ä¸åç³»ç»çå­ä½å®è£æ¹å¼ï¼ - Windows: -
-åå»éè¿å­ä½æ¥çå¨å®è£ - å¤å¶å°å­ä½æä»¶å¤¹ï¼`C:
+main/resources/fonts/consola.ttf) | `charpic` | | | [FZKaTong-M19S](https://
+www.foundertype.com/index.php/FontInfo/index/id/136) | [FZKATJW.ttf](https://
+github.com/MeetWq/meme-generator/blob/main/resources/fonts/FZKATJW.ttf) |
+`capoo_say` | æ¹æ­£å¡é | | [FZXS14](https://www.foundertype.com/index.php/
+FontInfo/index/id/208) | [FZXS14.ttf](https://github.com/MeetWq/meme-generator/
+blob/main/resources/fonts/FZXS14.ttf) | `nokia` | æ¹æ­£åç´ 14 | | [FZSJ-
+QINGCRJ](https://www.foundertype.com/index.php/FontInfo/index/id/5178) | [FZSJ-
+QINGCRJ.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/
+fonts/FZSJ-QINGCRJ.ttf) | `psyduck` | æ¹æ­£æè¿¹-éæ¥æ¥è®° | | [FZShaoEr-
+M11S](https://www.foundertype.com/index.php/FontInfo/index/id/149) |
+[FZSEJW.ttf](https://github.com/MeetWq/meme-generator/blob/main/resources/
+fonts/FZSEJW.ttf) | `raise_sign` | æ¹æ­£å°å¿ | | [NotoSansSC](https://
+fonts.google.com/noto/specimen/Noto+Sans+SC) | [NotoSansSC-Regular.otf](https:/
+/github.com/MeetWq/meme-generator/blob/main/resources/fonts/NotoSansSC-
+Regular.otf) | `5000choyen` | | | [NotoSerifSC](https://fonts.google.com/noto/
+specimen/Noto+Serif+SC) | [NotoSerifSC-Regular.otf](https://github.com/MeetWq/
+meme-generator/blob/main/resources/fonts/NotoSerifSC-Regular.otf) |
+`5000choyen` | | #### å­ä½å®è£æ¹å¼ ä¸åç³»ç»çå­ä½å®è£æ¹å¼ï¼ -
+Windows: - åå»éè¿å­ä½æ¥çå¨å®è£ - å¤å¶å°å­ä½æä»¶å¤¹ï¼`C:
 \Windows\Fonts` - Linux: å¨ `/usr/share/fonts` ç®å½ä¸æ°å»ºæä»¶å¤¹ï¼å¦
 `myfonts`ï¼å°å­ä½æä»¶å¤å¶å°è¯¥è·¯å¾ä¸ï¼
 è¿è¡å¦ä¸å½ä»¤å»ºç«å­ä½ç¼å­ï¼ ```bash fc-cache -fv ``` - Mac:
 ä½¿ç¨å­ä½åæå¼å­ä½æä»¶å®è£ ## ä½¿ç¨ ### éè¿ python
 ç¨åºè°ç¨ åè [docs/examples/test_meme.py](https://github.com/MeetWq/
 meme-generator/tree/main/docs/examples/test_meme.py) ### éè¿å½ä»¤è¡ä½¿ç¨
 ```bash meme -h/--help ``` - `meme list (ls)` ååºææå·²å è½½çè¡¨æ -
@@ -96,16 +98,22 @@
 è¡¨æåå¶ä½æä»¶ - [noneplugin/nonebot-plugin-memes-api](https://
 github.com/noneplugin/nonebot-plugin-memes-api) nonebot-plugin-memes è°ç¨ api
 çæ¬ - Yunzai - [ikechan8370/yunzai-meme](https://github.com/ikechan8370/
 yunzai-meme) Yunzaiæºå¨äººçè¡¨æåæä»¶ ## éç½®
 é»è®¤éç½®æä»¶ä½ç½®ï¼ - Windows: `C:
 \Users\\AppData\Roaming\meme_generator\config.toml` - Linux: `~/.config/
 meme_generator/config.toml` - Mac: `~/Library/Application Support/
-meme_generator/config.toml` é»è®¤éç½®ï¼ ```toml [meme] load_builtin_memes =
-true # æ¯å¦å è½½åç½®è¡¨æå meme_dirs = [] #
+meme_generator/config.toml` > **Warning** > > ä» v0.0.6
+çæ¬å¼å§ï¼ä¸åçæé»è®¤éç½®æä»¶ï¼ä¿®æ¹éç½®æ¶éå¨å¯¹åºçæä»¶ä½ç½®èªè¡åå»ºéç½®æä»¶
+> > ç±äº v0.0.6
+çæ¬æ´æ¹äºèµæºé¾æ¥çæ¼æ¥æ¹å¼ï¼å¦æè£è¿ä¹åççæ¬ï¼éè¦ä¿®æ¹éç½®ä¸­ç
+`resource_url` > >
+å»ºè®®å°éç½®æä»¶ä¸­ä¸éè¦æ´æ¹çéé¡¹å é¤ï¼ä»¥ä½¿ç¨é»è®¤éç½®
+é»è®¤éç½®ï¼ ```toml [meme] load_builtin_memes = true #
+æ¯å¦å è½½åç½®è¡¨æå meme_dirs = [] #
 å è½½å¶ä»ä½ç½®çè¡¨æåï¼å¡«åæä»¶å¤¹è·¯å¾ meme_disabled_list = []
 # ç¦ç¨çè¡¨æååè¡¨ï¼å¡«åè¡¨æç `key` [resource] resource_url =
 "https://ghproxy.com/https://raw.githubusercontent.com/MeetWq/meme-generator" #
 ä¸è½½åç½®è¡¨æåå¾çæ¶çèµæºé¾æ¥ [gif] gif_max_size = 10.0 #
 éå¶çæç gif æä»¶å¤§å°ï¼åä½ä¸º Mb gif_max_frames = 100 #
 éå¶çæç gif æä»¶å¸§æ° [translate] baidu_trans_appid = "" #
 ç¾åº¦ç¿»è¯apiç¸å³ï¼è¡¨æå `dianzhongdian` éè¦ä½¿ç¨
```

