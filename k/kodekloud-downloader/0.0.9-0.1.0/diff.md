# Comparing `tmp/kodekloud-downloader-0.0.9.tar.gz` & `tmp/kodekloud-downloader-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodekloud-downloader-0.0.9.tar", max compression
+gzip compressed data, was "kodekloud-downloader-0.1.0.tar", max compression
```

## Comparing `kodekloud-downloader-0.0.9.tar` & `kodekloud-downloader-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    14478 2023-04-24 15:03:07.269100 kodekloud-downloader-0.0.9/README.md
--rw-r--r--   0        0        0     1102 2023-04-24 15:03:15.241229 kodekloud-downloader-0.0.9/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-24 15:03:07.273100 kodekloud-downloader-0.0.9/src/kodekloud_downloader/__init__.py
--rw-r--r--   0        0        0     1843 2023-04-24 15:03:07.273100 kodekloud-downloader-0.0.9/src/kodekloud_downloader/cli.py
--rw-r--r--   0        0        0      134 2023-04-24 15:03:07.273100 kodekloud-downloader-0.0.9/src/kodekloud_downloader/enums.py
--rw-r--r--   0        0        0     2239 2023-04-24 15:03:07.273100 kodekloud-downloader-0.0.9/src/kodekloud_downloader/helpers.py
--rw-r--r--   0        0        0     3043 2023-04-24 15:03:07.273100 kodekloud-downloader-0.0.9/src/kodekloud_downloader/main.py
--rw-r--r--   0        0        0     2010 2023-04-24 15:03:07.273100 kodekloud-downloader-0.0.9/src/kodekloud_downloader/models.py
--rw-r--r--   0        0        0     1604 2023-04-24 15:03:07.273100 kodekloud-downloader-0.0.9/src/kodekloud_downloader/yt_dlp_patch.py
--rw-r--r--   0        0        0    15769 2023-04-24 15:03:16.712026 kodekloud-downloader-0.0.9/setup.py
--rw-r--r--   0        0        0    15366 2023-04-24 15:03:16.713453 kodekloud-downloader-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    14559 2023-04-29 09:51:40.609709 kodekloud-downloader-0.1.0/README.md
+-rw-r--r--   0        0        0     1102 2023-04-29 09:51:49.537732 kodekloud-downloader-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-29 09:51:40.609709 kodekloud-downloader-0.1.0/src/kodekloud_downloader/__init__.py
+-rw-r--r--   0        0        0     1883 2023-04-29 09:51:40.609709 kodekloud-downloader-0.1.0/src/kodekloud_downloader/cli.py
+-rw-r--r--   0        0        0      134 2023-04-29 09:51:40.609709 kodekloud-downloader-0.1.0/src/kodekloud_downloader/enums.py
+-rw-r--r--   0        0        0     4643 2023-04-29 09:51:40.609709 kodekloud-downloader-0.1.0/src/kodekloud_downloader/helpers.py
+-rw-r--r--   0        0        0     4506 2023-04-29 09:51:40.609709 kodekloud-downloader-0.1.0/src/kodekloud_downloader/main.py
+-rw-r--r--   0        0        0     2010 2023-04-29 09:51:40.609709 kodekloud-downloader-0.1.0/src/kodekloud_downloader/models.py
+-rw-r--r--   0        0        0     1604 2023-04-29 09:51:40.609709 kodekloud-downloader-0.1.0/src/kodekloud_downloader/yt_dlp_patch.py
+-rw-r--r--   0        0        0    15851 2023-04-29 09:51:50.983354 kodekloud-downloader-0.1.0/setup.py
+-rw-r--r--   0        0        0    15447 2023-04-29 09:51:50.984990 kodekloud-downloader-0.1.0/PKG-INFO
```

### Comparing `kodekloud-downloader-0.0.9/README.md` & `kodekloud-downloader-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 
 ---
 
 ## Features
 
 - [x] Download video lessons in selected quality
 - [x] Organizes downloaded content in a structured folder hierarchy
-- [ ] Download resources (PDFs, etc.) alongside video lessons
+- [x] Download resources (PDFs, etc.) alongside video lessons
 
 ---
 
 ## Prerequisites
 
+- **User need to enroll in the course before using the cli tool to download it**
 - Python 3.8 or higher
 - ffmpeg
 
 <details>
     <summary>How to Install FFmpeg on Linux, Mac, and Windows</summary>
 
 # How to Install FFmpeg on Linux, Mac, and Windows
```

### Comparing `kodekloud-downloader-0.0.9/pyproject.toml` & `kodekloud-downloader-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodekloud-downloader"
-version = "v0.0.9"
+version = "v0.1.0"
 description = "Simple downloaded for https://kodekloud.com/"
 readme = "README.md"
 authors = ["Roy, Debakar <debakar.roy@outlook.com>"]
 repository = "https://github.com/debakarr/kodekloud-downloader"
 packages = [
     { include = "kodekloud_downloader", from = "src" },
 ]
```

### Comparing `kodekloud-downloader-0.0.9/src/kodekloud_downloader/cli.py` & `kodekloud-downloader-0.1.0/src/kodekloud_downloader/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 from pathlib import Path
 from typing import Union
 
 import click
 import validators
 
 from kodekloud_downloader.enums import Quality
-from kodekloud_downloader.helpers import select_course
+from kodekloud_downloader.helpers import select_courses
 from kodekloud_downloader.main import download_course
 from kodekloud_downloader.models import get_all_course
 
 
 @click.group()
 @click.option("-v", "--verbose", count=True, help="Increase log level verbosity")
 def kodekloud(verbose):
-    logging.basicConfig(
-        format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
-    )
+    logging.basicConfig(format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO)
     if verbose == 1:
         logging.getLogger().setLevel(logging.INFO)
     elif verbose >= 2:
         logging.getLogger().setLevel(logging.DEBUG)
 
 
 @kodekloud.command()
@@ -43,25 +41,24 @@
     "-c",
     required=True,
     help="Cookie file. Course should be accessible via this.",
 )
 def dl(course_url, quality: str, output_dir: Union[Path, str], cookie):
     if course_url is None:
         courses = get_all_course()
-        selected_course = select_course(courses)
-        download_course(
-            url=selected_course.link,
-            cookie=cookie,
-            quality=quality,
-            output_dir=output_dir,
-        )
+        selected_courses = select_courses(courses)
+        for selected_course in selected_courses:
+            download_course(
+                url=selected_course.link,
+                cookie=cookie,
+                quality=quality,
+                output_dir=output_dir,
+            )
     elif validators.url(course_url):
-        download_course(
-            url=course_url, cookie=cookie, quality=quality, output_dir=output_dir
-        )
+        download_course(url=course_url, cookie=cookie, quality=quality, output_dir=output_dir)
     else:
         logging.error("Please enter a valid URL")
         SystemExit(1)
 
 
 if __name__ == "__main__":
     kodekloud()
```

### Comparing `kodekloud-downloader-0.0.9/src/kodekloud_downloader/models.py` & `kodekloud-downloader-0.1.0/src/kodekloud_downloader/models.py`

 * *Files identical despite different names*

### Comparing `kodekloud-downloader-0.0.9/src/kodekloud_downloader/yt_dlp_patch.py` & `kodekloud-downloader-0.1.0/src/kodekloud_downloader/yt_dlp_patch.py`

 * *Files identical despite different names*

### Comparing `kodekloud-downloader-0.0.9/setup.py` & `kodekloud-downloader-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'yt-dlp>=2023.3.4,<2024.0.0']
 
 entry_points = \
 {'console_scripts': ['kodekloud = kodekloud_downloader.cli:kodekloud']}
 
 setup_kwargs = {
     'name': 'kodekloud-downloader',
-    'version': '0.0.9',
+    'version': '0.1.0',
     'description': 'Simple downloaded for https://kodekloud.com/',
-    'long_description': "# KodeKloud Downloader\n\n## Disclaimer\nPlease read the following disclaimer carefully before using the Downloader CLI Tool.\n\n- The CLI Tool is intended for personal use only. By using this tool, you agree to use it at your own risk and assume full responsibility for any consequences that may arise from its use. The developers and contributors of this tool are not responsible for any damages or losses that may occur from its use.\n\n- The use of this tool to download premium courses is for educational purposes only. You must have the proper authorization or permission from the course provider to access the content legally.\n\n- It is strictly prohibited to distribute or share the downloaded content through any means, including but not limited to uploading to file-sharing platforms, torrent sites, or any other form of digital or physical distribution. Doing so is a violation of copyright laws and may result in legal consequences.\n\n---\n\n## Features\n\n- [x] Download video lessons in selected quality\n- [x] Organizes downloaded content in a structured folder hierarchy\n- [ ] Download resources (PDFs, etc.) alongside video lessons\n\n---\n\n## Prerequisites\n\n- Python 3.8 or higher\n- ffmpeg\n\n<details>\n    <summary>How to Install FFmpeg on Linux, Mac, and Windows</summary>\n\n# How to Install FFmpeg on Linux, Mac, and Windows\n\nFFmpeg is a powerful and flexible multimedia processing tool that can handle a wide range of tasks, such as video and audio conversion, streaming, and recording. In this guide, we will show you how to install FFmpeg on Linux, Mac, and Windows operating systems.\n\n## Linux\n\n### Ubuntu and Debian-based distributions\n\n1.  Update the package lists for upgrades and new package installations.\n\n`sudo apt update`\n\n1.  Install FFmpeg using the following command:\n\n`sudo apt install ffmpeg`\n\n### Fedora\n\n1.  Install FFmpeg using the following command:\n\n`sudo dnf install ffmpeg`\n\n### Arch Linux and Manjaro\n\n1.  Install FFmpeg using the following command:\n\n`sudo pacman -S ffmpeg`\n\n## Mac\n\n### Using Homebrew\n\nIf you don't have Homebrew installed, you can install it by following the instructions on the [official Homebrew website](https://brew.sh/).\n\nUpdate Homebrew to ensure you have the latest package information:\n\n`brew update`\n\n1.  Install FFmpeg using the following command:\n\n`brew install ffmpeg`\n\n### Using MacPorts\n\nIf you don't have MacPorts installed, you can install it by following the instructions on the [official MacPorts website](https://www.macports.org/install.php).\n\nUpdate MacPorts to ensure you have the latest package information:\n\n`sudo port selfupdate`\n\n1.  Install FFmpeg using the following command:\n\n`sudo port install ffmpeg`\n\n## Windows\n\n### Using Chocolatey\n\nIf you don't have Chocolatey installed, you can install it by following the instructions on the [official Chocolatey website](https://chocolatey.org/install).\n\nOpen an elevated Command Prompt (run as Administrator) and install FFmpeg using the following command:\n\n`choco install ffmpeg`\n\n### Using Scoop\n\nIf you don't have Scoop installed, you can install it by following the instructions on the [official Scoop website](https://scoop.sh/).\n\nOpen a PowerShell terminal and install FFmpeg using the following command:\n\n`scoop install ffmpeg`\n\nAfter following these steps, FFmpeg should be installed on your system. You can check the installation by running the following command in your terminal or command prompt:\n\n`ffmpeg -version`\n\nThis will display the FFmpeg version and build information, confirming that the installation was successful.\n\n</details>\n\n\n\n## How to get cookie\n- Sign in to kodekloud.com\n- Download extension such as [Get cookies.txt LOCALLY](https://chrome.google.com/webstore/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc/related)\n- Download the cookie and save it in some location (You can name it something like `cookie.txt`).\n\n![](/static/cookie-demo.png)\n\n## 💻 Installation\n\nTo install kodekloud-downloader, simply run the following command:\n\n```console\npip install -U kodekloud-downloader\n```\n\nYou can also install the latest main changes:\n```console\npip install -U git+https://github.com/debakarr/kodekloud-downloader.git\n```\n\n## 📚 Usage\n\nAfter installing the package, you can use the `kodekloud dl` command to download shows from the command line.\n\n```css\nkodekloud dl --help\nUsage: kodekloud dl [OPTIONS] [COURSE_URL]\n\nOptions:\n  -q, --quality [360p|480p|540p|720p|1080p]\n                                  Quality of the video to be downloaded.\n  -o, --output-dir TEXT           Output directory where downloaded files will\n                                  be store.\n  -c, --cookie TEXT               Cookie to download the courses.  [required]\n  --help                          Show this message and exit.\n```\n\nHere is an example:\n\n### 🔍 Download entire course from list of available course in current folder\n\n```css\nkodekloud dl -o . -c /path/to/cookie.txt\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| No. | Name                                                                        | Type    | Categories                                                 |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| 1   | Ultimate Certified Kubernetes Application Developer (CKAD) Mock Exam Series | Premium | Challenges, Containers, Kubernetes                         |\n| 2   | GCP DevOps Project                                                          | Premium | Cloud, GCP                                                 |\n| 3   | 12 Factor App                                                               | Premium | Productivity                                               |\n| 4   | AZ-305: Microsoft Azure Solutions Architect Expert                          | Premium | Certification, Cloud, Devops                               |\n| 5   | Ultimate Certified Kubernetes Administrator (CKA) Mock Exam Series          | Free    | Container Orchestration, Kubernetes, Devops, Certification |\n| 6   | AWS Lambda                                                                  | Premium | AWS, Cloud                                                 |\n| 7   | Linux Professional Institute LPIC-1 Exam 101                                | Premium | Certification, Linux                                       |\n| 8   | Advanced Golang                                                             | Premium | Programming                                                |\n| 9   | Prometheus Certified Associate (PCA)                                        | Premium | Certification, Kubernetes, Monitoring                      |\n| 10  | GCP Cloud Digital Leader Certification                                      | Premium | Cloud, GCP, Certification                                  |\n| 11  | OpenShift 4                                                                 | Premium | Container Orchestration, Devops, Red Hat                   |\n| 12  | HashiCorp : Terraform Cloud                                                 | Premium | Cloud, Devops, HashiCorp                                   |\n| 13  | ArgoCD                                                                      | Premium | CI/CD, Devops, Kubernetes                                  |\n| 14  | Amazon Elastic Container Service (AWS ECS)                                  | Free    | AWS, Devops                                                |\n| 15  | Red Hat Certified System Administrator(RHCSA)                               | Premium | Devops, Linux, Red Hat, Certification                      |\n| 16  | Open Source for Beginners                                                   | Premium | Productivity                                               |\n| 17  | Kustomize                                                                   | Premium | Devops, Kubernetes                                         |\n| 18  | DevSecOps – Kubernetes DevOps & Security                                    | Premium | Devops, DevSecOps, Kubernetes                              |\n| 19  | AZ-104: Microsoft Azure Administrator                                       | Premium | Cloud, Devops, Certification                               |\n| 20  | DevOps Interview Preparation Course                                         | Premium | Devops                                                     |\n| 21  | Terraform Challenges                                                        | Free    | Challenges, Devops, IAC                                    |\n| 22  | HashiCorp Certified: Consul Associate Certification                         | Premium | Devops, HashiCorp                                          |\n| 23  | HashiCorp Certified: Vault Associate Certification                          | Premium | Devops, HashiCorp                                          |\n| 24  | Kubernetes Challenges                                                       | Free    | Challenges, Devops                                         |\n| 25  | Linux Challenges                                                            | Free    | Challenges, Devops, Linux                                  |\n| 26  | HashiCorp Certified: Vault Operations Professional 2022                     | Premium | Container Orchestration, Containers, Devops, HashiCorp     |\n| 27  | CKS – Challenges                                                            | Free    | Challenges, Container Orchestration, Containers, Devops    |\n| 28  | Linux Foundation Certified System Administrator (LFCS)                      | Premium | Devops, Linux, Certification                               |\n| 29  | Jenkins                                                                     | Premium | Automation, CI/CD, Devops                                  |\n| 30  | Golang                                                                      | Premium | Devops, Programming                                        |\n| 31  | Terraform Associate Certification: HashiCorp Certified                      | Premium | Container Orchestration, Devops, IAC, Certification        |\n| 32  | Helm for Beginners                                                          | Premium | Container Orchestration, Containers, Devops                |\n| 33  | PCAP – Python Certification Course                                          | Premium | Devops, Programming, Python, Certification                 |\n| 34  | Istio Service Mesh                                                          | Premium | Devops                                                     |\n| 35  | Jinja2 Basics (Mini Course)                                                 | Free    | Devops                                                     |\n| 36  | Certified Kubernetes Security Specialist (CKS)                              | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 37  | Certified Python Entry-Level Programmer: PCEP-30-02                         | Premium | Devops, Programming, Python, Certification                 |\n| 38  | JSON Path Test – Free Course                                                | Free    | Devops                                                     |\n| 39  | Docker Certified Associate Exam Course                                      | Premium | Containers, Devops, Certification                          |\n| 40  | Terraform Basics Training Course                                            | Premium | Automation, Devops, IAC                                    |\n| 41  | CKA Certification Course – Certified Kubernetes Administrator               | Premium | Container Orchestration, Containers, Devops                |\n| 42  | Certified Kubernetes Application Developer (CKAD)                           | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 43  | Kubernetes for the Absolute Beginners – Hands-on Tutorial                   | Premium | Container Orchestration, Containers, Kubernetes, Devops    |\n| 44  | Docker Training Course for the Absolute Beginner                            | Premium | Containers, Devops                                         |\n| 45  | Chef for the Absolute Beginners                                             | Premium | Automation, Devops                                         |\n| 46  | OpenShift 3 for the Absolute Beginners                                      | Premium | Container Orchestration, Containers, Devops                |\n| 47  | Ansible Advanced Course                                                     | Premium | Automation, Devops, IAC                                    |\n| 48  | Learn Ansible Basics – Beginners Course                                     | Premium | Automation, Devops, IAC                                    |\n| 49  | Docker – SWARM | SERVICES | STACKS – Hands-on                               | Premium | Containers, Devops                                         |\n| 50  | DevOps Pre-Requisite Course                                                 | Premium | Automation, Devops, IAC                                    |\n| 51  | Learning Linux Basics Course & Labs                                         | Premium | Devops, Linux                                              |\n| 52  | Shell Scripts for Beginners                                                 | Premium | Devops                                                     |\n| 53  | Puppet for the Absolute Beginners Course                                    | Premium | Automation, Devops, IAC                                    |\n| 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\nEnter the number of the course you want to select: 35\n```\n\n![](static/demo-select-download.gif)\n\n## Colab Notebook to download directly in Personal GDrive\n\nYou can open [this notebook](https://colab.research.google.com/drive/1GsgFcqa_43GYeDKmoa0CXsRfDySrzvzT?usp=sharing) with your google account were you want to download the course. Please note that you should open with the same account for which you want to link the drive.\n",
+    'long_description': "# KodeKloud Downloader\n\n## Disclaimer\nPlease read the following disclaimer carefully before using the Downloader CLI Tool.\n\n- The CLI Tool is intended for personal use only. By using this tool, you agree to use it at your own risk and assume full responsibility for any consequences that may arise from its use. The developers and contributors of this tool are not responsible for any damages or losses that may occur from its use.\n\n- The use of this tool to download premium courses is for educational purposes only. You must have the proper authorization or permission from the course provider to access the content legally.\n\n- It is strictly prohibited to distribute or share the downloaded content through any means, including but not limited to uploading to file-sharing platforms, torrent sites, or any other form of digital or physical distribution. Doing so is a violation of copyright laws and may result in legal consequences.\n\n---\n\n## Features\n\n- [x] Download video lessons in selected quality\n- [x] Organizes downloaded content in a structured folder hierarchy\n- [x] Download resources (PDFs, etc.) alongside video lessons\n\n---\n\n## Prerequisites\n\n- **User need to enroll in the course before using the cli tool to download it**\n- Python 3.8 or higher\n- ffmpeg\n\n<details>\n    <summary>How to Install FFmpeg on Linux, Mac, and Windows</summary>\n\n# How to Install FFmpeg on Linux, Mac, and Windows\n\nFFmpeg is a powerful and flexible multimedia processing tool that can handle a wide range of tasks, such as video and audio conversion, streaming, and recording. In this guide, we will show you how to install FFmpeg on Linux, Mac, and Windows operating systems.\n\n## Linux\n\n### Ubuntu and Debian-based distributions\n\n1.  Update the package lists for upgrades and new package installations.\n\n`sudo apt update`\n\n1.  Install FFmpeg using the following command:\n\n`sudo apt install ffmpeg`\n\n### Fedora\n\n1.  Install FFmpeg using the following command:\n\n`sudo dnf install ffmpeg`\n\n### Arch Linux and Manjaro\n\n1.  Install FFmpeg using the following command:\n\n`sudo pacman -S ffmpeg`\n\n## Mac\n\n### Using Homebrew\n\nIf you don't have Homebrew installed, you can install it by following the instructions on the [official Homebrew website](https://brew.sh/).\n\nUpdate Homebrew to ensure you have the latest package information:\n\n`brew update`\n\n1.  Install FFmpeg using the following command:\n\n`brew install ffmpeg`\n\n### Using MacPorts\n\nIf you don't have MacPorts installed, you can install it by following the instructions on the [official MacPorts website](https://www.macports.org/install.php).\n\nUpdate MacPorts to ensure you have the latest package information:\n\n`sudo port selfupdate`\n\n1.  Install FFmpeg using the following command:\n\n`sudo port install ffmpeg`\n\n## Windows\n\n### Using Chocolatey\n\nIf you don't have Chocolatey installed, you can install it by following the instructions on the [official Chocolatey website](https://chocolatey.org/install).\n\nOpen an elevated Command Prompt (run as Administrator) and install FFmpeg using the following command:\n\n`choco install ffmpeg`\n\n### Using Scoop\n\nIf you don't have Scoop installed, you can install it by following the instructions on the [official Scoop website](https://scoop.sh/).\n\nOpen a PowerShell terminal and install FFmpeg using the following command:\n\n`scoop install ffmpeg`\n\nAfter following these steps, FFmpeg should be installed on your system. You can check the installation by running the following command in your terminal or command prompt:\n\n`ffmpeg -version`\n\nThis will display the FFmpeg version and build information, confirming that the installation was successful.\n\n</details>\n\n\n\n## How to get cookie\n- Sign in to kodekloud.com\n- Download extension such as [Get cookies.txt LOCALLY](https://chrome.google.com/webstore/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc/related)\n- Download the cookie and save it in some location (You can name it something like `cookie.txt`).\n\n![](/static/cookie-demo.png)\n\n## 💻 Installation\n\nTo install kodekloud-downloader, simply run the following command:\n\n```console\npip install -U kodekloud-downloader\n```\n\nYou can also install the latest main changes:\n```console\npip install -U git+https://github.com/debakarr/kodekloud-downloader.git\n```\n\n## 📚 Usage\n\nAfter installing the package, you can use the `kodekloud dl` command to download shows from the command line.\n\n```css\nkodekloud dl --help\nUsage: kodekloud dl [OPTIONS] [COURSE_URL]\n\nOptions:\n  -q, --quality [360p|480p|540p|720p|1080p]\n                                  Quality of the video to be downloaded.\n  -o, --output-dir TEXT           Output directory where downloaded files will\n                                  be store.\n  -c, --cookie TEXT               Cookie to download the courses.  [required]\n  --help                          Show this message and exit.\n```\n\nHere is an example:\n\n### 🔍 Download entire course from list of available course in current folder\n\n```css\nkodekloud dl -o . -c /path/to/cookie.txt\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| No. | Name                                                                        | Type    | Categories                                                 |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| 1   | Ultimate Certified Kubernetes Application Developer (CKAD) Mock Exam Series | Premium | Challenges, Containers, Kubernetes                         |\n| 2   | GCP DevOps Project                                                          | Premium | Cloud, GCP                                                 |\n| 3   | 12 Factor App                                                               | Premium | Productivity                                               |\n| 4   | AZ-305: Microsoft Azure Solutions Architect Expert                          | Premium | Certification, Cloud, Devops                               |\n| 5   | Ultimate Certified Kubernetes Administrator (CKA) Mock Exam Series          | Free    | Container Orchestration, Kubernetes, Devops, Certification |\n| 6   | AWS Lambda                                                                  | Premium | AWS, Cloud                                                 |\n| 7   | Linux Professional Institute LPIC-1 Exam 101                                | Premium | Certification, Linux                                       |\n| 8   | Advanced Golang                                                             | Premium | Programming                                                |\n| 9   | Prometheus Certified Associate (PCA)                                        | Premium | Certification, Kubernetes, Monitoring                      |\n| 10  | GCP Cloud Digital Leader Certification                                      | Premium | Cloud, GCP, Certification                                  |\n| 11  | OpenShift 4                                                                 | Premium | Container Orchestration, Devops, Red Hat                   |\n| 12  | HashiCorp : Terraform Cloud                                                 | Premium | Cloud, Devops, HashiCorp                                   |\n| 13  | ArgoCD                                                                      | Premium | CI/CD, Devops, Kubernetes                                  |\n| 14  | Amazon Elastic Container Service (AWS ECS)                                  | Free    | AWS, Devops                                                |\n| 15  | Red Hat Certified System Administrator(RHCSA)                               | Premium | Devops, Linux, Red Hat, Certification                      |\n| 16  | Open Source for Beginners                                                   | Premium | Productivity                                               |\n| 17  | Kustomize                                                                   | Premium | Devops, Kubernetes                                         |\n| 18  | DevSecOps – Kubernetes DevOps & Security                                    | Premium | Devops, DevSecOps, Kubernetes                              |\n| 19  | AZ-104: Microsoft Azure Administrator                                       | Premium | Cloud, Devops, Certification                               |\n| 20  | DevOps Interview Preparation Course                                         | Premium | Devops                                                     |\n| 21  | Terraform Challenges                                                        | Free    | Challenges, Devops, IAC                                    |\n| 22  | HashiCorp Certified: Consul Associate Certification                         | Premium | Devops, HashiCorp                                          |\n| 23  | HashiCorp Certified: Vault Associate Certification                          | Premium | Devops, HashiCorp                                          |\n| 24  | Kubernetes Challenges                                                       | Free    | Challenges, Devops                                         |\n| 25  | Linux Challenges                                                            | Free    | Challenges, Devops, Linux                                  |\n| 26  | HashiCorp Certified: Vault Operations Professional 2022                     | Premium | Container Orchestration, Containers, Devops, HashiCorp     |\n| 27  | CKS – Challenges                                                            | Free    | Challenges, Container Orchestration, Containers, Devops    |\n| 28  | Linux Foundation Certified System Administrator (LFCS)                      | Premium | Devops, Linux, Certification                               |\n| 29  | Jenkins                                                                     | Premium | Automation, CI/CD, Devops                                  |\n| 30  | Golang                                                                      | Premium | Devops, Programming                                        |\n| 31  | Terraform Associate Certification: HashiCorp Certified                      | Premium | Container Orchestration, Devops, IAC, Certification        |\n| 32  | Helm for Beginners                                                          | Premium | Container Orchestration, Containers, Devops                |\n| 33  | PCAP – Python Certification Course                                          | Premium | Devops, Programming, Python, Certification                 |\n| 34  | Istio Service Mesh                                                          | Premium | Devops                                                     |\n| 35  | Jinja2 Basics (Mini Course)                                                 | Free    | Devops                                                     |\n| 36  | Certified Kubernetes Security Specialist (CKS)                              | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 37  | Certified Python Entry-Level Programmer: PCEP-30-02                         | Premium | Devops, Programming, Python, Certification                 |\n| 38  | JSON Path Test – Free Course                                                | Free    | Devops                                                     |\n| 39  | Docker Certified Associate Exam Course                                      | Premium | Containers, Devops, Certification                          |\n| 40  | Terraform Basics Training Course                                            | Premium | Automation, Devops, IAC                                    |\n| 41  | CKA Certification Course – Certified Kubernetes Administrator               | Premium | Container Orchestration, Containers, Devops                |\n| 42  | Certified Kubernetes Application Developer (CKAD)                           | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 43  | Kubernetes for the Absolute Beginners – Hands-on Tutorial                   | Premium | Container Orchestration, Containers, Kubernetes, Devops    |\n| 44  | Docker Training Course for the Absolute Beginner                            | Premium | Containers, Devops                                         |\n| 45  | Chef for the Absolute Beginners                                             | Premium | Automation, Devops                                         |\n| 46  | OpenShift 3 for the Absolute Beginners                                      | Premium | Container Orchestration, Containers, Devops                |\n| 47  | Ansible Advanced Course                                                     | Premium | Automation, Devops, IAC                                    |\n| 48  | Learn Ansible Basics – Beginners Course                                     | Premium | Automation, Devops, IAC                                    |\n| 49  | Docker – SWARM | SERVICES | STACKS – Hands-on                               | Premium | Containers, Devops                                         |\n| 50  | DevOps Pre-Requisite Course                                                 | Premium | Automation, Devops, IAC                                    |\n| 51  | Learning Linux Basics Course & Labs                                         | Premium | Devops, Linux                                              |\n| 52  | Shell Scripts for Beginners                                                 | Premium | Devops                                                     |\n| 53  | Puppet for the Absolute Beginners Course                                    | Premium | Automation, Devops, IAC                                    |\n| 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\nEnter the number of the course you want to select: 35\n```\n\n![](static/demo-select-download.gif)\n\n## Colab Notebook to download directly in Personal GDrive\n\nYou can open [this notebook](https://colab.research.google.com/drive/1GsgFcqa_43GYeDKmoa0CXsRfDySrzvzT?usp=sharing) with your google account were you want to download the course. Please note that you should open with the same account for which you want to link the drive.\n",
     'author': 'Roy, Debakar',
     'author_email': 'debakar.roy@outlook.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/debakarr/kodekloud-downloader',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `kodekloud-downloader-0.0.9/PKG-INFO` & `kodekloud-downloader-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodekloud-downloader
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple downloaded for https://kodekloud.com/
 Home-page: https://github.com/debakarr/kodekloud-downloader
 Author: Roy, Debakar
 Author-email: debakar.roy@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -33,20 +33,21 @@
 
 ---
 
 ## Features
 
 - [x] Download video lessons in selected quality
 - [x] Organizes downloaded content in a structured folder hierarchy
-- [ ] Download resources (PDFs, etc.) alongside video lessons
+- [x] Download resources (PDFs, etc.) alongside video lessons
 
 ---
 
 ## Prerequisites
 
+- **User need to enroll in the course before using the cli tool to download it**
 - Python 3.8 or higher
 - ffmpeg
 
 <details>
     <summary>How to Install FFmpeg on Linux, Mac, and Windows</summary>
 
 # How to Install FFmpeg on Linux, Mac, and Windows
```

