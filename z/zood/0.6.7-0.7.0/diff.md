# Comparing `tmp/zood-0.6.7.tar.gz` & `tmp/zood-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.6.7.tar", max compression
+gzip compressed data, was "zood-0.7.0.tar", max compression
```

## Comparing `zood-0.6.7.tar` & `zood-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      550 2023-04-19 13:14:12.551676 zood-0.6.7/pyproject.toml
--rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.6.7/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.6.7/zood/__init__.py
--rw-r--r--   0        0        0     5924 2023-04-01 23:48:51.709845 zood-0.6.7/zood/config/_config.yml
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.6.7/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.6.7/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.6.7/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.6.7/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.6.7/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.6.7/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.6.7/zood/config/img/sun.png
--rw-r--r--   0        0        0    17324 2023-04-19 11:34:46.154555 zood-0.6.7/zood/config/index.css
--rw-r--r--   0        0        0     3547 2023-02-19 10:19:17.056632 zood-0.6.7/zood/config/js/change_mode.js
--rw-r--r--   0        0        0      955 2023-04-02 00:07:20.610243 zood-0.6.7/zood/config/js/check_box.js
--rw-r--r--   0        0        0     1282 2023-04-19 11:38:57.244766 zood-0.6.7/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.6.7/zood/config/js/next_front.js
--rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.6.7/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.6.7/zood/config/js/picture_title.js
--rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.6.7/zood/config/js/prismjs/prism.css
--rw-r--r--   0        0        0    52330 2023-03-23 13:29:38.926084 zood-0.6.7/zood/config/js/prismjs/prism.js
--rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.6.7/zood/config/js/search.js
--rw-r--r--   0        0        0      980 2023-02-24 16:17:35.264950 zood-0.6.7/zood/config/template.html
--rw-r--r--   0        0        0     4224 2023-04-03 14:22:34.682079 zood-0.6.7/zood/main.py
--rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.6.7/zood/md_parser.py
--rw-r--r--   0        0        0     4290 2023-04-03 14:22:32.130915 zood-0.6.7/zood/util.py
--rw-r--r--   0        0        0     8017 2023-03-08 03:42:01.835849 zood-0.6.7/zood/zood.py
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.6.7/setup.py
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-04-29 06:51:12.010576 zood-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.7.0/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.7.0/zood/__init__.py
+-rw-r--r--   0        0        0     6257 2023-04-29 06:11:53.294334 zood-0.7.0/zood/config/_config.yml
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.7.0/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.7.0/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.7.0/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.7.0/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.7.0/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.7.0/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.7.0/zood/config/img/sun.png
+-rw-r--r--   0        0        0    18370 2023-04-29 06:41:40.209081 zood-0.7.0/zood/config/index.css
+-rw-r--r--   0        0        0     3993 2023-04-29 02:33:40.621393 zood-0.7.0/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0     1040 2023-04-29 02:59:13.107114 zood-0.7.0/zood/config/js/check_box.js
+-rw-r--r--   0        0        0     2654 2023-04-29 06:50:24.299560 zood-0.7.0/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0      561 2023-04-29 04:53:40.454412 zood-0.7.0/zood/config/js/navigator.js
+-rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.7.0/zood/config/js/next_front.js
+-rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.7.0/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.7.0/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.7.0/zood/config/js/prismjs/prism.css
+-rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.7.0/zood/config/js/prismjs/prism.js
+-rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.7.0/zood/config/js/search.js
+-rw-r--r--   0        0        0      546 2023-04-27 06:18:09.762970 zood-0.7.0/zood/config/template.html
+-rw-r--r--   0        0        0     4224 2023-04-03 14:22:34.682079 zood-0.7.0/zood/main.py
+-rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.7.0/zood/md_parser.py
+-rw-r--r--   0        0        0     4290 2023-04-03 14:22:32.130915 zood-0.7.0/zood/util.py
+-rw-r--r--   0        0        0     8706 2023-04-29 06:09:49.501448 zood-0.7.0/zood/zood.py
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.7.0/setup.py
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.7.0/PKG-INFO
```

### Comparing `zood-0.6.7/pyproject.toml` & `zood-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zood"
-version = "0.6.7"
+version = "0.7.0"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
```

### Comparing `zood-0.6.7/zood/config/_config.yml` & `zood-0.7.0/zood/config/_config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -39,25 +39,30 @@
 
   # 是否启用代码高亮
   enable_highlight: true
 
   # 是否启用右侧上一个下一个
   enable_next_front: true
 
+  # 是否启用目录导航栏
+  enable_navigator: true
+
   # 是否启用查询搜索
   enable_search:
     enable: false
     search_scope: []
 
   # 是否保留图片的标题
   enable_picture_title: false
 
   # 图片是否可以被放大预览
   enable_picture_preview: true
 
+  # 支持 mermaid
+  enable_mermaid: false
 
 # 页面布局
 position:
 
   # markdown左侧距离
   markdown_body_left: "20%"
   
@@ -76,32 +81,41 @@
   # 目录宽度
   dir_width: "10%"
 
   # 按钮的右侧距离
   button_right: 6%;
 
   # 按钮顶部距离
-  button_top: 40%;
+  button_top: 60%;
 
   # 按钮宽度
   button_width: 10%;
 
+  # 导航栏距离左侧距离 -> 左对齐
+  navigator_left: 83%
+
+  # 导航栏顶部距离
+  navigator_top: 10%
 
   # 一级条目上下间距
   dir_item_margin: "25px"
 
   # 一级条目左间距
   dir_item_margin_left: "-10px"
 
   # 二级条目上下间距
   dir_second_item_margin: "0px"
 
   # 二级条目左间距
   dir_second_item_margin_left: "5px"
 
+  navigator_margin: "10px"
+
+  navigator_item_margin_left: "-10px"
+
   # 图片被放大后的宽度
   image_preview_width: "60%"
 
 # 主题颜色配置，其他不生效的地方请使用自定义 css 解决，配色可以在下方链接中获得启发
 # Theme color, please use custom CSS to solve other colors, color schema can be inspired by the links below
 # See: https://www.webdesignrankings.com/resources/lolcolors/
 color:
@@ -225,9 +239,11 @@
   font_size: 16px
   font_family: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial, sans-serif, Apple Color Emoji, Segoe UI Emoji
   letter_spacing: 0.02em
 
   # 一级条目字体大小
   dir_item_font_size: 18px
 
+  navigator_item_font_size: 14px
+
   # 二级条目字体大小
   dir_second_item_font_size: 16px
```

### Comparing `zood-0.6.7/zood/config/img/enter.png` & `zood-0.7.0/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.6.7/zood/config/index.css` & `zood-0.7.0/zood/config/index.css`

 * *Files 2% similar despite different names*

```diff
@@ -238,17 +238,17 @@
   margin-top: 16px;
 }
 
 .markdown-body li + li {
   margin-top: 0.25em;
 }
 
-.markdown-body  ul ul li:first-child {
-    padding-top: 15px; /* 你希望的距离 */
-  }
+.markdown-body ul ul li:first-child {
+  padding-top: 15px; /* 你希望的距离 */
+}
 
 .markdown-body table {
   border-spacing: 0;
   border-collapse: collapse;
 }
 
 .markdown-body table th {
@@ -279,15 +279,15 @@
 .markdown-dark table tr {
   background-color: #444444;
   border-top: 1px solid #c6cbd1;
   color: white;
 }
 
 .markdown-dark table tr:nth-child(2n) {
-  background-color: #808080 ;
+  background-color: #808080;
   color: white;
 }
 
 .markdown-body h1,
 .markdown-body h2,
 .markdown-body h3,
 .markdown-body h4,
@@ -295,70 +295,71 @@
 .markdown-body h6 {
   margin-top: 24px;
   margin-bottom: 16px;
   font-weight: 600;
   line-height: 1.25;
 }
 
-.markdown-body > ul>li:has(input) {
+.markdown-body > ul > li:has(input) {
   padding-left: 0;
   margin-bottom: 0;
 }
 
-.markdown-body  ul>li:has(input)>ul {
-    list-style-type: none;
-    padding-left: 8px;
+.markdown-body ul > li:has(input) > ul {
+  list-style-type: none;
+  padding-left: 8px;
 }
 
-
 .markdown-body img {
   max-width: 80%;
   display: block;
   margin: 0 auto;
   box-shadow: "<%markdown_picture_box_shadow%>";
   border-radius: 5px;
 }
 
 .markdown-body pre {
   position: relative;
-}
-
-.changeMode {
-  position: absolute;
-  right: 50px;
-  top: 50px;
-  padding: 5px;
-  border-radius: 50%;
-  background-color: #e3e3e3;
-  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
-    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
-    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
+  overflow-x: scroll;
 }
 
 .markdown-body pre #code_copy {
   position: absolute;
   right: 10px;
   top: 50%;
   margin-top: -16px;
   padding: 3px;
   opacity: 0.9;
   border: 1px solid rgba(149, 157, 165, 0.2);
   border-radius: 5px;
+  z-index: 1;
 }
 
 .markdown-light pre #code_copy {
   background-color: rgb(196, 196, 196);
 }
 
 .markdown-body pre #code_copy:hover {
   background-color: #ffffff;
   box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
   border-radius: 5px;
 }
 
+.changeMode {
+  position: absolute;
+  right: 50px;
+  top: 50px;
+  padding: 5px;
+  border-radius: 50%;
+  background-color: #e3e3e3;
+  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px,
+    rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px,
+    rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
+}
+
 .markdown-light :not(pre) > code[class*="language-"],
 .markdown-light pre[class*="language-"] {
   background: "<%markdown_code_bg_color%>";
 }
 
 .markdown-dark :not(pre) > code[class*="language-"],
 .markdown-dark pre[class*="language-"] {
@@ -689,18 +690,18 @@
 .link-active {
   font-weight: bold !important;
   border-bottom: 2px solid #555;
   padding-bottom: 2px;
 }
 
 .link-active-dark {
-    font-weight: bold !important;
-    border-bottom: 2px solid #f3f3f3;
-    padding-bottom: 2px;
-  }
+  font-weight: bold !important;
+  border-bottom: 2px solid #f3f3f3;
+  padding-bottom: 2px;
+}
 
 /* 图片下的文字的样式 */
 
 .markdown-body p > p {
   color: "<%picture_text_color%>";
   margin-top: 10px;
   text-align: center;
@@ -831,7 +832,49 @@
   top: 50%;
   transform: translateY(-50%);
   height: 60%;
   opacity: 0.5;
   /* transition: all 0.5s; */
   /* border-radius: 5px; */
 }
+
+.header-navigator {
+  display: none;
+  position: fixed;
+  left: "<%navigator_left%>";
+  top: "<%navigator_top%>";
+  font-family: "<%font_family%>";
+  font-size: "<%dir_item_font_size%>";
+  letter-spacing: "<%letter_spacing%>";
+  scrollbar-width: none; /* Firefox */
+  -ms-overflow-style: none; /* IE 10+ */
+  text-overflow: ellipsis; /*  过长文字省略号 */
+  white-space: nowrap; /*禁止文字折行*/
+  list-style: none;
+}
+
+.header-navigator::-webkit-scrollbar {
+  display: none; /* Chrome Safari */
+}
+
+.header-navigator a {
+  text-decoration: none;
+}
+
+.header-navigator a:hover {
+  font-weight: bolder;
+}
+
+.header-navigator ul {
+  font-family: "<%font_family%>";
+  font-size: "<%navigator_item_font_size%>";
+  letter-spacing: "<%letter_spacing%>";
+  margin-top: "<%navigator_margin%>";
+  margin-bottom: "<%navigator_margin%>";
+  margin-left: "<%navigator_item_margin_left%>";
+  list-style: none;
+  position: relative;
+}
+
+.header-navigator ul ul {
+  margin-left: -20px;
+}
```

### Comparing `zood-0.6.7/zood/config/js/change_mode.js` & `zood-0.7.0/zood/config/js/change_mode.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -10,14 +10,21 @@
     }
     var dirTree = document.querySelector('.dir-tree');
     dirTree.style.background = '#f6f8fa';
     var allLinks = dirTree.querySelectorAll('a');
     for (var i = 0; i < allLinks.length; i++) {
         allLinks[i].style.color = 'black';
     }
+
+    var navigator = document.querySelector('.header-navigator');
+    var allLinks = navigator.querySelectorAll('a');
+    for (var i = 0; i < allLinks.length; i++) {
+        allLinks[i].style.color = 'black';
+    }
+
     var activate_links = dirTree.querySelectorAll('.link-active-dark');
     for (var activate_link of activate_links) {
         activate_link.className = 'link-active';
     }
     var search_bar = document.querySelector('.search-bar');
     if (search_bar) {
         search_bar.style.background = '#f6f8fa';
@@ -35,14 +42,21 @@
     }
     var dirTree = document.querySelector('.dir-tree');
     dirTree.style.background = '#252D38';
     var allLinks = dirTree.querySelectorAll('a');
     for (var i = 0; i < allLinks.length; i++) {
         allLinks[i].style.color = 'white';
     }
+
+    var navigator = document.querySelector('.header-navigator');
+    var allLinks = navigator.querySelectorAll('a');
+    for (var i = 0; i < allLinks.length; i++) {
+        allLinks[i].style.color = 'white';
+    }
+
     var activate_links = dirTree.querySelectorAll('.link-active');
     for (var activate_link of activate_links) {
         activate_link.className = 'link-active-dark';
     }
     var search_bar = document.querySelector('.search-bar');
     if (search_bar) {
         search_bar.style.background = '#252D38';
```

### Comparing `zood-0.6.7/zood/config/js/check_box.js` & `zood-0.7.0/zood/config/js/check_box.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -13,14 +13,19 @@
 var dirTree = document.querySelector(".dir-tree");
 var links = dirTree.querySelectorAll("a");
 // 主题保持
 const savedTheme = localStorage.getItem('theme');
 // 如果保存的主题存在，则设置当前主题为保存的主题
 links.forEach(function(link) {
     if (link.href === currentUrl) {
+        link.scrollIntoView({
+            block: 'center',
+            inline: 'nearest',
+            container: dirTree
+        });
         if (savedTheme) {
             if (savedTheme == 'dark') {
                 link.classList.add("link-active-dark");
             } else {
                 link.classList.add("link-active");
             }
         } else {
```

### Comparing `zood-0.6.7/zood/config/js/next_front.js` & `zood-0.7.0/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.6.7/zood/config/js/picture_preview.js` & `zood-0.7.0/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.6.7/zood/config/js/prismjs/prism.css` & `zood-0.7.0/zood/config/js/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `zood-0.6.7/zood/config/js/prismjs/prism.js` & `zood-0.7.0/zood/config/js/prismjs/prism.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -631,14 +631,15 @@
     keyword: /\b(?:break|catch|continue|do|else|finally|for|function|if|in|instanceof|new|null|return|throw|try|while)\b/,
     boolean: /\b(?:false|true)\b/,
     function: /\b\w+(?=\()/,
     number: /\b0x[\da-f]+\b|(?:\b\d+(?:\.\d*)?|\B\.\d+)(?:e[+-]?\d+)?/i,
     operator: /[<>]=?|[!=]=?=?|--?|\+\+?|&&?|\|\|?|[?*/~^%]/,
     punctuation: /[{}[\];(),.:]/,
 };
+
 !(function(e) {
     var t =
         "\\b(?:BASH|BASHOPTS|BASH_ALIASES|BASH_ARGC|BASH_ARGV|BASH_CMDS|BASH_COMPLETION_COMPAT_DIR|BASH_LINENO|BASH_REMATCH|BASH_SOURCE|BASH_VERSINFO|BASH_VERSION|COLORTERM|COLUMNS|COMP_WORDBREAKS|DBUS_SESSION_BUS_ADDRESS|DEFAULTS_PATH|DESKTOP_SESSION|DIRSTACK|DISPLAY|EUID|GDMSESSION|GDM_LANG|GNOME_KEYRING_CONTROL|GNOME_KEYRING_PID|GPG_AGENT_INFO|GROUPS|HISTCONTROL|HISTFILE|HISTFILESIZE|HISTSIZE|HOME|HOSTNAME|HOSTTYPE|IFS|INSTANCE|JOB|LANG|LANGUAGE|LC_ADDRESS|LC_ALL|LC_IDENTIFICATION|LC_MEASUREMENT|LC_MONETARY|LC_NAME|LC_NUMERIC|LC_PAPER|LC_TELEPHONE|LC_TIME|LESSCLOSE|LESSOPEN|LINES|LOGNAME|LS_COLORS|MACHTYPE|MAILCHECK|MANDATORY_PATH|NO_AT_BRIDGE|OLDPWD|OPTERR|OPTIND|ORBIT_SOCKETDIR|OSTYPE|PAPERSIZE|PATH|PIPESTATUS|PPID|PS1|PS2|PS3|PS4|PWD|RANDOM|REPLY|SECONDS|SELINUX_INIT|SESSION|SESSIONTYPE|SESSION_MANAGER|SHELL|SHELLOPTS|SHLVL|SSH_AUTH_SOCK|TERM|UID|UPSTART_EVENTS|UPSTART_INSTANCE|UPSTART_JOB|UPSTART_SESSION|USER|WINDOWID|XAUTHORITY|XDG_CONFIG_DIRS|XDG_CURRENT_DESKTOP|XDG_DATA_DIRS|XDG_GREETER_DATA_DIR|XDG_MENU_PREFIX|XDG_RUNTIME_DIR|XDG_SEAT|XDG_SEAT_PATH|XDG_SESSION_DESKTOP|XDG_SESSION_ID|XDG_SESSION_PATH|XDG_SESSION_TYPE|XDG_VTNR|XMODIFIERS)\\b",
         a = {
             pattern: /(^(["']?)\w+\2)[ \t]+\S.*/,
             lookbehind: !0,
             alias: "punctuation",
@@ -1554,14 +1555,15 @@
     },
     keyword: /\b(?:_(?=\s*:)|and|as|assert|async|await|break|case|class|continue|def|del|elif|else|except|exec|finally|for|from|global|if|import|in|is|lambda|match|nonlocal|not|or|pass|print|raise|return|try|while|with|yield)\b/,
     builtin: /\b(?:__import__|abs|all|any|apply|ascii|basestring|bin|bool|buffer|bytearray|bytes|callable|chr|classmethod|cmp|coerce|compile|complex|delattr|dict|dir|divmod|enumerate|eval|execfile|file|filter|float|format|frozenset|getattr|globals|hasattr|hash|help|hex|id|input|int|intern|isinstance|issubclass|iter|len|list|locals|long|map|max|memoryview|min|next|object|oct|open|ord|pow|property|range|raw_input|reduce|reload|repr|reversed|round|set|setattr|slice|sorted|staticmethod|str|sum|super|tuple|type|unichr|unicode|vars|xrange|zip)\b/,
     boolean: /\b(?:False|None|True)\b/,
     number: /\b0(?:b(?:_?[01])+|o(?:_?[0-7])+|x(?:_?[a-f0-9])+)\b|(?:\b\d+(?:_\d+)*(?:\.(?:\d+(?:_\d+)*)?)?|\B\.\d+(?:_\d+)*)(?:e[+-]?\d+(?:_\d+)*)?j?(?!\w)/i,
     operator: /[-+%=]=?|!=|:=|\*\*?=?|\/\/?=?|<[<=>]?|>[=>]?|[&|^~]/,
     punctuation: /[{}[\];(),.:]/,
+
 }),
 (Prism.languages.python[
     "string-interpolation"
 ].inside.interpolation.inside.rest = Prism.languages.python),
 (Prism.languages.py = Prism.languages.python);
 !(function(e) {
     var n = /[*&][^\s[\]{},]+/,
```

### Comparing `zood-0.6.7/zood/config/js/search.js` & `zood-0.7.0/zood/config/js/search.js`

 * *Files identical despite different names*

### Comparing `zood-0.6.7/zood/main.py` & `zood-0.7.0/zood/main.py`

 * *Files identical despite different names*

### Comparing `zood-0.6.7/zood/md_parser.py` & `zood-0.7.0/zood/md_parser.py`

 * *Files identical despite different names*

### Comparing `zood-0.6.7/zood/util.py` & `zood-0.7.0/zood/util.py`

 * *Files identical despite different names*

### Comparing `zood-0.6.7/zood/zood.py` & `zood-0.7.0/zood/zood.py`

 * *Files 13% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             file_path = os.path.join(md_dir_name,dir_name,file_name+'.md')
             if not os.path.exists(file_path):
                 printInfo('[zood解析失败]: 请检查 dir.yml')
                 printInfo('找不到文件 ' + file_path)
                 exit(0)
             else:
                 with open(file_path,'r',encoding='utf-8') as f:
-                    markdown_htmls[file_path] = MarkdownParser.parse(f.read())
+                    markdown_htmls[file_path] = MarkdownParser.parse_withtag(f.read())
                 file_names.append(file_name)
         directory_tree.append({dir_name:file_names})
         
     return directory_tree,markdown_htmls
             
 
 def parseConfig(config,markdown_htmls):
@@ -115,15 +115,16 @@
     basic_html_template = basic_html_template.replace('js-scope',js_scope)
     
     # css 部分
     prism_src = '../../../css/prism.css'
     index_src = '../../../css/index.css'
 
     css_scope = ''
-    css_scope += f"<link rel='stylesheet' href={prism_src} />"
+    if config['options']['enable_highlight']:
+        css_scope += f"<link rel='stylesheet' href={prism_src} />"
     css_scope += f"<link rel='stylesheet' href={index_src} />"
     basic_html_template = basic_html_template.replace('css-scope',css_scope)
     
     with open(css_template_path,'r',encoding='utf-8') as f:
         basic_css_template = f.read()
     favicon_url = config['favicon']
     if favicon_url[:4] == 'http':
@@ -176,14 +177,19 @@
         
     if config['options']['enable_copy_code']:
         
         js_code = insertJScode('enable_copy_code',html_dir_name)
         js_code += f"<script>addCodeCopy(\"../../../img/before_copy.png\",\"../../../img/after_copy.png\")</script>"
         js_scope += js_code
         
+    if config['options']['enable_navigator']:
+        js_code = insertJScode('enable_navigator',html_dir_name)
+        js_scope += js_code
+
+
     if config['options']['enable_highlight']:
         # 复制prismjs
         shutil.copy(os.path.join(os.path.dirname(__file__),'config','js','prismjs','prism.css'),f'{html_dir_name}/css')
         shutil.copy(os.path.join(os.path.dirname(__file__),'config','js','prismjs','prism.js'),f'{html_dir_name}/js')
         src = "../../../js/prism.js"
         highlight = f"<script type=\"text/javascript\" src=\"{src}\"></script>"
         js_scope += highlight
@@ -199,14 +205,26 @@
         
     if config['options']['enable_search']['enable']:
         js_code = insertJScode('enable_search',html_dir_name)
         all_api_text = getAllAPIText(markdown_htmls,config['options']['enable_search']['search_scope'],md_dir_name)
         js_code += f"<script>addSearchBar({all_api_text},\"../../../img/search.svg\",\"../../../img/enter.svg\",\"Ctrl+K\")</script>"
         js_scope += js_code
 
+    if config['options']['enable_mermaid']:
+        js_code = '<script type=\"module\">\
+const codeBlocks = document.querySelectorAll(\'.language-mermaid\');\
+codeBlocks.forEach(codeBlock => {\
+    codeBlock.classList.remove(\'language-mermaid\');\
+    codeBlock.classList.add(\'mermaid\');\
+});\
+import mermaid from \'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs\';\
+mermaid.initialize({ startOnLoad: true });\
+</script>'
+        js_scope += js_code
+
     js_scope += insertJScode('enable_check_box',html_dir_name)
 
     return js_scope
 
 def insertJScode(file_name,html_dir_name):
     file_name = file_name[7:] # 跳过enable_
     # 文件同名
```

### Comparing `zood-0.6.7/setup.py` & `zood-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ['MarkdownParser', 'PyYAML>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['zood = zood.main:main']}
 
 setup_kwargs = {
     'name': 'zood',
-    'version': '0.6.7',
+    'version': '0.7.0',
     'description': 'web page documentation & comment generation documentation',
     'long_description': '# zood\n\nzood 是一个辅助文档生成的Python库, zood的页面风格更倾向于纯文档内容而非博客\n\n## 主题预览\n\n[![20230101121438](https://raw.githubusercontent.com/learner-lu/picbed/master/20230101121438.png)](https://luzhixing12345.github.io/zood/)\n\n## 安装与使用\n\n```bash\npip install zood\n```\n\n参见 [用户使用文档](https://luzhixing12345.github.io/zood/)\n\n## 参考\n\n- [UI](https://remixicon.com/)',
     'author': 'kamilu',
     'author_email': 'luzhixing12345@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/luzhixing12345/zood',
```

### Comparing `zood-0.6.7/PKG-INFO` & `zood-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.6.7
+Version: 0.7.0
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

