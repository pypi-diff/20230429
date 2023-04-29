# Comparing `tmp/dspawpy-0.9.0-py3-none-any.whl.zip` & `tmp/dspawpy-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 70357 bytes, number of entries: 20
+Zip file size: 70630 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/__init__.py
 -rw-rw-rw-  2.0 fat    29208 b- defN 23-Apr-25 05:34 dspawpy/plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
--rw-rw-rw-  2.0 fat    23956 b- defN 23-Apr-25 05:50 dspawpy/analysis/aimdtools.py
+-rw-rw-rw-  2.0 fat    24557 b- defN 23-Apr-29 05:39 dspawpy/analysis/aimdtools.py
 -rw-rw-rw-  2.0 fat    20152 b- defN 23-Apr-04 06:32 dspawpy/analysis/vacf.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/diffusion/__init__.py
--rw-rw-rw-  2.0 fat     9639 b- defN 23-Apr-25 05:34 dspawpy/diffusion/neb.py
--rw-rw-rw-  2.0 fat    53458 b- defN 23-Apr-25 06:36 dspawpy/diffusion/nebtools.py
+-rw-rw-rw-  2.0 fat     3592 b- defN 23-Apr-26 09:25 dspawpy/diffusion/neb.py
+-rw-rw-rw-  2.0 fat    53467 b- defN 23-Apr-26 09:25 dspawpy/diffusion/nebtools.py
 -rw-rw-rw-  2.0 fat    11045 b- defN 23-Apr-25 05:34 dspawpy/diffusion/pathfinder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
--rw-rw-rw-  2.0 fat    41491 b- defN 23-Apr-25 06:36 dspawpy/io/read.py
+-rw-rw-rw-  2.0 fat    48925 b- defN 23-Apr-29 02:43 dspawpy/io/read.py
 -rw-rw-rw-  2.0 fat     7721 b- defN 23-Apr-25 05:46 dspawpy/io/read_json.py
--rw-rw-rw-  2.0 fat    13268 b- defN 23-Apr-25 06:36 dspawpy/io/structure.py
--rw-rw-rw-  2.0 fat    25265 b- defN 23-Apr-25 05:34 dspawpy/io/utils.py
--rw-rw-rw-  2.0 fat    17401 b- defN 23-Apr-25 06:36 dspawpy/io/write.py
+-rw-rw-rw-  2.0 fat     6163 b- defN 23-Apr-26 09:44 dspawpy/io/structure.py
+-rw-rw-rw-  2.0 fat    25241 b- defN 23-Apr-26 09:44 dspawpy/io/utils.py
+-rw-rw-rw-  2.0 fat    24416 b- defN 23-Apr-26 09:25 dspawpy/io/write.py
 -rw-rw-rw-  2.0 fat     1761 b- defN 23-Apr-25 05:51 dspawpy/io/write_json.py
--rw-rw-rw-  2.0 fat     1766 b- defN 23-Apr-26 02:17 dspawpy-0.9.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-26 02:17 dspawpy-0.9.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-26 02:17 dspawpy-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1582 b- defN 23-Apr-26 02:17 dspawpy-0.9.0.dist-info/RECORD
-20 files, 257813 bytes uncompressed, 67807 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     2036 b- defN 23-Apr-29 06:57 dspawpy-0.9.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 06:57 dspawpy-0.9.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-29 06:57 dspawpy-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1581 b- defN 23-Apr-29 06:57 dspawpy-0.9.1.dist-info/RECORD
+20 files, 259965 bytes uncompressed, 68080 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: dspawpy/io/write.py
 Comment: 
 
 Filename: dspawpy/io/write_json.py
 Comment: 
 
-Filename: dspawpy-0.9.0.dist-info/METADATA
+Filename: dspawpy-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-0.9.0.dist-info/WHEEL
+Filename: dspawpy-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-0.9.0.dist-info/top_level.txt
+Filename: dspawpy-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-0.9.0.dist-info/RECORD
+Filename: dspawpy-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/analysis/aimdtools.py

```diff
@@ -124,15 +124,29 @@
         self.ngrid = ngrid
 
         self.dr = (self.rmax - self.rmin) / (self.ngrid - 1)  # end points are on grid
         self.r = np.linspace(self.rmin, self.rmax, self.ngrid)  # type: ignore
 
         max_r = self.rmax + self.dr / 2.0  # add a small shell to improve robustness
 
-        self.neighbor_lists = [i.get_neighbor_list(max_r) for i in self.structures]
+        print(f"Calculating neighbor lists for {len(self.structures)} structures,")
+        self.neighbor_lists = []
+        for _c, i in enumerate(self.structures):
+            if _c == 0:
+                print('0%...', end='', flush=True)
+            elif _c/len(self.structures)*100 == 25:
+                print('25%...', end='', flush=True)
+            elif _c/len(self.structures)*100 == 50:
+                print('50%...', end='', flush=True)
+            elif _c/len(self.structures)*100 == 75:
+                print('75%...', end='', flush=True)
+            elif _c == len(self.structures)-1:
+                print('100%')
+            self.neighbor_lists.append(i.get_neighbor_list(max_r))
+
         # each neighbor list is a tuple of
         # center_indices, neighbor_indices, image_vectors, distances
         (
             self.center_indices,
             self.neighbor_indices,
             self.image_vectors,
             self.distances,  # 完整的距离列表（遍历体系所有原子）
@@ -154,15 +168,14 @@
                     j / self.structures[s_index].volume
                 )  # 原子数除以体积
 
         self.volumes = 4.0 * np.pi * self.r**2 * self.dr  # 分母的一部分
         self.volumes[self.volumes < 1e-8] = 1e8  # avoid divide by zero
         self.n_structures = len(self.structures)
         self.sigma = np.ceil(sigma / self.dr)
-        # print(elements)
 
     def _dist_to_counts(self, d):
         """Convert a distance array for counts in the bin
 
         Parameter
         ---------
             d: (1D np.array)
```

## dspawpy/diffusion/neb.py

```diff
@@ -1,24 +1,15 @@
-# -*- coding: utf-8 -*-
-import json
 import os
-from typing import List
-
-import matplotlib.pyplot as plt
-import numpy as np
-from pymatgen.core import Structure
-from scipy.interpolate import interp1d
 
 from dspawpy.diffusion.pathfinder import IDPPSolver
-from dspawpy.io.read import load_h5
-from dspawpy.io.structure import to_file
+from dspawpy.io.write import to_file
 
 
 class NEB:
-    """
+    """NEB插值算法
 
     Parameters
     ----------
     initial_structure: Structure
         初态
     final_structure: Structure
         终态
@@ -63,124 +54,16 @@
         step_size=0.05,
         max_disp=0.05,
         spring_const=5.0,
     ):
         return self.iddp.run(maxiter, tol, gtol, step_size, max_disp, spring_const)
 
 
-def plot_neb_barrier(
-    datafile: str,
-    ri: float = None,
-    rf: float = None,
-    ei: float = None,
-    ef: float = None,
-    show: bool = True,
-    figname: str = "neb_reaction_coordinate.png",
-):
-    """根据neb.json或者neb.h5绘制能垒图
-
-    如果NEB任务不计算初末态的自洽，这两个文件中将缺失相关信息，需要手动输入
-
-    Parameters
-    ----------
-    datafile : str
-        neb.json或neb.h5文件路径
-    ri : float
-        初态反应坐标
-    rf : float
-        末态反应坐标
-    ei : float
-        初态自洽能量
-    ef : float
-        末态自洽能量
-    show : bool, optional
-        是否展示交互式绘图窗口, 默认展示
-    figname : str
-        保存的图片名称, 默认'neb_reaction_coordinate.png'
-
-    Returns
-    -------
-    NEB能垒图
-
-    Examples
-    --------
-    >>> from dspawpy.diffusion.neb import plot_neb_barrier
-    >>> plot_neb_barrier("neb.h5") # neb.iniFin = true
-    >>> plot_neb_barrier("neb.h5",ri=0.0,rf=1.0,ei=-1.0,ef=-2.0) # neb.iniFin = false
-    """
-    # search datafile in the given directory
-    if os.path.isdir(datafile):
-        directory = datafile  # specified datafile is actually a directory
-        print("您指定了一个文件夹，正在查找相关h5或json文件...")
-        if os.path.exists(os.path.join(directory, "neb.h5")):
-            datafile = os.path.join(directory, "neb.h5")
-            print("Reading neb.h5...")
-        elif os.path.exists(os.path.join(directory, "neb.json")):
-            datafile = os.path.join(directory, "neb.json")
-            print("Reading neb.json...")
-        else:
-            raise FileNotFoundError("未找到neb.h5/neb.json文件！")
-
-    if datafile.endswith(".h5"):
-        neb = load_h5(datafile)
-        if "/BarrierInfo/ReactionCoordinate" in neb.keys():
-            reaction_coordinate = neb["/BarrierInfo/ReactionCoordinate"]
-            energy = neb["/BarrierInfo/TotalEnergy"]
-        else:  # old version
-            reaction_coordinate = neb["/Distance/ReactionCoordinate"]
-            energy = neb["/Energy/TotalEnergy"]
-    elif datafile.endswith(".json"):
-        with open(datafile, "r") as fin:
-            neb = json.load(fin)
-        if "BarrierInfo" in neb.keys():
-            reaction_coordinate = neb["BarrierInfo"]["ReactionCoordinate"]
-            energy = neb["BarrierInfo"]["TotalEnergy"]
-        else:  # old version
-            reaction_coordinate = neb["Distance"]["ReactionCoordinate"]
-            energy = neb["Energy"]["TotalEnergy"]
-    else:
-        raise TypeError("仅支持读取h5或json文件！")
-
-    x = []
-    for c in reaction_coordinate:
-        if len(x) > 0:
-            x.append(x[-1] + c)
-        else:
-            x.append(c)
-
-    y = [x - energy[0] for x in energy]
-    # initial and final info
-    if ri is not None:  # add initial reaction coordinate
-        x.insert(0, ri)
-    if rf is not None:  # add final reaction coordinate
-        x.append(rf)
-
-    if ei is not None:  # add initial energy
-        y.insert(0, ei)
-    if ef is not None:  # add final energy
-        y.append(ef)
-
-    inter_f = interp1d(x, y, kind="cubic")
-    xnew = np.linspace(x[0], x[-1], 100)
-    ynew = inter_f(xnew)
-
-    plt.plot(xnew, ynew, c="b")
-    plt.scatter(x, y, c="r")
-    plt.xlabel("Reaction Coordinate")
-    plt.ylabel("Energy")
-
-    if figname:
-        plt.tight_layout()
-        plt.savefig(figname)
-    if show:
-        plt.show()
-
-
 def write_neb_structures(
-    structures: List[Structure],
+    structures,
     coords_are_cartesian=True,
     fmt: str = "json",
     path: str = ".",
     prefix="structure",
 ):
     """插值并生成中间构型文件
 
@@ -198,24 +81,30 @@
     Returns
     -------
     file
         保存构型文件
 
     Examples
     --------
-    >>> from pymatgen.core import Structure
-    # 先调用pymatgen写好的from_file方法读取cif构型文件，生成structure对象
-    >>> initial_structure = Structure.from_file("initial.cif")
-    >>> final_structure = Structure.from_file("final.cif")
-    # 插值并生成中间构型文件
+
+    先读取as文件创建structure对象
+
+    >>> from dspawpy.io.structure import build_Structures_from_datafile
+    >>> initial_structure = build_Structures_from_datafile("structure00.as")[0]
+    >>> final_structure = build_Structures_from_datafile("structure06.as")[0]
+
+    然后，插值并生成中间构型文件
+
     >>> from dspawpy.diffusion.neb import NEB,write_neb_structures
     >>> neb = NEB(initial_structure,final_structure,10)
     >>> neb = NEB(init_struct,final_struct,5) # 设置插点个数
     >>> structures = neb.idpp_interpolate() # idpp插值，生成中间构型
-    # 可指定保存到neb文件夹下
+
+    插值完成的构型可指定保存到neb文件夹下
+
     >>> write_neb_structures(structures,coords_are_cartesian=True,fmt="as",path="neb")
     """
     N = len(str(len(structures)))
     if N <= 2:
         N = 2
     for i, structure in enumerate(structures):
         path_name = str(i).zfill(N)
@@ -225,75 +114,7 @@
         else:
             filename = os.path.join(
                 path, path_name, "%s%s.%s" % (prefix, path_name, fmt)
             )
             to_file(
                 structure, filename, coords_are_cartesian=coords_are_cartesian, fmt=fmt
             )
-
-
-def plot_neb_converge(neb_dir: str, image_key="01"):
-    # for compatibility
-    if neb_dir.endswith(".h5"):
-        neb_total = load_h5(neb_dir)
-        maxforce = np.array(neb_total["/Iteration/" + image_key + "/MaxForce"])
-        total_energy = np.array(neb_total["/Iteration/" + image_key + "/TotalEnergy"])
-    elif neb_dir.endswith(".json"):
-        with open(neb_dir, "r") as fin:
-            neb_total = json.load(fin)
-        try:
-            neb = neb_total["LoopInfo"][image_key]
-        except:
-            neb = neb_total["Iteration"][image_key]
-        maxforce = []
-        total_energy = []
-        for n in neb:
-            maxforce.append(n["MaxForce"])
-            total_energy.append(n["TotalEnergy"])
-
-    elif os.path.exists(f"{neb_dir}/neb.h5"):
-        neb_total = load_h5(f"{neb_dir}/neb.h5")
-        maxforce = np.array(neb_total["/Iteration/" + image_key + "/MaxForce"])
-        total_energy = np.array(neb_total["/Iteration/" + image_key + "/TotalEnergy"])
-
-    elif os.path.exists(f"{neb_dir}/neb.json"):
-        with open(f"{neb_dir}/neb.json", "r") as fin:
-            neb_total = json.load(fin)
-        try:
-            neb = neb_total["LoopInfo"][image_key]
-        except:
-            neb = neb_total["Iteration"][image_key]
-        maxforce = []
-        total_energy = []
-        for n in neb:
-            print(n)
-            maxforce.append(n["MaxForce"])
-            total_energy.append(n["TotalEnergy"])
-
-        maxforce = np.array(maxforce)
-        total_energy = np.array(total_energy)
-
-    else:
-        print(f"{neb_dir}路径中找不到neb.h5或者neb.json文件")
-
-    x = np.arange(len(maxforce))
-
-    force = maxforce
-    energy = total_energy
-
-    fig = plt.figure()
-    ax1 = fig.add_subplot(111)
-
-    ax1.plot(x, force, label="Max Force", c="black")
-    ax1.set_xlabel("Number of ionic step")
-    ax1.set_ylabel("Force")
-
-    ax2 = ax1.twinx()
-    ax2.plot(x, energy, label="Energy", c="r")
-    ax2.set_xlabel("Number of ionic step")
-    ax2.set_ylabel("Energy")
-    ax2.ticklabel_format(useOffset=False)  # y轴坐标显示绝对值而不是相对值
-
-    fig.legend(loc=1, bbox_to_anchor=(1, 1), bbox_transform=ax1.transAxes)
-    plt.tight_layout()
-
-    return ax1, ax2
```

## dspawpy/diffusion/nebtools.py

```diff
@@ -31,41 +31,45 @@
     Returns
     -------
     float
         距离
 
     Examples
     --------
-    >>> from dspawpy.diffusion.nebtools import get_distance
-    >>> from dspawpy.io.utils import get_spo_ele_lat
-    >>> # 先读取两个构型的分数坐标、元素列表和晶胞信息
-    >>> spo1, ele1, lat1 = get_spo_ele_lat('structure01.as')
+
+    先读取两个构型的分数坐标、元素列表和晶胞信息
+
+    >>> from dspawpy.io.read import pel_from_as
+    >>> spo1, ele1, lat1 = pel_from_as('structure01.as', sacled=True)
     >>> spo1
     array([[0.25      , 0.25      , 0.11784996],
            [0.75      , 0.25      , 0.11784996],
            ...，
            [0.04062186, 0.45937779, 0.43038044]])
     >>> ele1
     ['Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt']
     >>> lat1
     array([[ 5.6058,  0.    ,  0.    ],
            [ 0.    ,  5.6058,  0.    ],
            [ 0.    ,  0.    , 16.8174]])
-    >>> spo2, ele2, lat2 = get_spo_ele_lat('structure02.as')
+    >>> spo2, ele2, lat2 = pel_from_as('structure02.as', sacled=True)
     >>> spo2
     array([[0.25      , 0.25      , 0.11784996],
            ...，
            [0.08124389, 0.41875557, 0.41408303]])
     >>> ele2
     ['Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt']
     >>> lat2
     array([[ 5.6058,  0.    ,  0.    ],
            [ 0.    ,  5.6058,  0.    ],
            [ 0.    ,  0.    , 16.8174]])
-    >>> # 计算两个构型的距离
+
+    计算两个构型的距离
+
+    >>> from dspawpy.diffusion.nebtools import get_distance
     >>> dist = get_distance(spo1, spo2, lat1, lat2)
     >>> dist
     0.5987379724194888
     """
     diff_spo = spo1 - spo2  # 分数坐标差
     avglatv = 0.5 * (lat1 + lat2)  # 平均晶格矢量
     pbc_diff_spo = set_pbc(diff_spo)  # 笛卡尔坐标差
```

## dspawpy/io/read.py

```diff
@@ -13,29 +13,149 @@
 from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
 from pymatgen.electronic_structure.core import Orbital, Spin
 from pymatgen.electronic_structure.dos import CompleteDos, Dos
 from pymatgen.phonon.bandstructure import PhononBandStructureSymmLine
 from pymatgen.phonon.dos import PhononDos
 
 
-def get_lines_without_comment(filename: str, comment: str = "#"):
-    lines = []
-    """Filter out comment lines"""
-    with open(filename) as file:
-        while True:
-            line = file.readline()
-            if line:
-                line = re.sub(comment + r".*$", "", line)  # remove comment
-                line = line.strip()
-                if line:
-                    lines.append(line)
-            else:
-                break
+def get_band_data(band_dir: str, efermi: float = None) -> BandStructureSymmLine:
+    """读取h5或json文件中的能带数据，构建BandStructureSymmLine对象
 
-    return lines
+    Parameters
+    ----------
+    band_dir : str
+        能带文件路径，band.h5 / band.json
+    efermi : float, optional
+        费米能级，如果h5文件中的费米能级不正确，可以通过此参数指定费米能级
+
+    Returns
+    -------
+    BandStructureSymmLine
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_band_data
+    >>> band = get_band_data(band_dir='band.h5')
+    >>> band.branches
+    [{'start_index': 0, 'end_index': 100, 'name': 'R-G'}, {'start_index': 101, 'end_index': 201, 'name': 'G-X'}]
+    """
+    if band_dir.endswith(".h5"):
+        band = load_h5(band_dir)
+        raw = h5py.File(band_dir, "r").keys()
+        if "/WannBandInfo/NumberOfBand" in raw:
+            (
+                structure,
+                kpoints,
+                eigenvals,
+                rEf,
+                labels_dict,
+                projections,
+            ) = _get_band_data_h5(band, iwan=True)
+        elif "/BandInfo/NumberOfBand" in raw:
+            (
+                structure,
+                kpoints,
+                eigenvals,
+                rEf,
+                labels_dict,
+                projections,
+            ) = _get_band_data_h5(band, iwan=False)
+        else:
+            print("BandInfo or WannBandInfo key not found in h5file!")
+            return
+    elif band_dir.endswith(".json"):
+        with open(band_dir, "r") as fin:
+            band = json.load(fin)
+        if "WannBandInfo" in band.keys():
+            (
+                structure,
+                kpoints,
+                eigenvals,
+                rEf,
+                labels_dict,
+                projections,
+            ) = _get_band_data_json(band, iwan=True)
+        elif "BandInfo" in band.keys():
+            (
+                structure,
+                kpoints,
+                eigenvals,
+                rEf,
+                labels_dict,
+                projections,
+            ) = _get_band_data_json(band, iwan=False)
+        else:
+            print("BandInfo or WannBandInfo key not found in json file!")
+            return
+    else:
+        raise TypeError(f"{os.path.abspath(band_dir)} must be h5 or json file!")
+
+    if efermi:  # 从h5直接读取的费米能级可能是错的，此时需要用户自行指定
+        rEf = efermi  # 这只是个临时解决方案
+
+    lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
+    return BandStructureSymmLine(
+        kpoints=kpoints,
+        eigenvals=eigenvals,
+        lattice=lattice_new,
+        efermi=rEf,
+        labels_dict=labels_dict,
+        structure=structure,
+        projections=projections,
+    )
+
+
+def get_dos_data(dos_dir: str) -> CompleteDos or Dos:
+    """读取h5或json文件中的态密度数据，构建CompleteDos或DOS对象
+
+    Parameters
+    ----------
+    dos_dir : str
+        态密度文件路径，dos.h5 / dos.json
+
+    Returns
+    -------
+    CompleteDos or Dos
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_dos_data
+    >>> dos = get_dos_data(dos_dir='dos.h5')
+    >>> print(dos)
+    Complete DOS for Full Formula (Cu4)
+    Reduced Formula: Cu
+    abc   :   3.614700   3.614700   3.614700
+    angles:  90.000000  90.000000  90.000000
+    pbc   :       True       True       True
+    Sites (4)
+    #  SP       a     b     c
+    ---  ----  ----  ----  ----
+    0  Cu    0.25  0.25  0.25
+    1  Cu    0.75  0.75  0.25
+    2  Cu    0.75  0.25  0.75
+    3  Cu    0.25  0.75  0.75
+    """
+    if dos_dir.endswith(".h5"):
+        dos = load_h5(dos_dir)
+        if dos["/DosInfo/Project"][0]:
+            return _get_complete_dos(dos)
+        else:
+            return _get_total_dos(dos)
+
+    elif dos_dir.endswith(".json"):
+        with open(dos_dir, "r") as fin:
+            dos = json.load(fin)
+
+        if dos["DosInfo"]["Project"]:
+            return _get_complete_dos_json(dos)
+        else:
+            return _get_total_dos_json(dos)
+
+    else:
+        raise TypeError(f"{os.path.abspath(dos_dir)} must be h5 or json file!")
 
 
 def get_ele_from_h5(hpath: str = "aimd.h5"):
     """从h5文件中读取元素列表；
     多离子步并不会在每个离子步的Structure中保存元素信息，只能读取初始结构的元素信息
 
     Parameters
@@ -46,35 +166,155 @@
     Returns
     -------
     ele : list
         元素列表, Natom x 1
 
     Examples
     --------
-    >>> from dspawpy.io.utils import get_ele_from_h5
+    >>> from dspawpy.io.read import get_ele_from_h5
     >>> ele = get_ele_from_h5(hpath='aimd.h5')
+    >>> ele
     ['H', 'H', 'O']
     """
     data = h5py.File(hpath)
     Elements_bytes = np.array(data.get("/AtomInfo/Elements"))
     tempdata = np.array([i.decode() for i in Elements_bytes])
     ele = "".join(tempdata).split(";")
 
     return ele
 
 
+def get_lines_without_comment(filename: str, comment: str = "#"):
+    """读取as文件内容，移除批注后返回行列表
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_lines_without_comment
+    >>> lines = get_lines_without_comment(filename='structure.as', comment='#')
+    >>> lines
+    ['Total number of atoms', '12', 'Lattice', '5.04621935 0.00000000 0.00000000', '0.00000000 5.07315250 0.00000000', '0.00000000 0.00000000 5.25768906', 'Cartesian', 'Hf 1.34815269 1.22145223 0.17639072', 'Hf 1.34815269 3.75802848 2.45245381', 'Hf 3.69806666 1.22145223 2.80523525', 'Hf 3.69806666 3.75802848 5.08129834', 'O 0.35195212 1.93667285 1.92589951', 'O 0.35195212 4.47324910 0.70294502', 'O 2.32678304 2.48829365 3.85528784', 'O 2.32678304 5.02486990 4.03124575', 'O 2.71943630 5.02486990 1.40240122', 'O 2.71943630 2.48829365 1.22644331', 'O 4.69426723 1.93667285 4.55474404', 'O 4.69426723 4.47324910 3.33178955']
+    """
+    lines = []
+    """Filter out comment lines"""
+    with open(filename) as file:
+        while True:
+            line = file.readline()
+            if line:
+                line = re.sub(comment + r".*$", "", line)  # remove comment
+                line = line.strip()
+                if line:
+                    lines.append(line)
+            else:
+                break
+
+    return lines
+
+
+def get_phonon_band_data(phonon_band_dir: str) -> PhononBandStructureSymmLine:
+    """读取h5或json文件中的声子能带数据，构建PhononBandStructureSymmLine对象
+
+    Parameters
+    ----------
+    phonon_band_dir : str
+        能带文件路径，phonon.h5 / phonon.json
+
+    Returns
+    -------
+    PhononBandStructureSymmLine
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_phonon_band_data
+    >>> phband = get_phonon_band_data(phonon_band_dir='phonon.h5')
+    >>> phband.branches
+    [{'start_index': 0, 'end_index': 50, 'name': 'G-X'}, {'start_index': 51, 'end_index': 101, 'name': 'X-W'}, {'start_index': 102, 'end_index': 152, 'name': 'W-G'}, {'start_index': 153, 'end_index': 203, 'name': 'G-M'}]
+    """
+    if phonon_band_dir.endswith(".h5"):
+        band = load_h5(phonon_band_dir)
+        (
+            symmmetry_kpoints,
+            symmetry_kPoints_index,
+            kpoints,
+            structure,
+            frequencies,
+        ) = _get_phonon_band_data_h5(band)
+    elif phonon_band_dir.endswith(".json"):
+        with open(phonon_band_dir, "r") as fin:
+            band = json.load(fin)
+        (
+            symmmetry_kpoints,
+            symmetry_kPoints_index,
+            kpoints,
+            structure,
+            frequencies,
+        ) = _get_phonon_band_data_json(band)
+    else:
+        raise TypeError(f"{os.path.abspath(phonon_band_dir)} must be h5 or json file")
+
+    labels_dict = {}
+    for i, s in enumerate(symmmetry_kpoints):
+        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
+    lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
+
+    return PhononBandStructureSymmLine(
+        qpoints=kpoints,
+        frequencies=frequencies,
+        lattice=lattice_new,
+        has_nac=False,
+        labels_dict=labels_dict,
+        structure=structure,
+    )
+
+
+def get_phonon_dos_data(phonon_dos_dir: str) -> PhononDos:
+    """读取h5或json文件中的声子态密度数据，构建PhononDos对象
+
+    Parameters
+    ----------
+    phonon_dos_dir : str
+        声子态密度文件路径，phonon_dos.h5 / phonon_dos.json
+
+    Returns
+    -------
+    PhononDos
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import get_phonon_dos_data
+    >>> phdos = get_phonon_dos_data(phonon_dos_dir='phonon_dos.h5')
+    >>> phdos.frequencies
+    array([ 0. ,  0.1,  0.2,  0.3,  0.4,  0.5,  0.6,  0.7,  0.8,  0.9,  1. ,
+            1.1,  1.2,  1.3,  1.4,  1.5,  1.6,  1.7,  1.8,  1.9,  2. ,  2.1,
+            ...
+            39.6, 39.7, 39.8, 39.9, 40. ])
+    """
+    if phonon_dos_dir.endswith(".h5"):
+        dos = load_h5(phonon_dos_dir)
+        frequencies = np.asarray(dos["/DosInfo/DosEnergy"])
+        densities = dos["/DosInfo/Spin1/Dos"]
+    elif phonon_dos_dir.endswith(".json"):
+        with open(phonon_dos_dir, "r") as fin:
+            dos = json.load(fin)
+        frequencies = np.asarray(dos["DosInfo"]["DosEnergy"])
+        densities = dos["DosInfo"]["Spin1"]["Dos"]
+    else:
+        raise TypeError(f"{os.path.abspath(phonon_dos_dir)} must be h5 or json file")
+
+    return PhononDos(frequencies, densities)
+
+
 def get_sinfo(datafile: str, scaled=False, index=None, ele=None, ai=None):
-    """Wrapper to get structure information from h5/json/as file
+    """Wrapper to get structure information from h5/json/as file.
 
     从datafile中读取结构信息
 
     Parameters
     ----------
     datafile : str
-        h5文件或json结果文件路径
+        h5 / json结果文件或as结构文件路径
     scaled : bool, optional
         是否返回分数坐标，默认False
     index : int or list or str, optional
         运动轨迹中的第几步，从1开始计数
         如果要切片，用字符串写法： '1, 10'
         默认为None，返回所有步
     ele : list, optional
@@ -85,39 +325,55 @@
         如果要切片，用字符串写法： '1, 10'
         默认为None，返回所有离子步
 
     Returns
     -------
     Nstep : int
         总离子步数（几个构型）
-    pos : np.ndarray
-        坐标分量数组，Natom x 3
     ele : list
         元素列表, Natom x 1
+    pos : np.ndarray
+        坐标分量数组，Nstep x Natom x 3
     latv : np.ndarray
-        晶胞矢量数组，3 x 3
+        晶胞矢量数组，Nstep x 3 x 3
     D_mag_fix : dict
         磁矩、自由度相关信息
 
     Examples
     --------
+
     >>> from dspawpy.io.read import get_sinfo
+    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='aimd.h5', scaled=False, index=None, ele=None, ai=None)
+    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='relax.json', scaled=False, index=None, ele=None, ai=None)
+    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='rho.json', scaled=False)
+    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='structure.as', scaled=False)
+
+    这些信息可以用于进一步构建Structure对象，
+    具体参考 dspawpy.io.structure.build_Structures_from_datafile 函数
     """
     if datafile.endswith(".h5"):
         assert os.path.exists(datafile), f"{os.path.abspath(datafile)} does not exist!"
         Nstep, eles, pos, latv, D_mag_fix = _sinfo_from_h5(
             hpath=datafile, index=index, ele=ele, ai=ai, return_scaled=scaled
         )
     elif datafile.endswith(".json"):
         assert os.path.exists(datafile), f"{os.path.abspath(datafile)} does not exist!"
         Nstep, eles, pos, latv, D_mag_fix = _sinfo_from_json(
-            jpath=datafile, return_scaled=scaled
+            jpath=datafile, index=index, ele=ele, ai=ai, return_scaled=scaled
         )
+    elif datafile.endswith(".as"):
+        print("Reading mag & fix info from .as file is not supported yet!")
+        p, e, l = pel_from_as(spath=datafile, scaled=scaled)
+        pos = [p]
+        eles = e
+        latv = [l]
+        Nstep = 1
+        D_mag_fix = None
     else:
-        raise ValueError("datafile must be .h5 / .json file!")
+        raise ValueError("datafile must be .h5 / .json / .as file!")
 
     return Nstep, eles, pos, latv, D_mag_fix
 
 
 def pel_from_as(spath: str, scaled=False):
     """Extract structure information from .as file
 
@@ -152,14 +408,15 @@
     ['Mo', 'S', 'S']
     >>> latv
     array([[ 3.18406646,  0.        ,  0.        ],
            [-1.59203323,  2.75748245,  0.        ],
            [ 0.        ,  0.        , 30.        ]])
 
     if scaled=True, return scaled coordinates
+
     >>> spos, ele, latv = pel_from_as(spath='structure.as', scaled=True)
     >>> spos
     array([[0.        , 0.        , 0.30211854],
            [0.66666667, 0.33333333, 0.35423709],
            [0.66666667, 0.33333333, 0.25      ]])
     >>> ele
     ['Mo', 'S', 'S']
@@ -191,133 +448,242 @@
             pos = spos
         else:
             pos = np.dot(spos, latv)
 
     return pos, ele, latv
 
 
+def load_h5(dir_h5: str) -> dict:
+    """遍历读取h5文件中的数据，保存为字典格式
+
+    慎用此函数，因为会读取很多不需要的数据，耗时很长。
+
+    Parameters
+    ----------
+    dir_h5 : str
+        h5文件路径
+
+    Returns
+    -------
+    datas: dict
+        数据字典
+
+    Examples
+    --------
+    >>> from dspawpy.io.read import load_h5
+    >>> datas = load_h5(dir_h5)
+    """
+
+    def get_names(key, h5_object):
+        names.append(h5_object.name)
+
+    def is_dataset(name):
+        for name_inTheList in names:
+            if name_inTheList.find(name + "/") != -1:
+                return False
+        return True
+
+    def get_datas(key, h5_object):
+        if is_dataset(h5_object.name):
+            data = np.asarray(h5_object)
+            if data.dtype == "|S1":  # 转成字符串 并根据";"分割
+                byte2str = [str(bi, "utf-8") for bi in data]
+                string = ""
+                for char in byte2str:
+                    string += char
+                data = np.array([elem for elem in string.strip().split(";")])
+            # "/group1/group2/.../groupN/dataset" : value
+            datas[h5_object.name] = data.tolist()
+
+    with h5py.File(dir_h5, "r") as fin:
+        names = []
+        datas = {}
+        fin.visititems(get_names)
+        fin.visititems(get_datas)
+
+        return datas
+
+
+def load_h5_todict(dir_h5: str) -> dict:
+    """与上一个函数区别在于合并了部分同类数据，例如
+
+    /Structures/Step-1/* 和 /Structures/Step-2/* 并入 /Structures/ 组内
+    """
+
+    def create_dict(L: list, D: dict):
+        if len(L) == 2:
+            D[L[0]] = L[1]
+            return
+        else:
+            if not (L[0] in D.keys()):
+                D[L[0]] = {}
+            create_dict(L[1:], D[L[0]])
+
+    datas = load_h5(dir_h5)
+
+    groups_value_list = []
+    for key in datas.keys():
+        tmp_list = key[1:].strip().split("/")  # [1:] 截去root
+        tmp_list.append(datas[key])
+        # groups_value_list[i]结构: [group1, group2, ..., groupN, dataset, value]
+        groups_value_list.append(tmp_list)
+
+    groups_value_dict = {}
+    for data in groups_value_list:
+        create_dict(data, groups_value_dict)
+
+    return groups_value_dict
+
+
 def _sinfo_from_h5(
     hpath: str,
     index=None,
     ele=None,
     ai=None,
     return_scaled: bool = False,
 ):
     print(f"Reading {os.path.abspath(hpath)} ...")
     hf = h5py.File(hpath)  # 加载h5文件
-    Total_step = len(np.array(hf.get("/Structures"))) - 2  # 总步数
 
-    if ele is not None and ai is not None:
-        raise ValueError("暂不支持同时指定元素和原子序号")
-    # 步数
-    if index is not None:
-        if isinstance(index, int):  # 1
-            indices = [index]
+    # decide task type by check the internal key
+    if "/Structures" in hf.keys():  # multi-steps
+        Total_step = np.array(hf.get("/Structures/FinalStep"))[0]  # 总步数
+
+        if ele is not None and ai is not None:
+            raise ValueError("暂不支持同时指定元素和原子序号")
+        # 步数
+        if index is not None:
+            if isinstance(index, int):  # 1
+                indices = [index]
 
-        elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-            indices = index
+            elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                indices = index
 
-        elif isinstance(index, str):  # ':', '-3:'
-            indices = __parse_indices(index, Total_step)
+            elif isinstance(index, str):  # ':', '-3:'
+                indices = __parse_indices(index, Total_step)
+
+            else:
+                raise ValueError("请输入正确格式的index")
 
+            Nstep = len(indices)
         else:
-            raise ValueError("请输入正确格式的index")
+            Nstep = Total_step
+            indices = list(range(1, Nstep + 1))
 
-        Nstep = len(indices)
-    else:
-        Nstep = Total_step
-        indices = list(range(1, Nstep + 1))
+        # 读取元素列表，这个列表不会随步数改变，也不会“合并同类项”
+        Elements = np.array(get_ele_from_h5(hpath), dtype=object)
 
-    # 读取元素列表，这个列表不会随步数改变，也不会“合并同类项”
-    Elements = np.array(get_ele_from_h5(hpath), dtype=object)
+        # 开始读取晶胞和原子位置
+        lattices = np.empty((Nstep, 3, 3))  # Nstep x 3 x 3
+        location = []
+        if ele is not None:  # 如果用户指定元素
+            if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
+                ele_list = np.array(ele, dtype=object)
+                location = np.where(Elements == ele_list)[0]
+            # 多个元素符号组成的列表，例如 ['Fe', 'O']
+            elif isinstance(ele, list) or isinstance(ele, np.ndarray):
+                for e in ele:
+                    loc = np.where(Elements == e)[0]
+                    location.append(loc)
+                location = np.concatenate(location)
+            else:
+                raise TypeError("请输入正确的元素或元素列表")
+            elements = Elements[location]
 
-    # 开始读取晶胞和原子位置
-    lattices = np.empty((Nstep, 3, 3))  # Nstep x 3 x 3
-    location = []
-    if ele is not None:  # 如果用户指定元素
-        if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
-            ele_list = np.array(ele, dtype=object)
-            location = np.where(Elements == ele_list)[0]
-        # 多个元素符号组成的列表，例如 ['Fe', 'O']
-        elif isinstance(ele, list) or isinstance(ele, np.ndarray):
-            for e in ele:
-                loc = np.where(Elements == e)[0]
-                location.append(loc)
-            location = np.concatenate(location)
-        else:
-            raise TypeError("请输入正确的元素或元素列表")
-        elements = Elements[location]
+        elif ai is not None:  # 如果用户指定原子序号
+            if isinstance(ai, int):  # 1
+                ais = [ai]
+            elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                ais = ai
+            elif isinstance(ai, str):  # ':', '-3:'
+                ais = __parse_indices(ai, Total_step)
+            else:
+                raise ValueError("请输入正确格式的ai")
+            ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
+            elements = Elements[ais]
+            location = ais
 
-    elif ai is not None:  # 如果用户指定原子序号
-        if isinstance(ai, int):  # 1
-            ais = [ai]
-        elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-            ais = ai
-        elif isinstance(ai, str):  # ':', '-3:'
-            ais = __parse_indices(ai, Total_step)
-        else:
-            raise ValueError("请输入正确格式的ai")
-        ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
-        elements = Elements[ais]
-        location = ais
-
-    else:  # 如果都没指定
-        elements = Elements
-        location = list(range(len(Elements)))
-
-    elements = elements.tolist()  # for pretty output
-
-    mags = []  # must be Nstep x Natom x ?
-
-    poses = np.empty(shape=(len(indices), len(elements), 3))
-    for i, ind in enumerate(indices):  # 步数
-        lats = np.array(hf.get("/Structures/Step-" + str(ind) + "/Lattice"))
-        lattices[i] = lats
-        # [x1,y1,z1,x2,y2,z2,x3,y3,z3], ...
-        # 结构优化时输出的都是分数坐标，不管CoordinateType写的是啥！
-        pos = np.array(hf.get("/Structures/Step-" + str(ind) + "/Position"))
-        wrapped_pos = pos - np.floor(pos)  # wrap into [0,1)
-        wrapped_pos = wrapped_pos.flatten().reshape(-1, 3).T  # reshape
-
-        try:  # 自旋计算
-            mag = np.array(hf.get("/Structures/Step-" + str(ind) + "/Mag"))
-            if mag == None:
-                mag = np.zeros(shape=(len(elements), 1))
-        except Exception as e:
-            print(e)
-            mag = np.zeros(shape=(len(elements), 1))
-        mags.append(mag)
-
-    try:  # fix atom
-        atomfixs = np.array(hf.get("/AtomInfo/Fix")).astype(bool).flatten()
-        assert atomfixs.shape == (12,)  # np.ndarray (Natom x 3, )
-        atomfixs = atomfixs.reshape(-1, 3)  # (Natom, 3)
-    except Exception as e:
-        print(e)
-        atomfixs = np.full(shape=(len(elements), 3), fill_value=False)
-
-    mags = np.array(mags).reshape(Nstep, len(elements), -1)
-    # repeat atomfixs to Nstep x Natom x 3
-    atomfixs = np.repeat(atomfixs[np.newaxis, :, :], Nstep, axis=0).tolist()
-
-    D_mag_fix = {"Mags": mags, "AtomFixs": atomfixs}
-    print(
-        f"This function does not handle lattice fix info, \n you must manually set it before starting new calculations.."
-    )
+        else:  # 如果都没指定
+            elements = Elements
+            location = list(range(len(Elements)))
 
-    if return_scaled:  # Fractional coordinates
-        for i, ind in enumerate(indices):  # 步数
-            for j, sli in enumerate(location):
-                poses[i, j, :] = np.dot(wrapped_pos[:, sli], np.eye(3, 3))
-    else:  # Cartesian coordinates
+        elements = elements.tolist()  # for pretty output
+
+        mags = []  # must be Nstep x Natom x ?
+
+        poses = np.empty(shape=(len(indices), len(elements), 3))
+        wrapped_poses = np.empty(shape=(len(indices), 3, len(elements)))
         for i, ind in enumerate(indices):  # 步数
-            for j, sli in enumerate(location):
-                poses[i, j, :] = np.dot(wrapped_pos[:, sli], lats)
+            # print(f'{ind=}')
+            lats = np.array(hf.get("/Structures/Step-" + str(ind) + "/Lattice"))
+            lattices[i] = lats
+            # [x1,y1,z1,x2,y2,z2,x3,y3,z3], ...
+            # 结构优化时输出的都是分数坐标，不管CoordinateType写的是啥！
+            pos = np.array(hf.get("/Structures/Step-" + str(ind) + "/Position"))
+            wrapped_pos = pos - np.floor(pos)  # wrap into [0,1)
+            wrapped_pos = wrapped_pos.flatten().reshape(-1, 3).T  # reshape to 3 x Natom
+            wrapped_poses[i] = wrapped_pos
+
+            try:  # 自旋计算
+                mag = np.array(hf.get("/Structures/Step-" + str(ind) + "/Mag"))
+                if mag == None:
+                    mag = np.zeros(shape=(len(elements), 1))
+            except Exception as e:
+                if str(e): # ignore empty AssertionError()
+                    print(e)
+                mag = np.zeros(shape=(len(elements), 1))
+            mags.append(mag)
+
+        try:  # fix atom
+            atomfixs = np.array(hf.get("/AtomInfo/Fix")).astype(bool).flatten()
+            assert atomfixs.shape == (12,)  # np.ndarray (Natom x 3, )
+            atomfixs = atomfixs.reshape(-1, 3)  # (Natom, 3)
+        except Exception as e:
+            if str(e): # ignore empty AssertionError()
+                print(e)
+            atomfixs = np.full(shape=(len(elements), 3), fill_value=False)
+
+        mags = np.array(mags).reshape(Nstep, len(elements), -1)
+        # repeat atomfixs to Nstep x Natom x 3
+        atomfixs = np.repeat(atomfixs[np.newaxis, :, :], Nstep, axis=0).tolist()
+
+        D_mag_fix = {"Mags": mags, "AtomFixs": atomfixs}
+
+        if return_scaled:  # Fractional coordinates
+            for k, ind in enumerate(indices):  # 步数
+                for j, sli in enumerate(location):  # atom index
+                    poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
+        else:  # Cartesian coordinates
+            for k, ind in enumerate(indices):  # 步数
+                for j, sli in enumerate(location):
+                    poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
+
+        return Nstep, elements, poses, lattices, D_mag_fix
+
+    elif "/UnrelaxStructure" in hf.keys():  # single-step
+        raise NotImplementedError(
+            "Read from neb.h5 is not implemented yet!\n you may try neb01.h5.."
+        )
+    elif "/UnitAtomInfo" in hf.keys():  # phonon
+        raise NotImplementedError(
+            "Read from phonon.h5 is not implemented yet!\n you may try phonon001.h5.."
+        )
+    else:  # rho, potential, elf, pcharge
+        hfDict = load_h5(hpath)
+        s = _get_structure(hfDict, "/AtomInfo")
+        elements = s.species
+        poses = [s.cart_coords]
+        lattices = [s.lattice.matrix]
+        Nstep = 1
+        D_mag_fix = None
+        # print(
+        #     "You should check lattice fix info and manually set it before starting new calculations.."
+        # )
 
-    return Nstep, elements, poses, lattices, D_mag_fix
+        return Nstep, elements, poses, lattices, D_mag_fix
 
 
 def _sinfo_from_json(
     jpath: str,
     index=None,
     ele=None,
     ai=None,
@@ -337,156 +703,172 @@
     - positions: 原子位置, list, Nstep x Natom x 3
     - lattices: 晶胞, list, Nstep x 3 x 3
     """
     print(f"Reading {os.path.abspath(jpath)}...")
     with open(jpath, "r") as f:
         data = json.load(f)  # 加载json文件
 
-    if "Structures" in data:
-        Total_step = len(data["Structures"])  # aimd.json
-    else:
-        Total_step = len(data)  # relax.json, neb01.json
+    # decide the task type by checking the internal keys
+    if "AtomInfo" in data:  # single-step task
+        s = _get_structure_json(data["AtomInfo"])
+        elements = s.species
+        poses = [s.cart_coords]
+        lattices = [s.lattice.matrix]
+        Nstep = 1
+        D_mag_fix = None
+        return Nstep, elements, poses, lattices, D_mag_fix
+
+    elif "UnitAtomInfo" in data:  # phonon task
+        raise NotImplementedError("Read from phonon.json is not supported yet.")
+    elif "IniFin" in data:  # neb.json
+        raise NotImplementedError("Read from neb.json is not supported yet.")
+    elif "WannierInfo" in data:
+        raise NotImplementedError("wannier.json has no stucture info!")
+    else:  # multi-steps task
+        if "Structures" in data:
+            Total_step = len(data["Structures"])  # aimd.json
+        else:
+            Total_step = len(data)  # relax.json, neb01.json
 
-    if ele is not None and ai is not None:
-        raise ValueError("暂不支持同时指定元素和原子序号")
-    # 步数
-    if index is not None:
-        if isinstance(index, int):  # 1
-            indices = [index]
+        if ele is not None and ai is not None:
+            raise ValueError("暂不支持同时指定元素和原子序号")
+        # 步数
+        if index is not None:
+            if isinstance(index, int):  # 1
+                indices = [index]
 
-        elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-            indices = index
+            elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                indices = index
 
-        elif isinstance(index, str):  # ':', '-3:'
-            indices = __parse_indices(index, Total_step)
+            elif isinstance(index, str):  # ':', '-3:'
+                indices = __parse_indices(index, Total_step)
 
-        else:
-            raise ValueError("请输入正确格式的index")
+            else:
+                raise ValueError("请输入正确格式的index")
 
-        Nstep = len(indices)
-    else:
-        Nstep = Total_step
-        indices = list(range(1, Nstep + 1))  # [1,Nstep+1)
+            Nstep = len(indices)
+        else:
+            Nstep = Total_step
+            indices = list(range(1, Nstep + 1))  # [1,Nstep+1)
 
-    # 预先读取全部元素的总列表，这个列表不会随步数改变，也不会“合并同类项”
-    # 这样可以避免在循环内部频繁判断元素是否符合用户需要
+        # 预先读取全部元素的总列表，这个列表不会随步数改变，也不会“合并同类项”
+        # 这样可以避免在循环内部频繁判断元素是否符合用户需要
 
-    if "Structures" in data:
-        Nele = len(data["Structures"][0]["Atoms"])  # relax.json
-        total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
-        for i in range(Nele):
-            element = data["Structures"][0]["Atoms"][i]["Element"]
-            total_elements[i] = element
-    else:
-        Nele = len(data[0]["Atoms"])
-        total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
-        for i in range(Nele):
-            element = data[0]["Atoms"][i]["Element"]
-            total_elements[i] = element
-
-    Natom = len(total_elements)
-
-    # 开始读取晶胞和原子位置
-    # 在data['Structures']['%d' % index]['Atoms']中根据元素所在序号选择结构
-    if ele is not None:  # 用户指定要某些元素
-        location = []
-        if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
-            ele_list = list(ele)
-        # 多个元素符号组成的列表，例如 ['Fe', 'O']
-        elif isinstance(ele, list) or isinstance(ele, np.ndarray):
-            ele_list = ele
+        if "Structures" in data:
+            Nele = len(data["Structures"][0]["Atoms"])  # relax.json
+            total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
+            for i in range(Nele):
+                element = data["Structures"][0]["Atoms"][i]["Element"]
+                total_elements[i] = element
         else:
-            raise TypeError("请输入正确的元素或元素列表")
-        for e in ele_list:
-            location.append(np.where(total_elements == e)[0])
-        location = np.concatenate(location)
-
-    elif ai is not None:  # 如果用户指定原子序号，也要据此筛选元素列表
-        if isinstance(ai, int):  # 1
-            ais = [ai]
-        elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-            ais = ai
-        elif isinstance(ai, str):  # ':', '-3:'
-            ais = __parse_indices(ai, Total_step)
+            if "Atoms" not in data[0]:
+                raise NotImplementedError("nebXX.json has no structure info!")
+            Nele = len(data[0]["Atoms"])
+            total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
+            for i in range(Nele):
+                element = data[0]["Atoms"][i]["Element"]
+                total_elements[i] = element
+
+        Natom = len(total_elements)
+
+        # 开始读取晶胞和原子位置
+        # 在data['Structures']['%d' % index]['Atoms']中根据元素所在序号选择结构
+        if ele is not None:  # 用户指定要某些元素
+            location = []
+            if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
+                ele_list = list(ele)
+            # 多个元素符号组成的列表，例如 ['Fe', 'O']
+            elif isinstance(ele, list) or isinstance(ele, np.ndarray):
+                ele_list = ele
+            else:
+                raise TypeError("请输入正确的元素或元素列表")
+            for e in ele_list:
+                location.append(np.where(total_elements == e)[0])
+            location = np.concatenate(location)
+
+        elif ai is not None:  # 如果用户指定原子序号，也要据此筛选元素列表
+            if isinstance(ai, int):  # 1
+                ais = [ai]
+            elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                ais = ai
+            elif isinstance(ai, str):  # ':', '-3:'
+                ais = __parse_indices(ai, Total_step)
+            else:
+                raise ValueError("请输入正确格式的ai")
+            ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
+            location = ais
+            # read lattices and poses
+
+        else:  # 如果都没指定
+            location = list(range(Natom))
+
+        # 满足用户需要的elements列表
+        elements = np.empty(shape=(Natom,), dtype=object)
+        for i in range(len(location)):
+            elements[i] = total_elements[location[i]]
+
+        # Nstep x Natom x 3, positions are all fractional
+        positions = np.empty(shape=(len(indices), len(elements), 3))
+        lattices = np.empty(shape=(Nstep, 3, 3))  # Nstep x 3 x 3
+        mags = []  # Nstep x Natom x ?
+        Atomfixs = []  # Nstep x Natom x 3
+
+        if "Structures" in data:  # relax.json
+            for i, ind in enumerate(indices):  # for every ionic step
+                lat = data["Structures"][ind - 1]["Lattice"]
+                lattices[i] = np.array(lat).reshape(3, 3)
+                mag_for_each_step = []
+                fix_for_each_step = []
+                for j, sli in enumerate(location):
+                    ati = data["Structures"][ind - 1]["Atoms"][sli]
+                    positions[i, j, :] = ati["Position"][:]
+
+                    mag_for_each_atom = ati["Mag"][:]
+                    mag_for_each_step.append(mag_for_each_atom)
+
+                    fix_for_each_atom = ati["Fix"][:]
+                    if fix_for_each_atom == []:
+                        fix_for_each_atom = [0, 0, 0]
+                    fix_for_each_atom = [bool(i) for i in fix_for_each_atom]
+                    fix_for_each_step.append(fix_for_each_atom)
+
+                mags.append(mag_for_each_step)
+                Atomfixs.append(fix_for_each_step)
+                if not return_scaled:
+                    positions = np.dot(positions, lattices[i])
         else:
-            raise ValueError("请输入正确格式的ai")
-        ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
-        location = ais
-        # read lattices and poses
-
-    else:  # 如果都没指定
-        location = list(range(Natom))
-
-    # 满足用户需要的elements列表
-    elements = np.empty(shape=(Natom,), dtype=object)
-    for i in range(len(location)):
-        elements[i] = total_elements[location[i]]
-
-    # Nstep x Natom x 3, positions are all fractional
-    positions = np.empty(shape=(len(indices), len(elements), 3))
-    lattices = np.empty(shape=(Nstep, 3, 3))  # Nstep x 3 x 3
-    mags = []  # Nstep x Natom x ?
-    Atomfixs = []  # Nstep x Natom x 3
-
-    if "Structures" in data:  # relax.json
-        for i, ind in enumerate(indices):  # for every ionic step
-            lat = data["Structures"][ind - 1]["Lattice"]
-            lattices[i] = np.array(lat).reshape(3, 3)
-            mag_for_each_step = []
-            fix_for_each_step = []
-            for j, sli in enumerate(location):
-                ati = data["Structures"][ind - 1]["Atoms"][sli]
-                positions[i, j, :] = ati["Position"][:]
-
-                mag_for_each_atom = ati["Mag"][:]
-                mag_for_each_step.append(mag_for_each_atom)
-
-                fix_for_each_atom = ati["Fix"][:]
-                if fix_for_each_atom == []:
-                    fix_for_each_atom = [0, 0, 0]
-                fix_for_each_atom = [bool(i) for i in fix_for_each_atom]
-                fix_for_each_step.append(fix_for_each_atom)
-
-            mags.append(mag_for_each_step)
-            Atomfixs.append(fix_for_each_step)
-            if not return_scaled:
-                positions = np.dot(positions, lattices[i])
-    else:
-        for i, ind in enumerate(indices):  # for every ionic step
-            lat = data[ind - 1]["Lattice"]
-            lattices[i] = np.array(lat).reshape(3, 3)
-            mag_for_each_step = []
-            fix_for_each_step = []
-            for j, sli in enumerate(location):
-                ati = data[ind - 1]["Atoms"][sli]
-                positions[i, j, :] = ati["Position"][:]
-
-                mag_for_each_atom = ati["Mag"][:]
-                mag_for_each_step.append(mag_for_each_atom)
-
-                fix_for_each_atom = ati["Fix"][:]
-                if fix_for_each_atom == []:
-                    fix_for_each_atom = [0, 0, 0]
-                fix_for_each_atom = [bool(i) for i in fix_for_each_atom]
-                fix_for_each_step.append(fix_for_each_atom)
-
-            mags.append(mag_for_each_step)
-            Atomfixs.append(fix_for_each_step)
-            if not return_scaled:
-                positions = np.dot(positions, lattices[i])
-
-    elements = elements.tolist()
-    Mags = np.array(mags)  # (Nstep, Natom, ?) or (Nstep, 0,)
-
-    D_mag_fix = {"Mags": Mags, "AtomFixs": Atomfixs}
-    print(
-        f"This function does not handle lattice fix info, \n you must manually set it before starting new calculations.."
-    )
+            for i, ind in enumerate(indices):  # for every ionic step
+                lat = data[ind - 1]["Lattice"]
+                lattices[i] = np.array(lat).reshape(3, 3)
+                mag_for_each_step = []
+                fix_for_each_step = []
+                for j, sli in enumerate(location):
+                    ati = data[ind - 1]["Atoms"][sli]
+                    positions[i, j, :] = ati["Position"][:]
+
+                    mag_for_each_atom = ati["Mag"][:]
+                    mag_for_each_step.append(mag_for_each_atom)
+
+                    fix_for_each_atom = ati["Fix"][:]
+                    if fix_for_each_atom == []:
+                        fix_for_each_atom = [0, 0, 0]
+                    fix_for_each_atom = [bool(i) for i in fix_for_each_atom]
+                    fix_for_each_step.append(fix_for_each_atom)
+
+                mags.append(mag_for_each_step)
+                Atomfixs.append(fix_for_each_step)
+                if not return_scaled:
+                    positions = np.dot(positions, lattices[i])
+
+        elements = elements.tolist()
+        Mags = np.array(mags)  # (Nstep, Natom, ?) or (Nstep, 0,)
+
+        D_mag_fix = {"Mags": Mags, "AtomFixs": Atomfixs}
 
-    return Nstep, elements, positions, lattices, D_mag_fix
+        return Nstep, elements, positions, lattices, D_mag_fix
 
 
 def __parse_indices(index: str, total_step) -> list:
     """解析用户输入的原子序号字符串
 
     输入：
         - index: 用户输入的原子序号/元素字符串，例如 '1:3,5,7:10'
@@ -588,119 +970,15 @@
             [zlo_bound, zhi_bound, yz],
         ]
     )
 
     return box_bounds
 
 
-def load_h5(dir_h5: str) -> dict:
-    """遍历读取h5文件中的数据，保存为字典格式
-
-    慎用此函数，因为会读取很多不需要的数据，耗时很长。
-
-    Parameters
-    ----------
-    dir_h5 : str
-        h5文件路径
-
-    Returns
-    -------
-    datas: dict
-        数据字典
-
-    Examples
-    --------
-    >>> from dspawpy.io.read import load_h5
-    >>> datas = load_h5(dir_h5)
-    """
-
-    def get_names(key, h5_object):
-        names.append(h5_object.name)
-
-    def is_dataset(name):
-        for name_inTheList in names:
-            if name_inTheList.find(name + "/") != -1:
-                return False
-        return True
-
-    def get_datas(key, h5_object):
-        if is_dataset(h5_object.name):
-            data = np.asarray(h5_object)
-            if data.dtype == "|S1":  # 转成字符串 并根据";"分割
-                byte2str = [str(bi, "utf-8") for bi in data]
-                string = ""
-                for char in byte2str:
-                    string += char
-                data = np.array([elem for elem in string.strip().split(";")])
-            # "/group1/group2/.../groupN/dataset" : value
-            datas[h5_object.name] = data.tolist()
-
-    with h5py.File(dir_h5, "r") as fin:
-        names = []
-        datas = {}
-        fin.visititems(get_names)
-        fin.visititems(get_datas)
-
-        return datas
-
-
-def load_h5_todict(dir_h5: str) -> dict:
-    """与上一个函数区别在于合并了部分同类数据，例如
-
-    /Structures/Step-1/* 和 /Structures/Step-2/* 并入 /Structures/ 组内
-    """
-
-    def create_dict(L: list, D: dict):
-        if len(L) == 2:
-            D[L[0]] = L[1]
-            return
-        else:
-            if not (L[0] in D.keys()):
-                D[L[0]] = {}
-            create_dict(L[1:], D[L[0]])
-
-    datas = load_h5(dir_h5)
-
-    groups_value_list = []
-    for key in datas.keys():
-        tmp_list = key[1:].strip().split("/")  # [1:] 截去root
-        tmp_list.append(datas[key])
-        # groups_value_list[i]结构: [group1, group2, ..., groupN, dataset, value]
-        groups_value_list.append(tmp_list)
-
-    groups_value_dict = {}
-    for data in groups_value_list:
-        create_dict(data, groups_value_dict)
-
-    return groups_value_dict
-
-
-def get_dos_data(dos_dir: str):
-    if dos_dir.endswith(".h5"):
-        dos = load_h5(dos_dir)
-        if dos["/DosInfo/Project"][0]:
-            return get_complete_dos(dos)
-        else:
-            return get_total_dos(dos)
-
-    elif dos_dir.endswith(".json"):
-        with open(dos_dir, "r") as fin:
-            dos = json.load(fin)
-
-        if dos["DosInfo"]["Project"]:
-            return get_complete_dos_json(dos)
-        else:
-            return get_total_dos_json(dos)
-
-    else:
-        print("file - " + dos_dir + " :  Unsupported format!")
-        return
-
-
-def get_total_dos(dos: dict) -> Dos:
+def _get_total_dos(dos: dict) -> Dos:
     # h5 -> Dos Obj
     energies = np.asarray(dos["/DosInfo/DosEnergy"])
     if dos["/DosInfo/SpinType"][0] == "none":
         densities = {Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"])}
     else:
         densities = {
             Spin.up: np.asarray(dos["/DosInfo/Spin1/Dos"]),
@@ -708,18 +986,32 @@
         }
 
     efermi = dos["/DosInfo/EFermi"][0]
 
     return Dos(efermi, energies, densities)
 
 
-def get_complete_dos(dos: dict) -> CompleteDos:
+def _get_total_dos_json(dos: dict) -> Dos:
+    # json -> Dos Obj
+    energies = np.asarray(dos["DosInfo"]["DosEnergy"])
+    if dos["DosInfo"]["SpinType"] == "none":
+        densities = {Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"])}
+    else:
+        densities = {
+            Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"]),
+            Spin.down: np.asarray(dos["DosInfo"]["Spin2"]["Dos"]),
+        }
+    efermi = dos["DosInfo"]["EFermi"]
+    return Dos(efermi, energies, densities)
+
+
+def _get_complete_dos(dos: dict) -> CompleteDos:
     # h5 -> CompleteDos Obj
-    total_dos = get_total_dos(dos)
-    structure = get_structure(dos, "/AtomInfo")
+    total_dos = _get_total_dos(dos)
+    structure = _get_structure(dos, "/AtomInfo")
     N = len(structure)
     pdos = [{} for i in range(N)]
     number_of_spin = 1 if dos["/DosInfo/SpinType"][0] == "none" else 2
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
@@ -742,32 +1034,18 @@
                     pdos[atom_index][orbit_name] = {spin: Contribution}
 
     pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
 
     return CompleteDos(structure, total_dos, pdoss)
 
 
-def get_total_dos_json(dos: dict) -> Dos:
-    # json -> Dos Obj
-    energies = np.asarray(dos["DosInfo"]["DosEnergy"])
-    if dos["DosInfo"]["SpinType"] == "none":
-        densities = {Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"])}
-    else:
-        densities = {
-            Spin.up: np.asarray(dos["DosInfo"]["Spin1"]["Dos"]),
-            Spin.down: np.asarray(dos["DosInfo"]["Spin2"]["Dos"]),
-        }
-    efermi = dos["DosInfo"]["EFermi"]
-    return Dos(efermi, energies, densities)
-
-
-def get_complete_dos_json(dos: dict) -> CompleteDos:
+def _get_complete_dos_json(dos: dict) -> CompleteDos:
     # json -> CompleteDos Obj
-    total_dos = get_total_dos_json(dos)
-    structure = get_structure_json(dos["AtomInfo"])
+    total_dos = _get_total_dos_json(dos)
+    structure = _get_structure_json(dos["AtomInfo"])
     N = len(structure)
     pdos = [{} for i in range(N)]
     number_of_spin = 1 if dos["DosInfo"]["SpinType"] == "none" else 2
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
@@ -781,49 +1059,60 @@
             else:
                 pdos[atom_index][orbit_name] = {spin: p["Contribution"]}
     pdoss = {structure[i]: pd for i, pd in enumerate(pdos)}
 
     return CompleteDos(structure, total_dos, pdoss)
 
 
-def get_structure(hdf5: dict, key: str) -> Structure:
+def _get_structure(hdf5: dict, key: str) -> Structure:
+    """For single-step task
+    Examples
+    --------
+    >>> from dspawpy.io.read import load_h5, get_structure
+    >>> hdf5Dict = load_h5('rho.h5')
+    >>> structure = get_structure(hdf5Dict, '/AtomInfo')
+    >>> structure
+    """
     # load_h5 -> Structure Obj
     lattice = np.asarray(hdf5[key + "/Lattice"]).reshape(3, 3)
     elements = hdf5[key + "/Elements"]
     positions = hdf5[key + "/Position"]
     coords = np.asarray(positions).reshape(-1, 3)
     is_direct = hdf5[key + "/CoordinateType"][0] == "Direct"
+
+    # replace '_1' or '_2' with '' in elements
+    # elements = [re.sub(r"_\d", "", e) for e in elements]
+
     return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
 
 
-def get_structure_json(atominfo) -> Structure:
+def _get_structure_json(atominfo) -> Structure:
+    """For single-step task
+    Examples
+    --------
+    >>> import json
+    >>> with open('rho.json') as f:
+    >>>     atominfo = json.load(f)['AtomInfo']
+    >>> from dspawpy.io.read import get_structure_json
+    >>> structure = get_structure_json(atominfo)
+    >>> structure
+    """
     lattice = np.asarray(atominfo["Lattice"]).reshape(3, 3)
     elements = []
     positions = []
     for atom in atominfo["Atoms"]:
         elements.append(atom["Element"])
         positions.extend(atom["Position"])
 
     coords = np.asarray(positions).reshape(-1, 3)
     is_direct = atominfo["CoordinateType"] == "Direct"
     return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
 
 
-def get_structure_from_json(jsonfile: str) -> Structure:
-    with open(jsonfile, "r") as file:
-        j = json.load(file)
-    lattice = np.asarray(j["AtomInfo"]["Lattice"]).reshape(3, 3)
-    elements = j["AtomInfo"]["Elements"]
-    positions = j["AtomInfo"]["Position"]
-    coords = np.asarray(positions).reshape(-1, 3)
-    is_direct = j["AtomInfo"]["CoordinateType"][0] == "Direct"
-    return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
-
-
-def get_band_data_h5(band: dict, iwan=False):
+def _get_band_data_h5(band: dict, iwan=False):
     if iwan:
         bd = "WannBandInfo"
     else:
         bd = "BandInfo"
     number_of_band = band[f"/{bd}/NumberOfBand"][0]
     number_of_kpoints = band[f"/{bd}/NumberOfKpoints"][0]
     if (
@@ -852,15 +1141,15 @@
         band_data = np.array(data).reshape((number_of_kpoints, number_of_band)).T
         eigenvals[spin] = band_data
 
     kpoints = np.asarray(band[f"/{bd}/CoordinatesOfKPoints"]).reshape(
         number_of_kpoints, 3
     )
 
-    structure = get_structure(band, "/AtomInfo")
+    structure = _get_structure(band, "/AtomInfo")
     labels_dict = {}
 
     for i, s in enumerate(band[f"/{bd}/SymmetryKPoints"]):
         labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
 
     # read projection data
     projections = None
@@ -894,15 +1183,15 @@
                             .T
                         )
                 projections[spin] = projection
 
     return structure, kpoints, eigenvals, efermi, labels_dict, projections
 
 
-def get_band_data_json(band: dict, iwan=False):
+def _get_band_data_json(band: dict, iwan=False):
     if iwan:
         bd = "WannBandInfo"
     else:
         bd = "BandInfo"
 
     number_of_band = band[f"{bd}"]["NumberOfBand"]
     number_of_kpoints = band[f"{bd}"]["NumberOfKpoints"]
@@ -935,15 +1224,15 @@
 
         eigenvals[spin] = band_data
 
     kpoints = np.asarray(band[f"{bd}"]["CoordinatesOfKPoints"]).reshape(
         number_of_kpoints, 3
     )
 
-    structure = get_structure_json(band["AtomInfo"])
+    structure = _get_structure_json(band["AtomInfo"])
     labels_dict = {}
 
     for i, s in enumerate(band[f"{bd}"]["SymmetryKPoints"]):
         labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
 
     # read projection data
     projections = None
@@ -971,84 +1260,15 @@
                     )
 
                 projections[spin] = projection
 
     return structure, kpoints, eigenvals, efermi, labels_dict, projections
 
 
-def get_band_data(band_dir: str, efermi: float = None) -> BandStructureSymmLine:
-    # modify BandStructureSymmLine.efermi after it was created will cause error
-    if band_dir.endswith(".h5"):
-        band = load_h5(band_dir)
-        raw = h5py.File(band_dir, "r").keys()
-        if "/WannBandInfo/NumberOfBand" in raw:
-            (
-                structure,
-                kpoints,
-                eigenvals,
-                rEf,
-                labels_dict,
-                projections,
-            ) = get_band_data_h5(band, iwan=True)
-        elif "/BandInfo/NumberOfBand" in raw:
-            (
-                structure,
-                kpoints,
-                eigenvals,
-                rEf,
-                labels_dict,
-                projections,
-            ) = get_band_data_h5(band, iwan=False)
-        else:
-            print("BandInfo or WannBandInfo key not found in h5file!")
-            return
-    elif band_dir.endswith(".json"):
-        with open(band_dir, "r") as fin:
-            band = json.load(fin)
-        if "WannBandInfo" in band.keys():
-            (
-                structure,
-                kpoints,
-                eigenvals,
-                rEf,
-                labels_dict,
-                projections,
-            ) = get_band_data_json(band, iwan=True)
-        elif "BandInfo" in band.keys():
-            (
-                structure,
-                kpoints,
-                eigenvals,
-                rEf,
-                labels_dict,
-                projections,
-            ) = get_band_data_json(band, iwan=False)
-        else:
-            print("BandInfo or WannBandInfo key not found in json file!")
-            return
-    else:
-        print("file - " + band_dir + " :  Unsupported format!")
-        return
-
-    if efermi:  # 从h5直接读取的费米能级可能是错的，此时需要用户自行指定
-        rEf = efermi  # 这只是个临时解决方案
-
-    lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
-    return BandStructureSymmLine(
-        kpoints=kpoints,
-        eigenvals=eigenvals,
-        lattice=lattice_new,
-        efermi=rEf,
-        labels_dict=labels_dict,
-        structure=structure,
-        projections=projections,
-    )
-
-
-def get_phonon_band_data_h5(band: dict):
+def _get_phonon_band_data_h5(band: dict):
     number_of_band = band["/BandInfo/NumberOfBand"][0]
     number_of_kpoints = band["/BandInfo/NumberOfQPoints"][0]
     number_of_spin = 1
     symmmetry_kpoints = band["/BandInfo/SymmetryQPoints"]
     symmetry_kPoints_index = band["/BandInfo/SymmetryQPointsIndex"]
     eigenvals = {}
     for i in range(number_of_spin):
@@ -1063,21 +1283,21 @@
             return
         frequencies = np.array(data).reshape((number_of_kpoints, number_of_band)).T
         eigenvals[spin] = frequencies
     kpoints = np.asarray(band["/BandInfo/CoordinatesOfQPoints"]).reshape(
         number_of_kpoints, 3
     )
     if "/SupercellAtomInfo/CoordinateType" in band.keys():
-        structure = get_structure(band, "/SupercellAtomInfo")
+        structure = _get_structure(band, "/SupercellAtomInfo")
     else:
-        structure = get_structure(band, "/AtomInfo")
+        structure = _get_structure(band, "/AtomInfo")
     return symmmetry_kpoints, symmetry_kPoints_index, kpoints, structure, frequencies
 
 
-def get_phonon_band_data_json(band: dict):
+def _get_phonon_band_data_json(band: dict):
     number_of_band = band["BandInfo"]["NumberOfBand"]
     number_of_kpoints = band["BandInfo"]["NumberOfQPoints"]
     number_of_spin = 1
     symmmetry_kpoints = band["BandInfo"]["SymmetryQPoints"]
     symmetry_kPoints_index = band["BandInfo"]["SymmetryQPointsIndex"]
 
     eigenvals = {}
@@ -1095,68 +1315,12 @@
         eigenvals[spin] = frequencies
 
     kpoints = np.asarray(band["BandInfo"]["CoordinatesOfQPoints"]).reshape(
         number_of_kpoints, 3
     )
 
     if "SupercellAtomInfo" in band.keys():
-        structure = get_structure_json(band["SupercellAtomInfo"])
+        structure = _get_structure_json(band["SupercellAtomInfo"])
     else:
-        structure = get_structure_json(band["AtomInfo"])
+        structure = _get_structure_json(band["AtomInfo"])
 
     return symmmetry_kpoints, symmetry_kPoints_index, kpoints, structure, frequencies
-
-
-def get_phonon_band_data(phonon_band_dir: str) -> PhononBandStructureSymmLine:
-    if phonon_band_dir.endswith(".h5"):
-        band = load_h5(phonon_band_dir)
-        (
-            symmmetry_kpoints,
-            symmetry_kPoints_index,
-            kpoints,
-            structure,
-            frequencies,
-        ) = get_phonon_band_data_h5(band)
-    elif phonon_band_dir.endswith(".json"):
-        with open(phonon_band_dir, "r") as fin:
-            band = json.load(fin)
-        (
-            symmmetry_kpoints,
-            symmetry_kPoints_index,
-            kpoints,
-            structure,
-            frequencies,
-        ) = get_phonon_band_data_json(band)
-    else:
-        print("file - " + phonon_band_dir + " :  Unsupported format!")
-        return
-
-    labels_dict = {}
-    for i, s in enumerate(symmmetry_kpoints):
-        labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
-    lattice_new = Lattice(structure.lattice.reciprocal_lattice.matrix)
-
-    return PhononBandStructureSymmLine(
-        qpoints=kpoints,
-        frequencies=frequencies,
-        lattice=lattice_new,
-        has_nac=False,
-        labels_dict=labels_dict,
-        structure=structure,
-    )
-
-
-def get_phonon_dos_data(phonon_dos_dir: str) -> PhononDos:
-    if phonon_dos_dir.endswith(".h5"):
-        dos = load_h5(phonon_dos_dir)
-        frequencies = np.asarray(dos["/DosInfo/DosEnergy"])
-        densities = dos["/DosInfo/Spin1/Dos"]
-    elif phonon_dos_dir.endswith(".json"):
-        with open(phonon_dos_dir, "r") as fin:
-            dos = json.load(fin)
-        frequencies = np.asarray(dos["DosInfo"]["DosEnergy"])
-        densities = dos["DosInfo"]["Spin1"]["Dos"]
-    else:
-        print("file - " + phonon_dos_dir + " :  Unsupported format!")
-        return
-
-    return PhononDos(frequencies, densities)
```

## dspawpy/io/structure.py

```diff
@@ -1,20 +1,17 @@
 """
-Functions to build structures,
+Functions to build structures
 """
 
-import json
-from typing import Dict, List, Union
+from typing import List, Union
 
-import h5py
 import numpy as np
 from pymatgen.core import Structure
 
-from dspawpy.io.read import (_sinfo_from_h5, get_lines_without_comment,
-                             get_sinfo)
+from dspawpy.io.read import get_lines_without_comment, get_sinfo
 
 
 def build_Structures_from_datafile(datafile: Union[str, List[str]]) -> List[Structure]:
     """读取一/多个h5/json文件，返回pymatgen的Structures列表
 
     Parameters
     ----------
@@ -35,24 +32,27 @@
     # 当datafile为列表时，将依次读取多个文件，合并成一个Structures列表
     >>> pymatgen_Structures = build_Structures_from_datafile(datafile=['aimd1.h5','aimd2.h5'])
     """
     dfs = []
     if isinstance(datafile, list):  # 续算模式，给的是多个文件
         dfs = datafile
     else:  # 单次计算模式，处理单个文件
-        if datafile.endswith(".h5") or datafile.endswith(".json"):
+        if (
+            datafile.endswith(".h5")
+            or datafile.endswith(".json")
+            or datafile.endswith(".as")
+        ):
             df = datafile
         else:
             raise FileNotFoundError("未找到h5或json文件！")
         dfs.append(df)
 
     # 读取结构数据
     pymatgen_Structures = []
     for df in dfs:
-        # TODO 支持选取特定帧
         structure_list = _get_structure_list(df)
         pymatgen_Structures.extend(structure_list)
 
     return pymatgen_Structures
 
 
 def _get_structure_list(df: str = "aimd.h5") -> List[Structure]:
@@ -73,31 +73,40 @@
     >>> structure_list = get_structure_list(df='aimd.h5')
     """
 
     # create Structure structure_list from aimd.h5
     Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(df)
     strs = []
     for i in range(Nstep):
-        strs.append(
-            Structure(
-                lattices[i],
-                elements,
-                positions[i],
-                coords_are_cartesian=False,
-                site_properties={
-                    "Mags": D_mag_fix["Mags"][i],
-                    "AtomFixs": D_mag_fix["AtomFixs"][i],
-                },
+        if D_mag_fix:
+            strs.append(
+                Structure(
+                    lattices[i],
+                    elements,
+                    positions[i],
+                    coords_are_cartesian=False,
+                    site_properties={
+                        "Mags": D_mag_fix["Mags"][i],
+                        "AtomFixs": D_mag_fix["AtomFixs"][i],
+                    },
+                )
+            )
+        else:
+            strs.append(
+                Structure(
+                    lattices[i],
+                    elements,
+                    positions[i],
+                    coords_are_cartesian=False,
+                )
             )
-        )
-
     return strs
 
 
-def from_dspaw_as(as_file: str = "structure.as") -> Structure:
+def _from_dspaw_as(as_file: str = "structure.as") -> Structure:
     """从DSPAW的as结构文件中读取结构信息
 
     Parameters
     ----------
     as_file : str
         DSPAW的as结构文件, 默认'structure.as'
 
@@ -150,15 +159,15 @@
             elements,
             coords,
             coords_are_cartesian=(not is_direct),
             site_properties=D,
         )
 
 
-def from_hzw(hzw_file) -> Structure:
+def _from_hzw(hzw_file) -> Structure:
     """从hzw结构文件中读取结构信息
 
     Parameters
     ----------
     hzw_file : str
         hzw结构文件，以 .hzw 结尾
 
@@ -188,201 +197,7 @@
     for i in range(N):
         atom = lines[i + 5].strip().split()
         elements.append(atom[0])
         positions.extend([float(atom[1]), float(atom[2]), float(atom[3])])
 
     coords = np.asarray(positions).reshape(-1, 3)
     return Structure(lattice, elements, coords, coords_are_cartesian=True)
-
-
-def to_file(structure: Structure, filename: str, fmt, coords_are_cartesian=True):
-    """往结构文件中写入信息
-
-    Parameters
-    ----------
-    structure : Structure
-        pymatgen的Structure对象
-    filename : str
-        结构文件名
-    fmt : str
-        结构文件类型，支持 "json","as","hzw"
-    coords_are_cartesian : bool
-        坐标是否为笛卡尔坐标，默认为True
-
-    Examples
-    --------
-    >>> from dspawpy.io.structure import to_file
-    >>> to_file(structure, filename='Si.json', fmt='json')
-    >>> to_file(structure, filename='Si.as', fmt='as')
-    >>> to_file(structure, filename='Si.hzw', fmt='hzw')
-    """
-    if fmt == "json":
-        to_dspaw_json(structure, filename, coords_are_cartesian)
-    elif fmt == "as":
-        to_dspaw_as(structure, filename, coords_are_cartesian)
-    elif fmt == "hzw":
-        to_hzw(structure, filename)
-
-
-def from_dspaw_atominfo(hpath, index: int = None) -> Structure:
-    if not isinstance(hpath, str):  # for compatibility with aimd2pdb.py
-        atominfo = hpath
-        lattice = np.asarray(atominfo["Lattice"]).reshape(3, 3)
-        elements = []
-        positions = []
-        for atom in atominfo["Atoms"]:
-            elements.append(atom["Element"])
-            positions.extend(atom["Position"])
-
-        coords = np.asarray(positions).reshape(-1, 3)
-        is_direct = atominfo["CoordinateType"] == "Direct"
-        return Structure(
-            lattice, elements, coords, coords_are_cartesian=(not is_direct)
-        )
-    Nstep, elements, positions, lattices = _sinfo_from_h5(hpath, index)
-    return Structure(lattices[0], elements, positions[0], coords_are_cartesian=True)
-
-
-def from_dspaw_atominfo_json(atominfo: dict) -> Structure:
-    lattice = np.asarray(atominfo["Lattice"]).reshape(3, 3)
-    elements = []
-    positions = []
-    for atom in atominfo["Atoms"]:
-        elements.append(atom["Element"])
-        positions.extend(atom["Position"])
-
-    coords = np.asarray(positions).reshape(-1, 3)
-    is_direct = atominfo["CoordinateType"] == "Direct"
-    return Structure(lattice, elements, coords, coords_are_cartesian=(not is_direct))
-
-
-def from_dspaw_atominfos(aimd_dir: str) -> List[Structure]:
-    structures = []
-    if isinstance(aimd_dir, list) or isinstance(aimd_dir, np.ndarray):
-        for atominfo in aimd_dir:
-            structures.append(from_dspaw_atominfo(atominfo))
-    elif aimd_dir.endswith(".h5"):
-        aimd = h5py.File(aimd_dir)
-        steps = int(np.array(aimd.get("/Structures/FinalStep"))[0])
-        for i in range(steps):
-            structures.append(from_dspaw_atominfo(aimd_dir, i + 1))
-    elif aimd_dir.endswith(".json"):
-        with open(aimd_dir, "r") as fin:
-            aimd = json.load(fin)
-        for atominfo in aimd["Structures"]:
-            structures.append(from_dspaw_atominfo_json(atominfo))
-    else:
-        print("file - " + aimd_dir + " :  Unsupported format!")
-        return
-
-    return structures
-
-
-def to_dspaw_as(structure: Structure, filename: str, coords_are_cartesian=True):
-    """write dspaw as file
-    If converted from as file, will copy the mag and fix info,
-        otherwise, those info will be ignored!
-    """
-    with open(filename, "w", encoding="utf-8") as file:
-        file.write("Total number of atoms\n")
-        file.write("%d\n" % len(structure))
-
-        file.write("Lattice\n")
-        for v in structure.lattice.matrix:
-            file.write("%.6f %.6f %.6f\n" % (v[0], v[1], v[2]))
-
-        i = 0
-        for site in structure:
-            if i == 0:
-                if "line6s" in site.properties:
-                    file.write("%s\n" % site.properties["line6s"])
-                else:
-                    if coords_are_cartesian:
-                        file.write("Cartesian\n")
-                    else:
-                        file.write("Direct\n")
-            i += 1
-
-            coords = site.coords if coords_are_cartesian else site.frac_coords
-            if "others" in site.properties:
-                sp = " ".join(site.properties["others"])  # flatten str list
-                file.write(
-                    "%s %.6f %.6f %.6f %s\n"
-                    % (site.species_string, coords[0], coords[1], coords[2], sp)
-                )
-            else:  # the most common case
-                file.write(
-                    "%s %.6f %.6f %.6f\n"
-                    % (site.species_string, coords[0], coords[1], coords[2])
-                )
-
-
-def to_hzw(structure: Structure, filename: str):
-    with open(filename, "w", encoding="utf-8") as file:
-        file.write("% The number of probes \n")
-        file.write("0\n")
-        file.write("% Uni-cell vector\n")
-
-        for v in structure.lattice.matrix:
-            file.write("%.6f %.6f %.6f\n" % (v[0], v[1], v[2]))
-
-        file.write("% Total number of device_structure\n")
-        file.write("%d\n" % len(structure))
-        file.write("% Atom site\n")
-
-        for site in structure:
-            file.write(
-                "%s %.6f %.6f %.6f\n"
-                % (site.species_string, site.coords[0], site.coords[1], site.coords[2])
-            )
-
-
-def to_dspaw_dict(structure: Structure, coords_are_cartesian=True) -> Dict:
-    lattice = structure.lattice.matrix.flatten().tolist()
-    atoms = []
-    for site in structure:
-        coords = site.coords if coords_are_cartesian else site.frac_coords
-        atoms.append({"Element": site.species_string, "Position": coords.tolist()})
-
-    coordinate_type = "Cartesian" if coords_are_cartesian else "Direct"
-    return {"Lattice": lattice, "CoordinateType": coordinate_type, "Atoms": atoms}
-
-
-def to_dspaw_json(structure: Structure, filename: str, coords_are_cartesian=True):
-    d = to_dspaw_dict(structure, coords_are_cartesian)
-    with open(filename, "w", encoding="utf-8") as file:
-        json.dump(d, file, indent=4)
-
-
-def to_pdb(structures: List[Structure], pdb_filename: str):
-    with open(pdb_filename, "w", encoding="utf-8") as file:
-        for i, s in enumerate(structures):
-            file.write("MODEL         %d\n" % (i + 1))
-            file.write("REMARK   Converted from Structures\n")
-            file.write("REMARK   Converted using dspawpy\n")
-            lengths = s.lattice.lengths
-            angles = s.lattice.angles
-            file.write(
-                "CRYST1{0:9.3f}{1:9.3f}{2:9.3f}{3:7.2f}{4:7.2f}{5:7.2f}\n".format(
-                    lengths[0], lengths[1], lengths[2], angles[0], angles[1], angles[2]
-                )
-            )
-            for j, site in enumerate(s):
-                file.write(
-                    "%4s%7d%4s%5s%6d%4s%8.3f%8.3f%8.3f%6.2f%6.2f%12s\n"
-                    % (
-                        "ATOM",
-                        j + 1,
-                        site.species_string,
-                        "MOL",
-                        1,
-                        "    ",
-                        site.coords[0],
-                        site.coords[1],
-                        site.coords[2],
-                        1.0,
-                        0.0,
-                        site.species_string,
-                    )
-                )
-            file.write("TER\n")
-            file.write("ENDMDL\n")
```

## dspawpy/io/utils.py

```diff
@@ -269,24 +269,14 @@
 ]
 
 atomic_numbers = {}
 for Z, symbol in enumerate(chemical_symbols):
     atomic_numbers[symbol] = Z
 
 
-def symbols2numbers(symbols) -> List[int]:
-    numbers = []
-    for s in symbols:
-        if isinstance(s, str):
-            numbers.append(atomic_numbers[s])
-        else:
-            numbers.append(int(s))
-    return numbers
-
-
 def eles2masses(eles: List[str]) -> List[float]:
     """将元素列表转换为质量列表
 
     Parameters
     ----------
     eles : List[str]
         元素列表
@@ -338,15 +328,15 @@
 
     I = np.array([[I11, I12, I13], [I12, I22, I23], [I13, I23, I33]])
 
     evals, evecs = np.linalg.eigh(I)
     return evals
 
 
-class IdealGasThermo:  # TODO remove atoms obj
+class IdealGasThermo:
     """import from ase.thermochemistry.IdealGasThermo
 
     Parameters
     ----------
     vib_energies : list
         List of vibrational energies in eV.
     geometry : str
@@ -891,7 +881,17 @@
     0.18362317157111566
     """
 
     ZPE = getZPE(fretxt=fretxt)
     sum_S = getTSads(fretxt=fretxt, T=T)
 
     return ZPE, sum_S
+
+
+def _symbols2numbers(symbols) -> List[int]:
+    numbers = []
+    for s in symbols:
+        if isinstance(s, str):
+            numbers.append(atomic_numbers[s])
+        else:
+            numbers.append(int(s))
+    return numbers
```

## dspawpy/io/write.py

```diff
@@ -13,172 +13,226 @@
 
 def write_xyz_traj(
     datafile="aimd.h5",
     ai=None,
     ele=None,
     index=None,
     xyzfile="aimdTraj.xyz",
+    icombine=False,
 ):
     """保存xyz格式的轨迹文件
 
     Parameters
     ----------
     datafile : str or list
         DSPAW计算完成后保存的h5/json文件或包含它们的文件夹路径
     ai : int
         原子编号列表（体系中的第几号原子，不是质子数）
     ele : str
         元素，例如 'C'，'H'，'O'，'N'
     index : int
         优化过程中的第几步
-
-    Returns
-    -------
-    xyzfile: str
+    xyzfile : str
         写入xyz格式的轨迹文件，默认为aimdTraj.xyz
+    icombine : bool
+        是否将多个文件合并为一个文件，默认为False
 
     Example
     -------
-    >>> from dspawpy.analysis.aimdtools import write_xyz_traj
+    >>> from dspawpy.analysis.write import write_xyz_traj
     >>> write_xyz_traj(datafile='aimd.h5', ai=[1,2,3], index=1, xyzfile='aimdTraj.xyz')
     """
     if isinstance(datafile, list):
-        for i, df in enumerate(datafile):
-            write_xyz_traj(df, ai, ele, index, str(i + 1) + xyzfile)
-        return f"{xyzfile} 文件已保存！"
-    # search datafile in the given directory
-    elif os.path.isdir(datafile):
-        directory = datafile  # specified datafile is actually a directory
-        print("您指定了一个文件夹，正在查找相关h5或json文件...")
-        if os.path.exists(os.path.join(directory, "aimd.h5")):
-            datafile = os.path.join(directory, "aimd.h5")
-            print("Reading aimd.h5...")
-        elif os.path.exists(os.path.join(directory, "aimd.json")):
-            datafile = os.path.join(directory, "aimd.json")
-            print("Reading aimd.json...")
-        else:
-            raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
-    if datafile.endswith(".h5"):
-        Nstep, eles, poses, lats, line6s = _sinfo_from_h5(datafile, index, ele, ai)
-    elif datafile.endswith(".json"):
-        Nstep, eles, poses, lats, line6s = _sinfo_from_json(datafile, index, ele, ai)
+        dfs = datafile
+    elif isinstance(datafile, str):
+        dfs = [datafile]
     else:
-        raise TypeError("仅支持读取h5或json文件！")
+        raise TypeError("datafile must be a str or a list of str!")
 
-    # 写入文件
-    with open(xyzfile, "w") as f:
-        # Nstep
-        for n in range(Nstep):
-            # 原子数不会变，就是不合并的元素总数
-            f.write("%d\n" % len(eles))
-            # lattice
-            f.write(
-                'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
-                % (
-                    lats[n, 0, 0],
-                    lats[n, 0, 1],
-                    lats[n, 0, 2],
-                    lats[n, 1, 0],
-                    lats[n, 1, 1],
-                    lats[n, 1, 2],
-                    lats[n, 2, 0],
-                    lats[n, 2, 1],
-                    lats[n, 2, 2],
-                )
+    xyzs = []
+    for i, df in enumerate(dfs):
+        if len(dfs) == 1:
+            xyzfilename = xyzfile
+        else:
+            xyzfilename = str(i + 1) + xyzfile
+        xyzs.append(xyzfilename)
+
+        # search df in the given directory
+        if os.path.isdir(df):
+            directory = df  # specified df is actually a directory
+            print("您指定了一个文件夹，正在查找相关h5或json文件...")
+            if os.path.exists(os.path.join(directory, "aimd.h5")):
+                df = os.path.join(directory, "aimd.h5")
+                print("Reading aimd.h5...")
+            elif os.path.exists(os.path.join(directory, "aimd.json")):
+                df = os.path.join(directory, "aimd.json")
+                print("Reading aimd.json...")
+            else:
+                raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
+
+        if df.endswith(".h5"):
+            Nstep, eles, poses, lats, D_mag_fix = _sinfo_from_h5(
+                df, index, ele, ai, return_scaled=True
             )
-            # position and element
-            for i in range(len(eles)):
+        elif df.endswith(".json"):
+            Nstep, eles, poses, lats, D_mag_fix = _sinfo_from_json(df, index, ele, ai)
+        else:
+            raise TypeError("仅支持读取h5或json文件！")
+
+        # 写入文件
+        with open(xyzfilename, "w") as f:
+            # Nstep
+            for n in range(Nstep):
+                # 原子数不会变，就是不合并的元素总数
+                f.write("%d\n" % len(eles))
+                # lattice
                 f.write(
-                    "%s %f %f %f\n"
-                    % (eles[i], poses[n, i, 0], poses[n, i, 1], poses[n, i, 2])
+                    'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
+                    % (
+                        lats[n, 0, 0],
+                        lats[n, 0, 1],
+                        lats[n, 0, 2],
+                        lats[n, 1, 0],
+                        lats[n, 1, 1],
+                        lats[n, 1, 2],
+                        lats[n, 2, 0],
+                        lats[n, 2, 1],
+                        lats[n, 2, 2],
+                    )
                 )
-    print(f"{xyzfile} 文件已保存！")
+                # position and element
+                for j in range(len(eles)):
+                    f.write(
+                        "%s %f %f %f\n"
+                        % (eles[j], poses[n, j, 0], poses[n, j, 1], poses[n, j, 2])
+                    )
+        print(f"{xyzfilename} 文件已保存！")
+
+    if icombine and isinstance(datafile, list):
+        # combine xyz by calling python internal utility
+        lines = []
+        for xyzFile in xyzs:
+            with open(xyzFile, "r") as f:
+                lines.extend(f.readlines())
+        with open(f"total_{xyzFile}", "w") as f:
+            f.writelines(lines)
+
+        print(f"total_{xyzfile} 文件已保存！")
 
 
 def write_dump_traj(
     datafile="aimd.h5",
     ai=None,
     ele=None,
     index=None,
     dumpfile="aimdTraj.dump",
+    icombine=False,
 ):
     """保存为lammps的dump格式的轨迹文件，暂时只支持正交晶胞
 
     Parameters
     ----------
     datafile : str or list
         DSPAW计算完成后保存的h5/json文件或包含它们的文件夹路径
     ai : int
         原子编号列表（体系中的第几号原子，不是质子数）
     ele : str
         元素，例如 'C'，'H'，'O'，'N'
     index : int
         优化过程中的第几步
-
-    Returns
-    -------
-    dumpfile: str
-        写入dump格式的轨迹文件，默认为aimdTraj.dump
+    dumpfile : str
+        dump格式的轨迹文件名，默认为aimdTraj.dump
+    icombine : bool
+        是否将多个文件合并为一个文件，默认为False
 
     Example
     -------
-    >>> from dspawpy.analysis.aimdtools import write_dump_traj
+    >>> from dspawpy.analysis.write import write_dump_traj
     >>> write_dump_traj(datafile='aimd.h5', ai=[1,2,3], index=1, dumpfile='aimdTraj.dump')
     """
     if isinstance(datafile, list):
-        for i, df in enumerate(datafile):
-            write_dump_traj(df, ai, ele, index, str(i + 1) + dumpfile)
-        return f"{dumpfile} 文件已保存！"
-    # search datafile in the given directory
-    elif os.path.isdir(datafile):
-        directory = datafile  # specified datafile is actually a directory
-        print("您指定了一个文件夹，正在查找相关h5或json文件...")
-        if os.path.exists(os.path.join(directory, "aimd.h5")):
-            datafile = os.path.join(directory, "aimd.h5")
-            print("Reading aimd.h5...")
-        elif os.path.exists(os.path.join(directory, "aimd.json")):
-            datafile = os.path.join(directory, "aimd.json")
-            print("Reading aimd.json...")
-        else:
-            raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
-    if datafile.endswith(".h5"):
-        Nstep, eles, poses, lats, line6s = _sinfo_from_h5(datafile, index, ele, ai)
-    elif datafile.endswith(".json"):
-        Nstep, eles, poses, lats, line6s = _sinfo_from_json(datafile, index, ele, ai)
+        dfs = datafile
+    elif isinstance(datafile, str):
+        dfs = [datafile]
     else:
-        raise TypeError("仅支持读取h5或json文件！")
+        raise TypeError("datafile must be a str or a list of str!")
 
-    # 写入文件
-    with open(dumpfile, "w") as f:
-        for n in range(Nstep):
-            box_bounds = _get_lammps_non_orthogonal_box(lats[n])
-            f.write("ITEM: TIMESTEP\n%d\n" % n)
-            f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(eles)))
-            f.write("ITEM: BOX BOUNDS xy xz yz xx yy zz\n")
-            f.write(
-                "%f %f %f\n%f %f %f\n %f %f %f\n"
-                % (
-                    box_bounds[0][0],
-                    box_bounds[0][1],
-                    box_bounds[0][2],
-                    box_bounds[1][0],
-                    box_bounds[1][1],
-                    box_bounds[1][2],
-                    box_bounds[2][0],
-                    box_bounds[2][1],
-                    box_bounds[2][2],
-                )
-            )
-            f.write("ITEM: ATOMS type x y z id\n")
-            for i in range(len(eles)):
+    dumps = []
+    for i, df in enumerate(dfs):
+        if len(dfs) == 1:
+            dumpfilename = dumpfile
+        else:
+            dumpfilename = str(i + 1) + dumpfile
+        dumps.append(dumpfilename)
+
+        # search df in the given directory
+        if os.path.isdir(df):
+            directory = df  # specified df is actually a directory
+            print("您指定了一个文件夹，正在查找相关h5或json文件...")
+            if os.path.exists(os.path.join(directory, "aimd.h5")):
+                df = os.path.join(directory, "aimd.h5")
+                print("Reading aimd.h5...")
+            elif os.path.exists(os.path.join(directory, "aimd.json")):
+                df = os.path.join(directory, "aimd.json")
+                print("Reading aimd.json...")
+            else:
+                raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
+
+        if df.endswith(".h5"):
+            Nstep, eles, poses, lats, D_mag_fix = _sinfo_from_h5(df, index, ele, ai)
+        elif df.endswith(".json"):
+            Nstep, eles, poses, lats, D_mag_fix = _sinfo_from_json(df, index, ele, ai)
+        else:
+            raise TypeError("仅支持读取h5或json文件！")
+
+        # 写入文件
+        with open(dumpfilename, "w") as f:
+            for n in range(Nstep):
+                box_bounds = _get_lammps_non_orthogonal_box(lats[n])
+                f.write("ITEM: TIMESTEP\n%d\n" % n)
+                f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(eles)))
+                f.write("ITEM: BOX BOUNDS xy xz yz xx yy zz\n")
                 f.write(
-                    "%s %f %f %f %d\n"
-                    % (eles[i], poses[n, i, 0], poses[n, i, 1], poses[n, i, 2], i + 1)
+                    "%f %f %f\n%f %f %f\n %f %f %f\n"
+                    % (
+                        box_bounds[0][0],
+                        box_bounds[0][1],
+                        box_bounds[0][2],
+                        box_bounds[1][0],
+                        box_bounds[1][1],
+                        box_bounds[1][2],
+                        box_bounds[2][0],
+                        box_bounds[2][1],
+                        box_bounds[2][2],
+                    )
                 )
-    print(f"{dumpfile} 文件已保存！")
+                f.write("ITEM: ATOMS type x y z id\n")
+                for i in range(len(eles)):
+                    f.write(
+                        "%s %f %f %f %d\n"
+                        % (
+                            eles[i],
+                            poses[n, i, 0],
+                            poses[n, i, 1],
+                            poses[n, i, 2],
+                            i + 1,
+                        )
+                    )
+        print(f"{dumpfilename} 文件已保存！")
+
+    if icombine and isinstance(datafile, list):
+        # combine xyz by calling python internal utility
+        lines = []
+        for dumpFile in dumps:
+            with open(dumpFile, "r") as f:
+                lines.extend(f.readlines())
+        with open(f"total_{dumpfile}", "w") as f:
+            f.writelines(lines)
+
+        print(f"total_{dumpfile} 文件已保存！")
 
 
 def write_VESTA(in_filename: str, data_type, out_filename="DS-PAW.vesta"):
     """从包含电子体系信息的json或h5文件中读取数据并写入VESTA格式的文件中
 
     Parameters
     ----------
@@ -198,51 +252,51 @@
     --------
     >>> from dspawpy.io.write import write_VESTA
     >>> write_VESTA("DS-PAW.json", "rho")
     """
     if in_filename.endswith(".h5"):
         data = load_h5(in_filename)
         if data_type.lower() == "rho" or data_type.lower() == "boundcharge":
-            write_VESTA_format(data, ["/Rho/TotalCharge"], out_filename)
+            _write_VESTA_format(data, ["/Rho/TotalCharge"], out_filename)
         elif data_type.lower() == "potential":
-            write_VESTA_format(
+            _write_VESTA_format(
                 data,
                 [
                     "/Potential/TotalElectrostaticPotential",
                 ],
                 out_filename,
             )
         elif data_type.lower() == "elf":
-            write_VESTA_format(data, ["/ELF/TotalELF"], out_filename)
+            _write_VESTA_format(data, ["/ELF/TotalELF"], out_filename)
         elif data_type.lower() == "pcharge":
-            write_VESTA_format(data, ["/Pcharge/1/TotalCharge"], out_filename)
+            _write_VESTA_format(data, ["/Pcharge/1/TotalCharge"], out_filename)
         else:
             raise NotImplementedError("仅支持rho/potential/elf/pcharge/boundcharge")
 
     elif in_filename.endswith(".json"):
         with open(in_filename, "r") as fin:
             data = json.load(fin)
         if data_type.lower() == "rho" or data_type.lower() == "boundcharge":
-            write_VESTA_format_json(
+            _write_VESTA_format_json(
                 data["AtomInfo"], [data["Rho"]["TotalCharge"]], out_filename
             )
         elif data_type.lower() == "potential":
-            write_VESTA_format_json(
+            _write_VESTA_format_json(
                 data["AtomInfo"],
                 [
                     data["Potential"]["TotalElectrostaticPotential"],
                 ],
                 out_filename,
             )
         elif data_type.lower() == "elf":
-            write_VESTA_format_json(
+            _write_VESTA_format_json(
                 data["AtomInfo"], [data["ELF"]["TotalELF"]], out_filename
             )
         elif data_type.lower() == "pcharge":
-            write_VESTA_format_json(
+            _write_VESTA_format_json(
                 data["AtomInfo"], [data["Pcharge"][0]["TotalCharge"]], out_filename
             )
         else:
             raise NotImplementedError("仅支持rho/potential/elf/pcharge/boundcharge")
 
     else:
         raise NotImplementedError("仅支持json或h5格式文件")
@@ -371,15 +425,46 @@
                     ind = ind + 1
                     if ind % 5 == 0:
                         out.write("\n")
 
     print(f"成功写入 {output}")
 
 
-def write_atoms(fileobj, hdf5):
+def to_file(structure, filename: str, fmt, coords_are_cartesian=True):
+    """往结构文件中写入信息
+
+    Parameters
+    ----------
+    structure : Structure
+        pymatgen的Structure对象
+    filename : str
+        结构文件名
+    fmt : str
+        结构文件类型，支持 "json","as","hzw"
+    coords_are_cartesian : bool
+        坐标是否为笛卡尔坐标，默认为True
+
+    Examples
+    --------
+    >>> from dspawpy.io.write import to_file
+    >>> to_file(structure, filename='Si.json', fmt='json')
+    >>> to_file(structure, filename='Si.as', fmt='as')
+    >>> to_file(structure, filename='Si.hzw', fmt='hzw')
+    """
+    if fmt == "json":
+        _to_dspaw_json(structure, filename, coords_are_cartesian)
+    elif fmt == "as":
+        _to_dspaw_as(structure, filename, coords_are_cartesian)
+    elif fmt == "hzw":
+        _to_hzw(structure, filename)
+    elif fmt == "pdb":
+        _to_pdb(structure, filename)
+
+
+def _write_atoms(fileobj, hdf5):
     fileobj.write("DS-PAW Structure\n")
     fileobj.write("  1.00\n")
     lattice = np.asarray(hdf5["/AtomInfo/Lattice"]).reshape(-1, 1)  # 将列表lattice下的多个列表整合
     fileobj.write(
         "%10.6f %10.6f %10.6f\n" % (lattice[0][0], lattice[1][0], lattice[2][0])
     )
     fileobj.write(
@@ -413,17 +498,17 @@
     for i, p in enumerate(hdf5["/AtomInfo/Position"]):
         fileobj.write("%10.6f" % p)
         if (i + 1) % 3 == 0:
             fileobj.write("\n")
     fileobj.write("\n")
 
 
-def write_VESTA_format(hdf5: dict, datakeys: list, filename):
+def _write_VESTA_format(hdf5: dict, datakeys: list, filename):
     with open(filename, "w") as file:
-        write_atoms(file, hdf5)
+        _write_atoms(file, hdf5)
         for key in datakeys:
             d = np.asarray(hdf5[key]).reshape(-1, 1)  # 将列表hdf5[key]下的多个列表整合
             file.write("%5d %5d %5d\n" % tuple(hdf5["/AtomInfo/Grid"]))
             i = 0
             while i < len(d):
                 for j in range(10):
                     file.write("%10.5f " % d[i])
@@ -431,15 +516,15 @@
                     if i >= len(d):
                         break
                 file.write("\n")
 
             file.write("\n")
 
 
-def write_atoms_json(fileobj, atom_info):
+def _write_atoms_json(fileobj, atom_info):
     fileobj.write("DS-PAW Structure\n")
     fileobj.write("  1.00\n")
     lattice = atom_info["Lattice"]
 
     fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[0], lattice[1], lattice[2]))
     fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[3], lattice[4], lattice[5]))
     fileobj.write("%10.6f %10.6f %10.6f\n" % (lattice[6], lattice[7], lattice[8]))
@@ -466,22 +551,130 @@
     else:
         fileobj.write("Cartesian\n")
     for atom in atom_info["Atoms"]:
         fileobj.write("%10.6f %10.6f %10.6f\n" % tuple(atom["Position"]))
     fileobj.write("\n")
 
 
-def write_VESTA_format_json(atom_info: dict, data: list, filename):
+def _write_VESTA_format_json(atom_info: dict, data: list, filename):
     with open(filename, "w") as file:
-        write_atoms_json(file, atom_info)
+        _write_atoms_json(file, atom_info)
         for d in data:
             file.write("%5d %5d %5d\n" % tuple(atom_info["Grid"]))
             i = 0
             while i < len(d):
                 for j in range(10):
                     file.write("%10.5f " % d[i])
                     i += 1
                     if i >= len(d):
                         break
                 file.write("\n")
 
             file.write("\n")
+
+
+def _to_dspaw_as(structure, filename: str, coords_are_cartesian=True):
+    """write dspaw as file
+    If converted from as file, will copy the mag and fix info,
+        otherwise, those info will be ignored!
+    """
+    with open(filename, "w", encoding="utf-8") as file:
+        file.write("Total number of atoms\n")
+        file.write("%d\n" % len(structure))
+
+        file.write("Lattice\n")
+        for v in structure.lattice.matrix:
+            file.write("%.6f %.6f %.6f\n" % (v[0], v[1], v[2]))
+
+        i = 0
+        for site in structure:
+            if i == 0:
+                if "line6s" in site.properties:
+                    file.write("%s\n" % site.properties["line6s"])
+                else:
+                    if coords_are_cartesian:
+                        file.write("Cartesian\n")
+                    else:
+                        file.write("Direct\n")
+            i += 1
+
+            coords = site.coords if coords_are_cartesian else site.frac_coords
+            if "others" in site.properties:
+                sp = " ".join(site.properties["others"])  # flatten str list
+                file.write(
+                    "%s %.6f %.6f %.6f %s\n"
+                    % (site.species_string, coords[0], coords[1], coords[2], sp)
+                )
+            else:  # the most common case
+                file.write(
+                    "%s %.6f %.6f %.6f\n"
+                    % (site.species_string, coords[0], coords[1], coords[2])
+                )
+
+
+def _to_hzw(structure, filename: str):
+    with open(filename, "w", encoding="utf-8") as file:
+        file.write("% The number of probes \n")
+        file.write("0\n")
+        file.write("% Uni-cell vector\n")
+
+        for v in structure.lattice.matrix:
+            file.write("%.6f %.6f %.6f\n" % (v[0], v[1], v[2]))
+
+        file.write("% Total number of device_structure\n")
+        file.write("%d\n" % len(structure))
+        file.write("% Atom site\n")
+
+        for site in structure:
+            file.write(
+                "%s %.6f %.6f %.6f\n"
+                % (site.species_string, site.coords[0], site.coords[1], site.coords[2])
+            )
+
+
+def _to_dspaw_json(structure, filename: str, coords_are_cartesian=True):
+    lattice = structure.lattice.matrix.flatten().tolist()
+    atoms = []
+    for site in structure:
+        coords = site.coords if coords_are_cartesian else site.frac_coords
+        atoms.append({"Element": site.species_string, "Position": coords.tolist()})
+
+    coordinate_type = "Cartesian" if coords_are_cartesian else "Direct"
+    d = {"Lattice": lattice, "CoordinateType": coordinate_type, "Atoms": atoms}
+
+    with open(filename, "w", encoding="utf-8") as file:
+        json.dump(d, file, indent=4)
+
+
+def _to_pdb(structures, pdb_filename: str):
+    with open(pdb_filename, "w", encoding="utf-8") as file:
+        for i, s in enumerate(structures):
+            file.write("MODEL         %d\n" % (i + 1))
+            file.write("REMARK   Converted from Structures\n")
+            file.write("REMARK   Converted using dspawpy\n")
+            lengths = s.lattice.lengths
+            angles = s.lattice.angles
+            file.write(
+                "CRYST1{0:9.3f}{1:9.3f}{2:9.3f}{3:7.2f}{4:7.2f}{5:7.2f}\n".format(
+                    lengths[0], lengths[1], lengths[2], angles[0], angles[1], angles[2]
+                )
+            )
+            for j, site in enumerate(s):
+                file.write(
+                    "%4s%7d%4s%5s%6d%4s%8.3f%8.3f%8.3f%6.2f%6.2f%12s\n"
+                    % (
+                        "ATOM",
+                        j + 1,
+                        site.species_string,
+                        "MOL",
+                        1,
+                        "    ",
+                        site.coords[0],
+                        site.coords[1],
+                        site.coords[2],
+                        1.0,
+                        0.0,
+                        site.species_string,
+                    )
+                )
+            file.write("TER\n")
+            file.write("ENDMDL\n")
```

## Comparing `dspawpy-0.9.0.dist-info/METADATA` & `dspawpy-0.9.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: pymatgen (>=2021.2.8.1)
@@ -27,14 +27,21 @@
 
 再重新用pip安装。
 
 详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
 
 ## 版本更新简述
 
+### 0.9.1
+
+- 重要变更： 精简合并多个函数，统一调用方法
+- 新增功能： 支持合并多个xyz和dump文件
+- 细节优化： 读取h5或json文件后若无错误，不再打印空行
+- 细节优化： 耗时的RDF计算显示进度百分比
+
 ### 0.9.0
 
 - 重要变更： 一些函数合并、所在模块迁移，请确认版本
 - 新增功能： 支持读取含多离子步计算结果的h5/json文件中的磁矩信息
 - BUG修复： get_band_data 函数指定efermi不生效
 
 ### 0.8.9
```

## Comparing `dspawpy-0.9.0.dist-info/RECORD` & `dspawpy-0.9.1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 dspawpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/plot.py,sha256=ocLkU08WfMb2fyETrBSSZvxZFSg2sPX8rLusXZLT5BM,29208
 dspawpy/analysis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/analysis/aimdtools.py,sha256=olmINWb4xRDZvdBohA2oUE3KzBiWq508w5DdslTEAWI,23956
+dspawpy/analysis/aimdtools.py,sha256=vNSr_6lKBGEsfmxzN2EjQQCEhtwxflxNseJCPTiU614,24557
 dspawpy/analysis/vacf.py,sha256=g5IS6Q7QGYa17XBVnYEH-MubGSpkUsDPpMaI_ELacw4,20152
 dspawpy/diffusion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/diffusion/neb.py,sha256=dQEofdCZ7MbRwdfQKzp1_YMZwyZDcYceBYjXyahXL1c,9639
-dspawpy/diffusion/nebtools.py,sha256=4z0hFkGABLXFKugTTw6vaw-Sf2fUn0okBAdUmwL7RSk,53458
+dspawpy/diffusion/neb.py,sha256=U6J7lSlE_xp1rCON5mgfWWi5DFHVZYVb5xjqLlGxXXI,3592
+dspawpy/diffusion/nebtools.py,sha256=tfQCQPUmZKELz7ImwyiJiiFfXahC9U3doarExspL-DU,53467
 dspawpy/diffusion/pathfinder.py,sha256=HhCVoh42Q2qIksBAruZ1atULfR5D55uzZvbaCtUxSig,11045
 dspawpy/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/io/read.py,sha256=aq8LtjRqKHzBGmgP3gScovh4qdabe0T5cmY9L022t9k,41491
+dspawpy/io/read.py,sha256=BfyiGH-aJLjQAMMNAF9tuThQHIyJGzCa6R0zzqkXMpE,48925
 dspawpy/io/read_json.py,sha256=2bcNQP51SR2yMyFE7c2TIutYp93K8IH-dpLmH5yy4bo,7721
-dspawpy/io/structure.py,sha256=CTENSGY9bEX0B3BCY4mgQYu20TEYOBOlgNNHJhgkREA,13268
-dspawpy/io/utils.py,sha256=1VDBKhXHiM0er2nGcHhu6_wD4cLpteOhS6W0UxT3MMo,25265
-dspawpy/io/write.py,sha256=7y35-1RxtjE3moma8ke9BUZKsyMFuJRLVRcz6AiJJ_k,17401
+dspawpy/io/structure.py,sha256=HqhBLKqAJcHclFCZH4lEiaX7yR_qv8ygACOsPHyLKn0,6163
+dspawpy/io/utils.py,sha256=FdbFbZqKfnDOGBJ4OaKD-4IBAAlqjtQ0l1NppvkMKOM,25241
+dspawpy/io/write.py,sha256=CKgyqSGFvjkIcrzeeVDyZS4W2Otvpz1FlewlPOqieP0,24416
 dspawpy/io/write_json.py,sha256=n3GhdDnFFtW7eY4U5u7czdlpbSWnsGP7WUD5eS1ZmqI,1761
-dspawpy-0.9.0.dist-info/METADATA,sha256=HSirmPHTTKR0-WmU6ZKp0ihYBbOzuTSKKhWymnWRiT4,1766
-dspawpy-0.9.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dspawpy-0.9.0.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
-dspawpy-0.9.0.dist-info/RECORD,,
+dspawpy-0.9.1.dist-info/METADATA,sha256=EQov-UB9e9O0p886lOUr6Oj9MDfA-PJyMgfyTlVSVIk,2036
+dspawpy-0.9.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dspawpy-0.9.1.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
+dspawpy-0.9.1.dist-info/RECORD,,
```

