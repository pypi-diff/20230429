# Comparing `tmp/sittagger-0.6.2.tar.gz` & `tmp/sittagger-1.0.0.tar.gz`

## Comparing `sittagger-0.6.2.tar` & `sittagger-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger.desktop
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger.png
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/__main__.py
--rwxr-xr-x   0        0        0     4769 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/app.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/birdeye.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/canvas.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/cli.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/dbtag.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/dirwidgets.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/fileoperationdialog.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/fm_interop.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/fsops.py
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/fullscreenviewer.py
--rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/imagewidgets.py
--rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/mainwindow.ui
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/tagwidgets.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/thumbnailmaker.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/videogrid.py
--rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 sittagger-0.6.2/sittagger/videowidgets.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sittagger-0.6.2/.gitignore
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 sittagger-0.6.2/COPYING.WTFPL
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 sittagger-0.6.2/README.rst
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 sittagger-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sittagger-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger.desktop
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger.png
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/__main__.py
+-rwxr-xr-x   0        0        0     4782 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/app.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/birdeye.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/canvas.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/cli.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/dbtag.py
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/dirwidgets.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/fileoperationdialog.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/fm_interop.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/fsops.py
+-rw-r--r--   0        0        0    10273 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/fullscreenviewer.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/imagewidgets.py
+-rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/mainwindow.ui
+-rw-r--r--   0        0        0     5319 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/tagwidgets.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/thumbnailmaker.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/videogrid.py
+-rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 sittagger-1.0.0/sittagger/videowidgets.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 sittagger-1.0.0/.gitignore
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 sittagger-1.0.0/COPYING.WTFPL
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 sittagger-1.0.0/README.rst
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 sittagger-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sittagger-1.0.0/PKG-INFO
```

### Comparing `sittagger-0.6.2/sittagger.desktop` & `sittagger-1.0.0/sittagger.desktop`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.2/sittagger.png` & `sittagger-1.0.0/sittagger.png`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.2/sittagger/app.py` & `sittagger-1.0.0/sittagger/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from importlib import import_module
 import mimetypes
 from pathlib import Path
 import sys
 import os
 
-from PyQt5.QtCore import pyqtSlot as Slot, QUrl
-from PyQt5.QtGui import QIcon, QPixmap, QDesktopServices
-from PyQt5.QtWidgets import (
+from PyQt6.QtCore import pyqtSlot as Slot, QUrl
+from PyQt6.QtGui import QIcon, QPixmap, QDesktopServices
+from PyQt6.QtWidgets import (
 	QMainWindow, QListWidgetItem, QApplication, QAbstractItemView,
 )
-from PyQt5.uic import loadUiType
+from PyQt6.uic import loadUiType
 
 from . import dbtag
 from .fullscreenviewer import ImageViewer
 
 
 def load_ui_class(package, module_name, class_name):
 	try:
@@ -64,15 +64,15 @@
 		self.dirChooser.selectionModel().currentChanged.connect(self.browseSelectedDir)
 		self.dirChooser.selectPath(folder)
 		self.dirChooser.openTo(folder)
 
 	def _init_imagelist(self):
 		self.imageList.itemSelectionChanged.connect(self._editTagsItems)
 		self.imageList.activated.connect(self._openFile)
-		self.imageList.setSelectionMode(QAbstractItemView.ExtendedSelection)
+		self.imageList.setSelectionMode(QAbstractItemView.SelectionMode.ExtendedSelection)
 		self.imageList.pasteRequested.connect(self._onListPaste)
 
 	def _init_tabs(self):
 		self.tabWidget.currentChanged.connect(self._tabSelected)
 		self.hSplitter.setStretchFactor(1, 1)
 
 	def _init_tagchooser(self):
@@ -171,12 +171,12 @@
 	app = QApplication(sys.argv)
 	app.setApplicationDisplayName('SIT-Tagger')
 	app.setApplicationName('SIT-Tagger')
 
 	opts = parse_options(list(app.arguments())[1:])
 	win = Win(opts)
 	win.show()
-	app.exec_()
+	app.exec()
 
 
 if __name__ == '__main__':
 	main()
```

### Comparing `sittagger-0.6.2/sittagger/birdeye.py` & `sittagger-1.0.0/sittagger/birdeye.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import locale
 import mimetypes
 from pathlib import Path
 import re
 import sys
 
-from PyQt5.QtCore import *
-from PyQt5.QtGui import *
-from PyQt5.QtWidgets import *
+from PyQt6.QtCore import *
+from PyQt6.QtGui import *
+from PyQt6.QtWidgets import *
 
 Signal = pyqtSignal
 Slot = pyqtSlot
 
 import vignette
 
 
@@ -118,16 +118,16 @@
 			pix.load(self.thumb)
 			if pix.isNull():
 				# TODO does NULLPIX count in cache more than once?
 				pix = NULLPIX
 			else:
 				pix = pix.scaled(
 					NULLPIX.size(),
-					Qt.KeepAspectRatio,
-					Qt.SmoothTransformation,
+					Qt.AspectRatioMode.KeepAspectRatio,
+					Qt.TransformationMode.SmoothTransformation,
 				)
 
 			QPixmapCache.insert(self.thumb, pix)
 		return pix
 
 	def paintEvent(self, ev):
 		pix = self.buildPix()
@@ -138,16 +138,16 @@
 		else:
 			pnt = QStylePainter(self)
 
 			option = QStyleOptionButton()
 			option.initFrom(self)
 			option.backgroundColor = self.palette().color(QPalette.Background)
 			option.iconSize = pix.size()
-			#pnt.drawPrimitive(int(QStyle.CE_PushButton), option)
-			#pnt.drawControl(QStyle.CE_PushButton, option)
+			#pnt.drawPrimitive(int(QStyle.ControlElement.CE_PushButton), option)
+			#pnt.drawControl(QStyle.ControlElement.CE_PushButton, option)
 
 			pnt.drawItemPixmap(option.rect, Qt.AlignCenter, pix)
 
 	def sizeHint(self):
 		return NULLPIX.size()
 
 	minimumSizeHint = sizeHint
@@ -163,15 +163,15 @@
 
 	def add_file(self, sub):
 		row, col = divmod(len(self.files), COLUMNS)
 		self.files.append(sub)
 		self.layout().addWidget(LazyImageView(sub), row * 2, col, Qt.AlignCenter)
 
 		label = FileButton(sub, label=sub.name)
-		label.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Minimum)
+		label.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Minimum)
 		#label.setWordWrap(True)
 		self.layout().addWidget(label, row * 2 + 1, col)
 
 
 class BirdEye(QWidget):
 	def __init__(self):
 		super().__init__()
@@ -196,15 +196,15 @@
 
 if __name__ == "__main__":
 	QPixmapCache.setCacheLimit(100 << 10)
 
 	app = QApplication(sys.argv)
 	#NULLPIX = QPixmap(QSize(256, 256))
 	NULLPIX = QPixmap(QSize(128, 128))
-	NULLPIX.fill(Qt.black)
+	NULLPIX.fill(Qt.GlobalColor.black)
 
 	beye = BirdEye()
 	scroller = QScrollArea()
 	scroller.setWidgetResizable(True)
 	#beye.show()
 	scroller.setWidget(beye)
 	scroller.show()
```

### Comparing `sittagger-0.6.2/sittagger/canvas.py` & `sittagger-1.0.0/sittagger/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: WTFPL
 
 import math
 
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QPixmapCache, QTransform, QPixmap
-from PyQt5.QtWidgets import QGraphicsView, QGraphicsItem, QGraphicsScene, QGraphicsPixmapItem
+from PyQt6.QtCore import Qt
+from PyQt6.QtGui import QPixmapCache, QTransform, QPixmap
+from PyQt6.QtWidgets import QGraphicsView, QGraphicsItem, QGraphicsScene, QGraphicsPixmapItem
 
 
 MODE_MOVE = 0
 MODE_ZOOM = 1
 MODE_ROT = 2
 
 
@@ -70,15 +70,15 @@
 class Image(ItemMixin, QGraphicsPixmapItem):
 	def __init__(self, path):
 		super().__init__()
 
 		pix = QPixmap(path)
 		QPixmapCache.insert(path, pix)
 
-		self.setTransformationMode(Qt.SmoothTransformation)
+		self.setTransformationMode(Qt.TransformationMode.SmoothTransformation)
 
 		self.setPixmap(pix)
 
 
 class Scene(QGraphicsScene):
 	def __init__(self, *args):
 		super().__init__(*args)
@@ -112,14 +112,14 @@
 		super().__init__(*args)
 		self.setScene(Scene(self))
 
 	def addItem(self, item):
 		self.scene().addItem(item)
 
 	def keyPressEvent(self, ev):
-		if ev.key() == Qt.Key_F1:
+		if ev.key() == Qt.Key.Key_F1:
 			self.scene().setMoveMode()
-		elif ev.key() == Qt.Key_F2:
+		elif ev.key() == Qt.Key.Key_F2:
 			self.scene().setZoomMode()
-		elif ev.key() == Qt.Key_F3:
+		elif ev.key() == Qt.Key.Key_F3:
 			self.scene().setRotMode()
 		return super().keyPressEvent(ev)
```

### Comparing `sittagger-0.6.2/sittagger/cli.py` & `sittagger-1.0.0/sittagger/cli.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.2/sittagger/dbtag.py` & `sittagger-1.0.0/sittagger/dbtag.py`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.2/sittagger/dirwidgets.py` & `sittagger-1.0.0/sittagger/dirwidgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # SPDX-License-Identifier: WTFPL
 
 from pathlib import Path
 
-from PyQt5.QtCore import QDir, pyqtSlot as Slot, Qt, pyqtSignal as Signal, QMimeData
-from PyQt5.QtGui import QKeySequence
-from PyQt5.QtWidgets import (
-	QTreeView, QFileSystemModel, QAction, QInputDialog, QLineEdit,
-	QMessageBox,
+from PyQt6.QtCore import QDir, pyqtSlot as Slot, Qt, pyqtSignal as Signal, QMimeData, QCoreApplication
+from PyQt6.QtCore import QTimer
+from PyQt6.QtGui import QKeySequence, QAction, QFileSystemModel
+from PyQt6.QtWidgets import (
+	QTreeView, QInputDialog, QLineEdit,
+	QMessageBox, QHeaderView,
 )
 
 from .fileoperationdialog import FileOperationProgressDialog
 from .fsops import rename_folder, FileOperation
 from .fm_interop import ClipQt, get_files_clipboard, MIME_LIST, _parse_url
 
 
 class FSModelWithDND(QFileSystemModel):
 	def flags(self, qidx):
 		flags = super().flags(qidx)
 		if qidx.isValid():
-			flags |= Qt.ItemIsDragEnabled | Qt.ItemIsDropEnabled
+			flags |= Qt.ItemFlag.ItemIsDragEnabled | Qt.ItemFlag.ItemIsDropEnabled
 		return flags
 
 	def mimeTypes(self):
 		return [MIME_LIST]
 
 	def mimeData(self, qindexes):
 		ret = QMimeData()
@@ -32,15 +33,15 @@
 				Path(self.filePath(qidx)).absolute().as_uri().encode("ascii")
 				for qidx in qindexes
 			) + b"\r\n"
 		)
 		return ret
 
 	def supportedDropActions(self):
-		return Qt.CopyAction | Qt.MoveAction
+		return Qt.DropAction.CopyAction | Qt.DropAction.MoveAction
 
 	def canDropMimeData(self, qmime, action, row, column, parent_qidx):
 		if column > 0 or row > -1:
 			# row is -1 when pointing to a qmodelindex
 			# row is >= 0 when pointing between rows
 			return False
 
@@ -64,17 +65,17 @@
 		if not self.canDropMimeData(qmime, action, row, column, parent_qidx):
 			return False
 
 		files = self._getDroppedPaths(qmime, parent_qidx)
 
 		parent_path = Path(self.filePath(parent_qidx))
 
-		if action == Qt.MoveAction:
+		if action == Qt.DropAction.MoveAction:
 			op = "cut"
-		elif action == Qt.CopyAction:
+		elif action == Qt.DropAction.CopyAction:
 			op = "copy"
 		else:
 			raise NotImplementedError()
 
 		treeop = FileOperation(parent_path, files, op, None)
 		self.fileOperation.emit(treeop)
 
@@ -83,47 +84,51 @@
 
 
 class DirTreeView(QTreeView):
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 
 		mdl = FSModelWithDND(parent=self)
-		mdl.setFilter(QDir.AllDirs | QDir.Drives | QDir.NoDotAndDotDot)
+		mdl.setFilter(QDir.Filter.AllDirs | QDir.Filter.Drives | QDir.Filter.NoDotAndDotDot)
 		self.setModel(mdl)
 		mdl.fileOperation.connect(self.modelFileOperation)
 
+		# all sections/columns but "filename" are hidden, so filename is the last section
+		# it must not be auto-stretched if we want it to auto-expand past the widget's size
+		self.header().setStretchLastSection(False)
+		self.header().setSectionResizeMode(QHeaderView.ResizeMode.ResizeToContents)
 		for col in range(1, self.header().count()):
 			self.setColumnHidden(col, True)
 
 		# actions
 		action = QAction(self.tr("&Rename folder..."), self)
 		action.setShortcut(QKeySequence("F2"))
-		action.setShortcutContext(Qt.WidgetShortcut)
+		action.setShortcutContext(Qt.ShortcutContext.WidgetShortcut)
 		action.triggered.connect(self.popRenameSelected)
 		self.addAction(action)
 
 		act = QAction(self.tr("&Create folder..."), self)
 		act.triggered.connect(self._createFolder)
 		self.addAction(act)
 
 		action = QAction(self.tr("Show &hidden folders"), self)
 		action.setCheckable(True)
 		action.toggled.connect(self.toggleHidden)
 		self.addAction(action)
 
-		self.setContextMenuPolicy(Qt.ActionsContextMenu)
+		self.setContextMenuPolicy(Qt.ContextMenuPolicy.ActionsContextMenu)
 
 	def setRootPath(self, path):
 		self.root_path = path
 		qidx = self.model().setRootPath(path)
 		self.setRootIndex(qidx)
 
 	def openTo(self, path):
 		qidx = self.model().index(path)
-		self.scrollTo(qidx, self.PositionAtCenter)
+		self.scrollTo(qidx, QTreeView.ScrollHint.PositionAtCenter)
 
 	def selectPath(self, path):
 		qidx = self.model().index(path)
 		self.setCurrentIndex(qidx)
 
 	def selectedPath(self):
 		return self.model().filePath(self.currentIndex())
@@ -133,15 +138,15 @@
 		db = self.window().db
 		current = Path(self.selectedPath()).absolute()
 
 		new, ok = QInputDialog.getText(
 			self,
 			self.tr("Rename directory"),
 			self.tr("New name for directory"),
-			QLineEdit.Normal,
+			QLineEdit.EchoMode.Normal,
 			current.name
 		)
 
 		if not ok or not new or new == current.name:
 			return
 		if "/" in new:
 			QMessageBox.critical(
@@ -182,15 +187,15 @@
 	def _createFolder(self):
 		current = Path(self.selectedPath()).absolute()
 
 		new, ok = QInputDialog.getText(
 			self,
 			self.tr("Create directory"),
 			self.tr("Name for new directory"),
-			QLineEdit.Normal,
+			QLineEdit.EchoMode.Normal,
 			self.tr("new_folder")
 		)
 
 		if not ok or not new:
 			return
 		if "/" in new:
 			QMessageBox.critical(
@@ -202,10 +207,16 @@
 
 		current.joinpath(new).mkdir()
 
 	@Slot(bool)
 	def toggleHidden(self, show):
 		model = self.model()
 		if show:
-			model.setFilter(model.filter() | QDir.Hidden)
+			model.setFilter(model.filter() | QDir.Filter.Hidden)
 		else:
-			model.setFilter(model.filter() & ~QDir.Hidden)
+			model.setFilter(model.filter() & ~QDir.Filter.Hidden)
+
+	def wheelEvent(self, event):
+		if event.modifiers() & Qt.KeyboardModifier.ShiftModifier:
+			QCoreApplication.sendEvent(self.horizontalScrollBar(), event)
+		else:
+			super().wheelEvent(event)
```

### Comparing `sittagger-0.6.2/sittagger/fileoperationdialog.py` & `sittagger-1.0.0/sittagger/fileoperationdialog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: WTFPL
 
-from PyQt5.QtCore import pyqtSlot as Slot
-from PyQt5.QtWidgets import QProgressDialog
+from PyQt6.QtCore import pyqtSlot as Slot
+from PyQt6.QtWidgets import QProgressDialog
 
 
 class FileOperationProgressDialog(QProgressDialog):
 	def __init__(self, parent):
 		super().__init__(parent)
 		self.setAutoReset(False)
 		self.setAutoClose(False)
```

### Comparing `sittagger-0.6.2/sittagger/fm_interop.py` & `sittagger-1.0.0/sittagger/fm_interop.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 """File managers inter-operability for copy/pasting files
 """
 
 from urllib.parse import urlparse, unquote
 from pathlib import Path
 
-from PyQt5.QtGui import QGuiApplication
-from PyQt5.QtCore import QMimeData
+from PyQt6.QtGui import QGuiApplication
+from PyQt6.QtCore import QMimeData
 
 
 MIME_GNOME = "x-special/gnome-copied-files"
 MIME_LIST = "text/uri-list"
 MIME_TEXT = "text/plain"
```

### Comparing `sittagger-0.6.2/sittagger/fsops.py` & `sittagger-1.0.0/sittagger/fsops.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from logging import getLogger
 import os
 from pathlib import Path
 import shutil
 import subprocess
 from threading import Event
 
-from PyQt5.QtCore import QThread, pyqtSignal as Signal, pyqtSlot as Slot
+from PyQt6.QtCore import QThread, pyqtSignal as Signal, pyqtSlot as Slot
 import vignette
 
 
 LOGGER = getLogger(__name__)
 
 
 _os_rename = os.rename
```

### Comparing `sittagger-0.6.2/sittagger/fullscreenviewer.py` & `sittagger-1.0.0/sittagger/fullscreenviewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: WTFPL
 
-from PyQt5.QtCore import (
+from PyQt6.QtCore import (
 	Qt, QEvent, pyqtSignal as Signal, pyqtSlot as Slot, QTimer, QPointF,
 )
-from PyQt5.QtGui import (
+from PyQt6.QtGui import (
 	QKeySequence, QPalette, QPixmap, QMovie, QIcon, QImageReader, QCursor,
 )
-from PyQt5.QtWidgets import QMainWindow, QScrollArea, QDockWidget, QToolBar, QLabel
+from PyQt6.QtWidgets import QMainWindow, QScrollArea, QDockWidget, QToolBar, QLabel, QFrame
 
 from .tagwidgets import TagEditor
 
 
 ZOOM_FACTOR = 0
 ZOOM_FITALL = 1
 ZOOM_FITCUT = 2
@@ -40,18 +40,18 @@
 	def _init_widgets(self):
 		#self.toolbar = AutoHideToolBar()
 		self.toolbar = QToolBar()
 		self.addToolBar(self.toolbar)
 		self.toolbar.hide()
 
 		act = self.toolbar.addAction(QIcon.fromTheme('go-previous'), 'Previous')
-		act.setShortcut(QKeySequence(Qt.Key_Backspace))
+		act.setShortcut(QKeySequence(Qt.Key.Key_Backspace))
 		act.triggered.connect(self.showPreviousFile)
 		act = self.toolbar.addAction(QIcon.fromTheme('go-next'), 'Next')
-		act.setShortcut(QKeySequence(Qt.Key_Space))
+		act.setShortcut(QKeySequence(Qt.Key.Key_Space))
 		act.triggered.connect(self.showNextFile)
 		self.toolbar.addSeparator()
 
 		self.scrollview = ImageViewerCenter()
 		self.scrollview.installEventFilter(self) ### !
 		self.setCentralWidget(self.scrollview)
 
@@ -69,42 +69,42 @@
 		self.toolbar.addAction('Copy tags').triggered.connect(self.copyPreviousTags)
 
 		self.tageditor = TagEditor()
 		self.tageditor.setDb(self.db)
 
 		self.docktagger = AutoHideDock()
 		self.docktagger.setWidget(self.tageditor)
-		self.addDockWidget(Qt.LeftDockWidgetArea, self.docktagger)
+		self.addDockWidget(Qt.DockWidgetArea.LeftDockWidgetArea, self.docktagger)
 		self.docktagger.hide()
 
 		self.scrollview.topZoneEntered.connect(self.toolbar.show)
 		self.scrollview.topZoneLeft.connect(self.toolbar.hide)
 		self.scrollview.leftZoneEntered.connect(self.docktagger.show)
 		self.scrollview.leftZoneLeft.connect(self.docktagger.hide)
 
 	def eventFilter(self, sview, ev):
-		if ev.type() == QEvent.KeyPress:
-			if ev.key() == Qt.Key_Escape:
+		if ev.type() == QEvent.Type.KeyPress:
+			if ev.key() == Qt.Key.Key_Escape:
 				self.fullscreenAction.setChecked(False)
 				return True
-			elif ev.key() in [Qt.Key_PageUp, Qt.Key_Backspace]: # qactions
+			elif ev.key() in [Qt.Key.Key_PageUp, Qt.Key.Key_Backspace]: # qactions
 				self.showPreviousFile()
 				return True
-			elif ev.key() in [Qt.Key_PageDown, Qt.Key_Space]:
+			elif ev.key() in [Qt.Key.Key_PageDown, Qt.Key.Key_Space]:
 				self.showNextFile()
 				return True
 		return super().eventFilter(sview, ev)
 
 	def spawn(self, files, currentFile):
 		self.files = files
 		self.currentIndex = files.index(currentFile)
 
 		self.setFile(currentFile)
 		if self.isHidden():
-			#~ self.setWindowState(self.windowState() | Qt.WindowMaximized)
+			#~ self.setWindowState(self.windowState() | Qt.WindowState.WindowMaximized)
 			#~ self.show()
 			self.fullscreenAction.setChecked(False)
 			self.fullscreenAction.setChecked(True)
 			#~ self.showMaximized()
 		else:
 			self.show()
 
@@ -153,24 +153,24 @@
 		self.zoomMode = ZOOM_FACTOR
 		self.zoomFactor = 1
 		self.oldZoomFactor = self.zoomFactor
 		self.moving = None
 
 		imgWidget = QLabel()
 		imgWidget.setMouseTracking(True)
-		imgWidget.setAlignment(Qt.AlignCenter)
+		imgWidget.setAlignment(Qt.AlignmentFlag.AlignCenter)
 		self.setWidget(imgWidget)
 
-		self.setAlignment(Qt.AlignCenter)
+		self.setAlignment(Qt.AlignmentFlag.AlignCenter)
 		self.setMouseTracking(True)
-		self.setFrameShape(self.NoFrame)
+		self.setFrameShape(QFrame.Shape.NoFrame)
 		self.setWidgetResizable(True)
 
 		pal = QPalette()
-		pal.setColor(QPalette.Window, Qt.black)
+		pal.setColor(QPalette.ColorRole.Window, Qt.GlobalColor.black)
 		self.setPalette(pal)
 
 		self.leftZone = False
 		self.topZone = False
 
 		self.file = None
 		self.movie = None
@@ -185,47 +185,47 @@
 
 	def mouseMoveEvent(self, ev):
 		if self.moving:
 			p = ev.pos()
 			self.horizontalScrollBar().setValue(self.movingScrolls[0] - (p.x() - self.moving[0]))
 			self.verticalScrollBar().setValue(self.movingScrolls[1] - (p.y() - self.moving[1]))
 		else:
-			newLeft = (ev.x() < self.leftMargin)
+			newLeft = (ev.pos().x() < self.leftMargin)
 			if newLeft and not self.leftZone:
 				self.leftZoneEntered.emit()
 			elif self.leftZone and not newLeft:
 				self.leftZoneLeft.emit()
 			self.leftZone = newLeft
 
-			newTop = (ev.y() < self.topMargin)
+			newTop = (ev.pos().y() < self.topMargin)
 			if newTop and not self.topZone:
 				self.topZoneEntered.emit()
 			elif self.topZone and not newTop:
 				self.topZoneLeft.emit()
 			self.topZone = newTop
 
 	def resizeEvent(self, ev):
 		super().resizeEvent(ev)
 		if self.zoomMode != ZOOM_FACTOR:
 			self._rebuildZoom()
 
 	def keyPressEvent_(self, ev):
-		if ev.key() not in (Qt.Key_PageUp, Qt.Key_PageDown):
+		if ev.key() not in (Qt.Key.Key_PageUp, Qt.Key.Key_PageDown):
 			QScrollArea.keyPressEvent(self, ev)
 
 	def keyReleaseEvent_(self, ev):
-		if ev.key() == Qt.Key_PageUp:
+		if ev.key() == Qt.Key.Key_PageUp:
 			self.imageviewer.prevImage_s()
-		elif ev.key() == Qt.Key_PageDown:
+		elif ev.key() == Qt.Key.Key_PageDown:
 			self.imageviewer.nextImage_s()
 		else:
 			QScrollArea.keyReleaseEvent(self, ev)
 
 	def wheelEvent(self, event):
-		if not (event.modifiers() & Qt.ControlModifier):
+		if not (event.modifiers() & Qt.KeyboardModifier.ControlModifier):
 			return super().wheelEvent(event)
 
 		delta = event.angleDelta()
 		if delta.isNull() or not delta.y():
 			return
 		if delta.y() > 0:
 			self.zoom(at_cursor=True)
@@ -313,15 +313,15 @@
 				self._setPixmap(self._getScaledPixmap(self.originalPixmap.size() * self.zoomFactor))
 		elif self.zoomMode == ZOOM_FITALL:
 			newpix = self._getScaledPixmap(self.viewport().size())
 			self._setPixmap(newpix)
 			self.oldZoomFactor = self.zoomFactor
 			self.zoomFactor = newpix.size().width() / float(self.originalPixmap.size().width())
 		elif self.zoomMode == ZOOM_FITCUT:
-			newpix = self._getScaledPixmap(self.viewport().size(), Qt.KeepAspectRatioByExpanding)
+			newpix = self._getScaledPixmap(self.viewport().size(), Qt.AspectRatioMode.KeepAspectRatioByExpanding)
 			self._setPixmap(newpix)
 			self.oldZoomFactor = self.zoomFactor
 			self.zoomFactor = newpix.size().width() / float(self.originalPixmap.size().width())
 
 		def scroll_after_zoom():
 			hbar.setValue(int(scrollbarPos.x() + delta.x()))
 			vbar.setValue(int(scrollbarPos.y() + delta.y()))
@@ -329,12 +329,12 @@
 		newScale = self.zoomFactor
 		delta = deltaToPos * newScale - deltaToPos * oldScale
 
 		# XXX the pixmap is not fully loaded and displayed yet, so the scrollbars maximum values
 		# are not up to date yet, so we have to wait before restoring the relative scroll position
 		QTimer.singleShot(0, scroll_after_zoom)
 
-	def _getScaledPixmap(self, size, mode=Qt.KeepAspectRatio):
-		return self.originalPixmap.scaled(size, mode, Qt.SmoothTransformation)
+	def _getScaledPixmap(self, size, mode=Qt.AspectRatioMode.KeepAspectRatio):
+		return self.originalPixmap.scaled(size, mode, Qt.TransformationMode.SmoothTransformation)
 
 	def _setPixmap(self, pixmap):
 		self.widget().setPixmap(pixmap)
```

### Comparing `sittagger-0.6.2/sittagger/imagewidgets.py` & `sittagger-1.0.0/sittagger/imagewidgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-License-Identifier: WTFPL
 
 import difflib
 from pathlib import Path
 import re
 
-from PyQt5.QtCore import (
+from PyQt6.QtCore import (
 	QSize, Qt, pyqtSlot as Slot, pyqtSignal as Signal, QAbstractListModel, QVariant,
 	QModelIndex, QMimeData, QFileSystemWatcher,
 )
-from PyQt5.QtGui import QPixmap, QKeySequence, QPixmapCache, QColor
-from PyQt5.QtWidgets import (
-	QListView, QAction, QInputDialog, QLineEdit, QMessageBox,
+from PyQt6.QtGui import QPixmap, QKeySequence, QPixmapCache, QColor, QAction
+from PyQt6.QtWidgets import (
+	QListView, QInputDialog, QLineEdit, QMessageBox,
 )
 
 from .fileoperationdialog import FileOperationProgressDialog
 from .fm_interop import mark_for_copy, mark_for_cut, ClipQt, MIME_LIST, _parse_url
 from .fsops import rename_file, FileOperation, trash_items, can_trash
 from . import thumbnailmaker
 
@@ -52,37 +52,37 @@
 
 	def rowCount(self, qidx):
 		return len(self.entries)
 
 	def data(self, qidx, role):
 		path = self.entries[qidx.row()]
 
-		if role == Qt.DisplayRole:
+		if role == Qt.ItemDataRole.DisplayRole:
 			return QVariant(path.name)
-		elif role == Qt.DecorationRole:
+		elif role == Qt.ItemDataRole.DecorationRole:
 			thumbnailmaker.maker.reprioritizeTask(str(path))
 
 			try:
 				tpath = self.thumbs[str(path)]
 			except KeyError:
 				return QVariant(self.emptypix)
 			return QVariant(self._pixmap(tpath))
-		elif role == Qt.UserRole:
+		elif role == Qt.ItemDataRole.UserRole:
 			return QVariant(str(path))
 		else:
 			return QVariant()
 
 	def flags(self, qidx):
 		flags = super().flags(qidx)
 		if qidx.isValid():
 			flags |= (
-				Qt.ItemIsSelectable
-				| Qt.ItemIsEnabled
-				| Qt.ItemIsDragEnabled
-				| Qt.ItemNeverHasChildren
+				Qt.ItemFlag.ItemIsSelectable
+				| Qt.ItemFlag.ItemIsEnabled
+				| Qt.ItemFlag.ItemIsDragEnabled
+				| Qt.ItemFlag.ItemNeverHasChildren
 			)
 		return flags
 
 	def _pixmap(self, path):
 		path = str(path)
 		pix = QPixmapCache.find(path)
 		if not pix or not pix.isNull():
@@ -153,15 +153,15 @@
 			idx = self.entries.index(Path(origpath))
 		except ValueError:
 			return
 
 		self.thumbs[origpath] = thumbpath
 
 		qidx = self.index(idx)
-		self.dataChanged.emit(qidx, qidx, [Qt.DecorationRole])
+		self.dataChanged.emit(qidx, qidx, [Qt.ItemDataRole.DecorationRole])
 
 
 def key_name_ints(name):
 	"""key function to sort names by treating digits sequences as numbers.
 
 	Lexical order: bar < foo1 < foo10 < foo2 < quux
 	key_name_ints: bar < foo1 < foo2 < foo10 < quux
@@ -186,15 +186,15 @@
 		self.watcher = QFileSystemWatcher(self)
 		self.watcher.directoryChanged.connect(self._directoryChanged)
 		self.watcher.fileChanged.connect(self._fileChanged)
 
 	def flags(self, qidx):
 		flags = super().flags(qidx)
 		if not qidx.isValid():
-			flags |= Qt.ItemIsDropEnabled
+			flags |= Qt.ItemFlag.ItemIsDropEnabled
 		return flags
 
 	@Slot(str)
 	def _directoryChanged(self, path):
 		self.refreshDir()
 
 	@Slot(str)
@@ -240,15 +240,15 @@
 				self.entries[qidx.row()].absolute().as_uri().encode("ascii")
 				for qidx in qindexes
 			) + b"\r\n"
 		)
 		return ret
 
 	def supportedDropActions(self):
-		return Qt.CopyAction | Qt.MoveAction
+		return Qt.DropAction.CopyAction | Qt.DropAction.MoveAction
 
 	def canDropMimeData(self, qmime, action, row, column, parent_qidx):
 		if column > 0:
 			return False
 
 		files = self._getDroppedPaths(qmime)
 		if not files:
@@ -266,17 +266,17 @@
 		if not self.canDropMimeData(qmime, action, row, column, parent_qidx):
 			return False
 
 		files = self._getDroppedPaths(qmime)
 		if not files:
 			return False
 
-		if action == Qt.MoveAction:
+		if action == Qt.DropAction.MoveAction:
 			op = "cut"
-		elif action == Qt.CopyAction:
+		elif action == Qt.DropAction.CopyAction:
 			op = "copy"
 		else:
 			raise NotImplementedError()
 
 		treeop = FileOperation(self.path, files, op, db=None)
 		self.fileOperation.emit(treeop)
 
@@ -309,54 +309,58 @@
 	pasteRequested = Signal()
 
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 
 		action = QAction(self.tr("Re&name"), self)
 		action.setShortcut(QKeySequence("F2"))
-		action.setShortcutContext(Qt.WidgetShortcut)
+		action.setShortcutContext(Qt.ShortcutContext.WidgetShortcut)
 		action.triggered.connect(self.popRenameSelected)
 		self.addAction(action)
 
 		action = QAction(self.tr("&Copy files"), self)
-		action.setShortcut(QKeySequence(QKeySequence.Copy))
-		action.setShortcutContext(Qt.WidgetShortcut)
+		action.setShortcut(QKeySequence(QKeySequence.StandardKey.Copy))
+		action.setShortcutContext(Qt.ShortcutContext.WidgetShortcut)
 		action.triggered.connect(self.markForCopy)
 		self.addAction(action)
 
 		action = QAction(self.tr("Cut files"), self)
-		action.setShortcut(QKeySequence(QKeySequence.Cut))
-		action.setShortcutContext(Qt.WidgetShortcut)
+		action.setShortcut(QKeySequence(QKeySequence.StandardKey.Cut))
+		action.setShortcutContext(Qt.ShortcutContext.WidgetShortcut)
 		action.triggered.connect(self.markForCut)
 		self.addAction(action)
 
 		action = QAction(self.tr("&Paste files"), self)
-		action.setShortcut(QKeySequence(QKeySequence.Paste))
-		action.setShortcutContext(Qt.WidgetShortcut)
+		action.setShortcut(QKeySequence(QKeySequence.StandardKey.Paste))
+		action.setShortcutContext(Qt.ShortcutContext.WidgetShortcut)
 		action.triggered.connect(self.pasteRequested)
 		self.addAction(action)
 
 		action = QAction(self.tr("Trash selected"), self)
-		action.setShortcut(QKeySequence(QKeySequence.Delete))
-		action.setShortcutContext(Qt.WidgetShortcut)
+		action.setShortcut(QKeySequence(QKeySequence.StandardKey.Delete))
+		action.setShortcutContext(Qt.ShortcutContext.WidgetShortcut)
 		action.triggered.connect(self.trashSelected)
 		self.addAction(action)
 
-		self.setContextMenuPolicy(Qt.ActionsContextMenu)
+		self.setContextMenuPolicy(Qt.ContextMenuPolicy.ActionsContextMenu)
 
 	def selectionChanged(self, new, old):
 		self.itemSelectionChanged.emit()
 
 	itemSelectionChanged = Signal()
 
 	def showEvent(self, ev):
 		super().showEvent(ev)
 		self.verticalScrollBar().setSingleStep(32)
 
-	acceptedMouseButtons = {Qt.LeftButton, Qt.RightButton, Qt.MiddleButton}
+	acceptedMouseButtons = {
+		Qt.MouseButton.LeftButton,
+		Qt.MouseButton.RightButton,
+		Qt.MouseButton.MiddleButton,
+	}
 
 	def mousePressEvent(self, ev):
 		if ev.button() in self.acceptedMouseButtons:
 			super().mousePressEvent(ev)
 		ev.ignore()
 
 	def browseDir(self, path):
@@ -387,15 +391,15 @@
 
 		current = selected[0]
 
 		new, ok = QInputDialog.getText(
 			self,
 			self.tr("Rename file"),
 			self.tr("New name for file"),
-			QLineEdit.Normal,
+			QLineEdit.EchoMode.Normal,
 			current.name
 		)
 
 		if not ok or not new or new == current.name:
 			return
 		if "/" in new:
 			QMessageBox.critical(
@@ -411,15 +415,15 @@
 		# TODO update model
 
 	def selectedPaths(self):
 		return [Path(spath).absolute() for spath in self.selectedFiles()]
 
 	def selectedFiles(self):
 		return [
-			qidx.data(Qt.UserRole)
+			qidx.data(Qt.ItemDataRole.UserRole)
 			for qidx in self.selectedIndexes()
 		]
 
 	@Slot()
 	def markForCopy(self):
 		paths = self.selectedPaths()
 		if not paths:
@@ -454,11 +458,11 @@
 			return
 
 		button = QMessageBox.question(
 			self,
 			self.tr("Send to trash?"),
 			self.tr("Are you sure you want to send %d item(s) to trash?") % len(paths),
 		)
-		if button != QMessageBox.Yes:
+		if button != QMessageBox.StandardButton.Yes:
 			return
 
 		trash_items(paths)
```

### Comparing `sittagger-0.6.2/sittagger/mainwindow.ui` & `sittagger-1.0.0/sittagger/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.2/sittagger/tagwidgets.py` & `sittagger-1.0.0/sittagger/tagwidgets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: WTFPL
 
-from PyQt5.QtCore import Qt, pyqtSignal as Signal, pyqtSlot as Slot, QSortFilterProxyModel
-from PyQt5.QtGui import QStandardItem, QStandardItemModel
-from PyQt5.QtWidgets import QInputDialog, QVBoxLayout, QAction, QDialog, QListView, QLineEdit
+from PyQt6.QtCore import Qt, pyqtSignal as Signal, pyqtSlot as Slot, QSortFilterProxyModel
+from PyQt6.QtGui import QStandardItem, QStandardItemModel, QAction
+from PyQt6.QtWidgets import QInputDialog, QVBoxLayout, QDialog, QListView, QLineEdit
 
 
 class TagFilter(QLineEdit):
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.textChanged.connect(self.updateFilter)
 		self.widget = None
@@ -32,15 +32,15 @@
 		self.paths = []
 
 		self.data = QStandardItemModel(self)
 		self.proxy = QSortFilterProxyModel(self)
 		self.proxy.setSourceModel(self.data)
 		self.setModel(self.proxy)
 
-		self.setContextMenuPolicy(Qt.ActionsContextMenu)
+		self.setContextMenuPolicy(Qt.ContextMenuPolicy.ActionsContextMenu)
 		act = QAction('&Create tag', self)
 		act.triggered.connect(self._createTag)
 		self.addAction(act)
 
 		act = QAction('&Rename tag', self)
 		act.triggered.connect(self._renameTag)
 		self.addAction(act)
@@ -74,57 +74,57 @@
 		self.changedTags.emit()
 
 	def setFile(self, path):
 		return self.setFiles([path])
 
 	def _createItem(self, name):
 		item = QStandardItem(name)
-		item.setFlags(Qt.ItemIsSelectable | Qt.ItemIsUserCheckable | Qt.ItemIsEnabled)
-		item.setCheckState(Qt.Unchecked)
+		item.setFlags(Qt.ItemFlag.ItemIsSelectable | Qt.ItemFlag.ItemIsUserCheckable | Qt.ItemFlag.ItemIsEnabled)
+		item.setCheckState(Qt.CheckState.Unchecked)
 		return item
 
 	def setFiles(self, paths):
 		self.data.clear()
 		self.paths = paths
 
 		tags_per_file = {path: self.db.find_tags_by_file(path) for path in paths}
 		for tag in sorted(self.db.list_tags()):
 			item = self._createItem(tag)
 			item.setCheckState(self._state(tag, tags_per_file))
 			self.data.appendRow(item)
 
 	def _state(self, tag, tags_per_file):
 		if not tags_per_file:
-			return Qt.Unchecked
+			return Qt.CheckState.Unchecked
 
 		has_tag = any(tag in tags for tags in tags_per_file.values())
 		has_untag = any(tag not in tags for tags in tags_per_file.values())
 		if has_tag and has_untag:
-			return Qt.PartiallyChecked
+			return Qt.CheckState.PartiallyChecked
 		elif has_tag:
-			return Qt.Checked
+			return Qt.CheckState.Checked
 		elif has_untag:
-			return Qt.Unchecked
+			return Qt.CheckState.Unchecked
 		assert False
 
 		it = iter(tags_per_file.values())
 		first = (tag in it.next())
 		for tags in it:
 			current = (tag in tags)
 			if first != current:
-				return Qt.PartiallyChecked
+				return Qt.CheckState.PartiallyChecked
 		if first:
-			return Qt.Checked
+			return Qt.CheckState.Checked
 		else:
-			return Qt.Unchecked
+			return Qt.CheckState.Unchecked
 
 	@Slot('QStandardItem*')
 	def _tagStateChanged(self, item):
 		with self.db:
-			if item.checkState() == Qt.Unchecked:
+			if item.checkState() == Qt.CheckState.Unchecked:
 				for path in self.paths:
 					self.db.untag_file(path, [item.text()])
 			else:
 				for path in self.paths:
 					self.db.tag_file(path, [item.text()])
 
 	@Slot()
@@ -144,41 +144,41 @@
 		self.data = QStandardItemModel(self)
 		self.proxy = QSortFilterProxyModel(self)
 		self.proxy.setSourceModel(self.data)
 		self.setModel(self.proxy)
 
 		self.data.itemChanged.connect(self.changed)
 
-		self.setContextMenuPolicy(Qt.ActionsContextMenu)
+		self.setContextMenuPolicy(Qt.ContextMenuPolicy.ActionsContextMenu)
 		act = QAction('&Refresh tags', self)
 		act.triggered.connect(self.refreshTags)
 		self.addAction(act)
 
 	def setDb(self, db):
 		self.db = db
 
 		for t in sorted(self.db.list_tags()):
 			item = QStandardItem(t)
-			item.setFlags(Qt.ItemIsSelectable | Qt.ItemIsUserCheckable | Qt.ItemIsEnabled)
-			item.setCheckState(Qt.Unchecked)
+			item.setFlags(Qt.ItemFlag.ItemIsSelectable | Qt.ItemFlag.ItemIsUserCheckable | Qt.ItemFlag.ItemIsEnabled)
+			item.setCheckState(Qt.CheckState.Unchecked)
 			self.data.appendRow(item)
 
 	def setTags(self, tags):
 		for i in range(self.data.rowCount()):
 			item = self.data.item(i)
 			if item.text() in tags:
-				item.setCheckState(Qt.Checked)
+				item.setCheckState(Qt.CheckState.Checked)
 			else:
-				item.setCheckState(Qt.Unchecked)
+				item.setCheckState(Qt.CheckState.Unchecked)
 
 	def selectedTags(self):
 		tags = []
 		for i in range(self.data.rowCount()):
 			item = self.data.item(i)
-			if item.checkState() == Qt.Checked:
+			if item.checkState() == Qt.CheckState.Checked:
 				tags.append(item.text())
 		return tags
 
 	def matchingFiles(self):
 		tags = self.selectedTags()
 
 		if not tags:
```

### Comparing `sittagger-0.6.2/sittagger/thumbnailmaker.py` & `sittagger-1.0.0/sittagger/thumbnailmaker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: WTFPL
 
 from collections import OrderedDict
 import sys
 
-from PyQt5.QtCore import QObject, pyqtSlot as Slot, pyqtSignal as Signal, QProcess, QThread
+from PyQt6.QtCore import QObject, pyqtSlot as Slot, pyqtSignal as Signal, QProcess, QThread
 
 
 class ThumbnailMaker(QObject):
 	done = Signal(str, str)
 
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
```

### Comparing `sittagger-0.6.2/sittagger/videogrid.py` & `sittagger-1.0.0/sittagger/videogrid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: WTFPL
 
 import sys
 
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QSplitter, QMainWindow, QApplication, QInputDialog, QFileDialog
+from PyQt6.QtCore import Qt
+from PyQt6.QtWidgets import QSplitter, QMainWindow, QApplication, QInputDialog, QFileDialog
 
 from .videowidgets import BasicVideoWidget, VideoControl
 
 
 class GridManager(QSplitter):
 	def __init__(self, *args, **kwargs):
-		super().__init__(Qt.Horizontal, *args, **kwargs)
+		super().__init__(Qt.Orientation.Horizontal, *args, **kwargs)
 		self.addColumn()
 
 	def addColumn(self):
-		w = QSplitter(Qt.Vertical)
+		w = QSplitter(Qt.Orientation.Vertical)
 		self.addWidget(w)
 		w.splitterMoved.connect(self.subMoved)
 		return w
 
 	def subMoved(self, pos, index):
 		sender = self.sender()
 		for i in range(self.count()):
@@ -118,8 +118,8 @@
 		if f.startswith('/'):
 			v.load(f)
 		else:
 			v.loadUrl(f)
 		v.play()
 		w.centralWidget().addWidgetInGrid(v)
 
-	app.exec_()
+	app.exec()
```

### Comparing `sittagger-0.6.2/sittagger/videowidgets.py` & `sittagger-1.0.0/sittagger/videowidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # SPDX-License-Identifier: WTFPL
 
 import os.path
 
-from PyQt5.QtCore import pyqtSignal as Signal, pyqtSlot as Slot, QUrl, Qt
-from PyQt5.QtWidgets import QLabel, QWidget, QPushButton, QTableWidget, QTableWidgetItem, QSlider, QHBoxLayout, QVBoxLayout
-from PyQt5.QtMultimediaWidgets import QVideoWidget
-from PyQt5.QtMultimedia import (
+from PyQt6.QtCore import pyqtSignal as Signal, pyqtSlot as Slot, QUrl, Qt
+from PyQt6.QtWidgets import QLabel, QWidget, QPushButton, QTableWidget, QTableWidgetItem, QSlider, QHBoxLayout, QVBoxLayout
+from PyQt6.QtMultimediaWidgets import QVideoWidget
+from PyQt6.QtMultimedia import (
 	QMediaContent, QMediaPlayer, QMediaPlaylist,
 )
 
 from .tagwidgets import TagChooserDialog
 
 
 class SeekSlider(QSlider):
 	def __init__(self, mp):
-		super().__init__(Qt.Horizontal)
+		super().__init__(Qt.Orientation.Horizontal)
 		self.mediaPlayer = mp
 		self.mediaPlayer.durationChanged.connect(self._setMax)
 		self.mediaPlayer.seekableChanged.connect(self.setEnabled)
 		self.mediaPlayer.positionChanged.connect(self._slide)
 		self.valueChanged.connect(self.mediaPlayer.setPosition)
 
 		self.setEnabled(self.mediaPlayer.isSeekable())
@@ -258,15 +258,15 @@
 
 	def chooseTags(self, row):
 		row = self.table.currentRow()
 		taglist = self.table.item(row, 0).text().split(' ')
 
 		dialog = TagChooserDialog(self.db)
 		dialog.setTags(list(taglist))
-		dialog.exec_()
+		dialog.exec()
 		taglist = dialog.selectedTags()
 		self.table.item(row, 0).setText(' '.join(taglist))
 		#~ self.saveTags()
 
 	@Slot()
 	def rowSetStart(self):
 		ms = self.video.position()
```

### Comparing `sittagger-0.6.2/README.rst` & `sittagger-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `sittagger-0.6.2/pyproject.toml` & `sittagger-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
-    "PyQt5",
+    "PyQt6",
     "pyxdg",
     "vignette",
 ]
 
 [[project.authors]]
 name = "Hg"
 email = "dev@indigo.re"
@@ -53,15 +53,15 @@
 sit-tagger-cli = "sittagger.cli:main"
 
 [project.gui-scripts]
 sit-tagger = "sittagger.app:main"
 
 [project.urls]
 Homepage = "https://indigo.re/sit-tagger/"
-Project = "https://github.com/hydrargyrum/sit-tagger"
+Project = "https://gitlab.com/hydrargyrum/sit-tagger"
 PyPI = "https://pypi.org/project/sittagger/"
 
 [tool.hatch.version]
 path = "sittagger/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
```

### Comparing `sittagger-0.6.2/PKG-INFO` & `sittagger-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sittagger
-Version: 0.6.2
+Version: 1.0.0
 Summary: Image viewer with user-labels tag database
 Project-URL: Homepage, https://indigo.re/sit-tagger/
-Project-URL: Project, https://github.com/hydrargyrum/sit-tagger
+Project-URL: Project, https://gitlab.com/hydrargyrum/sit-tagger
 Project-URL: PyPI, https://pypi.org/project/sittagger/
 Author-email: Hg <dev@indigo.re>
 License-Expression: WTFPL
 License-File: COPYING.WTFPL
 Keywords: browser,database,image,label,labelling,photo,python,tag,tagging,viewer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: Qt
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment :: File Managers
 Classifier: Topic :: Multimedia :: Graphics :: Viewers
 Requires-Python: >=3.4
-Requires-Dist: pyqt5
+Requires-Dist: pyqt6
 Requires-Dist: pyxdg
 Requires-Dist: vignette
 Description-Content-Type: text/x-rst
 
 SIT-Tagger
 ==========
```

