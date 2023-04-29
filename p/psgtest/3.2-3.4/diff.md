# Comparing `tmp/psgtest-3.2.tar.gz` & `tmp/psgtest-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psgtest-3.2.tar", last modified: Sat Apr 22 14:35:21 2023, max compression
+gzip compressed data, was "dist\psgtest-3.4.tar", last modified: Sat Apr 29 11:50:19 2023, max compression
```

## Comparing `psgtest-3.2.tar` & `psgtest-3.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 14:35:21.000000 psgtest-3.2/
--rw-rw-rw-   0        0        0     8368 2023-04-22 14:35:21.000000 psgtest-3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest/
--rw-rw-rw-   0        0        0    40591 2023-04-22 14:27:57.000000 psgtest-3.2/psgtest/psgtest.py
--rw-rw-rw-   0        0        0    16958 2021-11-04 18:03:39.000000 psgtest-3.2/psgtest/psgtest_icon.ico
--rw-rw-rw-   0        0        0    20186 2021-10-30 20:48:11.000000 psgtest-3.2/psgtest/psgtest_icon.png
--rw-rw-rw-   0        0        0       23 2021-11-12 18:21:37.000000 psgtest-3.2/psgtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     8368 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       27 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0      295 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 14:35:21.000000 psgtest-3.2/psgtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6206 2023-04-22 14:29:57.000000 psgtest-3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 14:35:21.000000 psgtest-3.2/setup.cfg
--rw-rw-rw-   0        0        0     1481 2023-04-22 14:29:57.000000 psgtest-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 11:50:19.000000 psgtest-3.4/
+-rw-rw-rw-   0        0        0     8679 2023-04-29 11:50:19.000000 psgtest-3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 11:50:19.000000 psgtest-3.4/psgtest/
+-rw-rw-rw-   0        0        0    41232 2023-04-29 11:49:42.000000 psgtest-3.4/psgtest/psgtest.py
+-rw-rw-rw-   0        0        0    16958 2021-11-04 18:03:39.000000 psgtest-3.4/psgtest/psgtest_icon.ico
+-rw-rw-rw-   0        0        0    20186 2021-10-30 20:48:11.000000 psgtest-3.4/psgtest/psgtest_icon.png
+drwxrwxrwx   0        0        0        0 2023-04-29 11:50:19.000000 psgtest-3.4/psgtest.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-29 11:50:19.000000 psgtest-3.4/psgtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-29 11:50:19.000000 psgtest-3.4/psgtest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     8679 2023-04-29 11:50:19.000000 psgtest-3.4/psgtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2023-04-29 11:50:19.000000 psgtest-3.4/psgtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      275 2023-04-29 11:50:19.000000 psgtest-3.4/psgtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 11:50:19.000000 psgtest-3.4/psgtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6445 2023-04-29 11:48:45.000000 psgtest-3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 11:50:19.000000 psgtest-3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1481 2023-04-29 11:49:42.000000 psgtest-3.4/setup.py
```

### Comparing `psgtest-3.2/PKG-INFO` & `psgtest-3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psgtest
-Version: 3.2
+Version: 3.4
 Summary: Run your Python programs, capture the output, using your choice of interpreters
 Home-page: https://github.com/PySimpleGUI/psgtest
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Description: 
         <p align="center">
@@ -83,14 +83,23 @@
         You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
         
         Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
         
         
         ## Release Notes
         
+        ### 3.4   29-Apr-2023
+        
+        
+        - Allow non-python programs to be run.  If the file does not end in .py or .pyw, then the file will be executed directly
+        
+        ### 3.3   23-Apr-2023
+        
+        - Remove the entry from sp_to_filename when killing process
+        
         ### 3.2   22-Apr-2023
         
         - Added piped output for regression testing
         - Added cleanup of processes when exiting. If any processes are running, they will be killed.
         
         ### 3.0   21-Apr-2023
```

### Comparing `psgtest-3.2/psgtest/psgtest.py` & `psgtest-3.4/psgtest/psgtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import subprocess
 import PySimpleGUI as sg
 import time
 import psutil
 import signal
 
-version = '3.2'
+version = '3.4'
 
 """
                              dP                       dP   
                              88                       88   
 88d888b. .d8888b. .d8888b. d8888P .d8888b. .d8888b. d8888P 
 88'  `88 Y8ooooo. 88'  `88   88   88ooood8 Y8ooooo.   88   
 88.  .88       88 88.  .88   88   88.  ...       88   88   
@@ -19,14 +19,16 @@
 dP                 d8888P
 
 
 3.0 21-Apr-2023 - Expanded regression tests. Now works correctly. Added ability to run across all interpreters. Made regression threaded.
 3.1 21-Apr-2023 - Removed "Edit Me" button. Instead you should use the right-click Edit Me that is standard in PySimpleGUI utilities
 3.2 23-Apr-2023 - Added piped output for Regression Tests - now creates tabs for tests when running regression and will keep open any that fail
                   Added cleaning up of all potentially running processes upon exit. Makes quitting with lots of tests running MUCH easier since don't have to manually kill them
+3.3 23-Apr-2023 - Remove the entry from sp_to_filename when killing process
+3.4 29-Apr-2023 - Allow non-python programs to be run.  If the file does not end in .py or .pyw, then the file will be executed directly
 
     Copyright 2021, 2022, 2023 PySimpleGUI
 """
 
 
 DEFAULT_OUTPUT_SIZE = (80,5)
 file_list_dict = {}
@@ -199,33 +201,33 @@
     """
     if pid == os.getpid():
         raise RuntimeError("I refuse to kill myself")
     parent = psutil.Process(pid)
     parent.send_signal(sig)
     sg.Print(f'tried killing {pid} with parent {parent}')
 
-def kill_proc_tree(pid, sig=signal.SIGTERM, include_parent=True,
-                   timeout=None, on_terminate=None):
+def kill_proc_tree(pid, sig=signal.SIGTERM, include_parent=True, timeout=None, on_terminate=None):
     """Kill a process tree (including grandchildren) with signal
     "sig" and return a (gone, still_alive) tuple.
     "on_terminate", if specified, is a callabck function which is
     called as soon as a child terminates.
     """
     try:
         if pid == os.getpid():
             raise RuntimeError("I refuse to kill myself")
         parent = psutil.Process(pid)
         children = parent.children(recursive=True)
         if include_parent:
             children.append(parent)
         for p in children:
             p.send_signal(sig)
-        gone, alive = psutil.wait_procs(children, timeout=timeout,
-                                        callback=on_terminate)
-    except:
+        gone, alive = psutil.wait_procs(children, timeout=timeout, callback=on_terminate)
+    except Exception as e:
+        print(f'Error killing process {e}')
+        sg.cprint(f'Error killing process {e}', colors='white on red')
         return (None, None)
     return (gone, alive)
 
 
 '''
 MM"""""""`MM                                                       oo                   
 MM  mmmm,  M                                                                            
@@ -264,24 +266,15 @@
         tcprint(window, f'Testing interpreter {interpreter_path}', colors='white on blue')
         for iteration in range(iterations):
             tcprint(window, f'Starting Iteration Number {iteration}', 'white on red')
             for file, file_to_run in get_next_program(program_list):
                 tcprint(window, f'Starting {file_to_run}', 'white on purple')
                 sp = sg.execute_command_subprocess(interpreter_path, f'"{file_to_run}"', pipe_output=pipe_output)
                 if pipe_output:
-                    sp_to_filename[sp] = file
-                    mline_key = f'{file}-MLINE-'
-                    if mline_key not in sp_to_mline_dict.values():
-                        tab = make_output_tab(file, mline_key, file)
-                        window['-TABGROUP-'].add_tab(tab)
-                    else:
-                        if not window[file].visible:
-                            window[file].update(visible=True)
-                    sp_to_mline_dict[sp] = mline_key
-                    window[file].select()
+                    window.write_event_value('-MAKE TAB-', (sp, file))
                     window.start_thread(lambda: piped_output_thread(window, sp, regression=True), '-PIPE THREAD DONE-')
 
                 if kill_after is not None:
                     window.timer_start(kill_after * 1000, ('-TIMER THREAD-', sp), repeating=False)
                     if (block_count+1) % block_size == 0:
                         time.sleep(kill_after)
                 block_count += 1
@@ -426,20 +419,23 @@
 M  MM'  MM' .M 88 88'  `88 88'  `88 88'  `88 88  88  88 
 M  `' . '' .MM 88 88    88 88.  .88 88.  .88 88.88b.88' 
 M    .d  .dMMM dP dP    dP `88888P8 `88888P' 8888P Y8P  
 MMMMMMMMMMMMMM
 '''
 
 
-def make_window(sp_to_mline_dict=None, sp_to_filename=None):
+def make_window():
     """
     Creates the main window
     :return: The main window object
     :rtype: (sg.Window)
     """
+    global file_list_dict, sp_to_mline_dict, sp_to_filename
+
+
     icon = b'iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAYAAAAeP4ixAAAABmJLR0QA/wD/AP+gvaeTAAADv0lEQVRogd2Zy0tVQRzHP1bkDa1NtCgtolQIKwlcCJYtFRRsX0S7+gPS9tqDFlmLHhi1lhSF8LHQDKQnLYOgiMRF5SbBV6SW3Ra/3+mcbuece+aeOcfsC8O5zuM739/M/GZ+M0I6KAf6gHlN/UBlSn1bQzkwA2Rz0gxQtoa6jNGHCB9EhJcBQ5r3YA11GWMeEe0d/d2aN2urkw22iELwXb9FPmU/UujfGnqQ0R9C/KUcGNa8njXU9RdG+duRTdOTuCL8ptsUWQscEFPLJksioHAhVgYiDWdPBTZnxNYSKwg2ZuSpBY7Yzm4Tzg6UVP1Q/Dc+kqQh6zbi9S6VKBGv1aVlE15hUSLedWFIlIh3XTi7I9BGCJQ6vCPcT3DE2+dT/59BIyJqSv+uAr7g7+wVWmdK8xpTVRqCDPAWEdXuyS9DHHtOUx+uEWjdrLbNpKI0Dy4igt4BxQbtNgNvtG1nArqMcARYAX4CDQW0b9C2K8q1JigGXiMj2h2Dp1s5XmM2o9ZwRQVMAltj8JQA75XrsgVdRqhDXkBWgeMW+Oo9fEct8EVCBtdJr1nk7cLdxbZY5A3EDeK/muRL15M2ogGZ/qQNWaWwXTASMshZkQWuJtWJcjvnUiIH5eWkO1AU4/rgRdvkNcihFbSrHAJGgGVNw0B1jP6OaV8rwOEYPH9gA/AKGaGbPuWHcO8f3jRHPGNuKc9LLF0HzijhR/wPvhEtH0WCwgpgDDeMLxTbgE/KczoGDwClwGclO+lTXgQsafl+T36F5n0j3mieUp5PqqVgXFKiZwGCvIZ4Q/RKgg1pAcaBRWBBfzcH9F8EPFeuSwVZAOwAviJOVxtSz7n5jSEGVAKPcB8fvHBCfr8UFMrXqoavqskYHdrBQJ561Yhj5wqbBQ546rVo/hJwHtipqQ13VoNmZkDLO0yNKMV9l6qPUL8acewlZDkN5hgB8Fj5zvu0d26L4wH89bhX5ZIIen7jnDZ8YdIoD5wteqdP2S4tmw9p/0LrnPUrDHoOatXvvWgaU8F9/baG1srBNGL9HotCxpWzzafsAuFLC2Cv1pk26dRxvlh7dw6acZ29HVlOuxAjlgl3dpAYzGkfGZPaKGzbLQSdmG+/Dg5qvQ8mHd7RRr2mSiOgGVlCC+Q/EL3oVU23TTrbj5y8zguJzSVmilLgrmpZBPaZErQgI5ZFnj+7gCbkBdHmP1FzsUn7aNI+nafXBaLNnC9qgAmSv9rmSxPkuZdEjUzrgBPICVsFbAc2RmxrilXkBH+HBKsPkTtJKH4B042N7RpiCBAAAAAASUVORK5CYII='
     sg.set_options(icon=icon)
     theme = get_theme()
     if not theme:
         theme = sg.OFFICIAL_PYSIMPLEGUI_THEME
     sg.theme(theme)
     # First the window layout...2 columns
@@ -579,15 +575,18 @@
             sg.cprint(f'No valid interpreter has been chosen for {current_interpreter}', c='white on red')
             return
 
 
         for file, file_to_run in get_next_program(list_of_programs):
             sg.cprint(file_to_run, text_color='white', background_color='purple')
             pipe_output = values['-SHOW OUTPUT-']
-            sp = sg.execute_command_subprocess(interpreter_path, f'"{file_to_run}"', pipe_output=pipe_output)
+            if file_to_run.endswith(('.py', '.pyw')):
+                sp = sg.execute_command_subprocess(interpreter_path, f'"{file_to_run}"', pipe_output=pipe_output)
+            else:
+                sp = sg.execute_command_subprocess(f'"{file_to_run}"', pipe_output=pipe_output)
             # sg.Print(sg.obj_to_string_single_obj(sp))
             sp_to_filename[sp] = file
             mline_key = f'{file}-MLINE-'
             if mline_key not in sp_to_mline_dict.values():
                 tab = make_output_tab(file, mline_key, file)
                 window['-TABGROUP-'].add_tab(tab)
             else:
@@ -613,18 +612,17 @@
     file_list = get_file_list()
     try:
         window = make_window()
     except Exception as e:
         if sg.popup_yes_no('Exception making the Window... likely means a corrupt settings file.', f'Exception: {e}', 'Do you want to clear your settings?', title='Exception making window') == 'Yes':
             sg.user_settings_delete_filename(filename='psgtest.json')
             sg.popup_auto_close('Settings file deleted... please restart the program')
-            exit()
         else:
             sg.popup_auto_close('Cancelling operation... See what you can do about the problem...')
-            exit()
+        exit()
     window['-FILTER NUMBER-'].update(f'{len(file_list)} files')
     counter = 0
     dont_close_tab = {}
     regression_programs = []
     try:
         while True:
             event, values = window.read()
@@ -653,14 +651,16 @@
                 kill_proc_tree(thread_sp.pid)
                 try:
                     file = sp_to_filename[thread_sp]
                     if not dont_close_tab.get(file, False):
                         window[file].update(visible=False)
                 except:
                     pass
+                del sp_to_filename[thread_sp]
+                # del sp_to_mline_dict[thread_sp]
             elif event == '-THREAD-':                   # received message from thread to display
                 thread_sp = values['-THREAD-'][0]
                 line = values['-THREAD-'][1]
                 sg.cprint(line, key=sp_to_mline_dict[thread_sp])
                 if 'Traceback' in line:
                     sg.popup_error(f'Error during running {sp_to_filename[thread_sp]}', non_blocking=True)
                     dont_close_tab[sp_to_filename[thread_sp]] = True
@@ -680,25 +680,37 @@
                 for interpreter in interpreter_dict.keys():
                     if values['-SINGLE FILE-']:
                         start_batch([values['-SINGLE FILE-']], interpreter)
                     else:
                         start_batch(values['-DEMO LIST-'], interpreter)
             elif event == 'Version':
                 sg.cprint(sg.get_versions(), c='white on green')
+            elif event == '-MAKE TAB-':
+                sp, file = values[event]
+                sp_to_filename[sp] = file
+                mline_key = f'{file}-MLINE-'
+                if mline_key not in sp_to_mline_dict.values():
+                    tab = make_output_tab(file, mline_key, file)
+                    window['-TABGROUP-'].add_tab(tab)
+                else:
+                    if not window[file].visible:
+                        window[file].update(visible=True)
+                sp_to_mline_dict[sp] = mline_key
+                window[file].select()
             elif event == '-FILTER-':
                 new_list = [i for i in file_list if values['-FILTER-'].lower() in i.lower()]
                 window['-DEMO LIST-'].update(new_list)
                 window['-FILTER NUMBER-'].update(f'{len(new_list)} files')
             elif event == '-FOCUS FILTER-':
                 window['-FILTER-'].set_focus()
             elif event == 'Settings':
                 if settings_window() is True:
                     pipe_output = values['-SHOW OUTPUT-']
                     window.close()
-                    window = make_window(sp_to_mline_dict, sp_to_filename)
+                    window = make_window()
                     file_list_dict = get_file_list_dict()
                     file_list = get_file_list()
                     window['-FILTER NUMBER-'].update(f'{len(file_list)} files')
                     window['-SHOW OUTPUT-'].update(pipe_output)
             elif event == 'Clear':
                 file_list = get_file_list()
                 window['-FILTER-'].update('')
```

### Comparing `psgtest-3.2/psgtest/psgtest_icon.ico` & `psgtest-3.4/psgtest/psgtest_icon.ico`

 * *Files identical despite different names*

### Comparing `psgtest-3.2/psgtest/psgtest_icon.png` & `psgtest-3.4/psgtest/psgtest_icon.png`

 * *Files identical despite different names*

### Comparing `psgtest-3.2/psgtest.egg-info/PKG-INFO` & `psgtest-3.4/psgtest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psgtest
-Version: 3.2
+Version: 3.4
 Summary: Run your Python programs, capture the output, using your choice of interpreters
 Home-page: https://github.com/PySimpleGUI/psgtest
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Description: 
         <p align="center">
@@ -83,14 +83,23 @@
         You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
         
         Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
         
         
         ## Release Notes
         
+        ### 3.4   29-Apr-2023
+        
+        
+        - Allow non-python programs to be run.  If the file does not end in .py or .pyw, then the file will be executed directly
+        
+        ### 3.3   23-Apr-2023
+        
+        - Remove the entry from sp_to_filename when killing process
+        
         ### 3.2   22-Apr-2023
         
         - Added piped output for regression testing
         - Added cleanup of processes when exiting. If any processes are running, they will be killed.
         
         ### 3.0   21-Apr-2023
```

### Comparing `psgtest-3.2/README.md` & `psgtest-3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,23 @@
 You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
 
 Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
 
 
 ## Release Notes
 
+### 3.4   29-Apr-2023
+
+
+- Allow non-python programs to be run.  If the file does not end in .py or .pyw, then the file will be executed directly
+
+### 3.3   23-Apr-2023
+
+- Remove the entry from sp_to_filename when killing process
+
 ### 3.2   22-Apr-2023
 
 - Added piped output for regression testing
 - Added cleanup of processes when exiting. If any processes are running, they will be killed.
 
 ### 3.0   21-Apr-2023
```

### Comparing `psgtest-3.2/setup.py` & `psgtest-3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             return f.read()
     except IOError:
         return ''
 
 
 setuptools.setup(
     name="psgtest",
-    version="3.2",
+    version="3.4",
     author="PySimpleGUI",
     author_email="PySimpleGUI@PySimpleGUI.org",
     description="Run your Python programs, capture the output, using your choice of interpreters",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/PySimpleGUI/psgtest",
     packages=['psgtest'],
```

