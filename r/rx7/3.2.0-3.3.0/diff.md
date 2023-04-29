# Comparing `tmp/rx7-3.2.0.tar.gz` & `tmp/rx7-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rx7-3.2.0.tar", last modified: Fri Mar 10 08:56:20 2023, max compression
+gzip compressed data, was "rx7-3.3.0.tar", last modified: Sat Apr 29 15:54:26 2023, max compression
```

## Comparing `rx7-3.2.0.tar` & `rx7-3.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 08:56:20.227259 rx7-3.2.0/
--rw-rw-rw-   0        0        0    22541 2021-08-29 10:01:16.000000 rx7-3.2.0/COLORS.html
--rw-rw-rw-   0        0        0     7815 2022-12-20 17:30:11.000000 rx7-3.2.0/LICENSE
--rw-rw-rw-   0        0        0       20 2021-08-29 10:01:16.000000 rx7-3.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    37601 2023-03-10 08:56:20.223800 rx7-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    37217 2023-03-10 00:53:50.000000 rx7-3.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-10 08:56:20.203405 rx7-3.2.0/rx7/
--rw-rw-rw-   0        0        0    77344 2023-03-07 20:07:48.000000 rx7-3.2.0/rx7/__init__.py
--rw-rw-rw-   0        0        0     1134 2023-03-09 20:00:51.000000 rx7-3.2.0/rx7/__main__.py
--rw-rw-rw-   0        0        0    20066 2021-08-29 10:01:16.000000 rx7-3.2.0/rx7/removed.py
-drwxrwxrwx   0        0        0        0 2023-03-10 08:56:20.222809 rx7-3.2.0/rx7.egg-info/
--rw-rw-rw-   0        0        0    37601 2023-03-10 08:56:20.000000 rx7-3.2.0/rx7.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-03-10 08:56:20.000000 rx7-3.2.0/rx7.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 08:56:20.000000 rx7-3.2.0/rx7.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-03-10 08:56:20.000000 rx7-3.2.0/rx7.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-10 08:56:20.000000 rx7-3.2.0/rx7.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-10 08:56:20.228258 rx7-3.2.0/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-03-10 00:15:08.000000 rx7-3.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:54:26.058930 rx7-3.3.0/
+-rw-rw-rw-   0        0        0    22541 2021-08-29 10:01:16.000000 rx7-3.3.0/COLORS.html
+-rw-rw-rw-   0        0        0     7815 2022-12-20 17:30:11.000000 rx7-3.3.0/LICENSE
+-rw-rw-rw-   0        0        0       20 2021-08-29 10:01:16.000000 rx7-3.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    33137 2023-04-29 15:54:26.056903 rx7-3.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    32753 2023-04-29 15:43:56.000000 rx7-3.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 15:54:26.038952 rx7-3.3.0/rx7/
+-rw-rw-rw-   0        0        0    73831 2023-04-29 15:40:33.000000 rx7-3.3.0/rx7/__init__.py
+-rw-rw-rw-   0        0        0     1134 2023-03-09 20:00:51.000000 rx7-3.3.0/rx7/__main__.py
+-rw-rw-rw-   0        0        0    20066 2021-08-29 10:01:16.000000 rx7-3.3.0/rx7/removed.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:54:26.054909 rx7-3.3.0/rx7.egg-info/
+-rw-rw-rw-   0        0        0    33137 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-29 15:54:25.000000 rx7-3.3.0/rx7.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 15:54:26.059894 rx7-3.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      814 2023-04-29 15:46:03.000000 rx7-3.3.0/setup.py
```

### Comparing `rx7-3.2.0/COLORS.html` & `rx7-3.3.0/COLORS.html`

 * *Files identical despite different names*

### Comparing `rx7-3.2.0/LICENSE` & `rx7-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rx7-3.2.0/PKG-INFO` & `rx7-3.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: rx7
-Version: 3.2.0
-Summary: Shortcut for most usefull functions, High API, Special Features
-Home-page: https://github.com/Ramin-RX7/RX7-Lib
-Author: Ramin RX7
-Author-email: rawmin.rx@gmail.com
-License: LGPL
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >= 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![PyPI - License](https://img.shields.io/badge/downloads-32k%2Fmonth-brightgreen?style=plastic) ![PyPI - License](https://img.shields.io/pypi/l/rx7?color=orange&style=plastic) ![PyPI - License](https://img.shields.io/badge/status-stable-success?style=plastic)
 --------------------------------------------------------
 
 "rx7" library is here to help you make your code shorter!
 --------------------------------------------------------
 
 ### \- Most Usefull function and mexthods are collected.
@@ -51,47 +38,47 @@
 
 
 <br>
 
 
 List of Functions:
 ------------------
-|                                                          |                                                                                                  |
-|----------------------------------------------------------|--------------------------------------------------------------------------------------------------|
-| p()                                                      | print() function.                                                                                |
-| repeat(function,n)                                       | Repeat F_Name function for n times.                                                              |
-| rev(v)  (REMOVED 2.4.0)                                  | Reverse v and returns it. (Everything like str,list,int)                                         |
-| read(file)                                               | Return content of the file.                                                                      |
-| write(file,mode,text)                                    | Write things you want in file content. (Read Doc String)                                         |
-| wait(n)sleep(n)                                          | Stop code executing for n seconds                                                                |
-| cls()clear()                                             | It Clears the Terminal                                                                           |
-| progressbar() (*removed in v3.1)                         | In-App Progressbar. (Read Doc String)                                                            |
-| cons_integer(Frst,Lst)                                   | Return string from Frst to Lst (Read Doc String) (v1.7)                                          |
-| force(tpl,*var)                                          | Return tpl with adding var(s) to it.                                                             |
-| erase(tpl,*var)                                          | Return tpl with removing var(s) from it.                                                         |
-| replace(tpl,ind,var)                                     | Replace tpl[ind] with var                                                                        |
-| insert(tpl,ind,var)                                      | Set tpl[ind] to var. (Note that tpl[ind] will be tpl[ind+1])                                     |
-| pop(tpl,index)                                           | Remove member with index of 'index' from a tuple                                                 |
-| wait_for(button)                                         | Waits for user to press specific button.                                                         |
-| call_later(func,args,delay)                              | Call func(args) after delay time.                                                                |
-| convert_bytes(num)                                       | convert bytes to (KB,MB,GB,TB)                                                                   |
-| Input(prompt,default)                                    | Prompt an input message with default answer (value) (ONLY ON WINDOWS)                            |
-| default_input()                                          | Same as `default_input`                                                                          |
-| restart_app()                                            | Restart running python program                                                                   |
-| active_window_title()                                    | Return Active Window Title                                                                       |
-| open_image(path)                                         | Open image with default image viewer (Mac OS is not supported)                                   |
-| download(url)                                            | To download files with memory saver and progressbar                                              |
-| extract(file,path,pwd)                                   | Extract Zip file with password to path                                                           |
-| screenshot(name)                                         | Take a screenshot and save it.                                                                   |
-| func_info(function)                                      | Print information of function                                                                    |
-| Check_Type                                               | Decorator that raise TypeError if function argument type is wrong (Read Help)                    |
-| Progressbar()                                            | Generator of progressbar() which you can use it to do some stuff between your delays (Read Help) |
-| pixel_color(X,Y)                                         | Return RGB color of pixel[X,Y]                                                                   |
-| getpass(prompt)                                          | Prompt for a password, with echo turned off.                                                     |
-| import_module(path)                                      | Return given path (file with any extension) as a Module                                          |
+|                                  |                                                                                                  |
+|----------------------------------|--------------------------------------------------------------------------------------------------|
+| p()                              | print() function.                                                                                |
+| repeat(function,n)               | Repeat F_Name function for n times.                                                              |
+| rev(v)  (REMOVED 2.4.0)          | Reverse v and returns it. (Everything like str,list,int)                                         |
+| read(file)                       | Return content of the file.                                                                      |
+| write(file,mode,text)            | Write things you want in file content. (Read Doc String)                                         |
+| wait(n)sleep(n)                  | Stop code executing for n seconds                                                                |
+| cls()clear()                     | It Clears the Terminal                                                                           |
+| progressbar() (*removed in v3.1) | In-App Progressbar. (Read Doc String)                                                            |
+| cons_integer(Frst,Lst)           | Return string from Frst to Lst (Read Doc String) (v1.7)                                          |
+| force(tpl,*var)                  | Return tpl with adding var(s) to it.                                                             |
+| erase(tpl,*var)                  | Return tpl with removing var(s) from it.                                                         |
+| replace(tpl,ind,var)             | Replace tpl[ind] with var                                                                        |
+| insert(tpl,ind,var)              | Set tpl[ind] to var. (Note that tpl[ind] will be tpl[ind+1])                                     |
+| pop(tpl,index)                   | Remove member with index of 'index' from a tuple                                                 |
+| wait_for(button)                 | Waits for user to press specific button.                                                         |
+| call_later(func,args,delay)      | Call func(args) after delay time.                                                                |
+| convert_bytes(num)               | convert bytes to (KB,MB,GB,TB)                                                                   |
+| Input(prompt,default)            | Prompt an input message with default answer (value) (ONLY ON WINDOWS)                            |
+| default_input()                  | Same as `default_input`                                                                          |
+| restart_app()                    | Restart running python program                                                                   |
+| active_window_title()            | Return Active Window Title                                                                       |
+| open_image(path)                 | Open image with default image viewer (Mac OS is not supported)                                   |
+| download(url)                    | To download files with memory saver and progressbar                                              |
+| extract(file,path,pwd)           | Extract Zip file with password to path                                                           |
+| screenshot(name)                 | Take a screenshot and save it.                                                                   |
+| func_info(function)              | Print information of function                                                                    |
+| Check_Type                       | Decorator that raise TypeError if function argument type is wrong (Read Help)                    |
+| Progressbar()                    | Generator of progressbar() which you can use it to do some stuff between your delays (Read Help) |
+| pixel_color(X,Y)                 | Return RGB color of pixel[X,Y]                                                                   |
+| getpass(prompt)                  | Prompt for a password, with echo turned off.                                                     |
+| import_module(path)              | Return given path (file with any extension) as a Module                                          |
 
 
 <br>
 
 
 <h2>List of Classes:</h2>
 
@@ -106,108 +93,113 @@
 | shuffle(iterable)        | Return shuffled version of iterable            |
 
 <br>
 
 
 <h3>&nbsp; Class System:&nbsp; &nbsp;<em>Some system actions and information.</em></h3>
 
-|                               |                                                                                  |
-|-------------------------------|----------------------------------------------------------------------------------|
-| accname()                     |         return account username you have logged in.                              |
-| pid()                         |         Get pid number of terminal and return it.                                |
-| disk_usage(path)              | ########                                                                         |
-| chdir                         | Change directory of terminal.                                                    |
-| SHUT_DOWN()                   | Shut Down the PC.                                                                |
-| RESTART()                     | Restart the PC.                                                                  |
-| terminal_size()               | Return terminal size in tuple  (columns,lines).                                  |
-| cwd()                         | Return Carrent Working Directory.                                                |
-| ip_global()                   | Returns Global IP.                                                               |
-| ip_local()                    | Returns Local IP.                                                                |
-| ram_total()                   | Returns total ram of the system.                                                 |
-| ram_used()                    | Returns Used Space of the ram of the system.                                     |
-| ram_free()                    | Returns Available (Free) space of system ram.                                    |
-| boot_time()                   | Return system boot time in seconds since the epoch.                              |
-| device_name()                 | Returns Device Name                                                              |
-| ip_website(url)               | Returns url ip address                                                           |
-| win10_notification()          | Display windows 10 notification (READ DOCSTRING) (ONLY WIN10 SUPPORTED)          |
-| cpu_count(logical=True)       |         Return the number of logical/physical CPUs in the system                 |
-| pyshell_execute_bit()         |         To determine whether Python shell is executing in 32bit or 64bit         |
-| pids()                        |                 Return a list of current running PIDs                            |
-| pid_exists(pid)               | Return True if pid exists else False                                             |
-|         cpu_percent()         |         Return the current CPU utilization as a percentage                       |
+|                         |                                                                         |
+|-------------------------|-------------------------------------------------------------------------|
+| accname()               | return account username you have logged in.                             |
+| pid()                   | Get pid number of terminal and return it.                               |
+| disk_usage(path)        | ########                                                                |
+| chdir                   | Change directory of terminal.                                           |
+| SHUT_DOWN()             | Shut Down the PC.                                                       |
+| RESTART()               | Restart the PC.                                                         |
+| terminal_size()         | Return terminal size in tuple  (columns,lines).                         |
+| cwd()                   | Return Carrent Working Directory.                                       |
+| ip_global()             | Returns Global IP.                                                      |
+| ip_local()              | Returns Local IP.                                                       |
+| ram_total()             | Returns total ram of the system.                                        |
+| ram_used()              | Returns Used Space of the ram of the system.                            |
+| ram_free()              | Returns Available (Free) space of system ram.                           |
+| boot_time()             | Return system boot time in seconds since the epoch.                     |
+| device_name()           | Returns Device Name                                                     |
+| ip_website(url)         | Returns url ip address                                                  |
+| win10_notification()    | Display windows 10 notification (READ DOCSTRING) (ONLY WIN10 SUPPORTED) |
+| cpu_count(logical=True) | Return the number of logical/physical CPUs in the system                |
+| pyshell_execute_bit()   | To determine whether Python shell is executing in 32bit or 64bit        |
+| pids()                  | Return a list of current running PIDs                                   |
+| pid_exists(pid)         | Return True if pid exists else False                                    |
+| cpu_percent()           | Return the current CPU utilization as a percentage                      |
+| os_name()               | Returns OS name of machine                                              |
 
 
 
 <br>
 
 
 <h3>&nbsp; Class Files: (Static<strong style="font-size: 14px;">&nbsp;methods)&nbsp;</strong><em style="font-size: 14px;">Actions and information about files.</em></h3>
 
-| METHOD                                                        | DESCRIPTION                                                                   |
-|---------------------------------------------------------------|-------------------------------------------------------------------------------|
-| size(path)                                                    | Return size of the file in byte(s). Also work on                              |
-| delete(path)                                                  | Use this to delete a file (Not folder).                                       |
-| rename(path)                                                  | Rename files with this function.                                              |
-| abspath(path)                                                 | Return absolute path of given path.                                           |
-| exists(path)                                                  | Return Boolean. If exists True, else: False                                   |
-| mdftime(path)                                                 | Get last modify time of the file.                                             |
-| acstime(path)                                                 | Get last access time of the file.                                             |
-| move(src,dst)                                                 | Move file from src to dst. (Read Doc String of copy func)                     |
-| copy(src,dst,metadata=True)                                   | Copy file (with metadata) from src to dst. (Also work on folders)             |
-| hide(path)                                                    | Hide given path. (It can be file or directory.)                               |
-| read_only(path,mode=True)                                     | Make file or folder read-only. (Read Doc String)                              |
-| read(path)                                                    | Return content of the path                                                    |
-| write(path,text='',...)                                       | Same as write function.                                                       |
-| isdir(path)                                                   | Return True for directory and False for others.                               |
-| isfile(path)                                                  | Return True for file and False for others.                                    |
-| is_hidden(path)                                               | Check whether path is hidden or not                                           |
-| is_readonly(path)                                             | Check whether path is readonly or not                                         |
-| search_file(pattern,path,mode)                                | search for pattern in path (Read function doc string)                         |
-| search_content(path,word)                                     | Search for word in all files in path, return list of files that contain word  |
-| mkdir(path)                                                   | Make directory (More than one if its possible!)                               |
-| generate_tree(dir_path)                                       | Returns a visual tree of dir_path                                             |
-| get_drives()                                                  | (Windows only) Get currently available drives                                 |
-| &nbsp; &nbsp; &nbsp; &nbsp; MEMBERS (Family)                  |                                                                               |
-| MEMBERS.all_exactdir                                          | List of all things those are in exact directory                               |
-| MEMBERS.files_exactdir                                        | List of files which are in exact directory                                    |
-| MEMBERS.dirs_exactdir                                         | List of dirs which are in exact directory                                     |
-| MEMBERS.files_all                                             | List of files which are in exact directory and all sub-directories            |
-| MEMBERS.files_all_sep                                         | List of files which are in exact directory and all sub-directories seprated by their directories |
-| MEMBERS.dirs_all                                              | List of directories (Exact dir and all sub-dirs)                              |
-| MEMBERS.all_all_sep                                           | List of everything thing in path (exact dir &amp; sub-dirs)                   |
+| METHOD                                       | DESCRIPTION                                                                   |
+|----------------------------------------------|-------------------------------------------------------------------------------|
+| size(path)                                   | Return size of the file in byte(s). Also work on                              |
+| delete(path)                                 | Use this to delete a file (Not folder).                                       |
+| rename(path)                                 | Rename files with this function.                                              |
+| abspath(path)                                | Return absolute path of given path.                                           |
+| exists(path)                                 | Return Boolean. If exists True, else: False                                   |
+| mdftime(path)                                | Get last modify time of the file.                                             |
+| acstime(path)                                | Get last access time of the file.                                             |
+| move(src,dst)                                | Move file from src to dst. (Read Doc String of copy func)                     |
+| copy(src,dst,metadata=True)                  | Copy file (with metadata) from src to dst. (Also work on folders)             |
+| hide(path)                                   | Hide given path. (It can be file or directory.)                               |
+| read_only(path,mode=True)                    | Make file or folder read-only. (Read Doc String)                              |
+| read(path)                                   | Return content of the path                                                    |
+| write(path,text='',...)                      | Same as write function.                                                       |
+| isdir(path)                                  | Return True for directory and False for others.                               |
+| isfile(path)                                 | Return True for file and False for others.                                    |
+| is_hidden(path)                              | Check whether path is hidden or not                                           |
+| is_readonly(path)                            | Check whether path is readonly or not                                         |
+| search_file(pattern,path,mode)               | search for pattern in path (Read function doc string)                         |
+| search_content(path,word)                    | Search for word in all files in path, return list of files that contain word  |
+| mkdir(path)                                  | Make directory (More than one if its possible!)                               |
+| generate_tree(dir_path)                      | Returns a visual tree of dir_path                                             |
+| get_drives()                                 | (Windows only) Get currently available drives                                 |
+| basename(path)                               | Returns the final component of a pathname                                     |
+| dirname(path)                                | Returns the directory component of a pathname                                 |
+| join_paths(path)                             | Joins multiple paths together and returns it                                  |
+| &nbsp; &nbsp; &nbsp; &nbsp; MEMBERS (Family) |                                                                               |
+| MEMBERS.all_exactdir                         | List of all things those are in exact directory                               |
+| MEMBERS.files_exactdir                       | List of files which are in exact directory                                    |
+| MEMBERS.dirs_exactdir                        | List of dirs which are in exact directory                                     |
+| MEMBERS.files_all                            | List of files which are in exact directory and all sub-directories            |
+| MEMBERS.files_all_sep                        | List of files which are in exact directory and all sub-directories seprated by their directories |
+| MEMBERS.dirs_all                             | List of directories (Exact dir and all sub-dirs)                              |
+| MEMBERS.all_all_sep                          | List of everything thing in path (exact dir &amp; sub-dirs)                   |
 
 
 <br>
 
 
 <h3>&nbsp; Class Style:&nbsp; &nbsp; <em>Changing text Color,BG &amp; Style. (Read Doc String)</em></h3>
 
-|                                                         |                                                             |
-|---------------------------------------------------------|-------------------------------------------------------------|
-| print\(\*values, color, BG, style, end, sep\)           | Print txt with selected color,BG,style\.\(Read Doc String\) |
-| switch\(color,BG,style\)                                | Change Terminal Attributes Until another Call\.             |
-| switch\_default\(\)                                     | Restore Terminal Attributes\.                               |
-| reset                                                   | =switch\_default                                            |
-| log\_&nbsp; \(Family\)                                  | 5 Different Style\.print with ready color and style         |
+|                                               |                                                             |
+|-----------------------------------------------|-------------------------------------------------------------|
+| print\(\*values, color, BG, style, end, sep\) | Print txt with selected color,BG,style\.\(Read Doc String\) |
+| switch\(color,BG,style\)                      | Change Terminal Attributes Until another Call\.             |
+| switch\_default\(\)                           | Restore Terminal Attributes\.                               |
+| reset                                         | =switch\_default                                            |
+| log\_&nbsp; \(Family\)                        | 5 Different Style\.print with ready color and style         |
 
 
 <br>
 
 
 <h3>&nbsp; Class Record:&nbsp; &nbsp;<em>Record time of a certain actions. (Read Doc String)</em></h3>
 
-|                                                                     |                                                                            |
-|---------------------------------------------------------------------|----------------------------------------------------------------------------|
-| __init__()                                                          | Set Start Time.                                                            |
-| self.stop(self)                                                     | Stops Recording (You can not lap anymore)                                  |
-| self.lap(self, save=True, round=15)                                 | Rreturn time between start time. if save==True: add that time to self.laps |
-| self.laps                                                           | A list that contains all laps you have done                                |
-| self.reset(self, start=False)                                       | Empty self.laps, if start is True: set start time to now                   |
-| self.last_lap(save=True)                                            | Return elapsed time from last lap (save it in self.laps if save is true)   |
-| timeit(code,setup, times,globals_) | Run the 'code' for 'times' times and return time it needs (all, not once)  |
+|                                     |                                                                            |
+|-------------------------------------|----------------------------------------------------------------------------|
+| __init__()                          | Set Start Time.                                                            |
+| self.stop(self)                     | Stops Recording (You can not lap anymore)                                  |
+| self.lap(self, save=True, round=15) | Rreturn time between start time. if save==True: add that time to self.laps |
+| self.laps                           | A list that contains all laps you have done                                |
+| self.reset(self, start=False)       | Empty self.laps, if start is True: set start time to now                   |
+| self.last_lap(save=True)            | Return elapsed time from last lap (save it in self.laps if save is true)   |
+| timeit(code,setup, times,globals_)  | Run the 'code' for 'times' times and return time it needs (all, not once)  |
+| timer(f)                            | Decorator for functions to print out how much each call takes              |
 
 
 <br>
 
 
 <h3>&nbsp; Class Decorator:&nbsp; &nbsp;<em>Useful decorators you might want to use</em></h3>
 
@@ -280,289 +272,302 @@
 
 
 Releases and Changelog:
 ---------
 
 ####        (+ for new features, \* for changes, - for removed features)
 
-<table style="height: 10px; margin-left: 10px; width: 519px;" cellpadding="5">
+<table>
   <tbody>
 
   <tr style="height: 42px;">
     <td style="width: 119px; height: 42px; text-align: center;"><strong>Version</strong></td>
     <td style="width: 153px; height: 42px; text-align: center;"><strong>Release Date</strong></td>
     <td style="width: 513px; height: 42px; text-align: center;"><strong>New Features &amp; Changes</strong></td>
   </tr>
 
+  <tr>
+    <td>
+      <p style="text-align: center;">3.3.0</p>
+    </td>
+    <td style="text-align: center;">29/04/2023</td>
+    <td style="width: 513px; height: 25px; text-align: center;">
+      <div>+ Files.basename()</div>
+      <div>+ Files.dirname()</div>
+      <div>+ Files.join_paths()</div>
+      <div>* `pre_action` and `post_action` in IO  selective_input</div>
+      <div>+ Record.timer decorator</div>
+      <div>+ System.os_name()  </div>
+    </td>
+  </tr>
 
-  <tr style="height: 25px;">
-    <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
+  <tr>
+    <td>
       <p style="text-align: center;">3.2.0</p>
     </td>
-    <td style="width: 153px; height: 25px; text-align: center;">10/03/2023</td>
+    <td style="text-align: center;">10/03/2023</td>
     <td style="width: 513px; height: 25px; text-align: center;">
-      <div style="text-align: left;">+ `environ` variable: environment variables as a dict</div>
-      <div style="text-align: left;">+ `Terminal.get_size()`</div>
-      <div style="text-align: left;">+ `exit()`: sys.exit()</div>
-      <div style="text-align: left;">+ `files.get_drives()`</div>
-      <div style="text-align: left;">+ IO.selective_input `choices` argument upgrade</div>
-      <div style="text-align: left;">+ IO.selective_input `action` parameter</div>
-      <div style="text-align: left;">- IO.selective_input `error` parameter is removed</div>
-      <div style="text-align: left;">* Fixed `files.size()` for directories</div>
-      <div style="text-align: left;">* `files.is_readonly()` now also works on Unix</div>
-      <div style="text-align: left;">* Improved module call</div>
+      <div>+ `environ` variable: environment variables as a dict</div>
+      <div>+ `Terminal.size()`</div>
+      <div>+ `exit()`: sys.exit()</div>
+      <div>+ `files.get_drives()`</div>
+      <div>+ IO.selective_input `choices` argument upgrade</div>
+      <div>+ IO.selective_input `action` parameter</div>
+      <div>- IO.selective_input `error` parameter is removed</div>
+      <div>* Fixed `files.size()` for directories</div>
+      <div>* `files.is_readonly()` now also works on Unix</div>
+      <div>* Improved module call</div>
     </td>
   </tr>
 
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">3.1.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">23/12/2022</td>
+  <td style="text-align: center;">23/12/2022</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Record.timeit has default parameters now</div>
-  <div style="text-align: left;">- removed progressbar()</div>
-  <div style="text-align: left;">* Improved Style object creation</div>
-  <div style="text-align: left;">* Improved Style.print implementation</div>
-  <div style="text-align: left;">* Improved Style.log_ methods implementation</div>
-  <div style="text-align: left;">* Terminal.run() now return exit code</div>
-  <div style="text-align: left;">- Removed "Tuple" object</div>
+  <div>+ Record.timeit has default parameters now</div>
+  <div>- removed progressbar()</div>
+  <div>* Improved Style object creation</div>
+  <div>* Improved Style.print implementation</div>
+  <div>* Improved Style.log_ methods implementation</div>
+  <div>* Terminal.run() now return exit code</div>
+  <div>- Removed "Tuple" object</div>
   </td>
   </tr>
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">3.0.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/09/2021</td>
+  <td style="text-align: center;">01/09/2021</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;"><b>+ class Internet</b></div>
-  <div style="text-align: left;"><b>+ class DateTime</b></div>
-  <div style="text-align: left;">+ "Style.log" now has time prefix</div>
-  <div style="text-align: left;">+ call = call_later</div>
-  <div style="text-align: left;">+ IO.Input()</div>
-  <div style="text-align: left;">+ IO.getpass()</div>
-  <div style="text-align: left;">* io.selective_input choices can be dict</div>
-  <div style="text-align: left;">+ System.mac_address()</div>
+  <div><b>+ class Internet</b></div>
+  <div><b>+ class DateTime</b></div>
+  <div>+ "Style.log" now has time prefix</div>
+  <div>+ call = call_later</div>
+  <div>+ IO.Input()</div>
+  <div>+ IO.getpass()</div>
+  <div>* io.selective_input choices can be dict</div>
+  <div>+ System.mac_address()</div>
   </td>
   </tr>
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.9.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/12/2020</td>
+  <td style="text-align: center;">15/12/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ <b>IO Class</b>(wait_for_input() - selective_input() - yesno_input())</div>
-  <div style="text-align: left;">+ <b>Decorator Class</b> (attach_to_all ---&nbsp;Check_Type)</div>
-  <div style="text-align: left;">* IMPORT SPEED IS 20x FASTER!</div>
-  <div style="text-align: left;">+ argv (sys.argv)</div>
-  <div style="text-align: left;">- Record.EndError</div>
-  <div style="text-align: left;">+ overload (Decorator.overload)</div>
-  <div style="text-align: left;">+ ABC,ABCMeta</div>
+  <div>+ <b>IO Class</b>(wait_for_input() - selective_input() - yesno_input())</div>
+  <div>* IMPORT SPEED IS 20x FASTER!</div>
+  <div>+ argv (sys.argv)</div>
+  <div>- Record.EndError</div>
+  <div>+ overload (Decorator.overload)</div>
+  <div>+ ABC,ABCMeta</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.8.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/11/2020</td>
+  <td style="text-align: center;">15/11/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Decorator Class (attach_to_all ---&nbsp;Check_Type)</div>
-  <div style="text-align: left;">+ pop()</div>
-  <div style="text-align: left;">+ Tuple.pop()</div>
-  <div style="text-align: left;">+ Record.timeit()</div>
+  <div>+ Decorator Class (attach_to_all --- Check_Type)</div>
+  <div>+ pop()</div>
+  <div>+ Tuple.pop()</div>
+  <div>+ Record.timeit()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.7.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/10/2020</td>
+  <td style="text-align: center;">15/10/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ getpass()</div>
-  <div style="text-align: left;">+ style.log_ Family</div>
-  <div style="text-align: left;">+ style.reset() = style.switch_default()</div>
-  <div style="text-align: left;">+ load_module()</div>
-  <div style="text-align: left;">+ record.last_lap()</div>
+  <div>+ getpass()</div>
+  <div>+ style.log_ Family</div>
+  <div>+ style.reset() = style.switch_default()</div>
+  <div>+ load_module()</div>
+  <div>+ record.last_lap()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.6.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/10/2020</td>
+  <td style="text-align: center;">01/10/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ system.cpu_percent()</div>
-  <div style="text-align: left;">+ system.pid_exists()</div>
-  <div style="text-align: left;">+ Progressbar()&nbsp;<em>(Generator)</em></div>
-  <div style="text-align: left;">+ pixel_color()</div>
+  <div>+ system.cpu_percent()</div>
+  <div>+ system.pid_exists()</div>
+  <div>+ Progressbar()<em> (Generator)</em></div>
+  <div>+ pixel_color()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.5.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/09/2020</td>
+  <td style="text-align: center;">15/09/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Check_Type decorator</div>
-  <div style="text-align: left;">+ system.pyshell_execute_bit()</div>
-  <div style="text-align: left;">+ system.pids()</div>
-  <div style="text-align: left;">+ record.lap&nbsp;round&nbsp;arg</div>
+  <div>+ Check_Type decorator</div>
+  <div>+ system.pyshell_execute_bit()</div>
+  <div>+ system.pids()</div>
+  <div>+ record.lap round arg</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.4.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/09/2020</td>
+  <td style="text-align: center;">01/09/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">* rand -&gt; random</div>
-  <div>
-  <div style="text-align: left;">+ random.shuffle()</div>
-  <div>
-  <div style="text-align: left;">+ repeat function supports parameters</div>
-  <div>
-  <div style="text-align: left;">+ sleep = wait&nbsp; &nbsp;---&nbsp; &nbsp;clear = cls&nbsp; &nbsp;---&nbsp; &nbsp;default_input = Input</div>
-  <div style="text-align: left;">+ system.cpu_count()</div>
-  </div>
-  </div>
-  </div>
+  <div>* rand -&gt; random</div>
+  <div>+ random.shuffle()</div>
+  <div>+ repeat function supports parameters</div>
+  <div>+ sleep = wait&nbsp; &nbsp;---&nbsp; &nbsp;clear = cls&nbsp; &nbsp;---&nbsp; &nbsp;default_input = Input</div>
+  <div>+ system.cpu_count()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.3.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">19/08/2020</td>
+  <td style="text-align: center;">19/08/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ extract()</p>
-  <p style="text-align: left;">+ screenshot()</p>
-  <p style="text-align: left;">+ func_info()</p>
+  <div>+ extract()</div>
+  <div>+ screenshot()</div>
+  <div>+ func_info()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.2.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">03/08/2020</td>
+  <td style="text-align: center;">03/08/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ download()</p>
-  <p style="text-align: left;">+ system.ip_website()</p>
-  <p style="text-align: left;">+ system.win10_notification</p>
+  <div>+ download()</div>
+  <div>+ system.ip_website()</div>
+  <div>+ system.win10_notification</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.1.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/07/2020</td>
+  <td style="text-align: center;">15/07/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">* style class better performance in linux</p>
-  <p style="text-align: left;">+&nbsp;<span style="text-align: center;">MEMBERS&nbsp;group&nbsp;in&nbsp;files&nbsp;class</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+ File object:&nbsp; self.basename, self.ext</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+ system.device_name()</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+&nbsp;</span><span style="text-align: center;">active_window_title() --- open_image()</span></p>
+  <div>* style class better performance in linux</div>
+  <div>+&nbsp;<span style="text-align: center;">MEMBERS&nbsp;group&nbsp;in&nbsp;files&nbsp;class</span></div>
+  <div><span style="text-align: center;">+ File object:&nbsp; self.basename, self.ext</span></div>
+  <div><span style="text-align: center;">+ system.device_name()</span></div>
+  <div><span style="text-align: center;">+&nbsp;</span><span style="text-align: center;">active_window_title() --- open_image()</span></div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;"><strong>2.0.0</strong></p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;"><strong>01/07/2020</strong></td>
+  <td style="text-align: center;"><strong>01/07/2020</strong></td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ <strong>Tuple object&nbsp; &nbsp;---&nbsp; &nbsp;rxobject</strong></p>
-  <p style="text-align: left;">+ record.reset()&nbsp; &nbsp;---&nbsp; &nbsp;record.lap new arg</p>
-  <p style="text-align: left;">+ New methods of files</p>
-  <p style="text-align: left;">&nbsp; &nbsp; &nbsp; files.is_readonly()&nbsp; &nbsp;---&nbsp; &nbsp;files.is_hidden()</p>
-  <p style="text-align: left;"><strong>&nbsp; &nbsp; &nbsp; files.search_file()&nbsp; &nbsp;---&nbsp; &nbsp;files.search_content()</strong></p>
-  <p style="text-align: left;">&nbsp; &nbsp; &nbsp; files.copy new arg</p>
-  <p style="text-align: left;"><strong>&nbsp; &nbsp; &nbsp; files.generate_tree()</strong></p>
-  <p style="text-align: left;"><strong>+ File.MEMBERS </strong>(when in File(path), path is a directory&nbsp; (self.MEMBERS.TYPE_PATH)</p>
-  <p style="text-align: left;"><strong>+ File.tree&nbsp; &nbsp; ---&nbsp; &nbsp; &nbsp;File.tree_dirs</strong></p>
-  <p style="text-align: left;"><strong>+ Input()</strong>&nbsp; <em>(Only on windows)</em></p>
-  <p style="text-align: left;">+ restart_app()</p>
+  <div>+ <strong>Tuple object</strong></div>
+  <div>rxobject</div>
+  <div>+ record.reset()</div>
+  <div>record.lap new arg</div>
+  <div>+ New methods of files</div>
+  <div>&nbsp; &nbsp; &nbsp; files.is_readonly()&nbsp; &nbsp;---&nbsp; &nbsp;files.is_hidden()</div>
+  <div>&nbsp; &nbsp; &nbsp; files.search_file()&nbsp; &nbsp;---&nbsp; &nbsp;files.search_content()</div>
+  <div>&nbsp; &nbsp; &nbsp; files.copy new arg&nbsp; &nbsp;---&nbsp; &nbsp;files.generate_tree()</div>
+  <div><strong>+ File.MEMBERS </strong>(when in File(path), path is a directory&nbsp; (self.MEMBERS.TYPE_PATH)</div>
+  <div>+ File.tree&nbsp; &nbsp; ---&nbsp; &nbsp; &nbsp;File.tree_dirs</div>
+  <div>+ Input()&nbsp; <em>(Only on windows)</em></div>
+  <div>+ restart_app()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.9.0</td>
   <td style="width: 153px; height: 25px;">&nbsp; 09/06/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">* re() --&gt; repeat()</p>
-  <p style="text-align: left;">+ New Methods of System Class:&nbsp; ip_global(),&nbsp;ip_local(),&nbsp;ram_free(), ram_percent(),&nbsp;ram_total(),&nbsp;ram_used(), boot_time()</p>
-  <p style="text-align: left;">+ convert_bytes()</p>
+  <div>* re() --&gt; repeat()</div>
+  <div>+ New Methods of System Class:</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ip_global(),&nbsp;ip_local(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ram_free(), ram_percent(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ram_total(),&nbsp;ram_used(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; boot_time()</div>
+  <div>+ convert_bytes()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.8.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">24/05/2020</td>
+  <td style="text-align: center;">24/05/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ style.switch_default()</div>
+  <div>+ style.switch_default()</div>
   <div>
-  <div style="text-align: left;">+ Now Linux&nbsp;supports&nbsp;cls()</div>
+  <div>+ Now Linux&nbsp;supports&nbsp;cls()</div>
   <div>
-  <div style="text-align: left;">+ style&nbsp;object:&nbsp;supports&nbsp;multiply,add,index</div>
+  <div>+ style&nbsp;object:&nbsp;supports&nbsp;multiply,add,index</div>
   <div>
-  <div style="text-align: left;">+ rand.choice Choose &gt;1 &amp; duplicate</div>
-  <div style="text-align: left;">* rand.choice --&gt; rand.choose</div>
+  <div>+ rand.choice Choose &gt;1 &amp; duplicate</div>
+  <div>* rand.choice --&gt; rand.choose</div>
   </div>
   </div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.7.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">&nbsp; 08/05/2020</td>
+  <td style="text-align: center;">&nbsp; 08/05/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
   <div>
-  <div style="text-align: left;">+ call_later()&nbsp;&nbsp;-&nbsp;&nbsp;wait_for()</div>
-  <div style="text-align: left;">+ terminal_size()&nbsp;&nbsp;-&nbsp;&nbsp;cwd()</div>
-  <div style="text-align: left;">+ right_port,left_port arg for progressbar()</div>
-  <div style="text-align: left;">+ file.remove() for static usage</div>
-  <div style="text-align: left;">+ self.type in file class</div>
-  <div style="text-align: left;">+ if in file(x), x is a directory:<br />x.files , x.file_list , x.all_files , x.all_files_sep</div>
-  <div style="text-align: left;">+ file.isdir() , file.isfile() for static usage.</div>
-  <div style="text-align: left;">* string() =&gt; cons_int()</div>
-  <div style="text-align: left;">* progressbar() arg names</div>
-  <div style="text-align: left;">* file.delete() and file.delete_dir()&nbsp;=&gt;&nbsp;delete()</div>
-  <div style="text-align: left;">* Change replace() and insert() args oreder</div>
+  <div>+ call_later()&nbsp;&nbsp;-&nbsp;&nbsp;wait_for()</div>
+  <div>+ terminal_size()&nbsp;&nbsp;-&nbsp;&nbsp;cwd()</div>
+  <div>+ right_port,left_port arg for progressbar()</div>
+  <div>+ file.remove() for static usage</div>
+  <div>+ self.type in file class</div>
+  <div>+ if in file(x), x is a directory:<br />x.files , x.file_list , x.all_files , x.all_files_sep</div>
+  <div>+ file.isdir() , file.isfile() for static usage.</div>
+  <div>* string() =&gt; cons_int()</div>
+  <div>* progressbar() arg names</div>
+  <div>* file.delete() and file.delete_dir()&nbsp;=&gt;&nbsp;delete()</div>
+  <div>* Change replace() and insert() args oreder</div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.5.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">21/04/2020</td>
+  <td style="text-align: center;">21/04/2020</td>
   <td style="width: 513px; height: 25px; text-align: left;">
   <div>
   <div>
   <div>+ 'replace' and insert 'functions' for tuples</div>
   <div>+ 'end' arg for style.print()</div>
   <div>+ 'self.laps' in record class will display all laps</div>
   <div>* style.text =&gt; style.print</div>
   <div>* record.stop =&gt; record.lap</div>
   <div>* now 'record.stop()' will stop recording.</div>
   </div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.3.0</td>
   <td style="width: 153px; height: 25px;">
   <p style="text-align: center;">08/04/2020</p>
   </td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ __init__ &amp; read &amp; write &amp; content&nbsp; func&nbsp;of&nbsp;file&nbsp;class</div>
-  <div style="text-align: left;">* Prgoressbar&nbsp;default&nbsp;args</div>
+  <div>+ __init__ &amp; read &amp; write &amp; content&nbsp; func&nbsp;of&nbsp;file&nbsp;class</div>
+  <div>* Prgoressbar&nbsp;default&nbsp;args</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center;">
   <p style="text-align: center;">1.0.0</p>
   </td>
   <td style="width: 153px; height: 25px;">
   <p style="text-align: center;">18/03/2020</p>
   </td>
   <td style="width: 513px; height: 25px; text-align: center;">####</td>
   </tr>
   </tbody>
 </table>
+</body>
```

### Comparing `rx7-3.2.0/README.md` & `rx7-3.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: rx7
+Version: 3.3.0
+Summary: Shortcut for most usefull functions, High API, Special Features
+Home-page: https://github.com/Ramin-RX7/RX7-Lib
+Author: Ramin RX7
+Author-email: rawmin.rx@gmail.com
+License: LGPL
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >= 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![PyPI - License](https://img.shields.io/badge/downloads-32k%2Fmonth-brightgreen?style=plastic) ![PyPI - License](https://img.shields.io/pypi/l/rx7?color=orange&style=plastic) ![PyPI - License](https://img.shields.io/badge/status-stable-success?style=plastic)
 --------------------------------------------------------
 
 "rx7" library is here to help you make your code shorter!
 --------------------------------------------------------
 
 ### \- Most Usefull function and mexthods are collected.
@@ -38,47 +51,47 @@
 
 
 <br>
 
 
 List of Functions:
 ------------------
-|                                                          |                                                                                                  |
-|----------------------------------------------------------|--------------------------------------------------------------------------------------------------|
-| p()                                                      | print() function.                                                                                |
-| repeat(function,n)                                       | Repeat F_Name function for n times.                                                              |
-| rev(v)  (REMOVED 2.4.0)                                  | Reverse v and returns it. (Everything like str,list,int)                                         |
-| read(file)                                               | Return content of the file.                                                                      |
-| write(file,mode,text)                                    | Write things you want in file content. (Read Doc String)                                         |
-| wait(n)sleep(n)                                          | Stop code executing for n seconds                                                                |
-| cls()clear()                                             | It Clears the Terminal                                                                           |
-| progressbar() (*removed in v3.1)                         | In-App Progressbar. (Read Doc String)                                                            |
-| cons_integer(Frst,Lst)                                   | Return string from Frst to Lst (Read Doc String) (v1.7)                                          |
-| force(tpl,*var)                                          | Return tpl with adding var(s) to it.                                                             |
-| erase(tpl,*var)                                          | Return tpl with removing var(s) from it.                                                         |
-| replace(tpl,ind,var)                                     | Replace tpl[ind] with var                                                                        |
-| insert(tpl,ind,var)                                      | Set tpl[ind] to var. (Note that tpl[ind] will be tpl[ind+1])                                     |
-| pop(tpl,index)                                           | Remove member with index of 'index' from a tuple                                                 |
-| wait_for(button)                                         | Waits for user to press specific button.                                                         |
-| call_later(func,args,delay)                              | Call func(args) after delay time.                                                                |
-| convert_bytes(num)                                       | convert bytes to (KB,MB,GB,TB)                                                                   |
-| Input(prompt,default)                                    | Prompt an input message with default answer (value) (ONLY ON WINDOWS)                            |
-| default_input()                                          | Same as `default_input`                                                                          |
-| restart_app()                                            | Restart running python program                                                                   |
-| active_window_title()                                    | Return Active Window Title                                                                       |
-| open_image(path)                                         | Open image with default image viewer (Mac OS is not supported)                                   |
-| download(url)                                            | To download files with memory saver and progressbar                                              |
-| extract(file,path,pwd)                                   | Extract Zip file with password to path                                                           |
-| screenshot(name)                                         | Take a screenshot and save it.                                                                   |
-| func_info(function)                                      | Print information of function                                                                    |
-| Check_Type                                               | Decorator that raise TypeError if function argument type is wrong (Read Help)                    |
-| Progressbar()                                            | Generator of progressbar() which you can use it to do some stuff between your delays (Read Help) |
-| pixel_color(X,Y)                                         | Return RGB color of pixel[X,Y]                                                                   |
-| getpass(prompt)                                          | Prompt for a password, with echo turned off.                                                     |
-| import_module(path)                                      | Return given path (file with any extension) as a Module                                          |
+|                                  |                                                                                                  |
+|----------------------------------|--------------------------------------------------------------------------------------------------|
+| p()                              | print() function.                                                                                |
+| repeat(function,n)               | Repeat F_Name function for n times.                                                              |
+| rev(v)  (REMOVED 2.4.0)          | Reverse v and returns it. (Everything like str,list,int)                                         |
+| read(file)                       | Return content of the file.                                                                      |
+| write(file,mode,text)            | Write things you want in file content. (Read Doc String)                                         |
+| wait(n)sleep(n)                  | Stop code executing for n seconds                                                                |
+| cls()clear()                     | It Clears the Terminal                                                                           |
+| progressbar() (*removed in v3.1) | In-App Progressbar. (Read Doc String)                                                            |
+| cons_integer(Frst,Lst)           | Return string from Frst to Lst (Read Doc String) (v1.7)                                          |
+| force(tpl,*var)                  | Return tpl with adding var(s) to it.                                                             |
+| erase(tpl,*var)                  | Return tpl with removing var(s) from it.                                                         |
+| replace(tpl,ind,var)             | Replace tpl[ind] with var                                                                        |
+| insert(tpl,ind,var)              | Set tpl[ind] to var. (Note that tpl[ind] will be tpl[ind+1])                                     |
+| pop(tpl,index)                   | Remove member with index of 'index' from a tuple                                                 |
+| wait_for(button)                 | Waits for user to press specific button.                                                         |
+| call_later(func,args,delay)      | Call func(args) after delay time.                                                                |
+| convert_bytes(num)               | convert bytes to (KB,MB,GB,TB)                                                                   |
+| Input(prompt,default)            | Prompt an input message with default answer (value) (ONLY ON WINDOWS)                            |
+| default_input()                  | Same as `default_input`                                                                          |
+| restart_app()                    | Restart running python program                                                                   |
+| active_window_title()            | Return Active Window Title                                                                       |
+| open_image(path)                 | Open image with default image viewer (Mac OS is not supported)                                   |
+| download(url)                    | To download files with memory saver and progressbar                                              |
+| extract(file,path,pwd)           | Extract Zip file with password to path                                                           |
+| screenshot(name)                 | Take a screenshot and save it.                                                                   |
+| func_info(function)              | Print information of function                                                                    |
+| Check_Type                       | Decorator that raise TypeError if function argument type is wrong (Read Help)                    |
+| Progressbar()                    | Generator of progressbar() which you can use it to do some stuff between your delays (Read Help) |
+| pixel_color(X,Y)                 | Return RGB color of pixel[X,Y]                                                                   |
+| getpass(prompt)                  | Prompt for a password, with echo turned off.                                                     |
+| import_module(path)              | Return given path (file with any extension) as a Module                                          |
 
 
 <br>
 
 
 <h2>List of Classes:</h2>
 
@@ -93,108 +106,113 @@
 | shuffle(iterable)        | Return shuffled version of iterable            |
 
 <br>
 
 
 <h3>&nbsp; Class System:&nbsp; &nbsp;<em>Some system actions and information.</em></h3>
 
-|                               |                                                                                  |
-|-------------------------------|----------------------------------------------------------------------------------|
-| accname()                     |         return account username you have logged in.                              |
-| pid()                         |         Get pid number of terminal and return it.                                |
-| disk_usage(path)              | ########                                                                         |
-| chdir                         | Change directory of terminal.                                                    |
-| SHUT_DOWN()                   | Shut Down the PC.                                                                |
-| RESTART()                     | Restart the PC.                                                                  |
-| terminal_size()               | Return terminal size in tuple  (columns,lines).                                  |
-| cwd()                         | Return Carrent Working Directory.                                                |
-| ip_global()                   | Returns Global IP.                                                               |
-| ip_local()                    | Returns Local IP.                                                                |
-| ram_total()                   | Returns total ram of the system.                                                 |
-| ram_used()                    | Returns Used Space of the ram of the system.                                     |
-| ram_free()                    | Returns Available (Free) space of system ram.                                    |
-| boot_time()                   | Return system boot time in seconds since the epoch.                              |
-| device_name()                 | Returns Device Name                                                              |
-| ip_website(url)               | Returns url ip address                                                           |
-| win10_notification()          | Display windows 10 notification (READ DOCSTRING) (ONLY WIN10 SUPPORTED)          |
-| cpu_count(logical=True)       |         Return the number of logical/physical CPUs in the system                 |
-| pyshell_execute_bit()         |         To determine whether Python shell is executing in 32bit or 64bit         |
-| pids()                        |                 Return a list of current running PIDs                            |
-| pid_exists(pid)               | Return True if pid exists else False                                             |
-|         cpu_percent()         |         Return the current CPU utilization as a percentage                       |
+|                         |                                                                         |
+|-------------------------|-------------------------------------------------------------------------|
+| accname()               | return account username you have logged in.                             |
+| pid()                   | Get pid number of terminal and return it.                               |
+| disk_usage(path)        | ########                                                                |
+| chdir                   | Change directory of terminal.                                           |
+| SHUT_DOWN()             | Shut Down the PC.                                                       |
+| RESTART()               | Restart the PC.                                                         |
+| terminal_size()         | Return terminal size in tuple  (columns,lines).                         |
+| cwd()                   | Return Carrent Working Directory.                                       |
+| ip_global()             | Returns Global IP.                                                      |
+| ip_local()              | Returns Local IP.                                                       |
+| ram_total()             | Returns total ram of the system.                                        |
+| ram_used()              | Returns Used Space of the ram of the system.                            |
+| ram_free()              | Returns Available (Free) space of system ram.                           |
+| boot_time()             | Return system boot time in seconds since the epoch.                     |
+| device_name()           | Returns Device Name                                                     |
+| ip_website(url)         | Returns url ip address                                                  |
+| win10_notification()    | Display windows 10 notification (READ DOCSTRING) (ONLY WIN10 SUPPORTED) |
+| cpu_count(logical=True) | Return the number of logical/physical CPUs in the system                |
+| pyshell_execute_bit()   | To determine whether Python shell is executing in 32bit or 64bit        |
+| pids()                  | Return a list of current running PIDs                                   |
+| pid_exists(pid)         | Return True if pid exists else False                                    |
+| cpu_percent()           | Return the current CPU utilization as a percentage                      |
+| os_name()               | Returns OS name of machine                                              |
 
 
 
 <br>
 
 
 <h3>&nbsp; Class Files: (Static<strong style="font-size: 14px;">&nbsp;methods)&nbsp;</strong><em style="font-size: 14px;">Actions and information about files.</em></h3>
 
-| METHOD                                                        | DESCRIPTION                                                                   |
-|---------------------------------------------------------------|-------------------------------------------------------------------------------|
-| size(path)                                                    | Return size of the file in byte(s). Also work on                              |
-| delete(path)                                                  | Use this to delete a file (Not folder).                                       |
-| rename(path)                                                  | Rename files with this function.                                              |
-| abspath(path)                                                 | Return absolute path of given path.                                           |
-| exists(path)                                                  | Return Boolean. If exists True, else: False                                   |
-| mdftime(path)                                                 | Get last modify time of the file.                                             |
-| acstime(path)                                                 | Get last access time of the file.                                             |
-| move(src,dst)                                                 | Move file from src to dst. (Read Doc String of copy func)                     |
-| copy(src,dst,metadata=True)                                   | Copy file (with metadata) from src to dst. (Also work on folders)             |
-| hide(path)                                                    | Hide given path. (It can be file or directory.)                               |
-| read_only(path,mode=True)                                     | Make file or folder read-only. (Read Doc String)                              |
-| read(path)                                                    | Return content of the path                                                    |
-| write(path,text='',...)                                       | Same as write function.                                                       |
-| isdir(path)                                                   | Return True for directory and False for others.                               |
-| isfile(path)                                                  | Return True for file and False for others.                                    |
-| is_hidden(path)                                               | Check whether path is hidden or not                                           |
-| is_readonly(path)                                             | Check whether path is readonly or not                                         |
-| search_file(pattern,path,mode)                                | search for pattern in path (Read function doc string)                         |
-| search_content(path,word)                                     | Search for word in all files in path, return list of files that contain word  |
-| mkdir(path)                                                   | Make directory (More than one if its possible!)                               |
-| generate_tree(dir_path)                                       | Returns a visual tree of dir_path                                             |
-| get_drives()                                                  | (Windows only) Get currently available drives                                 |
-| &nbsp; &nbsp; &nbsp; &nbsp; MEMBERS (Family)                  |                                                                               |
-| MEMBERS.all_exactdir                                          | List of all things those are in exact directory                               |
-| MEMBERS.files_exactdir                                        | List of files which are in exact directory                                    |
-| MEMBERS.dirs_exactdir                                         | List of dirs which are in exact directory                                     |
-| MEMBERS.files_all                                             | List of files which are in exact directory and all sub-directories            |
-| MEMBERS.files_all_sep                                         | List of files which are in exact directory and all sub-directories seprated by their directories |
-| MEMBERS.dirs_all                                              | List of directories (Exact dir and all sub-dirs)                              |
-| MEMBERS.all_all_sep                                           | List of everything thing in path (exact dir &amp; sub-dirs)                   |
+| METHOD                                       | DESCRIPTION                                                                   |
+|----------------------------------------------|-------------------------------------------------------------------------------|
+| size(path)                                   | Return size of the file in byte(s). Also work on                              |
+| delete(path)                                 | Use this to delete a file (Not folder).                                       |
+| rename(path)                                 | Rename files with this function.                                              |
+| abspath(path)                                | Return absolute path of given path.                                           |
+| exists(path)                                 | Return Boolean. If exists True, else: False                                   |
+| mdftime(path)                                | Get last modify time of the file.                                             |
+| acstime(path)                                | Get last access time of the file.                                             |
+| move(src,dst)                                | Move file from src to dst. (Read Doc String of copy func)                     |
+| copy(src,dst,metadata=True)                  | Copy file (with metadata) from src to dst. (Also work on folders)             |
+| hide(path)                                   | Hide given path. (It can be file or directory.)                               |
+| read_only(path,mode=True)                    | Make file or folder read-only. (Read Doc String)                              |
+| read(path)                                   | Return content of the path                                                    |
+| write(path,text='',...)                      | Same as write function.                                                       |
+| isdir(path)                                  | Return True for directory and False for others.                               |
+| isfile(path)                                 | Return True for file and False for others.                                    |
+| is_hidden(path)                              | Check whether path is hidden or not                                           |
+| is_readonly(path)                            | Check whether path is readonly or not                                         |
+| search_file(pattern,path,mode)               | search for pattern in path (Read function doc string)                         |
+| search_content(path,word)                    | Search for word in all files in path, return list of files that contain word  |
+| mkdir(path)                                  | Make directory (More than one if its possible!)                               |
+| generate_tree(dir_path)                      | Returns a visual tree of dir_path                                             |
+| get_drives()                                 | (Windows only) Get currently available drives                                 |
+| basename(path)                               | Returns the final component of a pathname                                     |
+| dirname(path)                                | Returns the directory component of a pathname                                 |
+| join_paths(path)                             | Joins multiple paths together and returns it                                  |
+| &nbsp; &nbsp; &nbsp; &nbsp; MEMBERS (Family) |                                                                               |
+| MEMBERS.all_exactdir                         | List of all things those are in exact directory                               |
+| MEMBERS.files_exactdir                       | List of files which are in exact directory                                    |
+| MEMBERS.dirs_exactdir                        | List of dirs which are in exact directory                                     |
+| MEMBERS.files_all                            | List of files which are in exact directory and all sub-directories            |
+| MEMBERS.files_all_sep                        | List of files which are in exact directory and all sub-directories seprated by their directories |
+| MEMBERS.dirs_all                             | List of directories (Exact dir and all sub-dirs)                              |
+| MEMBERS.all_all_sep                          | List of everything thing in path (exact dir &amp; sub-dirs)                   |
 
 
 <br>
 
 
 <h3>&nbsp; Class Style:&nbsp; &nbsp; <em>Changing text Color,BG &amp; Style. (Read Doc String)</em></h3>
 
-|                                                         |                                                             |
-|---------------------------------------------------------|-------------------------------------------------------------|
-| print\(\*values, color, BG, style, end, sep\)           | Print txt with selected color,BG,style\.\(Read Doc String\) |
-| switch\(color,BG,style\)                                | Change Terminal Attributes Until another Call\.             |
-| switch\_default\(\)                                     | Restore Terminal Attributes\.                               |
-| reset                                                   | =switch\_default                                            |
-| log\_&nbsp; \(Family\)                                  | 5 Different Style\.print with ready color and style         |
+|                                               |                                                             |
+|-----------------------------------------------|-------------------------------------------------------------|
+| print\(\*values, color, BG, style, end, sep\) | Print txt with selected color,BG,style\.\(Read Doc String\) |
+| switch\(color,BG,style\)                      | Change Terminal Attributes Until another Call\.             |
+| switch\_default\(\)                           | Restore Terminal Attributes\.                               |
+| reset                                         | =switch\_default                                            |
+| log\_&nbsp; \(Family\)                        | 5 Different Style\.print with ready color and style         |
 
 
 <br>
 
 
 <h3>&nbsp; Class Record:&nbsp; &nbsp;<em>Record time of a certain actions. (Read Doc String)</em></h3>
 
-|                                                                     |                                                                            |
-|---------------------------------------------------------------------|----------------------------------------------------------------------------|
-| __init__()                                                          | Set Start Time.                                                            |
-| self.stop(self)                                                     | Stops Recording (You can not lap anymore)                                  |
-| self.lap(self, save=True, round=15)                                 | Rreturn time between start time. if save==True: add that time to self.laps |
-| self.laps                                                           | A list that contains all laps you have done                                |
-| self.reset(self, start=False)                                       | Empty self.laps, if start is True: set start time to now                   |
-| self.last_lap(save=True)                                            | Return elapsed time from last lap (save it in self.laps if save is true)   |
-| timeit(code,setup, times,globals_) | Run the 'code' for 'times' times and return time it needs (all, not once)  |
+|                                     |                                                                            |
+|-------------------------------------|----------------------------------------------------------------------------|
+| __init__()                          | Set Start Time.                                                            |
+| self.stop(self)                     | Stops Recording (You can not lap anymore)                                  |
+| self.lap(self, save=True, round=15) | Rreturn time between start time. if save==True: add that time to self.laps |
+| self.laps                           | A list that contains all laps you have done                                |
+| self.reset(self, start=False)       | Empty self.laps, if start is True: set start time to now                   |
+| self.last_lap(save=True)            | Return elapsed time from last lap (save it in self.laps if save is true)   |
+| timeit(code,setup, times,globals_)  | Run the 'code' for 'times' times and return time it needs (all, not once)  |
+| timer(f)                            | Decorator for functions to print out how much each call takes              |
 
 
 <br>
 
 
 <h3>&nbsp; Class Decorator:&nbsp; &nbsp;<em>Useful decorators you might want to use</em></h3>
 
@@ -267,289 +285,302 @@
 
 
 Releases and Changelog:
 ---------
 
 ####        (+ for new features, \* for changes, - for removed features)
 
-<table style="height: 10px; margin-left: 10px; width: 519px;" cellpadding="5">
+<table>
   <tbody>
 
   <tr style="height: 42px;">
     <td style="width: 119px; height: 42px; text-align: center;"><strong>Version</strong></td>
     <td style="width: 153px; height: 42px; text-align: center;"><strong>Release Date</strong></td>
     <td style="width: 513px; height: 42px; text-align: center;"><strong>New Features &amp; Changes</strong></td>
   </tr>
 
+  <tr>
+    <td>
+      <p style="text-align: center;">3.3.0</p>
+    </td>
+    <td style="text-align: center;">29/04/2023</td>
+    <td style="width: 513px; height: 25px; text-align: center;">
+      <div>+ Files.basename()</div>
+      <div>+ Files.dirname()</div>
+      <div>+ Files.join_paths()</div>
+      <div>* `pre_action` and `post_action` in IO  selective_input</div>
+      <div>+ Record.timer decorator</div>
+      <div>+ System.os_name()  </div>
+    </td>
+  </tr>
 
-  <tr style="height: 25px;">
-    <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
+  <tr>
+    <td>
       <p style="text-align: center;">3.2.0</p>
     </td>
-    <td style="width: 153px; height: 25px; text-align: center;">10/03/2023</td>
+    <td style="text-align: center;">10/03/2023</td>
     <td style="width: 513px; height: 25px; text-align: center;">
-      <div style="text-align: left;">+ `environ` variable: environment variables as a dict</div>
-      <div style="text-align: left;">+ `Terminal.get_size()`</div>
-      <div style="text-align: left;">+ `exit()`: sys.exit()</div>
-      <div style="text-align: left;">+ `files.get_drives()`</div>
-      <div style="text-align: left;">+ IO.selective_input `choices` argument upgrade</div>
-      <div style="text-align: left;">+ IO.selective_input `action` parameter</div>
-      <div style="text-align: left;">- IO.selective_input `error` parameter is removed</div>
-      <div style="text-align: left;">* Fixed `files.size()` for directories</div>
-      <div style="text-align: left;">* `files.is_readonly()` now also works on Unix</div>
-      <div style="text-align: left;">* Improved module call</div>
+      <div>+ `environ` variable: environment variables as a dict</div>
+      <div>+ `Terminal.size()`</div>
+      <div>+ `exit()`: sys.exit()</div>
+      <div>+ `files.get_drives()`</div>
+      <div>+ IO.selective_input `choices` argument upgrade</div>
+      <div>+ IO.selective_input `action` parameter</div>
+      <div>- IO.selective_input `error` parameter is removed</div>
+      <div>* Fixed `files.size()` for directories</div>
+      <div>* `files.is_readonly()` now also works on Unix</div>
+      <div>* Improved module call</div>
     </td>
   </tr>
 
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">3.1.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">23/12/2022</td>
+  <td style="text-align: center;">23/12/2022</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Record.timeit has default parameters now</div>
-  <div style="text-align: left;">- removed progressbar()</div>
-  <div style="text-align: left;">* Improved Style object creation</div>
-  <div style="text-align: left;">* Improved Style.print implementation</div>
-  <div style="text-align: left;">* Improved Style.log_ methods implementation</div>
-  <div style="text-align: left;">* Terminal.run() now return exit code</div>
-  <div style="text-align: left;">- Removed "Tuple" object</div>
+  <div>+ Record.timeit has default parameters now</div>
+  <div>- removed progressbar()</div>
+  <div>* Improved Style object creation</div>
+  <div>* Improved Style.print implementation</div>
+  <div>* Improved Style.log_ methods implementation</div>
+  <div>* Terminal.run() now return exit code</div>
+  <div>- Removed "Tuple" object</div>
   </td>
   </tr>
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">3.0.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/09/2021</td>
+  <td style="text-align: center;">01/09/2021</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;"><b>+ class Internet</b></div>
-  <div style="text-align: left;"><b>+ class DateTime</b></div>
-  <div style="text-align: left;">+ "Style.log" now has time prefix</div>
-  <div style="text-align: left;">+ call = call_later</div>
-  <div style="text-align: left;">+ IO.Input()</div>
-  <div style="text-align: left;">+ IO.getpass()</div>
-  <div style="text-align: left;">* io.selective_input choices can be dict</div>
-  <div style="text-align: left;">+ System.mac_address()</div>
+  <div><b>+ class Internet</b></div>
+  <div><b>+ class DateTime</b></div>
+  <div>+ "Style.log" now has time prefix</div>
+  <div>+ call = call_later</div>
+  <div>+ IO.Input()</div>
+  <div>+ IO.getpass()</div>
+  <div>* io.selective_input choices can be dict</div>
+  <div>+ System.mac_address()</div>
   </td>
   </tr>
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.9.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/12/2020</td>
+  <td style="text-align: center;">15/12/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ <b>IO Class</b>(wait_for_input() - selective_input() - yesno_input())</div>
-  <div style="text-align: left;">+ <b>Decorator Class</b> (attach_to_all ---&nbsp;Check_Type)</div>
-  <div style="text-align: left;">* IMPORT SPEED IS 20x FASTER!</div>
-  <div style="text-align: left;">+ argv (sys.argv)</div>
-  <div style="text-align: left;">- Record.EndError</div>
-  <div style="text-align: left;">+ overload (Decorator.overload)</div>
-  <div style="text-align: left;">+ ABC,ABCMeta</div>
+  <div>+ <b>IO Class</b>(wait_for_input() - selective_input() - yesno_input())</div>
+  <div>* IMPORT SPEED IS 20x FASTER!</div>
+  <div>+ argv (sys.argv)</div>
+  <div>- Record.EndError</div>
+  <div>+ overload (Decorator.overload)</div>
+  <div>+ ABC,ABCMeta</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.8.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/11/2020</td>
+  <td style="text-align: center;">15/11/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Decorator Class (attach_to_all ---&nbsp;Check_Type)</div>
-  <div style="text-align: left;">+ pop()</div>
-  <div style="text-align: left;">+ Tuple.pop()</div>
-  <div style="text-align: left;">+ Record.timeit()</div>
+  <div>+ Decorator Class (attach_to_all --- Check_Type)</div>
+  <div>+ pop()</div>
+  <div>+ Tuple.pop()</div>
+  <div>+ Record.timeit()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.7.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/10/2020</td>
+  <td style="text-align: center;">15/10/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ getpass()</div>
-  <div style="text-align: left;">+ style.log_ Family</div>
-  <div style="text-align: left;">+ style.reset() = style.switch_default()</div>
-  <div style="text-align: left;">+ load_module()</div>
-  <div style="text-align: left;">+ record.last_lap()</div>
+  <div>+ getpass()</div>
+  <div>+ style.log_ Family</div>
+  <div>+ style.reset() = style.switch_default()</div>
+  <div>+ load_module()</div>
+  <div>+ record.last_lap()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.6.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/10/2020</td>
+  <td style="text-align: center;">01/10/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ system.cpu_percent()</div>
-  <div style="text-align: left;">+ system.pid_exists()</div>
-  <div style="text-align: left;">+ Progressbar()&nbsp;<em>(Generator)</em></div>
-  <div style="text-align: left;">+ pixel_color()</div>
+  <div>+ system.cpu_percent()</div>
+  <div>+ system.pid_exists()</div>
+  <div>+ Progressbar()<em> (Generator)</em></div>
+  <div>+ pixel_color()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.5.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/09/2020</td>
+  <td style="text-align: center;">15/09/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Check_Type decorator</div>
-  <div style="text-align: left;">+ system.pyshell_execute_bit()</div>
-  <div style="text-align: left;">+ system.pids()</div>
-  <div style="text-align: left;">+ record.lap&nbsp;round&nbsp;arg</div>
+  <div>+ Check_Type decorator</div>
+  <div>+ system.pyshell_execute_bit()</div>
+  <div>+ system.pids()</div>
+  <div>+ record.lap round arg</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.4.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/09/2020</td>
+  <td style="text-align: center;">01/09/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">* rand -&gt; random</div>
-  <div>
-  <div style="text-align: left;">+ random.shuffle()</div>
-  <div>
-  <div style="text-align: left;">+ repeat function supports parameters</div>
-  <div>
-  <div style="text-align: left;">+ sleep = wait&nbsp; &nbsp;---&nbsp; &nbsp;clear = cls&nbsp; &nbsp;---&nbsp; &nbsp;default_input = Input</div>
-  <div style="text-align: left;">+ system.cpu_count()</div>
-  </div>
-  </div>
-  </div>
+  <div>* rand -&gt; random</div>
+  <div>+ random.shuffle()</div>
+  <div>+ repeat function supports parameters</div>
+  <div>+ sleep = wait&nbsp; &nbsp;---&nbsp; &nbsp;clear = cls&nbsp; &nbsp;---&nbsp; &nbsp;default_input = Input</div>
+  <div>+ system.cpu_count()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.3.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">19/08/2020</td>
+  <td style="text-align: center;">19/08/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ extract()</p>
-  <p style="text-align: left;">+ screenshot()</p>
-  <p style="text-align: left;">+ func_info()</p>
+  <div>+ extract()</div>
+  <div>+ screenshot()</div>
+  <div>+ func_info()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.2.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">03/08/2020</td>
+  <td style="text-align: center;">03/08/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ download()</p>
-  <p style="text-align: left;">+ system.ip_website()</p>
-  <p style="text-align: left;">+ system.win10_notification</p>
+  <div>+ download()</div>
+  <div>+ system.ip_website()</div>
+  <div>+ system.win10_notification</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.1.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/07/2020</td>
+  <td style="text-align: center;">15/07/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">* style class better performance in linux</p>
-  <p style="text-align: left;">+&nbsp;<span style="text-align: center;">MEMBERS&nbsp;group&nbsp;in&nbsp;files&nbsp;class</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+ File object:&nbsp; self.basename, self.ext</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+ system.device_name()</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+&nbsp;</span><span style="text-align: center;">active_window_title() --- open_image()</span></p>
+  <div>* style class better performance in linux</div>
+  <div>+&nbsp;<span style="text-align: center;">MEMBERS&nbsp;group&nbsp;in&nbsp;files&nbsp;class</span></div>
+  <div><span style="text-align: center;">+ File object:&nbsp; self.basename, self.ext</span></div>
+  <div><span style="text-align: center;">+ system.device_name()</span></div>
+  <div><span style="text-align: center;">+&nbsp;</span><span style="text-align: center;">active_window_title() --- open_image()</span></div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;"><strong>2.0.0</strong></p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;"><strong>01/07/2020</strong></td>
+  <td style="text-align: center;"><strong>01/07/2020</strong></td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ <strong>Tuple object&nbsp; &nbsp;---&nbsp; &nbsp;rxobject</strong></p>
-  <p style="text-align: left;">+ record.reset()&nbsp; &nbsp;---&nbsp; &nbsp;record.lap new arg</p>
-  <p style="text-align: left;">+ New methods of files</p>
-  <p style="text-align: left;">&nbsp; &nbsp; &nbsp; files.is_readonly()&nbsp; &nbsp;---&nbsp; &nbsp;files.is_hidden()</p>
-  <p style="text-align: left;"><strong>&nbsp; &nbsp; &nbsp; files.search_file()&nbsp; &nbsp;---&nbsp; &nbsp;files.search_content()</strong></p>
-  <p style="text-align: left;">&nbsp; &nbsp; &nbsp; files.copy new arg</p>
-  <p style="text-align: left;"><strong>&nbsp; &nbsp; &nbsp; files.generate_tree()</strong></p>
-  <p style="text-align: left;"><strong>+ File.MEMBERS </strong>(when in File(path), path is a directory&nbsp; (self.MEMBERS.TYPE_PATH)</p>
-  <p style="text-align: left;"><strong>+ File.tree&nbsp; &nbsp; ---&nbsp; &nbsp; &nbsp;File.tree_dirs</strong></p>
-  <p style="text-align: left;"><strong>+ Input()</strong>&nbsp; <em>(Only on windows)</em></p>
-  <p style="text-align: left;">+ restart_app()</p>
+  <div>+ <strong>Tuple object</strong></div>
+  <div>rxobject</div>
+  <div>+ record.reset()</div>
+  <div>record.lap new arg</div>
+  <div>+ New methods of files</div>
+  <div>&nbsp; &nbsp; &nbsp; files.is_readonly()&nbsp; &nbsp;---&nbsp; &nbsp;files.is_hidden()</div>
+  <div>&nbsp; &nbsp; &nbsp; files.search_file()&nbsp; &nbsp;---&nbsp; &nbsp;files.search_content()</div>
+  <div>&nbsp; &nbsp; &nbsp; files.copy new arg&nbsp; &nbsp;---&nbsp; &nbsp;files.generate_tree()</div>
+  <div><strong>+ File.MEMBERS </strong>(when in File(path), path is a directory&nbsp; (self.MEMBERS.TYPE_PATH)</div>
+  <div>+ File.tree&nbsp; &nbsp; ---&nbsp; &nbsp; &nbsp;File.tree_dirs</div>
+  <div>+ Input()&nbsp; <em>(Only on windows)</em></div>
+  <div>+ restart_app()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.9.0</td>
   <td style="width: 153px; height: 25px;">&nbsp; 09/06/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">* re() --&gt; repeat()</p>
-  <p style="text-align: left;">+ New Methods of System Class:&nbsp; ip_global(),&nbsp;ip_local(),&nbsp;ram_free(), ram_percent(),&nbsp;ram_total(),&nbsp;ram_used(), boot_time()</p>
-  <p style="text-align: left;">+ convert_bytes()</p>
+  <div>* re() --&gt; repeat()</div>
+  <div>+ New Methods of System Class:</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ip_global(),&nbsp;ip_local(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ram_free(), ram_percent(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ram_total(),&nbsp;ram_used(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; boot_time()</div>
+  <div>+ convert_bytes()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.8.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">24/05/2020</td>
+  <td style="text-align: center;">24/05/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ style.switch_default()</div>
+  <div>+ style.switch_default()</div>
   <div>
-  <div style="text-align: left;">+ Now Linux&nbsp;supports&nbsp;cls()</div>
+  <div>+ Now Linux&nbsp;supports&nbsp;cls()</div>
   <div>
-  <div style="text-align: left;">+ style&nbsp;object:&nbsp;supports&nbsp;multiply,add,index</div>
+  <div>+ style&nbsp;object:&nbsp;supports&nbsp;multiply,add,index</div>
   <div>
-  <div style="text-align: left;">+ rand.choice Choose &gt;1 &amp; duplicate</div>
-  <div style="text-align: left;">* rand.choice --&gt; rand.choose</div>
+  <div>+ rand.choice Choose &gt;1 &amp; duplicate</div>
+  <div>* rand.choice --&gt; rand.choose</div>
   </div>
   </div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.7.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">&nbsp; 08/05/2020</td>
+  <td style="text-align: center;">&nbsp; 08/05/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
   <div>
-  <div style="text-align: left;">+ call_later()&nbsp;&nbsp;-&nbsp;&nbsp;wait_for()</div>
-  <div style="text-align: left;">+ terminal_size()&nbsp;&nbsp;-&nbsp;&nbsp;cwd()</div>
-  <div style="text-align: left;">+ right_port,left_port arg for progressbar()</div>
-  <div style="text-align: left;">+ file.remove() for static usage</div>
-  <div style="text-align: left;">+ self.type in file class</div>
-  <div style="text-align: left;">+ if in file(x), x is a directory:<br />x.files , x.file_list , x.all_files , x.all_files_sep</div>
-  <div style="text-align: left;">+ file.isdir() , file.isfile() for static usage.</div>
-  <div style="text-align: left;">* string() =&gt; cons_int()</div>
-  <div style="text-align: left;">* progressbar() arg names</div>
-  <div style="text-align: left;">* file.delete() and file.delete_dir()&nbsp;=&gt;&nbsp;delete()</div>
-  <div style="text-align: left;">* Change replace() and insert() args oreder</div>
+  <div>+ call_later()&nbsp;&nbsp;-&nbsp;&nbsp;wait_for()</div>
+  <div>+ terminal_size()&nbsp;&nbsp;-&nbsp;&nbsp;cwd()</div>
+  <div>+ right_port,left_port arg for progressbar()</div>
+  <div>+ file.remove() for static usage</div>
+  <div>+ self.type in file class</div>
+  <div>+ if in file(x), x is a directory:<br />x.files , x.file_list , x.all_files , x.all_files_sep</div>
+  <div>+ file.isdir() , file.isfile() for static usage.</div>
+  <div>* string() =&gt; cons_int()</div>
+  <div>* progressbar() arg names</div>
+  <div>* file.delete() and file.delete_dir()&nbsp;=&gt;&nbsp;delete()</div>
+  <div>* Change replace() and insert() args oreder</div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.5.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">21/04/2020</td>
+  <td style="text-align: center;">21/04/2020</td>
   <td style="width: 513px; height: 25px; text-align: left;">
   <div>
   <div>
   <div>+ 'replace' and insert 'functions' for tuples</div>
   <div>+ 'end' arg for style.print()</div>
   <div>+ 'self.laps' in record class will display all laps</div>
   <div>* style.text =&gt; style.print</div>
   <div>* record.stop =&gt; record.lap</div>
   <div>* now 'record.stop()' will stop recording.</div>
   </div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.3.0</td>
   <td style="width: 153px; height: 25px;">
   <p style="text-align: center;">08/04/2020</p>
   </td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ __init__ &amp; read &amp; write &amp; content&nbsp; func&nbsp;of&nbsp;file&nbsp;class</div>
-  <div style="text-align: left;">* Prgoressbar&nbsp;default&nbsp;args</div>
+  <div>+ __init__ &amp; read &amp; write &amp; content&nbsp; func&nbsp;of&nbsp;file&nbsp;class</div>
+  <div>* Prgoressbar&nbsp;default&nbsp;args</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center;">
   <p style="text-align: center;">1.0.0</p>
   </td>
   <td style="width: 153px; height: 25px;">
   <p style="text-align: center;">18/03/2020</p>
   </td>
   <td style="width: 513px; height: 25px; text-align: center;">####</td>
   </tr>
   </tbody>
-</table>
+</table>
+</body>
```

### Comparing `rx7-3.2.0/rx7/__init__.py` & `rx7-3.3.0/rx7/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,61 +6,57 @@
 Also There is Collection of most usefull function and methods from popular modules of python.
 (Read Help of Functions)
 
 Official documentation in https://github.com/Ramin-RX7/RX7-Lib
 """
 '''
 Written By RX
-Last Update: 03-07-2022
+Last Update: 04-28-2022
 '''
-__version__ = '3.2.0'
+__version__ = '3.3.0'
+
+
 """
 < Release Changes >
 
-* Fixed files.size() for directories
-* files.is_readonly now also works on Unix
-+ files.get_drives()
-+ IO.selective_input choices argument can be a function that returns True if given input is valid
-+ IO.selective_input `action` parameter is a function that takes the given input (if valid)
-    and returns the converted
-- IO.selective_input error parameter is removed
-+ exit: sys.exit
-+ environ: environment variables as a dict
-+ Terminal.get_size(): same as system.get_terminal_size()
 """
 
 
 
 
 
 #START
 
 import os   as _os
 import re   as _re
 import sys  as _sys
 import abc  as _abc
 import time as _time
 import socket   as _socket
-import typing   as _typing
 import urllib   as _urllib
 import shutil   as _shutil
 import random   as _random
 import datetime as _datetime
 import calendar as _calendar
 import subprocess as _subprocess
+import platform as _platform
 # import requests as _requests
     # imported requests in any method that uses it to improve importing speed
 import psutil as _psutil
 
+from functools import wraps
 from typing import (Any,Iterable,Optional,Callable,
                     Union,Text,Generator,Literal)
 
 
 
 
+
+
+
 argv    = _sys.argv
 ABC     = _abc.ABC
 exit = _sys.exit
 environ = _os.environ
 
 write = ...
 read  = ...
@@ -68,14 +64,16 @@
 Check_Type = ...
 overload   = ...
 Input   = default_input  = ...
 getpass = password_input = ...
 
 
 
+
+
 #######       8888888888                         888    d8b                                  #######
 ####          888                                888    Y8P                                     ####
 ####          888                                888                                            ####
 ####          8888888 888  888 88888b.   .d8888b 888888 888  .d88b.  88888b.  .d8888b           ####
 ####          888     888  888 888 "88b d88P"    888    888 d88""88b 888 "88b 88K               ####
 ####          888     888  888 888  888 888      888    888 888  888 888  888 "Y8888b.          ####
 ####          888     Y88b 888 888  888 Y88b.    Y88b.  888 Y88..88P 888  888      X88          ####
@@ -491,14 +489,16 @@
     (TUPLE FUNCTION)
     pop method that is used in lists but for tuples
     '''
     return tuple(list(tuple).pop(index))
 
 
 """
+Terminal title in mac: "\033]0;{}\007".format(title)
+
  def screen_recorder():
     from screen_recorder_sdk import screen_recorder
     #screen_recorder.enable_dev_log ()
     screen_recorder.disable_log()
     pid = 2456
     screen_recorder.init_resources(pid)
     screen_recorder.start_video_recording ('video1.mp4', 30, 8000000, True)
@@ -633,14 +633,17 @@
 
         Arg:
             iterable (Iterable): The iterable you want to shuffle it's items
 
         Return:
             Iterable[Any]: shuffled version of given iterable
         """
+        # copied = type(iterable)(iterable)
+        # random.shuffle(copied)
+        # return copied
         real_type = type(iterable)
         new_iterable = list(iterable)
 
         _random.shuffle(new_iterable)
 
         if real_type in (set,tuple):
             return real_type(new_iterable)
@@ -660,33 +663,35 @@
 class Files:
     '''
     (STATIC METHODS)\n
     Actions and information about files.\n
     (READ FUNCTIONS DOCSTRING)
 
     GET INFORMATION:
-      - exists()
-      - size()
-      - abspath()
-      - mdftime()
-      - acstime()
-      - content (read function)()
-      - is file()
-      - is dir()
-      - is readonly()
-      - is hidden()
+      - exists
+      - size
+      - abspath
+      - mdftime
+      - acstime
+      - basename
+      - dirname
+      - content
+      - is_file
+      - is_dir
+      - is_readonly
+      - is_hidden
 
     ACTIONS:
-      - remove()
-      - rename()
-      - move()
-      - copy()
-      - hide()
-      - read only()
-      - write()
+      - remove
+      - rename
+      - move
+      - copy
+      - hide
+      - read only
+      - write
     '''
     @staticmethod
     def size(path:str) -> int:
         '''
         return size of the file in byte(s).
         Also work on directories.
         '''
@@ -783,15 +788,15 @@
             if preserve_metadata: _shutil.copy2(src,dest)
             else: _shutil.copy(src,dest)
 
     @staticmethod
     def hide(path:str, mode:bool=True) -> None:
         '''
         Hide file or folder.
-        If mode==False: makes 'not hide'
+        If mode==False: unhides the file/folder
         (WINDOWS ONLY)
         '''
         try:
             import win32api, win32con
         except:
             raise ImportError('Please install pywin32 via pip')
         if mode:
@@ -956,26 +961,43 @@
                     yield from inner(path, prefix=prefix+extension, level=level-1)
                 elif not limit_to_directories:
                     yield prefix + pointer + path.name
                     files += 1
         RETURN=''
         RETURN+=dir_path.name+'\n'
         iterator = inner(dir_path, level=level)
-        for line in islice(iterator, length_limit): RETURN+=line+'\n'
-        if next(iterator, None): RETURN+=f'... length_limit, {length_limit}, reached, counted:'
-        if print_info: RETURN+=f'\n{directories} directories' + (f', {files} files' if files else '')
+        for line in islice(iterator, length_limit):
+            RETURN+=line+'\n'
+        if next(iterator, None):
+            RETURN+=f'... length_limit, {length_limit}, reached, counted:'
+        if print_info:
+            RETURN+=f'\n{directories} directories' + (f', {files} files' if files else '')
         return RETURN
 
     @staticmethod
-    def get_drives():
+    def get_drives() -> tuple:
         """WINDOWS ONLY
 
         Gets devices and drives in windows
         """
-        return [drive for drive in "CDEFGHIJKLMNOPQRSTUVWXYZ" if files.exists(f"{drive}:/")]
+        return (drive for drive in "CDEFGHIJKLMNOPQRSTUVWXYZ" if files.exists(f"{drive}:/"))
+
+    @staticmethod
+    def basename(path:str) -> str:
+        """Returns the final component of a pathname"""
+        return _os.path.basename(path)
+
+    @staticmethod
+    def join_paths(path:str, *paths) -> str:
+        return _os.path.join(path,*paths)
+
+    @staticmethod
+    def dirname(path:str) -> str:
+        """Returns the directory component of a pathname"""
+        return _os.path.dirname(path)
 
     class MEMBERS:
         @staticmethod
         def all_exactdir(dir:str):
             return _os.listdir(dir)
         @staticmethod
         def all_all_sep(dir:str):
@@ -1095,21 +1117,20 @@
             IP = '127.0.0.1'
         finally:
             s.close()
         return IP
         '''
         import platform
         class NetworkError(Exception):
-            def __init__(self, message): super().__init__(message)
+            pass
         try:
             ip = _socket.gethostbyname(_socket.gethostname())
             if ip and ip != "127.0.1.1":
                 return ip
             elif platform.system() != "Windows":
-                import subprocess
                 command = _subprocess.Popen(["hostname", "-I"],stdout=_subprocess.PIPE,stderr=_subprocess.PIPE,stdin=_subprocess.PIPE,shell=False)
                 response = list(command.communicate())
                 if len(response[0]) > 0:
                     return str(response[0])[2:-4]
                 raise NetworkError('No Network Connection')
             raise NetworkError('No Network Connection')
         except:
@@ -1212,14 +1233,17 @@
     @staticmethod
     def mac_address(formatted:bool=False) -> str:
         import uuid
         mac = uuid.getnode()
         if formatted:
             return ':'.join(['{:02x}'.format((mac >> ele) & 0xff) for ele in range(0,8*6,8)][::-1])
         return hex(mac)
+    @staticmethod
+    def os_name():
+        return _platform.system()
 system = System
 
 
 
 from colored import fg   as  _fg
 from colored import bg   as  _bg
 from colored import attr as  _attr
@@ -1254,14 +1278,15 @@
         return self.styled
     def __add__(self, other):
         if type(other)!=style:
             return self.styled+other
         else:
             return self.styled+other.styled
 
+    from pprint import pprint,pformat
 
     @staticmethod
     def print(*values,color='default', BG='default', style=None, end='\n', sep=" "):
         '''
         text(text='Hello World',color='red',BG='white')
         output ==> 'Hello World' (With red color and white BG)
         Styles: bold - underlined - reverse - hidden
@@ -1303,37 +1328,38 @@
     @staticmethod
     def switch_default():
         '''Switch Terminal Attributes to its defaults'''
         print(f'{_attr(0)}', end='')
     reset = switch_default
 
 
-    def _get_now(add_time):
-        return _time.strftime('%H:%M:%S',_time.localtime()) if add_time else ''
-    def _log(text, color='green', BG='default', style=None, add_time=True):
+    def _get_now():
+        return _time.strftime('%H:%M:%S',_time.localtime())
+    def _log(pre, text, color='', BG='default', style=None, add_time=True):
         #globals()['style'].print(text, color, BG, style=style)
-        NOW = Style._get_now(add_time)
-        Style.switch(color=color, BG=BG)
-        Style.print(f"[{NOW}]  {text}")
-        Style.switch_default()
+        if add_time:
+            NOW = f"[{Style._get_now()}]  "
+        else:
+            NOW = ""
+        Style.print(f"{NOW}{text}", color=color, BG=BG, style=style)
     @staticmethod
     def log_success(text, color='green', BG='default', style=None, add_time=True):
-        Style._log(text,color,BG,style,add_time)
+        Style._log("[+]",text,color,BG,style,add_time)
     @staticmethod
-    def log_info(text, color='grey_93', BG='default', style=None, add_time=True):
-        Style._log(text,color,BG,style,add_time)
+    def log_info(text, color='dodger_blue_1', BG='default', style=None, add_time=True):
+        Style._log("[*]",text,color,BG,style,add_time)
     @staticmethod
     def log_warning(text, color='gold_3a', BG='default', style=None, add_time=True):
-        Style._log(text,color,BG,style,add_time)
+        Style._log("[*]",text,color,BG,style,add_time)
     @staticmethod
     def log_error(text, color='red', BG='default', style=None, add_time=True):
-        Style._log(text,color,BG,style,add_time)
+        Style._log("[!]",text,color,BG,style,add_time)
     @staticmethod
     def log_critical(text, color='red_1', BG='default', style='bold', add_time=True):
-        Style._log(text,color,BG,style,add_time)
+        Style._log("[!]",text,color,BG,style,add_time)
 style = Style
 
 
 
 class Record:
     '''
     Use this method to record an action time in second.
@@ -1384,14 +1410,25 @@
         '''
         ret = (self.lap(False)-self.laps[-1]) if self.laps else self.lap(False)
         if save:
             self.laps.append(self.lap())
         return ret
 
     @staticmethod
+    def timer(function):
+        @wraps(function)
+        def wrapper(*args, **kwargs):
+            t1 = _time.time()
+            result = function(*args, **kwargs)
+            t2 = _time.time()
+            print(f"{function.__name__} : {t2-t1}")
+            return result
+        return wrapper
+
+    @staticmethod
     def timeit(code="pass",setup="pass",times=1_000_000,globals_=None):
         '''
         Run the 'code' for 'times' times and return time it needs (all, not once)
         (If you need any initialization for your 'code', put it in setup arg)
         '''
         import timeit
         return timeit.timeit(stmt=code,setup=setup,number=times,globals=globals_)
@@ -1422,14 +1459,17 @@
         return _subprocess.getoutput(command)
     @staticmethod
     def size() -> tuple:
         '''
         Return terminal size in tuple (columns,rows)
         '''
         return _os.get_terminal_size()
+
+    def clear():
+        clear()
 terminal = Terminal
 
 
 
 class Decorator:
 
     class Check_Type:
@@ -1608,94 +1648,124 @@
 overload   = Decorator.overload
 
 
 
 class IO:
 
     @staticmethod
-    def wait_for_input(prompt):
+    def wait_for_input(prompt=""):
         answer= ''
         while not answer:
             answer = input(prompt).strip()
         return answer
 
     @staticmethod
-    def selective_input(prompt:Any, choices:Iterable|Callable=None, default=None,
+    def selective_input(prompt:Any, choices:Iterable|Callable[[str],bool], default:Any=None,
                         ignore_case:bool=False, invalid_message:Any='Invalid input',
-                        action:Callable=None):
+                        pre_action:Callable=...,post_action:Callable=...):
+
+        assert (callable(pre_action )  or  pre_action==...)
+        assert (callable(post_action)  or  post_action==...)
+
+
         if not callable(choices):
             Choices = choices
             if type(choices) == dict:
                 Choices = list(choices.keys())+list(choices.values())
             if ignore_case:
-                Choices = [item.lower() for item in Choices]
+                Choices = [item.lower() for item in Choices if isinstance(item,str)]
 
         while True:
             inp = input(prompt)
+            if pre_action != ...:
+                inp = pre_action(inp)
             inp = inp.lower() if ignore_case else inp
             if callable(choices):
                 if choices(inp):
                     break
+                elif invalid_message:
+                    style.print(invalid_message, color='red')
             elif not inp:
                 if default:
                     inp = default
                     break
                 else:
                     if invalid_message:
                         style.print(invalid_message, color='red')
-            elif inp not in Choices:
+            elif inp in Choices:
+                break
+            else:
                 if invalid_message:
                     style.print(invalid_message, color='red')
-            else:
-                break
+
         if type(choices) == dict:
             try:
                 inp = choices[inp]
             except KeyError:
                 pass
-        if action and callable(action):
-            inp = action(inp)
+
+        if post_action != ...:
+            inp = post_action(inp)
+
         return inp
 
     @staticmethod
     def yesno_input(prompt,default=None):
         error= "Invalid Input" if bool(default) else ""
-        return io.selective_input(prompt,['y','yes','n','no'],default,True,error)
+        def action(inp):
+            if inp.lower() in ("yes","y"):
+                return True
+            elif inp.lower() in ("no","n"):
+                return False
+        return IO.selective_input(prompt,['y','yes','n','no'],default,True,error,action)
 
     @staticmethod
     def Input(prompt:str ='', default_value:str =''):
         '''
+        (WINDOWS ONLY)
         Make Default Value For Your Input!
-        (THIS ONLY WORK ON WINDOWS (SORRY))
         prompt is what you want and it's input(prompt) .
         default_value is what there should be after prompt.
         E.g:
         >>> Input('Is rx7 Library Easy to Learn?  ', 'Yes')
         Is rx7 Library Easy to Learn?  Yes
         '''
-
         import win32console
         _stdin = win32console.GetStdHandle(win32console.STD_INPUT_HANDLE)
         keys = []
         for c in str(default_value):
             evt = win32console.PyINPUT_RECORDType(win32console.KEY_EVENT)
             evt.Char = c
             evt.RepeatCount = 1
             evt.KeyDown = True
             keys.append(evt)
         _stdin.WriteConsoleInput(keys)
         return input(str(prompt))
 
     @staticmethod
-    def getpass(prompt):
+    def getpass(prompt:str="Password: "):
         '''
         Prompt for a password, with echo turned off.
         '''
-        import getpass as Getpass
-        return Getpass.getpass(prompt=prompt)
+        import getpass
+        return getpass.getpass(prompt=prompt)
+
+    @staticmethod
+    def regex_input(prompt,pattern,method="match"):
+        """Checks the """
+        inp = input(prompt)
+        if method == "match":
+            result = _re.match(pattern,inp)
+        elif method == "search":
+            result = _re.search(pattern,inp)
+        else:
+            raise ValueError
+        if result:
+            return True
+        return False
 io = IO
 Input   = default_input  = io.Input
 getpass = password_input = io.getpass
 
 
 
 class Internet:
@@ -2116,177 +2186,31 @@
     @staticmethod
     def get_second():
         return _time.localtime().tm_sec
 date_time = datetime = DateTime
 
 
 
+'''
+class Developer:
 
+    @staticmethod
+    def reload(module):
+        import importlib
+        importlib.reload(module)
+    @staticmethod
+    def add_module_dir(path:str):
+        _sys.path.append(path)
+    @staticmethod
+    def path():
+        return _sys.path
+    @staticmethod
+    def python_version(sep=False):
+        if sep:
+            return _platform.python_version_tuple()
+        return _platform.python_version()
+    def run_path(path):
+        import runpy
+        return runpy.runpath(path)
 
-
-
-_Auto = 0
-class _Lang:
-
-    class Constant:
-        def __new__(cls,*args,array=True):
-            cls._init = False
-            return super(_Lang.Constant, cls).__new__(cls)
-        def __init__(self,*args,array=True):
-            '''
-            if array:
-                self.__members =  args
-            else:
-                if len(args) > 1:
-                    raise ValueError
-                self.__members = args[0]
-            '''
-            self.__members = args
-            self._init = True
-
-        def __str__(self):
-            #if len(self.__members) > 1:
-                return '<'+str(self.__members)[1:-1]+'>'  #‹›
-            #return self.__members
-        def __repr__(self):
-            return '<'+str(self.__members)[1:-1]+'>'
-
-        def __setattr__(self,_attr,value):
-            if self._init:
-                raise AttributeError(f"'Constant' object does not support item assignment")
-            else:
-                super(_Lang.Constant,self).__setattr__(_attr,value)
-
-        def __getitem__(self,index):
-            return self.__members[index]
-        def __contains__(self,obj):
-            return obj in self.__members
-        def __bool__(self):
-            return bool(len(self.__members))
-        #'''
-        def __hash__(self):
-            return hash(tuple(['Constant',len(self)]+list(self.__members)))
-        #'''
-        def __len__(self):
-            #if type(self.__members) == tuple:
-                return len(self.__members)
-
-        def _dict_getter(self):
-            raise AttributeError("Conatant object has no attribute '__dict__'")
-            #return {}
-        __dict__ = property(_dict_getter)
-
-        def __dir__(self):
-            ret = list(super().__dir__())#[:-2]
-            ret.remove('_init')
-            ret.remove('_dict_getter')
-            return ret
-    const = Const = constant = Constant
-
-
-    class Array:
-
-        # Sized Array
-
-        __Type_Error = "Array of type '{}' does not accept object with type '{}'"
-
-        def __init__(self,*args,type_=_Auto,size=_Auto):
-            self.__members = []
-            if type_:
-                self.__TYPE = type_
-            else:
-                self.__TYPE = type(args[0])
-            self.__TYPE_NAME  = self.__TYPE.__name__
-            if size:
-                self.__SIZE = size
-            else:
-                self.__SIZE = len(args)
-
-            for obj in args:
-                if type(obj) == self.__TYPE:
-                    self.__members.append(obj)
-                else:
-                    raise ValueError(_Lang.Array.__Type_Error.format(self.__TYPE_NAME,type(obj).__name__))
-        def __str__(self):
-            return '{'+str(self.__members)[1:-1]+'}'  #‹›
-        def __repr__(self):
-            return '{'+str(self.__members)[1:-1]+'}'
-
-
-        def __getitem__(self,index):
-            return self.__members[index]
-
-        def __contains__(self,obj):
-            return obj in self.__members
-        def __bool__(self):
-            return bool(len(self.__members))
-
-        def __len__(self):
-            return len(self.__members)
-
-        def __setitem__(self,index,obj):
-            if type(obj) == self.__TYPE:
-                self.__members.insert(index,obj)
-                return
-            raise ValueError(_Lang.Array.__Type_Error.format(self.__TYPE_NAME,type(obj).__name__))
-        def insert(self,index,obj):
-            if type(obj) == self.__TYPE:
-                self.__members.insert(index,obj)
-                return
-            raise ValueError(_Lang.Array.__Type_Error.format(self.__TYPE_NAME,type(obj).__name__))
-        def append(self,obj):
-            if type(obj) == self.__TYPE:
-                self.__members.append(obj)
-                return
-            raise ValueError(_Lang.Array.__Type_Error.format(self.__TYPE_NAME,type(obj).__name__))
-        add = append
-        def remove(self,obj):
-            self.__members.remove(obj)
-        def pop(self,index=-1):
-            self.__members.pop(index)
-    array = Array
-
-
-    class Types:
-        Str         =  str
-        Int         =  int
-        Float       =  float
-        Set         =  set
-        Tuple       =  tuple
-        Dict        =  dict
-        List        =  list
-        Bool        =  bool
-        Bytes       =  bytes
-
-        Class       =  type
-        Type        =  type
-        Object      =  object
-
-        Lambda      =  type(lambda: None)
-        Function    =  Lambda #type(lambda: None)
-
-        #Constant   =  type(_Lang.Constant(1))
-        #Array      =  type(_Lang.Array(1,1))
-
-        Any         =   type#_typing.Any
-        Callable    =  _typing.Callable
-        Container   =  _typing.Container
-        Generator   =   Lambda #type(_f) #Not Built-in(s)   #_types.GeneratorType || _typing.Generator
-        Iterable    =  _typing.Iterable
-        Iterator    =  _typing.Iterator
-        NoReturn    =  _typing.NoReturn
-        Optional    =  _typing.Optional
-        BuiltinFunction = type(len)
-        BuiltinMethod   = type([].append)
-        Module = type(_typing)
-        Method = type(globals()['Record']().lap)
-        #Mapping     =  _typing.Mapping
-        #OrderedDict =  _typing.OrderedDict
-        #Text        =  str
-        #Union  = _typing.Union
-        #_types.AsyncGeneratorType
-    types = Types
-#setattr(_Lang,'Const',type(_Lang.Constant(1)))
-#setattr(_Lang,'Array',type(_Lang.Array(1,1)))
-
-
+'''
 #END
```

### Comparing `rx7-3.2.0/rx7/__main__.py` & `rx7-3.3.0/rx7/__main__.py`

 * *Files identical despite different names*

### Comparing `rx7-3.2.0/rx7/removed.py` & `rx7-3.3.0/rx7/removed.py`

 * *Files identical despite different names*

### Comparing `rx7-3.2.0/rx7.egg-info/PKG-INFO` & `rx7-3.3.0/rx7.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rx7
-Version: 3.2.0
+Version: 3.3.0
 Summary: Shortcut for most usefull functions, High API, Special Features
 Home-page: https://github.com/Ramin-RX7/RX7-Lib
 Author: Ramin RX7
 Author-email: rawmin.rx@gmail.com
 License: LGPL
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyPI - License](https://img.shields.io/badge/downloads-32k%2Fmonth-brightgreen?style=plastic) ![PyPI - License](https://img.shields.io/pypi/l/rx7?color=orange&style=plastic) ![PyPI - License](https://img.shields.io/badge/status-stable-success?style=plastic)
 --------------------------------------------------------
 
 "rx7" library is here to help you make your code shorter!
@@ -51,47 +51,47 @@
 
 
 <br>
 
 
 List of Functions:
 ------------------
-|                                                          |                                                                                                  |
-|----------------------------------------------------------|--------------------------------------------------------------------------------------------------|
-| p()                                                      | print() function.                                                                                |
-| repeat(function,n)                                       | Repeat F_Name function for n times.                                                              |
-| rev(v)  (REMOVED 2.4.0)                                  | Reverse v and returns it. (Everything like str,list,int)                                         |
-| read(file)                                               | Return content of the file.                                                                      |
-| write(file,mode,text)                                    | Write things you want in file content. (Read Doc String)                                         |
-| wait(n)sleep(n)                                          | Stop code executing for n seconds                                                                |
-| cls()clear()                                             | It Clears the Terminal                                                                           |
-| progressbar() (*removed in v3.1)                         | In-App Progressbar. (Read Doc String)                                                            |
-| cons_integer(Frst,Lst)                                   | Return string from Frst to Lst (Read Doc String) (v1.7)                                          |
-| force(tpl,*var)                                          | Return tpl with adding var(s) to it.                                                             |
-| erase(tpl,*var)                                          | Return tpl with removing var(s) from it.                                                         |
-| replace(tpl,ind,var)                                     | Replace tpl[ind] with var                                                                        |
-| insert(tpl,ind,var)                                      | Set tpl[ind] to var. (Note that tpl[ind] will be tpl[ind+1])                                     |
-| pop(tpl,index)                                           | Remove member with index of 'index' from a tuple                                                 |
-| wait_for(button)                                         | Waits for user to press specific button.                                                         |
-| call_later(func,args,delay)                              | Call func(args) after delay time.                                                                |
-| convert_bytes(num)                                       | convert bytes to (KB,MB,GB,TB)                                                                   |
-| Input(prompt,default)                                    | Prompt an input message with default answer (value) (ONLY ON WINDOWS)                            |
-| default_input()                                          | Same as `default_input`                                                                          |
-| restart_app()                                            | Restart running python program                                                                   |
-| active_window_title()                                    | Return Active Window Title                                                                       |
-| open_image(path)                                         | Open image with default image viewer (Mac OS is not supported)                                   |
-| download(url)                                            | To download files with memory saver and progressbar                                              |
-| extract(file,path,pwd)                                   | Extract Zip file with password to path                                                           |
-| screenshot(name)                                         | Take a screenshot and save it.                                                                   |
-| func_info(function)                                      | Print information of function                                                                    |
-| Check_Type                                               | Decorator that raise TypeError if function argument type is wrong (Read Help)                    |
-| Progressbar()                                            | Generator of progressbar() which you can use it to do some stuff between your delays (Read Help) |
-| pixel_color(X,Y)                                         | Return RGB color of pixel[X,Y]                                                                   |
-| getpass(prompt)                                          | Prompt for a password, with echo turned off.                                                     |
-| import_module(path)                                      | Return given path (file with any extension) as a Module                                          |
+|                                  |                                                                                                  |
+|----------------------------------|--------------------------------------------------------------------------------------------------|
+| p()                              | print() function.                                                                                |
+| repeat(function,n)               | Repeat F_Name function for n times.                                                              |
+| rev(v)  (REMOVED 2.4.0)          | Reverse v and returns it. (Everything like str,list,int)                                         |
+| read(file)                       | Return content of the file.                                                                      |
+| write(file,mode,text)            | Write things you want in file content. (Read Doc String)                                         |
+| wait(n)sleep(n)                  | Stop code executing for n seconds                                                                |
+| cls()clear()                     | It Clears the Terminal                                                                           |
+| progressbar() (*removed in v3.1) | In-App Progressbar. (Read Doc String)                                                            |
+| cons_integer(Frst,Lst)           | Return string from Frst to Lst (Read Doc String) (v1.7)                                          |
+| force(tpl,*var)                  | Return tpl with adding var(s) to it.                                                             |
+| erase(tpl,*var)                  | Return tpl with removing var(s) from it.                                                         |
+| replace(tpl,ind,var)             | Replace tpl[ind] with var                                                                        |
+| insert(tpl,ind,var)              | Set tpl[ind] to var. (Note that tpl[ind] will be tpl[ind+1])                                     |
+| pop(tpl,index)                   | Remove member with index of 'index' from a tuple                                                 |
+| wait_for(button)                 | Waits for user to press specific button.                                                         |
+| call_later(func,args,delay)      | Call func(args) after delay time.                                                                |
+| convert_bytes(num)               | convert bytes to (KB,MB,GB,TB)                                                                   |
+| Input(prompt,default)            | Prompt an input message with default answer (value) (ONLY ON WINDOWS)                            |
+| default_input()                  | Same as `default_input`                                                                          |
+| restart_app()                    | Restart running python program                                                                   |
+| active_window_title()            | Return Active Window Title                                                                       |
+| open_image(path)                 | Open image with default image viewer (Mac OS is not supported)                                   |
+| download(url)                    | To download files with memory saver and progressbar                                              |
+| extract(file,path,pwd)           | Extract Zip file with password to path                                                           |
+| screenshot(name)                 | Take a screenshot and save it.                                                                   |
+| func_info(function)              | Print information of function                                                                    |
+| Check_Type                       | Decorator that raise TypeError if function argument type is wrong (Read Help)                    |
+| Progressbar()                    | Generator of progressbar() which you can use it to do some stuff between your delays (Read Help) |
+| pixel_color(X,Y)                 | Return RGB color of pixel[X,Y]                                                                   |
+| getpass(prompt)                  | Prompt for a password, with echo turned off.                                                     |
+| import_module(path)              | Return given path (file with any extension) as a Module                                          |
 
 
 <br>
 
 
 <h2>List of Classes:</h2>
 
@@ -106,108 +106,113 @@
 | shuffle(iterable)        | Return shuffled version of iterable            |
 
 <br>
 
 
 <h3>&nbsp; Class System:&nbsp; &nbsp;<em>Some system actions and information.</em></h3>
 
-|                               |                                                                                  |
-|-------------------------------|----------------------------------------------------------------------------------|
-| accname()                     |         return account username you have logged in.                              |
-| pid()                         |         Get pid number of terminal and return it.                                |
-| disk_usage(path)              | ########                                                                         |
-| chdir                         | Change directory of terminal.                                                    |
-| SHUT_DOWN()                   | Shut Down the PC.                                                                |
-| RESTART()                     | Restart the PC.                                                                  |
-| terminal_size()               | Return terminal size in tuple  (columns,lines).                                  |
-| cwd()                         | Return Carrent Working Directory.                                                |
-| ip_global()                   | Returns Global IP.                                                               |
-| ip_local()                    | Returns Local IP.                                                                |
-| ram_total()                   | Returns total ram of the system.                                                 |
-| ram_used()                    | Returns Used Space of the ram of the system.                                     |
-| ram_free()                    | Returns Available (Free) space of system ram.                                    |
-| boot_time()                   | Return system boot time in seconds since the epoch.                              |
-| device_name()                 | Returns Device Name                                                              |
-| ip_website(url)               | Returns url ip address                                                           |
-| win10_notification()          | Display windows 10 notification (READ DOCSTRING) (ONLY WIN10 SUPPORTED)          |
-| cpu_count(logical=True)       |         Return the number of logical/physical CPUs in the system                 |
-| pyshell_execute_bit()         |         To determine whether Python shell is executing in 32bit or 64bit         |
-| pids()                        |                 Return a list of current running PIDs                            |
-| pid_exists(pid)               | Return True if pid exists else False                                             |
-|         cpu_percent()         |         Return the current CPU utilization as a percentage                       |
+|                         |                                                                         |
+|-------------------------|-------------------------------------------------------------------------|
+| accname()               | return account username you have logged in.                             |
+| pid()                   | Get pid number of terminal and return it.                               |
+| disk_usage(path)        | ########                                                                |
+| chdir                   | Change directory of terminal.                                           |
+| SHUT_DOWN()             | Shut Down the PC.                                                       |
+| RESTART()               | Restart the PC.                                                         |
+| terminal_size()         | Return terminal size in tuple  (columns,lines).                         |
+| cwd()                   | Return Carrent Working Directory.                                       |
+| ip_global()             | Returns Global IP.                                                      |
+| ip_local()              | Returns Local IP.                                                       |
+| ram_total()             | Returns total ram of the system.                                        |
+| ram_used()              | Returns Used Space of the ram of the system.                            |
+| ram_free()              | Returns Available (Free) space of system ram.                           |
+| boot_time()             | Return system boot time in seconds since the epoch.                     |
+| device_name()           | Returns Device Name                                                     |
+| ip_website(url)         | Returns url ip address                                                  |
+| win10_notification()    | Display windows 10 notification (READ DOCSTRING) (ONLY WIN10 SUPPORTED) |
+| cpu_count(logical=True) | Return the number of logical/physical CPUs in the system                |
+| pyshell_execute_bit()   | To determine whether Python shell is executing in 32bit or 64bit        |
+| pids()                  | Return a list of current running PIDs                                   |
+| pid_exists(pid)         | Return True if pid exists else False                                    |
+| cpu_percent()           | Return the current CPU utilization as a percentage                      |
+| os_name()               | Returns OS name of machine                                              |
 
 
 
 <br>
 
 
 <h3>&nbsp; Class Files: (Static<strong style="font-size: 14px;">&nbsp;methods)&nbsp;</strong><em style="font-size: 14px;">Actions and information about files.</em></h3>
 
-| METHOD                                                        | DESCRIPTION                                                                   |
-|---------------------------------------------------------------|-------------------------------------------------------------------------------|
-| size(path)                                                    | Return size of the file in byte(s). Also work on                              |
-| delete(path)                                                  | Use this to delete a file (Not folder).                                       |
-| rename(path)                                                  | Rename files with this function.                                              |
-| abspath(path)                                                 | Return absolute path of given path.                                           |
-| exists(path)                                                  | Return Boolean. If exists True, else: False                                   |
-| mdftime(path)                                                 | Get last modify time of the file.                                             |
-| acstime(path)                                                 | Get last access time of the file.                                             |
-| move(src,dst)                                                 | Move file from src to dst. (Read Doc String of copy func)                     |
-| copy(src,dst,metadata=True)                                   | Copy file (with metadata) from src to dst. (Also work on folders)             |
-| hide(path)                                                    | Hide given path. (It can be file or directory.)                               |
-| read_only(path,mode=True)                                     | Make file or folder read-only. (Read Doc String)                              |
-| read(path)                                                    | Return content of the path                                                    |
-| write(path,text='',...)                                       | Same as write function.                                                       |
-| isdir(path)                                                   | Return True for directory and False for others.                               |
-| isfile(path)                                                  | Return True for file and False for others.                                    |
-| is_hidden(path)                                               | Check whether path is hidden or not                                           |
-| is_readonly(path)                                             | Check whether path is readonly or not                                         |
-| search_file(pattern,path,mode)                                | search for pattern in path (Read function doc string)                         |
-| search_content(path,word)                                     | Search for word in all files in path, return list of files that contain word  |
-| mkdir(path)                                                   | Make directory (More than one if its possible!)                               |
-| generate_tree(dir_path)                                       | Returns a visual tree of dir_path                                             |
-| get_drives()                                                  | (Windows only) Get currently available drives                                 |
-| &nbsp; &nbsp; &nbsp; &nbsp; MEMBERS (Family)                  |                                                                               |
-| MEMBERS.all_exactdir                                          | List of all things those are in exact directory                               |
-| MEMBERS.files_exactdir                                        | List of files which are in exact directory                                    |
-| MEMBERS.dirs_exactdir                                         | List of dirs which are in exact directory                                     |
-| MEMBERS.files_all                                             | List of files which are in exact directory and all sub-directories            |
-| MEMBERS.files_all_sep                                         | List of files which are in exact directory and all sub-directories seprated by their directories |
-| MEMBERS.dirs_all                                              | List of directories (Exact dir and all sub-dirs)                              |
-| MEMBERS.all_all_sep                                           | List of everything thing in path (exact dir &amp; sub-dirs)                   |
+| METHOD                                       | DESCRIPTION                                                                   |
+|----------------------------------------------|-------------------------------------------------------------------------------|
+| size(path)                                   | Return size of the file in byte(s). Also work on                              |
+| delete(path)                                 | Use this to delete a file (Not folder).                                       |
+| rename(path)                                 | Rename files with this function.                                              |
+| abspath(path)                                | Return absolute path of given path.                                           |
+| exists(path)                                 | Return Boolean. If exists True, else: False                                   |
+| mdftime(path)                                | Get last modify time of the file.                                             |
+| acstime(path)                                | Get last access time of the file.                                             |
+| move(src,dst)                                | Move file from src to dst. (Read Doc String of copy func)                     |
+| copy(src,dst,metadata=True)                  | Copy file (with metadata) from src to dst. (Also work on folders)             |
+| hide(path)                                   | Hide given path. (It can be file or directory.)                               |
+| read_only(path,mode=True)                    | Make file or folder read-only. (Read Doc String)                              |
+| read(path)                                   | Return content of the path                                                    |
+| write(path,text='',...)                      | Same as write function.                                                       |
+| isdir(path)                                  | Return True for directory and False for others.                               |
+| isfile(path)                                 | Return True for file and False for others.                                    |
+| is_hidden(path)                              | Check whether path is hidden or not                                           |
+| is_readonly(path)                            | Check whether path is readonly or not                                         |
+| search_file(pattern,path,mode)               | search for pattern in path (Read function doc string)                         |
+| search_content(path,word)                    | Search for word in all files in path, return list of files that contain word  |
+| mkdir(path)                                  | Make directory (More than one if its possible!)                               |
+| generate_tree(dir_path)                      | Returns a visual tree of dir_path                                             |
+| get_drives()                                 | (Windows only) Get currently available drives                                 |
+| basename(path)                               | Returns the final component of a pathname                                     |
+| dirname(path)                                | Returns the directory component of a pathname                                 |
+| join_paths(path)                             | Joins multiple paths together and returns it                                  |
+| &nbsp; &nbsp; &nbsp; &nbsp; MEMBERS (Family) |                                                                               |
+| MEMBERS.all_exactdir                         | List of all things those are in exact directory                               |
+| MEMBERS.files_exactdir                       | List of files which are in exact directory                                    |
+| MEMBERS.dirs_exactdir                        | List of dirs which are in exact directory                                     |
+| MEMBERS.files_all                            | List of files which are in exact directory and all sub-directories            |
+| MEMBERS.files_all_sep                        | List of files which are in exact directory and all sub-directories seprated by their directories |
+| MEMBERS.dirs_all                             | List of directories (Exact dir and all sub-dirs)                              |
+| MEMBERS.all_all_sep                          | List of everything thing in path (exact dir &amp; sub-dirs)                   |
 
 
 <br>
 
 
 <h3>&nbsp; Class Style:&nbsp; &nbsp; <em>Changing text Color,BG &amp; Style. (Read Doc String)</em></h3>
 
-|                                                         |                                                             |
-|---------------------------------------------------------|-------------------------------------------------------------|
-| print\(\*values, color, BG, style, end, sep\)           | Print txt with selected color,BG,style\.\(Read Doc String\) |
-| switch\(color,BG,style\)                                | Change Terminal Attributes Until another Call\.             |
-| switch\_default\(\)                                     | Restore Terminal Attributes\.                               |
-| reset                                                   | =switch\_default                                            |
-| log\_&nbsp; \(Family\)                                  | 5 Different Style\.print with ready color and style         |
+|                                               |                                                             |
+|-----------------------------------------------|-------------------------------------------------------------|
+| print\(\*values, color, BG, style, end, sep\) | Print txt with selected color,BG,style\.\(Read Doc String\) |
+| switch\(color,BG,style\)                      | Change Terminal Attributes Until another Call\.             |
+| switch\_default\(\)                           | Restore Terminal Attributes\.                               |
+| reset                                         | =switch\_default                                            |
+| log\_&nbsp; \(Family\)                        | 5 Different Style\.print with ready color and style         |
 
 
 <br>
 
 
 <h3>&nbsp; Class Record:&nbsp; &nbsp;<em>Record time of a certain actions. (Read Doc String)</em></h3>
 
-|                                                                     |                                                                            |
-|---------------------------------------------------------------------|----------------------------------------------------------------------------|
-| __init__()                                                          | Set Start Time.                                                            |
-| self.stop(self)                                                     | Stops Recording (You can not lap anymore)                                  |
-| self.lap(self, save=True, round=15)                                 | Rreturn time between start time. if save==True: add that time to self.laps |
-| self.laps                                                           | A list that contains all laps you have done                                |
-| self.reset(self, start=False)                                       | Empty self.laps, if start is True: set start time to now                   |
-| self.last_lap(save=True)                                            | Return elapsed time from last lap (save it in self.laps if save is true)   |
-| timeit(code,setup, times,globals_) | Run the 'code' for 'times' times and return time it needs (all, not once)  |
+|                                     |                                                                            |
+|-------------------------------------|----------------------------------------------------------------------------|
+| __init__()                          | Set Start Time.                                                            |
+| self.stop(self)                     | Stops Recording (You can not lap anymore)                                  |
+| self.lap(self, save=True, round=15) | Rreturn time between start time. if save==True: add that time to self.laps |
+| self.laps                           | A list that contains all laps you have done                                |
+| self.reset(self, start=False)       | Empty self.laps, if start is True: set start time to now                   |
+| self.last_lap(save=True)            | Return elapsed time from last lap (save it in self.laps if save is true)   |
+| timeit(code,setup, times,globals_)  | Run the 'code' for 'times' times and return time it needs (all, not once)  |
+| timer(f)                            | Decorator for functions to print out how much each call takes              |
 
 
 <br>
 
 
 <h3>&nbsp; Class Decorator:&nbsp; &nbsp;<em>Useful decorators you might want to use</em></h3>
 
@@ -280,289 +285,302 @@
 
 
 Releases and Changelog:
 ---------
 
 ####        (+ for new features, \* for changes, - for removed features)
 
-<table style="height: 10px; margin-left: 10px; width: 519px;" cellpadding="5">
+<table>
   <tbody>
 
   <tr style="height: 42px;">
     <td style="width: 119px; height: 42px; text-align: center;"><strong>Version</strong></td>
     <td style="width: 153px; height: 42px; text-align: center;"><strong>Release Date</strong></td>
     <td style="width: 513px; height: 42px; text-align: center;"><strong>New Features &amp; Changes</strong></td>
   </tr>
 
+  <tr>
+    <td>
+      <p style="text-align: center;">3.3.0</p>
+    </td>
+    <td style="text-align: center;">29/04/2023</td>
+    <td style="width: 513px; height: 25px; text-align: center;">
+      <div>+ Files.basename()</div>
+      <div>+ Files.dirname()</div>
+      <div>+ Files.join_paths()</div>
+      <div>* `pre_action` and `post_action` in IO  selective_input</div>
+      <div>+ Record.timer decorator</div>
+      <div>+ System.os_name()  </div>
+    </td>
+  </tr>
 
-  <tr style="height: 25px;">
-    <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
+  <tr>
+    <td>
       <p style="text-align: center;">3.2.0</p>
     </td>
-    <td style="width: 153px; height: 25px; text-align: center;">10/03/2023</td>
+    <td style="text-align: center;">10/03/2023</td>
     <td style="width: 513px; height: 25px; text-align: center;">
-      <div style="text-align: left;">+ `environ` variable: environment variables as a dict</div>
-      <div style="text-align: left;">+ `Terminal.get_size()`</div>
-      <div style="text-align: left;">+ `exit()`: sys.exit()</div>
-      <div style="text-align: left;">+ `files.get_drives()`</div>
-      <div style="text-align: left;">+ IO.selective_input `choices` argument upgrade</div>
-      <div style="text-align: left;">+ IO.selective_input `action` parameter</div>
-      <div style="text-align: left;">- IO.selective_input `error` parameter is removed</div>
-      <div style="text-align: left;">* Fixed `files.size()` for directories</div>
-      <div style="text-align: left;">* `files.is_readonly()` now also works on Unix</div>
-      <div style="text-align: left;">* Improved module call</div>
+      <div>+ `environ` variable: environment variables as a dict</div>
+      <div>+ `Terminal.size()`</div>
+      <div>+ `exit()`: sys.exit()</div>
+      <div>+ `files.get_drives()`</div>
+      <div>+ IO.selective_input `choices` argument upgrade</div>
+      <div>+ IO.selective_input `action` parameter</div>
+      <div>- IO.selective_input `error` parameter is removed</div>
+      <div>* Fixed `files.size()` for directories</div>
+      <div>* `files.is_readonly()` now also works on Unix</div>
+      <div>* Improved module call</div>
     </td>
   </tr>
 
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">3.1.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">23/12/2022</td>
+  <td style="text-align: center;">23/12/2022</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Record.timeit has default parameters now</div>
-  <div style="text-align: left;">- removed progressbar()</div>
-  <div style="text-align: left;">* Improved Style object creation</div>
-  <div style="text-align: left;">* Improved Style.print implementation</div>
-  <div style="text-align: left;">* Improved Style.log_ methods implementation</div>
-  <div style="text-align: left;">* Terminal.run() now return exit code</div>
-  <div style="text-align: left;">- Removed "Tuple" object</div>
+  <div>+ Record.timeit has default parameters now</div>
+  <div>- removed progressbar()</div>
+  <div>* Improved Style object creation</div>
+  <div>* Improved Style.print implementation</div>
+  <div>* Improved Style.log_ methods implementation</div>
+  <div>* Terminal.run() now return exit code</div>
+  <div>- Removed "Tuple" object</div>
   </td>
   </tr>
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">3.0.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/09/2021</td>
+  <td style="text-align: center;">01/09/2021</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;"><b>+ class Internet</b></div>
-  <div style="text-align: left;"><b>+ class DateTime</b></div>
-  <div style="text-align: left;">+ "Style.log" now has time prefix</div>
-  <div style="text-align: left;">+ call = call_later</div>
-  <div style="text-align: left;">+ IO.Input()</div>
-  <div style="text-align: left;">+ IO.getpass()</div>
-  <div style="text-align: left;">* io.selective_input choices can be dict</div>
-  <div style="text-align: left;">+ System.mac_address()</div>
+  <div><b>+ class Internet</b></div>
+  <div><b>+ class DateTime</b></div>
+  <div>+ "Style.log" now has time prefix</div>
+  <div>+ call = call_later</div>
+  <div>+ IO.Input()</div>
+  <div>+ IO.getpass()</div>
+  <div>* io.selective_input choices can be dict</div>
+  <div>+ System.mac_address()</div>
   </td>
   </tr>
 
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.9.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/12/2020</td>
+  <td style="text-align: center;">15/12/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ <b>IO Class</b>(wait_for_input() - selective_input() - yesno_input())</div>
-  <div style="text-align: left;">+ <b>Decorator Class</b> (attach_to_all ---&nbsp;Check_Type)</div>
-  <div style="text-align: left;">* IMPORT SPEED IS 20x FASTER!</div>
-  <div style="text-align: left;">+ argv (sys.argv)</div>
-  <div style="text-align: left;">- Record.EndError</div>
-  <div style="text-align: left;">+ overload (Decorator.overload)</div>
-  <div style="text-align: left;">+ ABC,ABCMeta</div>
+  <div>+ <b>IO Class</b>(wait_for_input() - selective_input() - yesno_input())</div>
+  <div>* IMPORT SPEED IS 20x FASTER!</div>
+  <div>+ argv (sys.argv)</div>
+  <div>- Record.EndError</div>
+  <div>+ overload (Decorator.overload)</div>
+  <div>+ ABC,ABCMeta</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.8.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/11/2020</td>
+  <td style="text-align: center;">15/11/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Decorator Class (attach_to_all ---&nbsp;Check_Type)</div>
-  <div style="text-align: left;">+ pop()</div>
-  <div style="text-align: left;">+ Tuple.pop()</div>
-  <div style="text-align: left;">+ Record.timeit()</div>
+  <div>+ Decorator Class (attach_to_all --- Check_Type)</div>
+  <div>+ pop()</div>
+  <div>+ Tuple.pop()</div>
+  <div>+ Record.timeit()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.7.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/10/2020</td>
+  <td style="text-align: center;">15/10/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ getpass()</div>
-  <div style="text-align: left;">+ style.log_ Family</div>
-  <div style="text-align: left;">+ style.reset() = style.switch_default()</div>
-  <div style="text-align: left;">+ load_module()</div>
-  <div style="text-align: left;">+ record.last_lap()</div>
+  <div>+ getpass()</div>
+  <div>+ style.log_ Family</div>
+  <div>+ style.reset() = style.switch_default()</div>
+  <div>+ load_module()</div>
+  <div>+ record.last_lap()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.6.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/10/2020</td>
+  <td style="text-align: center;">01/10/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ system.cpu_percent()</div>
-  <div style="text-align: left;">+ system.pid_exists()</div>
-  <div style="text-align: left;">+ Progressbar()&nbsp;<em>(Generator)</em></div>
-  <div style="text-align: left;">+ pixel_color()</div>
+  <div>+ system.cpu_percent()</div>
+  <div>+ system.pid_exists()</div>
+  <div>+ Progressbar()<em> (Generator)</em></div>
+  <div>+ pixel_color()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.5.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/09/2020</td>
+  <td style="text-align: center;">15/09/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ Check_Type decorator</div>
-  <div style="text-align: left;">+ system.pyshell_execute_bit()</div>
-  <div style="text-align: left;">+ system.pids()</div>
-  <div style="text-align: left;">+ record.lap&nbsp;round&nbsp;arg</div>
+  <div>+ Check_Type decorator</div>
+  <div>+ system.pyshell_execute_bit()</div>
+  <div>+ system.pids()</div>
+  <div>+ record.lap round arg</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.4.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">01/09/2020</td>
+  <td style="text-align: center;">01/09/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">* rand -&gt; random</div>
-  <div>
-  <div style="text-align: left;">+ random.shuffle()</div>
-  <div>
-  <div style="text-align: left;">+ repeat function supports parameters</div>
-  <div>
-  <div style="text-align: left;">+ sleep = wait&nbsp; &nbsp;---&nbsp; &nbsp;clear = cls&nbsp; &nbsp;---&nbsp; &nbsp;default_input = Input</div>
-  <div style="text-align: left;">+ system.cpu_count()</div>
-  </div>
-  </div>
-  </div>
+  <div>* rand -&gt; random</div>
+  <div>+ random.shuffle()</div>
+  <div>+ repeat function supports parameters</div>
+  <div>+ sleep = wait&nbsp; &nbsp;---&nbsp; &nbsp;clear = cls&nbsp; &nbsp;---&nbsp; &nbsp;default_input = Input</div>
+  <div>+ system.cpu_count()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.3.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">19/08/2020</td>
+  <td style="text-align: center;">19/08/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ extract()</p>
-  <p style="text-align: left;">+ screenshot()</p>
-  <p style="text-align: left;">+ func_info()</p>
+  <div>+ extract()</div>
+  <div>+ screenshot()</div>
+  <div>+ func_info()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.2.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">03/08/2020</td>
+  <td style="text-align: center;">03/08/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ download()</p>
-  <p style="text-align: left;">+ system.ip_website()</p>
-  <p style="text-align: left;">+ system.win10_notification</p>
+  <div>+ download()</div>
+  <div>+ system.ip_website()</div>
+  <div>+ system.win10_notification</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;">2.1.0</p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;">15/07/2020</td>
+  <td style="text-align: center;">15/07/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">* style class better performance in linux</p>
-  <p style="text-align: left;">+&nbsp;<span style="text-align: center;">MEMBERS&nbsp;group&nbsp;in&nbsp;files&nbsp;class</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+ File object:&nbsp; self.basename, self.ext</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+ system.device_name()</span></p>
-  <p style="text-align: left;"><span style="text-align: center;">+&nbsp;</span><span style="text-align: center;">active_window_title() --- open_image()</span></p>
+  <div>* style class better performance in linux</div>
+  <div>+&nbsp;<span style="text-align: center;">MEMBERS&nbsp;group&nbsp;in&nbsp;files&nbsp;class</span></div>
+  <div><span style="text-align: center;">+ File object:&nbsp; self.basename, self.ext</span></div>
+  <div><span style="text-align: center;">+ system.device_name()</span></div>
+  <div><span style="text-align: center;">+&nbsp;</span><span style="text-align: center;">active_window_title() --- open_image()</span></div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">
   <p style="text-align: center;"><strong>2.0.0</strong></p>
   </td>
-  <td style="width: 153px; height: 25px; text-align: center;"><strong>01/07/2020</strong></td>
+  <td style="text-align: center;"><strong>01/07/2020</strong></td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">+ <strong>Tuple object&nbsp; &nbsp;---&nbsp; &nbsp;rxobject</strong></p>
-  <p style="text-align: left;">+ record.reset()&nbsp; &nbsp;---&nbsp; &nbsp;record.lap new arg</p>
-  <p style="text-align: left;">+ New methods of files</p>
-  <p style="text-align: left;">&nbsp; &nbsp; &nbsp; files.is_readonly()&nbsp; &nbsp;---&nbsp; &nbsp;files.is_hidden()</p>
-  <p style="text-align: left;"><strong>&nbsp; &nbsp; &nbsp; files.search_file()&nbsp; &nbsp;---&nbsp; &nbsp;files.search_content()</strong></p>
-  <p style="text-align: left;">&nbsp; &nbsp; &nbsp; files.copy new arg</p>
-  <p style="text-align: left;"><strong>&nbsp; &nbsp; &nbsp; files.generate_tree()</strong></p>
-  <p style="text-align: left;"><strong>+ File.MEMBERS </strong>(when in File(path), path is a directory&nbsp; (self.MEMBERS.TYPE_PATH)</p>
-  <p style="text-align: left;"><strong>+ File.tree&nbsp; &nbsp; ---&nbsp; &nbsp; &nbsp;File.tree_dirs</strong></p>
-  <p style="text-align: left;"><strong>+ Input()</strong>&nbsp; <em>(Only on windows)</em></p>
-  <p style="text-align: left;">+ restart_app()</p>
+  <div>+ <strong>Tuple object</strong></div>
+  <div>rxobject</div>
+  <div>+ record.reset()</div>
+  <div>record.lap new arg</div>
+  <div>+ New methods of files</div>
+  <div>&nbsp; &nbsp; &nbsp; files.is_readonly()&nbsp; &nbsp;---&nbsp; &nbsp;files.is_hidden()</div>
+  <div>&nbsp; &nbsp; &nbsp; files.search_file()&nbsp; &nbsp;---&nbsp; &nbsp;files.search_content()</div>
+  <div>&nbsp; &nbsp; &nbsp; files.copy new arg&nbsp; &nbsp;---&nbsp; &nbsp;files.generate_tree()</div>
+  <div><strong>+ File.MEMBERS </strong>(when in File(path), path is a directory&nbsp; (self.MEMBERS.TYPE_PATH)</div>
+  <div>+ File.tree&nbsp; &nbsp; ---&nbsp; &nbsp; &nbsp;File.tree_dirs</div>
+  <div>+ Input()&nbsp; <em>(Only on windows)</em></div>
+  <div>+ restart_app()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.9.0</td>
   <td style="width: 153px; height: 25px;">&nbsp; 09/06/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <p style="text-align: left;">* re() --&gt; repeat()</p>
-  <p style="text-align: left;">+ New Methods of System Class:&nbsp; ip_global(),&nbsp;ip_local(),&nbsp;ram_free(), ram_percent(),&nbsp;ram_total(),&nbsp;ram_used(), boot_time()</p>
-  <p style="text-align: left;">+ convert_bytes()</p>
+  <div>* re() --&gt; repeat()</div>
+  <div>+ New Methods of System Class:</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ip_global(),&nbsp;ip_local(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ram_free(), ram_percent(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; ram_total(),&nbsp;ram_used(),</div>
+  <div>&nbsp; &nbsp; &nbsp; &nbsp; boot_time()</div>
+  <div>+ convert_bytes()</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.8.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">24/05/2020</td>
+  <td style="text-align: center;">24/05/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ style.switch_default()</div>
+  <div>+ style.switch_default()</div>
   <div>
-  <div style="text-align: left;">+ Now Linux&nbsp;supports&nbsp;cls()</div>
+  <div>+ Now Linux&nbsp;supports&nbsp;cls()</div>
   <div>
-  <div style="text-align: left;">+ style&nbsp;object:&nbsp;supports&nbsp;multiply,add,index</div>
+  <div>+ style&nbsp;object:&nbsp;supports&nbsp;multiply,add,index</div>
   <div>
-  <div style="text-align: left;">+ rand.choice Choose &gt;1 &amp; duplicate</div>
-  <div style="text-align: left;">* rand.choice --&gt; rand.choose</div>
+  <div>+ rand.choice Choose &gt;1 &amp; duplicate</div>
+  <div>* rand.choice --&gt; rand.choose</div>
   </div>
   </div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.7.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">&nbsp; 08/05/2020</td>
+  <td style="text-align: center;">&nbsp; 08/05/2020</td>
   <td style="width: 513px; height: 25px; text-align: center;">
   <div>
-  <div style="text-align: left;">+ call_later()&nbsp;&nbsp;-&nbsp;&nbsp;wait_for()</div>
-  <div style="text-align: left;">+ terminal_size()&nbsp;&nbsp;-&nbsp;&nbsp;cwd()</div>
-  <div style="text-align: left;">+ right_port,left_port arg for progressbar()</div>
-  <div style="text-align: left;">+ file.remove() for static usage</div>
-  <div style="text-align: left;">+ self.type in file class</div>
-  <div style="text-align: left;">+ if in file(x), x is a directory:<br />x.files , x.file_list , x.all_files , x.all_files_sep</div>
-  <div style="text-align: left;">+ file.isdir() , file.isfile() for static usage.</div>
-  <div style="text-align: left;">* string() =&gt; cons_int()</div>
-  <div style="text-align: left;">* progressbar() arg names</div>
-  <div style="text-align: left;">* file.delete() and file.delete_dir()&nbsp;=&gt;&nbsp;delete()</div>
-  <div style="text-align: left;">* Change replace() and insert() args oreder</div>
+  <div>+ call_later()&nbsp;&nbsp;-&nbsp;&nbsp;wait_for()</div>
+  <div>+ terminal_size()&nbsp;&nbsp;-&nbsp;&nbsp;cwd()</div>
+  <div>+ right_port,left_port arg for progressbar()</div>
+  <div>+ file.remove() for static usage</div>
+  <div>+ self.type in file class</div>
+  <div>+ if in file(x), x is a directory:<br />x.files , x.file_list , x.all_files , x.all_files_sep</div>
+  <div>+ file.isdir() , file.isfile() for static usage.</div>
+  <div>* string() =&gt; cons_int()</div>
+  <div>* progressbar() arg names</div>
+  <div>* file.delete() and file.delete_dir()&nbsp;=&gt;&nbsp;delete()</div>
+  <div>* Change replace() and insert() args oreder</div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.5.0</td>
-  <td style="width: 153px; height: 25px; text-align: center;">21/04/2020</td>
+  <td style="text-align: center;">21/04/2020</td>
   <td style="width: 513px; height: 25px; text-align: left;">
   <div>
   <div>
   <div>+ 'replace' and insert 'functions' for tuples</div>
   <div>+ 'end' arg for style.print()</div>
   <div>+ 'self.laps' in record class will display all laps</div>
   <div>* style.text =&gt; style.print</div>
   <div>* record.stop =&gt; record.lap</div>
   <div>* now 'record.stop()' will stop recording.</div>
   </div>
   </div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center; text-align: center;">1.3.0</td>
   <td style="width: 153px; height: 25px;">
   <p style="text-align: center;">08/04/2020</p>
   </td>
   <td style="width: 513px; height: 25px; text-align: center;">
-  <div style="text-align: left;">+ __init__ &amp; read &amp; write &amp; content&nbsp; func&nbsp;of&nbsp;file&nbsp;class</div>
-  <div style="text-align: left;">* Prgoressbar&nbsp;default&nbsp;args</div>
+  <div>+ __init__ &amp; read &amp; write &amp; content&nbsp; func&nbsp;of&nbsp;file&nbsp;class</div>
+  <div>* Prgoressbar&nbsp;default&nbsp;args</div>
   </td>
   </tr>
-  <tr style="height: 25px;">
+  <tr>
   <td style="width: 119px; height: 25px; text-align-last: center;">
   <p style="text-align: center;">1.0.0</p>
   </td>
   <td style="width: 153px; height: 25px;">
   <p style="text-align: center;">18/03/2020</p>
   </td>
   <td style="width: 513px; height: 25px; text-align: center;">####</td>
   </tr>
   </tbody>
 </table>
+</body>
```

### Comparing `rx7-3.2.0/setup.py` & `rx7-3.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup,find_packages
 
 with open("README.md", "r") as fh:
     long_descriptions = fh.read()
 
 s = setup(
     name = "rx7",
-    version = "3.2.0",
+    version = "3.3.0",
     license = "LGPL",
     description = "Shortcut for most usefull functions, High API, Special Features",
     url = "https://github.com/Ramin-RX7/RX7-Lib",
     packages = find_packages(), # ['rx7']
     install_requires = ['colored','psutil','requests'],
        # 'pyscreeze','keyboard', 'mouse','pyautogui'
        # 'whois','win10toast' #'pywin32'
-    python_requires = ">= 3.7",
+    python_requires = ">= 3.8",
     author = "Ramin RX7",
     author_email = "rawmin.rx@gmail.com",
     classifiers = [
         'Programming Language :: Python :: 3',
     ],
     long_description = long_descriptions,
     long_description_content_type = "text/markdown",
```

