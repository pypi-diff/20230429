# Comparing `tmp/Selenium-Screenshot-2.0.0.tar.gz` & `tmp/Selenium-Screenshot-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Selenium-Screenshot-2.0.0.tar", last modified: Wed Jul 27 05:59:09 2022, max compression
+gzip compressed data, was "dist\Selenium-Screenshot-2.1.0.tar", last modified: Sat Apr 29 06:45:53 2023, max compression
```

## Comparing `Selenium-Screenshot-2.0.0.tar` & `Selenium-Screenshot-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-07-27 05:59:09.624154 Selenium-Screenshot-2.0.0/
--rw-rw-rw-   0        0        0     1088 2022-06-23 08:14:16.000000 Selenium-Screenshot-2.0.0/LICENSE
--rw-rw-rw-   0        0        0       25 2022-06-23 08:14:16.000000 Selenium-Screenshot-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3634 2022-07-27 05:59:09.624154 Selenium-Screenshot-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3085 2022-07-27 05:53:19.000000 Selenium-Screenshot-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-07-27 05:59:09.577580 Selenium-Screenshot-2.0.0/Screenshot/
--rw-rw-rw-   0        0        0     9815 2022-07-27 05:21:48.000000 Selenium-Screenshot-2.0.0/Screenshot/Screenshot.py
--rw-rw-rw-   0        0        0       26 2022-07-27 05:43:07.000000 Selenium-Screenshot-2.0.0/Screenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-27 05:59:09.608586 Selenium-Screenshot-2.0.0/Selenium_Screenshot.egg-info/
--rw-rw-rw-   0        0        0     3634 2022-07-27 05:59:09.000000 Selenium-Screenshot-2.0.0/Selenium_Screenshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2022-07-27 05:59:09.000000 Selenium-Screenshot-2.0.0/Selenium_Screenshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-27 05:59:09.000000 Selenium-Screenshot-2.0.0/Selenium_Screenshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-07-27 05:59:09.000000 Selenium-Screenshot-2.0.0/Selenium_Screenshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-07-27 05:59:09.000000 Selenium-Screenshot-2.0.0/Selenium_Screenshot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       47 2022-07-27 05:59:09.624154 Selenium-Screenshot-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1064 2022-07-27 05:36:05.000000 Selenium-Screenshot-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-27 05:59:09.608586 Selenium-Screenshot-2.0.0/test/
--rw-rw-rw-   0        0        0        2 2022-06-23 08:14:16.000000 Selenium-Screenshot-2.0.0/test/__init__.py
--rw-rw-rw-   0        0        0      987 2022-07-27 05:36:05.000000 Selenium-Screenshot-2.0.0/test/test_IEdriver.py
--rw-rw-rw-   0        0        0     2086 2022-07-27 05:36:05.000000 Selenium-Screenshot-2.0.0/test/test_chrome_driver.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/
+-rw-rw-rw-   0        0        0     4559 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3268 2023-04-29 06:33:01.000000 Selenium-Screenshot-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/Screenshot/
+-rw-rw-rw-   0        0        0     7864 2023-04-29 06:38:34.000000 Selenium-Screenshot-2.1.0/Screenshot/Screenshot.py
+-rw-rw-rw-   0        0        0       26 2023-04-26 15:12:46.000000 Selenium-Screenshot-2.1.0/Screenshot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/Selenium_Screenshot.egg-info/
+-rw-rw-rw-   0        0        0     4559 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/Selenium_Screenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/Selenium_Screenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/Selenium_Screenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/Selenium_Screenshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/Selenium_Screenshot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-29 06:33:01.000000 Selenium-Screenshot-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/test/
+-rw-rw-rw-   0        0        0        2 2023-04-26 15:12:46.000000 Selenium-Screenshot-2.1.0/test/__init__.py
+-rw-rw-rw-   0        0        0     3311 2023-04-29 06:27:06.000000 Selenium-Screenshot-2.1.0/test/test_screenshot.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:45:53.000000 Selenium-Screenshot-2.1.0/test/util/
+-rw-rw-rw-   0        0        0        0 2023-04-29 06:25:49.000000 Selenium-Screenshot-2.1.0/test/util/__init__.py
+-rw-rw-rw-   0        0        0      731 2023-04-29 06:27:06.000000 Selenium-Screenshot-2.1.0/test/util/mock_server.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `Selenium-Screenshot-2.0.0/PKG-INFO` & `Selenium-Screenshot-2.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,109 +1,94 @@
-Metadata-Version: 2.1
-Name: Selenium-Screenshot
-Version: 2.0.0
-Summary: This package is used to Clipped Images of Html Elements of Selenium Webdriver
-Home-page: https://github.com/PyWizards/Selenium_Screenshot
-Author: PyWizard org
-Author-email: py.wizard.org@gmail.com
-License: MIT
-Platform: any
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 
-**Selenium Screenshot :**
+**Selenium Screenshot:**
 
 [![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://static.pepy.tech/personalized-badge/selenium-screenshot?period=total&units=none&left_color=yellowgreen&right_color=blue&left_text=Downloads)](https://pepy.tech/project/selenium-screenshot)
 [![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![PyPI version](https://badge.fury.io/py/Selenium-Screenshot.svg)](https://badge.fury.io/py/Selenium-Screenshot)
 ![Python package](https://github.com/sam4u3/Selenium_Screenshot/workflows/Python%20package/badge.svg)
 
 
-The Selenium Screenshot is used to clipped Html Element using Selenium Webdriver
+The Selenium Screenshot is used to clip Html pages and elements using Selenium.
 
-**Installation :**
+**Installation:**
 
 `pip install Selenium-Screenshot`
 
-This Package Support Python 3.6+ only
+This package supports Python 3.6+ only.
 
-**How to Use :**
+**How to Use:**
 
-**For Full Page ScreenShot :**
+**For Full Page Screenshot:**
 
 ```python
 from Screenshot import Screenshot
 from selenium import webdriver
 
 ob = Screenshot.Screenshot()
 driver = webdriver.Chrome()
 url = "https://github.com/sam4u3/Selenium_Screenshot/tree/master/test"
 driver.get(url)
-img_url = ob.full_Screenshot(driver, save_path=r'.', image_name='Myimage.png')
+img_url = ob.full_screenshot(driver, save_path=r'.', image_name='myimage.png', is_load_at_runtime=True,
+                                          load_wait_time=3)
 print(img_url)
 driver.close()
 
 driver.quit()
 ```
 
-**For Html Element Clipping :**
+**For Html Element Clipping:**
 
 ````python
 from Screenshot import Screenshot
 from selenium import webdriver
+from selenium.webdriver.common.by import By
 
 ob = Screenshot.Screenshot()
 driver = webdriver.Chrome()
 url = "https://github.com/sam4u3/Selenium_Screenshot/blob/master/Screenshot/Screenshot_Clipping.py"
 driver.get(url)
 
-element = driver.find_element_by_class_name('signup-prompt')
-img_url = ob.get_element(driver, element, r'.')
+element = driver.find_element(By.XPATH, "//img[@title='Donate via PayPal']")
+img_url = ob.get_element(driver, element, save_path=r'.', image_name='paypal.png')
 print(img_url)
-
 driver.close()
-
 driver.quit()
 
 ````
 
-**For Html Element Clipping with Hiding Element :**
+**For Html Element Clipping with Hiding Element:**
 
 ````python
 from Screenshot import Screenshot
 from selenium import webdriver
 
 ob = Screenshot.Screenshot()
 driver = webdriver.Chrome()
 url = "https://github.com/sam4u3"
 driver.get(url)
-Hide_elements = ['class=avatar width-full height-full avatar-before-user-status']  # Use full class name
-img_url = ob.full_Screenshot(driver, save_path=r'.', elements=Hide_elements, image_name='Myimage.png')
+hide_elements = ['class=position-relative js-header-wrapper ']
+img_url = ob.full_screenshot(driver, save_path=r'.', image_name='myimage.png',
+                                          hide_elements=hide_elements)
 print(img_url)
 driver.close()
 
 driver.quit()
 
 
 ````
 **Limitation:**
 
 - Screenshot can take only 10000 of height of website
 
 
-**Contact Information :**
+**Contact Information:**
 
 [Email:py.wizard.org@gmail.com](mailto::py.wizard.org@gmail.com)
 
-**Donation :**
+**Donation:**
 
-If you have found my softwares to be of any use to you, do consider helping me pay my internet bills. This would encourage me to create many such softwares.
+If you have found my software to be of any use to you, do consider helping me pay my internet bills. This would encourage me to maintain and create more projects.
 
 <a href="https://www.paypal.me/sam4u3" target="_blank"><img src="https://raw.githubusercontent.com/aha999/DonateButtons/master/Paypal.png" alt="Donate via PayPal" title="Donate via PayPal" /></a>
```

#### html2text {}

```diff
@@ -1,45 +1,39 @@
-Metadata-Version: 2.1 Name: Selenium-Screenshot Version: 2.0.0 Summary: This
-package is used to Clipped Images of Html Elements of Selenium Webdriver Home-
-page: https://github.com/PyWizards/Selenium_Screenshot Author: PyWizard org
-Author-email: py.wizard.org@gmail.com License: MIT Platform: any Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Requires-Python:
->=3.6.1 Description-Content-Type: text/markdown License-File: LICENSE [!
-[forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) **Selenium Screenshot :** [![Open Source
-Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://
-github.com/ellerbrock/open-source-badges/) [![License: MIT](https://
+[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-
+with-python.svg)](https://www.python.org/) **Selenium Screenshot:** [![Open
+Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)]
+(https://github.com/ellerbrock/open-source-badges/) [![License: MIT](https://
 img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/
 MIT) [![Downloads](https://static.pepy.tech/personalized-badge/selenium-
 screenshot?period=total&units=none&left_color=yellowgreen&right_color=blue&left_text=Downloads)]
 (https://pepy.tech/project/selenium-screenshot) [![Python 3.6](https://
 img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/
 release/python-360/) [![PyPI version](https://badge.fury.io/py/Selenium-
 Screenshot.svg)](https://badge.fury.io/py/Selenium-Screenshot) ![Python
 package](https://github.com/sam4u3/Selenium_Screenshot/workflows/
-Python%20package/badge.svg) The Selenium Screenshot is used to clipped Html
-Element using Selenium Webdriver **Installation :** `pip install Selenium-
-Screenshot` This Package Support Python 3.6+ only **How to Use :** **For Full
-Page ScreenShot :** ```python from Screenshot import Screenshot from selenium
+Python%20package/badge.svg) The Selenium Screenshot is used to clip Html pages
+and elements using Selenium. **Installation:** `pip install Selenium-
+Screenshot` This package supports Python 3.6+ only. **How to Use:** **For Full
+Page Screenshot:** ```python from Screenshot import Screenshot from selenium
 import webdriver ob = Screenshot.Screenshot() driver = webdriver.Chrome() url =
 "https://github.com/sam4u3/Selenium_Screenshot/tree/master/test" driver.get
-(url) img_url = ob.full_Screenshot(driver, save_path=r'.',
-image_name='Myimage.png') print(img_url) driver.close() driver.quit() ``` **For
-Html Element Clipping :** ````python from Screenshot import Screenshot from
-selenium import webdriver ob = Screenshot.Screenshot() driver =
-webdriver.Chrome() url = "https://github.com/sam4u3/Selenium_Screenshot/blob/
+(url) img_url = ob.full_screenshot(driver, save_path=r'.',
+image_name='myimage.png', is_load_at_runtime=True, load_wait_time=3) print
+(img_url) driver.close() driver.quit() ``` **For Html Element Clipping:**
+````python from Screenshot import Screenshot from selenium import webdriver
+from selenium.webdriver.common.by import By ob = Screenshot.Screenshot() driver
+= webdriver.Chrome() url = "https://github.com/sam4u3/Selenium_Screenshot/blob/
 master/Screenshot/Screenshot_Clipping.py" driver.get(url) element =
-driver.find_element_by_class_name('signup-prompt') img_url = ob.get_element
-(driver, element, r'.') print(img_url) driver.close() driver.quit() ```` **For
-Html Element Clipping with Hiding Element :** ````python from Screenshot import
-Screenshot from selenium import webdriver ob = Screenshot.Screenshot() driver =
-webdriver.Chrome() url = "https://github.com/sam4u3" driver.get(url)
-Hide_elements = ['class=avatar width-full height-full avatar-before-user-
-status'] # Use full class name img_url = ob.full_Screenshot(driver,
-save_path=r'.', elements=Hide_elements, image_name='Myimage.png') print
+driver.find_element(By.XPATH, "//img[@title='Donate via PayPal']") img_url =
+ob.get_element(driver, element, save_path=r'.', image_name='paypal.png') print
+(img_url) driver.close() driver.quit() ```` **For Html Element Clipping with
+Hiding Element:** ````python from Screenshot import Screenshot from selenium
+import webdriver ob = Screenshot.Screenshot() driver = webdriver.Chrome() url =
+"https://github.com/sam4u3" driver.get(url) hide_elements = ['class=position-
+relative js-header-wrapper '] img_url = ob.full_screenshot(driver,
+save_path=r'.', image_name='myimage.png', hide_elements=hide_elements) print
 (img_url) driver.close() driver.quit() ```` **Limitation:** - Screenshot can
-take only 10000 of height of website **Contact Information :** [Email:
-py.wizard.org@gmail.com](mailto::py.wizard.org@gmail.com) **Donation :** If you
-have found my softwares to be of any use to you, do consider helping me pay my
-internet bills. This would encourage me to create many such softwares. [Donate
-via_PayPal]
+take only 10000 of height of website **Contact Information:** [Email:
+py.wizard.org@gmail.com](mailto::py.wizard.org@gmail.com) **Donation:** If you
+have found my software to be of any use to you, do consider helping me pay my
+internet bills. This would encourage me to maintain and create more projects.
+[Donate_via_PayPal]
```

### Comparing `Selenium-Screenshot-2.0.0/Screenshot/Screenshot.py` & `Selenium-Screenshot-2.1.0/Screenshot/Screenshot.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from selenium.webdriver.remote.webelement import WebElement
 
 
 class Screenshot:
     """
        #================================================================================================================#
        #                                          Class: Screenshot                                                     #
-       #                                    Purpose: Captured full and element screenshot using selenium                #
+       #                                    Purpose: Capture full and element screenshot using Selenium                #
        #                                    a) Capture full webpage as image                                            #
        #                                    b) Capture element screenshots                                              #
        #================================================================================================================#
     """
 
     def __init__(self):
         """
@@ -26,38 +26,28 @@
         Returns:
             N/A
         Raises:
             N/A
         """
         pass
 
-    @staticmethod
-    # Take temporary screenshot of the web page to get the size of the image
-    def __get_screen_size(driver: WebDriver) -> dict:
-        driver.get_screenshot_as_file('screenshot.png')
-        image = Image.open('screenshot.png')
-        width, height = image.size
-
-        return {'width': width, 'height': height}
-
-    def full_Screenshot(self, driver: WebDriver, save_path: str = '', image_name: str = 'selenium_full_screenshot.png',
-                        elements: list = None, is_load_at_runtime: bool = False, load_wait_time: int = 5, multi_images: bool = False) -> str:
+    def full_screenshot(self, driver: WebDriver, save_path: str = '', image_name: str = 'selenium_full_screenshot.png',
+                        hide_elements: list = None, is_load_at_runtime: bool = False, load_wait_time: int = 5) -> str:
         """
         Take full screenshot of web page
         Args:
-            driver: The Selenium web driver object
-            save_path: The path where to store screenshot
-            image_name: The name of screenshot image
-            elements: List of Xpath of elements to hide from web pages
-            is_load_at_runtime: Page Load at runtime
-            load_wait_time: The Wait time while loading full screen
-            multi_images: The flag is uses to capture multiple images and create single image in vertical format
+            driver: Web driver instance
+            save_path: Path where to save image
+            image_name: The name of the image
+            hide_elements: List of Xpath elements to hide from web page
+            is_load_at_runtime: Page loads at runtime
+            load_wait_time: The wait time while loading full screen
 
         Returns:
-            str : The path of image
+            str: The image path
         """
         image_name = os.path.abspath(save_path + '/' + image_name)
 
         final_page_height = 0
         original_size = driver.get_window_size()
 
         if is_load_at_runtime:
@@ -66,16 +56,17 @@
                 if page_height != final_page_height and final_page_height <= 10000:
                     driver.execute_script("window.scrollTo(0, {})".format(page_height))
                     time.sleep(load_wait_time)
                     final_page_height = page_height
                 else:
                     break
 
+        self.hide_elements(driver, hide_elements)
+
         if isinstance(driver, webdriver.Ie):
-            self.hide_elements(driver, elements)
             required_width = driver.execute_script('return document.body.parentNode.scrollWidth')
             driver.set_window_size(required_width, final_page_height)
             driver.save_screenshot(image_name)
             driver.set_window_size(original_size['width'], original_size['height'])
             return image_name
 
         else:
@@ -96,122 +87,102 @@
                 while ii < total_width:
                     top_width = ii + viewport_width
                     if top_width > total_width:
                         top_width = total_width
                     rectangles.append((ii, i, top_width, top_height))
                     ii = ii + viewport_width
                 i = i + viewport_height
-            stitched_image = None
+            stitched_image = Image.new('RGB', (total_width, total_height))
             previous = None
             part = 0
 
-            # This value indicates if is the first part of the screenshot, or it is the rest of the screenshot
-            init_canvas = True
-            # Get the screenshot and save the dimensions of the image, this will be useful for create a
-            # correct canvas with correct dimensions
-            # and not show images with a wrong size or cut
-            size_screenshot = self.__get_screen_size(driver)
-            # Get temporary sum of height of the total pages
-            height_canvas = size_screenshot['height'] * len(rectangles)
-
-            # Compare if the screenshot it's only one part and assign the correct dimensions of the screenshot size
-            # Or assign the height of the total screenshot
-            if multi_images:
-                # Assign the height of the total screenshot at canvas even if not used at the moment
-                stitched_image = Image.new('RGB', (size_screenshot['width'], height_canvas))
-            else:
-                # Assign the dimensions corresponding to the size of the uniq screenshot
-                stitched_image = Image.new('RGB', (size_screenshot['width'], size_screenshot['height']))
-
-            # This constant is used top offset the image in the canvas
-            jump = round(size_screenshot['height'] / 2)
-            # With take multiple screenshots this value is used to adjust the position of the image in the canvas
-            # This value know update every time the screenshot is taken
-            top_offset = jump
-
             for rectangle in rectangles:
                 if previous is not None:
                     driver.execute_script("window.scrollTo({0}, {1})".format(rectangle[0], rectangle[1]))
                     time.sleep(1)
-                    self.hide_elements(driver, elements)
+
+                self.hide_elements(driver, hide_elements)
 
                 file_name = "part_{0}.png".format(part)
                 driver.get_screenshot_as_file(file_name)
                 screenshot = Image.open(file_name)
 
                 if rectangle[1] + viewport_height > total_height:
-                    offset = (rectangle[0], rectangle[1] + top_offset)
+                    offset = (rectangle[0], total_height - viewport_height)
                 else:
-                    if init_canvas:
-                        offset = (rectangle[0], rectangle[1])
-                        init_canvas = False
-                    else:
-                        offset = (rectangle[0], rectangle[1] + top_offset)
-                        top_offset = jump + top_offset
+                    offset = (rectangle[0], rectangle[1])
 
                 stitched_image.paste(screenshot, offset)
                 del screenshot
                 os.remove(file_name)
                 part = part + 1
                 previous = rectangle
             save_path = os.path.abspath(os.path.join(save_path, image_name))
             stitched_image.save(save_path)
             return save_path
 
-    def get_element(self, driver: WebDriver, element: WebElement, save_location: str, image_name: str = 'cropped_screenshot.png', to_hide: list = None) -> str:
+    def get_element(self, driver: WebDriver, element: WebElement, save_path: str, image_name: str = 'cropped_screenshot.png', hide_elements: list = None) -> str:
         """
          Usage:
-             Capture Element screenshot as a image
+             Capture element screenshot as an image
          Args:
              driver: Web driver instance
-             element : The element on web page to be captured
-             save_location  : Path where to save image
+             element: The element on the web page to be captured
+             save_path: Path where to save image
+             image_name: The name of the image
+             hide_elements: List of Xpath elements to hide from web page
          Returns:
-             img_url(str) : The path of image
+             img_url(str): The image path
          Raises:
              N/A
          """
-        image = self.full_Screenshot(driver, save_path=save_location, image_name='clipping_shot.png', elements=to_hide, multi_images=True)
+        image = self.full_screenshot(driver, save_path=save_path, image_name='clipping_shot.png', hide_elements=hide_elements)
+        # Need to scroll to top, to get absolute coordinates
+        driver.execute_script("window.scrollTo(0, 0)")
         location = element.location
         size = element.size
         x = location['x']
         y = location['y']
         w = size['width']
         h = size['height']
         width = x + w
         height = y + h
 
         image_object = Image.open(image)
         image_object = image_object.crop((int(x), int(y), int(width), int(height)))
-        img_url = os.path.abspath(os.path.join(save_location, f"{image_name}.png"))
+        img_url = os.path.abspath(os.path.join(save_path, image_name))
         image_object.save(img_url)
+
+        image_object.close()
+        os.remove(image)
+
         return img_url
 
     @staticmethod
     def hide_elements(driver: WebDriver, elements: list) -> None:
         """
          Usage:
              Hide elements from web page
          Args:
-             driver : The path of chromedriver
-             elements : The element on web page to be hide
+             driver: Web driver instance
+             elements: The elements on the web page to hide
          Returns:
              N/A
          Raises:
              N/A
          """
         if elements is not None:
             try:
                 for e in elements:
                     sp_xpath = e.split('=')
                     if 'id=' in e.lower():
                         driver.execute_script(
-                            "document.getElementById('{}').setAttribute('style', 'display:none;');".format(
+                            "document.getElementById('{}').setAttribute('style', 'display:none !important;');".format(
                                 sp_xpath[1]))
                     elif 'class=' in e.lower():
                         driver.execute_script(
-                            "document.getElementsByClassName('{}')[0].setAttribute('style', 'display:none;');".format(
+                            "document.getElementsByClassName('{}')[0].setAttribute('style', 'display:none !important;');".format(
                                 sp_xpath[1]))
                     else:
                         print('For Hiding Element works with ID and Class Selector only')
             except Exception as Error:
                 print('Error : ', str(Error))
```

### Comparing `Selenium-Screenshot-2.0.0/setup.py` & `Selenium-Screenshot-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 
 # This call to setup() does all the work
 setup(
     name="Selenium-Screenshot",
-    version="2.0.0",
+    version="2.1.0",
     description="This package is used to Clipped Images of Html Elements of Selenium Webdriver",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/PyWizards/Selenium_Screenshot",
     author="PyWizard org",
     author_email="py.wizard.org@gmail.com",
     license="MIT",
```

