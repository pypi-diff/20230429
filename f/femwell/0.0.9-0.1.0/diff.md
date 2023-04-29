# Comparing `tmp/femwell-0.0.9.tar.gz` & `tmp/femwell-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femwell-0.0.9.tar", max compression
+gzip compressed data, was "femwell-0.1.0.tar", max compression
```

## Comparing `femwell-0.0.9.tar` & `femwell-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0    35149 2023-02-09 21:22:39.959659 femwell-0.0.9/LICENSE
--rw-r--r--   0        0        0     1978 2023-02-09 21:22:39.959659 femwell-0.0.9/README.md
--rw-r--r--   0        0        0      255 2023-02-09 21:22:39.959659 femwell-0.0.9/femwell/__init__.py
--rw-r--r--   0        0        0     3080 2023-02-09 21:22:39.959659 femwell-0.0.9/femwell/culomb.py
--rw-r--r--   0        0        0    10175 2023-02-09 21:22:39.959659 femwell-0.0.9/femwell/eme.py
--rw-r--r--   0        0        0        0 2023-02-09 21:22:39.959659 femwell-0.0.9/femwell/examples/__init__.py
--rw-r--r--   0        0        0     5156 2023-02-09 21:22:39.959659 femwell-0.0.9/femwell/examples/coplanar_waveguide.py
--rw-r--r--   0        0        0     5931 2023-02-09 21:22:39.959659 femwell-0.0.9/femwell/examples/coupled_mode_theory.py
--rw-r--r--   0        0        0     2390 2023-02-09 21:22:39.959659 femwell-0.0.9/femwell/examples/overlap_integrals.py
--rw-r--r--   0        0        0     3716 2023-02-09 21:22:39.959659 femwell-0.0.9/femwell/examples/si_heater.py
--rw-r--r--   0        0        0     5762 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/fefd.py
--rw-r--r--   0        0        0     1304 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/fiber.py
--rw-r--r--   0        0        0      224 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mesh/__init__.py
--rw-r--r--   0        0        0    24207 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mesh/mesh.py
--rw-r--r--   0        0        0     7713 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mesh/meshtracker.py
--rw-r--r--   0        0        0     9318 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mesh/slice.py
--rw-r--r--   0        0        0    21379 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mesh.py
--rw-r--r--   0        0        0    11873 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mode_solver.py
--rw-r--r--   0        0        0     1033 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mode_solver_1d.py
--rw-r--r--   0        0        0     2900 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mode_solver_2d_periodic.py
--rw-r--r--   0        0        0     6950 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mode_solver_2d_periodic_quadratic.py
--rw-r--r--   0        0        0     4224 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/mode_solver_inplane.py
--rw-r--r--   0        0        0     4714 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/solver.py
--rw-r--r--   0        0        0     5897 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/tcad.py
--rw-r--r--   0        0        0     2820 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/tests/test_mesh.py
--rw-r--r--   0        0        0     5626 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/thermal.py
--rw-r--r--   0        0        0     7744 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/thermal_transient.py
--rw-r--r--   0        0        0     2139 2023-02-09 21:22:39.963659 femwell-0.0.9/femwell/waveguide.py
--rw-r--r--   0        0        0      879 2023-02-09 21:23:05.423435 femwell-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 femwell-0.0.9/setup.py
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 femwell-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-29 13:21:37.219888 femwell-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2480 2023-04-29 13:21:37.219888 femwell-0.1.0/README.md
+-rw-r--r--   0        0        0      255 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/__init__.py
+-rw-r--r--   0        0        0     3080 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/culomb.py
+-rw-r--r--   0        0        0    10175 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/eme.py.bak
+-rw-r--r--   0        0        0        0 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/examples/__init__.py
+-rw-r--r--   0        0        0     4820 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/examples/coplanar_waveguide.py
+-rw-r--r--   0        0        0     5762 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/fefd.py
+-rw-r--r--   0        0        0     1304 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/fiber.py
+-rw-r--r--   0        0        0     1782 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/laplace.py
+-rw-r--r--   0        0        0    16525 2023-04-29 13:21:37.219888 femwell-0.1.0/femwell/maxwell/waveguide.py
+-rw-r--r--   0        0        0      224 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh/__init__.py
+-rw-r--r--   0        0        0    26893 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh/mesh.py
+-rw-r--r--   0        0        0     7713 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh/meshtracker.py
+-rw-r--r--   0        0        0     9318 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh/slice.py
+-rw-r--r--   0        0        0    21359 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mesh.py
+-rw-r--r--   0        0        0     1033 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_1d.py
+-rw-r--r--   0        0        0     2922 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_2d_periodic.py
+-rw-r--r--   0        0        0     6950 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_2d_periodic_quadratic.py
+-rw-r--r--   0        0        0     4224 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_inplane.py
+-rw-r--r--   0        0        0     1243 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/mode_solver_schrodinger.py
+-rw-r--r--   0        0        0     8799 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/pn_analytical.py
+-rw-r--r--   0        0        0     6453 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/solver.py
+-rw-r--r--   0        0        0     5897 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/tcad.py
+-rw-r--r--   0        0        0     2820 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/tests/test_mesh.py
+-rw-r--r--   0        0        0     5880 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/thermal.py
+-rw-r--r--   0        0        0     8803 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/thermal_transient.py
+-rw-r--r--   0        0        0     2655 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/utils.py
+-rw-r--r--   0        0        0     1123 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/visualization.py
+-rw-r--r--   0        0        0     2089 2023-04-29 13:21:37.223888 femwell-0.1.0/femwell/waveguide.py
+-rw-r--r--   0        0        0      974 2023-04-29 13:21:50.956002 femwell-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 femwell-0.1.0/PKG-INFO
```

### Comparing `femwell-0.0.9/LICENSE` & `femwell-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/README.md` & `femwell-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,40 +4,56 @@
 
 [![Docs](https://github.com/helgegehring/femwell/actions/workflows/docs.yml/badge.svg)](https://HelgeGehring.github.io/femwell/)
 [![Build](https://github.com/helgegehring/femwell/actions/workflows/build.yml/badge.svg)](https://github.com/HelgeGehring/femwell/actions/workflows/build.yml)
 [![PiPy](https://img.shields.io/pypi/v/femwell)](https://pypi.org/project/femwell/)
 [![Downloads](https://static.pepy.tech/badge/femwell/month)](https://pepy.tech/project/femwell)
 
 Finite element based simulation tool for integrated circuits, electric and photonic!
-The documentation is lagging behind the state of code, so there's several features for which there are only examples in the code.
+The documentation is lagging behind the state of code,
+so there's several features for which there are only examples in the code.
 
-**You can try out the examples in the browser! Hover the rocket at the top on the example pages and click live code!**
+**You can try out the examples in the browser!**
+**Hover the rocket at the top on the example pages and click live code!**
 (Might take some time to load)
 
-# Working Features
+## Features
+
 - Photonic eigenmode solver
 - Periodic photonic eigenmode solver
 - Electric eigenmode solver
 - Thermal mode solver (static and transient)
 - Coulomb solver
 
-# Possible Simulations
+## Possible Simulations
+
 - Eigenmodes of waveguides and determining their effective refractive index
+- Coupling between neighboring waveguides
+- Eigenmodes of bent waveguides
+- Propagation loss of circular bends and mode mismatch loss with straight waveguides
+- Calculation of the group velocity and its dispersion
+- Calculation of overlap-integrals and confinement-factors
 - Bragg grating cells
 - Grating coupler cells
 - Eigenmode of a coaxial cable and its specific impedance
-- Eigenmodes of electric transmission lines and determining their propagation constant (in work)
+- Eigenmodes of electric transmission lines
+  and determining their propagation constant (in work)
 - Static thermal profiles
 - Transient thermal behavior
 - Static electric fields
 - Overlap integrals between waveguide modes
 - Overlap integral between a waveguide mode and a fiber mode
 - Coupled mode theory - coupling between adjacent waveguides
 - Heat based photonic phase shifters
 - Pockels based photonic phase shifters
+- PN junction depletion modulator (analytical)
+
+Something missing? Feel free to open an [issue](https://github.com/HelgeGehring/femwell/issues) :)
+
+## Contributors
 
-# Contributors
 - Helge Gehring (Google): Maintainer
-- Simon Bilodeau (Google): Meshes everything
+- Simon Bilodeau (Google): Meshes everything, Analytical PN model
 - Joaquin Matres (Google): Code simplifications
+- Marc de Cea Falco (Google): Documentation improvements
 
-Happy about every form of contribution - pull requests, feature requests, issues, questions, ... :)
+Happy about every form of contribution -
+pull requests, feature requests, issues, questions, ... :)
```

### Comparing `femwell-0.0.9/femwell/culomb.py` & `femwell-0.1.0/femwell/culomb.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/eme.py` & `femwell-0.1.0/femwell/eme.py.bak`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/examples/coplanar_waveguide.py` & `femwell-0.1.0/femwell/examples/coplanar_waveguide.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import numpy as np
 import scipy.constants
 import shapely
 import shapely.ops
 from shapely.geometry import LineString, box
 from skfem import Basis, ElementTriP0, Mesh
 
+from femwell.maxwell.waveguide import compute_modes
 from femwell.mesh import mesh_from_OrderedDict
-from femwell.mode_solver import calculate_hfield, compute_modes, plot_mode
 
 
 def mesh_waveguide(filename, wsim, hclad, hsi, wcore, hcore):
     core = box(-wcore / 2, -hcore / 2, wcore / 2, hcore / 2)
     clad = box(-wsim / 2, -hcore / 2, wsim / 2, -hcore / 2 + hclad)
     silicon = box(-wsim / 2, -hcore / 2, wsim / 2, -hcore / 2 - hsi)
 
-    all = shapely.ops.unary_union([core, clad, silicon])
+    combined = shapely.ops.unary_union([core, clad, silicon])
 
     polygons = OrderedDict(
-        boundary=LineString(all.exterior),
+        boundary=LineString(combined.exterior),
         interface=LineString(
             [
                 (-wsim / 2, -hcore / 2),
                 (wsim / 2, -hcore / 2),
             ]
         ),
         core_interface=core.exterior,
@@ -43,18 +43,18 @@
 
 def mesh_waveguide_1(filename, wsim, hclad, hsi, wcore, hcore, gap):
     core_l = box(-wcore - gap, -hcore / 2, -gap / 2, hcore / 2)
     core_r = box(wcore + gap, -hcore / 2, gap / 2, hcore / 2)
     clad = box(-wsim / 2, -hcore / 2, wsim / 2, -hcore / 2 + hclad)
     silicon = box(-wsim / 2, -hcore / 2, wsim / 2, -hcore / 2 - hsi)
 
-    all = shapely.ops.unary_union([core_l, core_r, clad, silicon])
+    combined = shapely.ops.unary_union([core_l, core_r, clad, silicon])
 
     polygons = OrderedDict(
-        boundary=LineString(all.exterior),
+        boundary=LineString(combined.exterior),
         interface=LineString(
             [
                 (-wsim / 2, -hcore / 2),
                 (wsim / 2, -hcore / 2),
             ]
         ),
         core_l_interface=core_l.exterior,
@@ -105,50 +105,39 @@
     epsilon = basis0.zeros().astype(complex)
     epsilon[basis0.get_dofs(elements="isolator")] = 1.29
     epsilon[basis0.get_dofs(elements="isolator2")] = 1.29
     epsilon[basis0.get_dofs(elements="core")] = 1 + 1j * 5.8e7 * 1e20 / frequency
     basis0.plot(np.real(epsilon), colorbar=True).show()
 
     conductors = ["isolator2___isolator"]
-    lams, basis, xs = compute_modes(
+    modes = compute_modes(
         basis0,
         epsilon,
         wavelength=scipy.constants.speed_of_light / frequency * 1e3,
         mu_r=1,
         num_modes=len(conductors),
         metallic_boundaries=True,
     )
-    print("propagation constants", 1 / lams)
+    print("propagation constants", 1 / modes.n_effs)
 
-    fig, axs = plot_mode(basis, np.real(xs[0]), plot_vectors=True)
-    plt.show()
+    modes[0].show(modes[0].E.real, plot_vectors=True)
 
     from skfem import *
     from skfem.helpers import *
 
     @Functional(dtype=np.complex64)
     def current_form(w):
         return inner(np.array([w.n[1], -w.n[0]]), w.H)
 
-    currents = np.zeros((len(conductors), len(lams)))
+    currents = np.zeros((len(conductors), len(modes)))
 
-    for mode_i in range(len(lams)):
-        xbs = calculate_hfield(
-            basis,
-            xs[mode_i],
-            lams[mode_i] * (2 * np.pi / (scipy.constants.speed_of_light / frequency * 1e3)),
-            omega=2 * np.pi * frequency * 1e-3,
-        )
+    for mode_i, mode in enumerate(modes):
+        mode.show(mode.H.real, plot_vectors=True)
 
-        fig, axs = plot_mode(basis, np.real(xbs), plot_vectors=True)
-        plt.show()
-
-        (ht, ht_basis), (hz, hz_basis) = basis.split(xbs)
+        (ht, ht_basis), (hz, hz_basis) = mode.basis.split(mode.H)
         for conductors_i, conductor in enumerate(conductors):
-            facet_basis = FacetBasis(
-                ht_basis.mesh, ht_basis.elem, facets=mesh.boundaries[conductor]
-            )
+            facet_basis = ht_basis.boundary(facets=mesh.boundaries[conductor])
             current = abs(current_form.assemble(facet_basis, H=facet_basis.interpolate(ht)))
             currents[conductors_i, mode_i] = current
 
     characteristic_impedances = np.linalg.inv(currents).T @ np.linalg.inv(currents)
     print("characteristic impedances", characteristic_impedances)
```

### Comparing `femwell-0.0.9/femwell/fefd.py` & `femwell-0.1.0/femwell/fefd.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/fiber.py` & `femwell-0.1.0/femwell/fiber.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/mesh/mesh.py` & `femwell-0.1.0/femwell/mesh/mesh.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,21 @@
     Point,
     Polygon,
 )
 from shapely.ops import linemerge, polygonize, split, unary_union
 
 from femwell.mesh.meshtracker import MeshTracker
 
+initial_settings = np.seterr()  # remove when shapely updated to more recent geos
+
 
 def break_line_(line, other_line):
+    np.seterr(invalid="ignore")
     intersections = line.intersection(other_line)
+    np.seterr(**initial_settings)
     if not intersections.is_empty:
         for intersection in (
             intersections.geoms if hasattr(intersections, "geoms") else [intersections]
         ):
             # if type == "", intersection.type != 'Point':
             if intersection.geom_type == "Point":
                 line = linemerge(split(line, intersection))
@@ -59,15 +63,17 @@
         model = geometry
 
         # Add overall bounding box
         total = unary_union(list(shapes_dict.values()))
         all_polygons = [total, *list(shapes_dict.values())]
         # Break up all shapes so that plane is tiled with non-overlapping layers, get the maximal number of fragments
         # Equivalent to BooleanFragments
+        np.seterr(invalid="ignore")
         listpoly = [a.intersection(b) for a, b in combinations(all_polygons, 2)]
+        np.seterr(**initial_settings)
         rings = [
             LineString(list(object.exterior.coords))
             for object in listpoly
             if not (object.geom_type in ["Point", "LineString"] or object.is_empty)
         ]
 
         union = unary_union(rings)
@@ -158,35 +164,41 @@
 
         # Extract all unique lines (TODO: identify interfaces in label)
         # i = 0
         # for index, line in enumerate(meshtracker.gmsh_xy_segments):
         #     model.add_physical(line, f"{meshtracker.xy_segments_main_labels[index]}_{meshtracker.xy_segments_secondary_labels[index]}_{i}")
         #     i += 1
 
+        # For periodicity
+
         mesh = geometry.generate_mesh(dim=2, verbose=verbose)
 
         if filename:
             gmsh.write(f"{filename}")
 
         return mesh
 
 
 def mesh_from_OrderedDict(
     shapes_dict: OrderedDict,
     resolutions: Optional[Dict[str, Dict[str, float]]] = None,
-    default_resolution_min: float = 0.01,
+    default_resolution_min: float = 1e-12,
     default_resolution_max: float = 0.5,
     filename: Optional[str] = None,
     gmsh_algorithm: int = 5,
     global_quad: Optional[bool] = False,
     verbose: bool = False,
+    periodic_lines: Optional[Tuple[(str, str)]] = None,
+    mesh_scaling_factor: float = 1.0,
 ):
     """
     Given an ordered dict of shapely Polygons, creates a mesh containing polygon surfaces according to the dict order.
     Returns a gmsh msh with physicals corresponding to the shapes_dict boundaries (which is the minimal number of surfaces for each key)
+
+    periodic_lines: (label1, label1) tuples forcing the mesh of line[label1] to map to the mesh of line[label2]. Currently only works if the lines are not intersected.
     """
 
     with pygmsh.occ.geometry.Geometry() as geometry:
         # geometry = pygmsh.occ.geometry.Geometry()
         geometry.characteristic_length_min = default_resolution_min
         geometry.characteristic_length_max = default_resolution_max
         gmsh.option.setNumber("Mesh.Algorithm", gmsh_algorithm)
@@ -279,17 +291,19 @@
                                     # Interiors
                                     for second_interior_line in (
                                         second_shape.interiors
                                         if second_shape.geom_type == "Polygon"
                                         else []
                                     ):
                                         second_interior_line = LineString(second_interior_line)
+                                        np.seterr(invalid="ignore")
                                         intersections = first_interior_line.intersection(
                                             second_interior_line
                                         )
+                                        np.seterr(**initial_settings)
                                         first_interior_line = break_line_(
                                             first_interior_line, second_interior_line
                                         )
                         first_shape_interiors.append(first_interior_line)
                 if first_shape.geom_type in ["Polygon", "MultiPolygon"]:
                     broken_shapes.append(Polygon(first_exterior_line, holes=first_shape_interiors))
                 else:
@@ -382,14 +396,37 @@
                     meshtracker.xy_segments_main_labels[index] == surface2
                     and meshtracker.xy_segments_secondary_labels[index] == surface1
                 ):
                     interfaces.append(line)
             if interfaces:
                 model.add_physical(interfaces, f"{surface1}___{surface2}")
 
+        gmsh.model.occ.synchronize()
+
+        # Force periodicity (experimental)
+        def validate_lines(line1, line2):
+            """TODO create a module for validating geometries."""
+
+        if periodic_lines:
+            for label1, label2 in periodic_lines:
+                # if validate_lines(): # TODO
+                line1 = shapes_dict[label1]
+                line2 = shapes_dict[label2]
+                gmsh.model.setCurrent("pygmsh model")
+                translation = np.array(line1.coords[0]) - np.array(line2.coords[0])
+                gmsh.model.mesh.setPeriodic(
+                    1,
+                    meshtracker.get_gmsh_xy_lines_from_label(label1),
+                    meshtracker.get_gmsh_xy_lines_from_label(label2),
+                    [1, 0, 0, translation[0], 0, 1, 0, translation[1], 0, 0, 1, 0, 0, 0, 0, 1],
+                )
+                # else: # TODO
+                #     raise ValueError("Periodic line pairs must be parallel and have the same straight length in the final, intersected geometry.")
+
+        gmsh.option.setNumber("Mesh.ScalingFactor", mesh_scaling_factor)
         mesh = geometry.generate_mesh(dim=2, verbose=verbose)
 
         if filename:
             gmsh.write(f"{filename}")
 
         import contextlib
         import tempfile
@@ -427,32 +464,59 @@
             (-width_wg_2 / 2, length_wg_2),
             (width_wg_2 / 2, length_wg_2),
             (width_wg_2 / 2, 0),
             (width_wg_1 / 2, 0),
             (width_wg_1 / 2, -length_wg_1),
         ]
     )
+    print(core)
+
+    box = Polygon(
+        [
+            (-width_wg_2 - 1, -6),
+            (-width_wg_2 - 1, 6),
+            (width_wg_2 - 0.5, 6),
+            (width_wg_2 - 0.5, -6),
+        ]
+    )
+    print(box)
 
     source = LineString([(width_wg_2 / 2, -length_wg_1 / 2), (-width_wg_2 / 2, -length_wg_1 / 2)])
     print(source)
 
+    left_wall_up = LineString([(-width_wg_2 - 1, -2), (-width_wg_2 - 1, 6)])
+    right_wall_up = LineString([(width_wg_2 - 0.5, -2), (width_wg_2 - 0.5, 6)])
+    left_wall_dw = LineString([(-width_wg_2 - 1, -6), (-width_wg_2 - 1, -2)])
+    right_wall_dw = LineString([(width_wg_2 - 0.5, -6), (width_wg_2 - 0.5, -2)])
+
     polygons = OrderedDict(
+        left_wall_up=left_wall_up,
+        right_wall_up=right_wall_up,
+        left_wall_dw=left_wall_dw,
+        right_wall_dw=right_wall_dw,
         source=source,
         core=core,
-        box=core.buffer(1, resolution=4) - core,
-        pml=core.buffer(2, resolution=4) - core.buffer(1, resolution=4),
+        box=box,
+        # pml=core.buffer(2, resolution=4) - core.buffer(1, resolution=4),
     )
 
     resolutions = dict(
         source={"resolution": 0.02, "distance": 1},
         core={"resolution": 0.02, "distance": 1},
+        # left_wall_up={"resolution": 1, "distance": 1},
+        # right_wall_up={"resolution": 0.5, "distance": 1},
     )
 
     mesh = mesh_from_OrderedDict(
-        polygons, resolutions, filename="mesh.msh", default_resolution_max=0.3
+        polygons,
+        resolutions,
+        filename="mesh.msh",
+        default_resolution_max=1,
+        # periodic_lines=[("left_wall_up", "right_wall_up"), ("left_wall_dw", "right_wall_dw")],
+        mesh_scaling_factor=1e-4,
     )
 
     # wmode = 1
     # wsim = 2
     # hclad = 2
     # hbox = 2
     # wcore = 0.5
```

### Comparing `femwell-0.0.9/femwell/mesh/meshtracker.py` & `femwell-0.1.0/femwell/mesh/meshtracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Point,
     Polygon,
 )
 from shapely.ops import linemerge, split
 
 
 class MeshTracker:
-    def __init__(self, model, atol=1e-3):
+    def __init__(self, model, atol=1e-6):
         """
         Map between shapely and gmsh
         Shapely is useful for built-in geometry equivalencies and extracting orientation, instead of doing it manually
         We can also track information about the entities using labels (useful for selective mesh refinement later)
         """
         self.shapely_points = []
         self.gmsh_points = []
```

### Comparing `femwell-0.0.9/femwell/mesh/slice.py` & `femwell-0.1.0/femwell/mesh/slice.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/mesh.py` & `femwell-0.1.0/femwell/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,17 +367,17 @@
         gmsh.model.mesh.field.setAsBackgroundMesh(n)
 
         gmsh.model.mesh.MeshSizeFromPoints = 0
         gmsh.model.mesh.MeshSizeFromCurvature = 0
         gmsh.model.mesh.MeshSizeExtendFromBoundary = 0
 
         # Fuse edges (bandaid)
-        # gmsh.model.occ.synchronize()
-        # gmsh.model.occ.removeAllDuplicates()
-        # gmsh.model.occ.synchronize()
+        gmsh.model.occ.synchronize()
+        gmsh.model.occ.removeAllDuplicates()
+        gmsh.model.occ.synchronize()
 
         # Extract all unique lines (TODO: identify interfaces in label)
         i = 0
         for index, line in enumerate(meshtracker.gmsh_xy_segments):
             model.add_physical(
                 line,
                 f"{meshtracker.xy_segments_main_labels[index]}_{meshtracker.xy_segments_secondary_labels[index]}_{i}",
@@ -417,18 +417,18 @@
     bottom_edge = LineString(
         [Point(-wsim / 2, -hcore / 2 - hbox), Point(wsim / 2, -hcore / 2 - hbox)]
     )
 
     # Polygons not only have an edge, but an interior
     core = Polygon(
         [
-            Point(-wcore / 2, -hcore / 2 + offset_core),
+            Point(-wcore / 2 - 0.5, -hcore / 2 + offset_core),
             Point(-wcore / 2, hcore / 2 + offset_core),
             Point(wcore / 2, hcore / 2 + offset_core),
-            Point(wcore / 2, -hcore / 2 + offset_core),
+            Point(wcore / 2 - 0.5, -hcore / 2 + offset_core),
         ]
     )
     core2 = Polygon(
         [
             Point(-wcore / 2, -hcore / 2 + offset_core2),
             Point(-wcore / 2, hcore / 2 + offset_core2),
             Point(wcore / 2, hcore / 2 + offset_core2),
@@ -478,15 +478,14 @@
 
     quad = False
     mesh = mesh_from_polygons(
         shapes,
         resolutions,
         filename="mesh.msh",
         default_resolution_max=0.3,
-        global_quad=quad,
     )
 
     # gmsh.write("mesh.msh")
     # gmsh.clear()
     # mesh.__exit__()
 
     import meshio
```

### Comparing `femwell-0.0.9/femwell/mode_solver.py` & `femwell-0.1.0/femwell/maxwell/waveguide.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 """Waveguide analysis based on https://doi.org/10.1080/02726340290084012."""
+from dataclasses import dataclass
+from functools import cached_property
+from typing import List
+
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.constants
 import scipy.sparse.linalg
+from numpy.typing import NDArray
+from scipy.constants import epsilon_0, speed_of_light
 from skfem import (
     Basis,
     BilinearForm,
     ElementDG,
     ElementTriN1,
     ElementTriN2,
     ElementTriP0,
@@ -19,25 +25,182 @@
     condense,
     solve,
 )
 from skfem.helpers import cross, curl, dot, grad, inner
 from skfem.utils import solver_eigen_scipy
 
 
+@dataclass(frozen=True)
+class Mode:
+    frequency: float
+    """Frequency of the light"""
+    k: float
+    """Propagation constant of the mode"""
+    basis_epsilon_r: Basis
+    """Basis used for epsilon_r"""
+    epsilon_r: NDArray
+    """Epsilon_r with which the mode was calculated"""
+    basis: Basis
+    """Basis on which the mode was calculated and E/H are defined"""
+    E: NDArray
+    """Electric field of the mode"""
+    H: NDArray
+    """Magnetic field of the mode"""
+
+    @property
+    def omega(self):
+        """Angular frequency of the light"""
+        return 2 * np.pi * self.frequency
+
+    @property
+    def k0(self):
+        """Vacuum propagation constant of the light"""
+        return self.omega / speed_of_light
+
+    @property
+    def wavelength(self):
+        """Vacuum wavelength of the light"""
+        return speed_of_light / self.frequency
+
+    @property
+    def n_eff(self):
+        """Effective refractive index of the mode"""
+        return self.k / self.k0
+
+    @cached_property
+    def te_fraction(self):
+        """TE-fraction of the mode"""
+
+        @Functional
+        def ex(w):
+            return np.abs(w.E[0][0]) ** 2
+
+        @Functional
+        def ey(w):
+            return np.abs(w.E[0][1]) ** 2
+
+        ex_sum = ex.assemble(self.basis, E=self.basis.interpolate(self.E))
+        ey_sum = ey.assemble(self.basis, E=self.basis.interpolate(self.E))
+
+        return ex_sum / (ex_sum + ey_sum)
+
+    @cached_property
+    def tm_fraction(self):
+        """TM-fraction of the mode"""
+
+        return 1 - self.te_fraction
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(k: {self.k}, n_eff:{self.n_eff})"
+
+    def calculate_overlap(self, mode, elements=None):
+        return calculate_overlap(self.basis, self.E, self.H, mode.basis, mode.E, mode.H)
+
+    def calculate_coupling_coefficient(self, mode, delta_epsilon):
+        @Functional(dtype=complex)
+        def overlap(w):
+            return w["delta_epsilon"] * (
+                dot(np.conj(w["E_i"][0]), w["E_j"][0]) + np.conj(w["E_i"][1]) * w["E_j"][1]
+            )
+
+        return overlap.assemble(
+            self.basis,
+            E_i=self.basis.interpolate(self.E),
+            E_j=self.basis.interpolate(mode.E),
+            delta_epsilon=self.basis_epsilon_r.interpolate(delta_epsilon),
+        )
+
+    def calculate_propagation_loss(self, distance):
+        return -20 / np.log(10) * self.k0 * np.imag(self.n_eff) * distance
+
+    def calculate_power(self, elements=None):
+        if not elements:
+            basis = self.basis
+        else:
+            basis = self.basis.with_elements(elements)
+        return calculate_overlap(basis, self.E, self.H, basis, self.E, self.H)
+
+    def calculate_confinement_factor(self, elements):
+        @Functional
+        def factor(w):
+            return np.sqrt(w["epsilon"]) * (
+                dot(np.conj(w["E"][0]), w["E"][0]) + np.conj(w["E"][1]) * w["E"][1]
+            )
+
+        basis = self.basis.with_elements(elements)
+        basis_epsilon_r = self.basis_epsilon_r.with_elements(elements)
+        return (
+            speed_of_light
+            * epsilon_0
+            * factor.assemble(
+                basis,
+                E=basis.interpolate(self.E),
+                epsilon=basis_epsilon_r.interpolate(self.epsilon_r),
+            )
+        )
+
+    def calculate_pertubated_neff(self, delta_epsilon):
+        return (
+            self.n_eff
+            + self.calculate_coupling_coefficient(self, delta_epsilon)
+            * scipy.constants.epsilon_0
+            * scipy.constants.speed_of_light
+            * 0.5
+        )
+
+    def plot(self, field, plot_vectors=False, colorbar=True, direction="y", title="E"):
+        return plot_mode(
+            self.basis,
+            field,
+            plot_vectors=plot_vectors,
+            colorbar=colorbar,
+            title=title,
+            direction=direction,
+        )
+
+    def show(self, field, **kwargs):
+        self.plot(field=field, **kwargs)
+        plt.show()
+
+
+@dataclass(frozen=True)
+class Modes:
+    modes: List
+
+    def __getitem__(self, idx) -> Mode:
+        return self.modes[idx]
+
+    def __len__(self) -> int:
+        return len(self.modes)
+
+    def __repr__(self) -> str:
+        modes = "\n\t" + "\n\t".join(repr(mode) for mode in self.modes) + "\n"
+        return f"{self.__class__.__name__}(modes=({modes}))"
+
+    def sorted(self, key):
+        return Modes(modes=sorted(self.modes, key=key))
+
+    @property
+    def n_effs(self):
+        return np.array([mode.n_eff for mode in self.modes])
+
+
 def compute_modes(
     basis_epsilon_r,
     epsilon_r,
     wavelength,
-    mu_r,
-    num_modes,
+    *,
+    mu_r=1,
+    num_modes=1,
     order=1,
     metallic_boundaries=False,
     radius=np.inf,
-    solver="scipy",
-):
+    n_guess=None,
+    solver="slepc",
+) -> Modes:
     if solver == "scipy":
         solver = solver_eigen_scipy
     elif solver == "slepc":
         from femwell.solver import solver_eigen_slepc
 
         solver = solver_eigen_slepc
     else:
@@ -53,60 +216,84 @@
         raise AssertionError("Only order 1 and 2 implemented by now.")
 
     basis = basis_epsilon_r.with_element(element)
     basis_epsilon_r = basis.with_element(basis_epsilon_r.elem)  # adjust quadrature
 
     @BilinearForm(dtype=epsilon_r.dtype)
     def aform(e_t, e_z, v_t, v_z, w):
-        epsilon = w.epsilon * (1 + w.x[0] / radius)
+        epsilon = w.epsilon * (1 + w.x[0] / radius) ** 2
 
         return (
-            1 / mu_r * curl(e_t) * curl(v_t)
-            - k0**2 * epsilon * dot(e_t, v_t)
+            1 / mu_r * curl(e_t) * curl(v_t) / k0**2
+            - epsilon * dot(e_t, v_t)
             + 1 / mu_r * dot(grad(e_z), v_t)
             + epsilon * inner(e_t, grad(v_z))
-            - epsilon * e_z * v_z
+            - epsilon * e_z * v_z * k0**2
         )
 
     @BilinearForm(dtype=epsilon_r.dtype)
     def bform(e_t, e_z, v_t, v_z, w):
-        return -1 / mu_r * dot(e_t, v_t)
+        return -1 / mu_r * dot(e_t, v_t) / k0**2
 
     A = aform.assemble(basis, epsilon=basis_epsilon_r.interpolate(epsilon_r))
     B = bform.assemble(basis, epsilon=basis_epsilon_r.interpolate(epsilon_r))
 
+    if n_guess:
+        sigma = sigma = k0**2 * n_guess**2
+    else:
+        sigma = sigma = k0**2 * np.max(epsilon_r) ** 2
+
     if metallic_boundaries:
         lams, xs = solve(
-            *condense(-A, -B, D=basis.get_dofs()),
-            solver=solver(k=num_modes, sigma=k0**2 * np.max(epsilon_r) ** 2),
+            *condense(
+                -A,
+                -B,
+                D=basis.get_dofs(None if metallic_boundaries is True else metallic_boundaries),
+                x=basis.zeros(dtype=complex),
+            ),
+            solver=solver(k=num_modes, sigma=sigma),
         )
     else:
         lams, xs = solve(
             -A,
             -B,
-            solver=solver(k=num_modes, sigma=k0**2 * np.max(epsilon_r) ** 2),
+            solver=solver(k=num_modes, sigma=sigma),
         )
 
-    idx = np.abs(np.real(lams)).argsort()[::-1]
-    lams = lams[idx]
-    xs = xs[:, idx]
-
-    xs = xs.T
-    xs[:, basis.split_indices()[1]] /= 1j * np.sqrt(
-        lams[:, np.newaxis]
+    xs[basis.split_indices()[1], :] /= 1j * np.sqrt(
+        lams[np.newaxis, :] / k0**4
     )  # undo the scaling E_3,new = beta * E_3
 
+    hs = []
     for i, lam in enumerate(lams):
-        H = calculate_hfield(basis, xs[i], np.sqrt(lam), omega=k0 * scipy.constants.speed_of_light)
-        xs[i] /= np.sqrt(calculate_overlap(basis, xs[i], H, basis, xs[i], H))
-
-    return np.sqrt(lams)[:num_modes] / k0, basis, xs[:num_modes]
+        H = calculate_hfield(
+            basis, xs[:, i], np.sqrt(lam), omega=k0 * scipy.constants.speed_of_light
+        )
+        power = calculate_overlap(basis, xs[:, i], H, basis, xs[:, i], H)
+        xs[:, i] /= np.sqrt(power)
+        H /= np.sqrt(power)
+        hs.append(H)
+
+    return Modes(
+        modes=[
+            Mode(
+                frequency=speed_of_light / wavelength,
+                k=np.sqrt(lams[i]),
+                basis_epsilon_r=basis_epsilon_r,
+                epsilon_r=epsilon_r,
+                basis=basis,
+                E=xs[:, i],
+                H=hs[i],
+            )
+            for i in range(num_modes)
+        ]
+    )
 
 
-def calculate_hfield(basis, xs, beta, omega=1):
+def calculate_hfield(basis, xs, beta, omega):
     @BilinearForm(dtype=np.complex64)
     def aform(e_t, e_z, v_t, v_z, w):
         return (
             (-1j * beta * e_t[1] + e_z.grad[1]) * v_t[0]
             + (1j * beta * e_t[0] - e_z.grad[0]) * v_t[1]
             + e_t.curl * v_z
         )
@@ -141,15 +328,15 @@
 
     b_operator = bform.assemble(basis_energy)
 
     return basis_energy, scipy.sparse.linalg.spsolve(b_operator, a_operator)
 
 
 def calculate_overlap(basis_i, E_i, H_i, basis_j, E_j, H_j):
-    @Functional
+    @Functional(dtype=np.complex64)
     def overlap(w):
         return cross(np.conj(w["E_i"][0]), w["H_j"][0]) + cross(w["E_j"][0], np.conj(w["H_i"][0]))
 
     if basis_i == basis_j:
         return 0.5 * overlap.assemble(
             basis_i,
             E_i=basis_i.interpolate(E_i),
@@ -201,44 +388,14 @@
             np.conj(w["E_i"][0]),
             np.array((ht_x_basis.interpolator(ht_x)(w.x), ht_y_basis.interpolator(ht_y)(w.x))),
         )
 
     return overlap.assemble(basis_i, E_i=basis_i.interpolate(E_i))
 
 
-def calculate_coupling_coefficient(basis_epsilon, delta_epsilon, basis, E_i, E_j):
-    @Functional
-    def overlap(w):
-        return w["delta_epsilon"] * (
-            dot(np.conj(w["E_i"][0]), w["E_j"][0]) + np.conj(w["E_i"][1]) * w["E_j"][1]
-        )
-
-    return overlap.assemble(
-        basis,
-        E_i=basis.interpolate(E_i),
-        E_j=basis.interpolate(E_j),
-        delta_epsilon=basis_epsilon.interpolate(delta_epsilon),
-    )
-
-
-def calculate_te_frac(basis, x):
-    @Functional
-    def ex(w):
-        return np.abs(w.E[0][0]) ** 2
-
-    @Functional
-    def ey(w):
-        return np.abs(w.E[0][1]) ** 2
-
-    ex_sum = ex.assemble(basis, E=basis.interpolate(x))
-    ey_sum = ey.assemble(basis, E=basis.interpolate(x))
-
-    return ex_sum / (ex_sum + ey_sum)
-
-
 def plot_mode(basis, mode, plot_vectors=False, colorbar=True, title="E", direction="y"):
     from mpl_toolkits.axes_grid1 import make_axes_locatable
 
     (et, et_basis), (ez, ez_basis) = basis.split(mode)
 
     if plot_vectors:
         rc = (2, 1) if direction != "x" else (1, 2)
@@ -281,14 +438,15 @@
         if colorbar == "same":
             plt.colorbar(axs[0].collections[-1], ax=axs.ravel().tolist())
         else:
             for ax in axs:
                 divider = make_axes_locatable(ax)
                 cax = divider.append_axes("right", size="5%", pad=0.05)
                 plt.colorbar(ax.collections[-1], cax=cax)
+            plt.tight_layout()
 
     return fig, axs
 
 
 if __name__ == "__main__":
     from collections import OrderedDict
 
@@ -333,46 +491,50 @@
         ),
     )
 
     resolutions = dict(core={"resolution": 0.05, "distance": 1})
 
     mesh_from_OrderedDict(polygons, resolutions, filename="mesh.msh", default_resolution_max=0.2)
 
-    mesh = Mesh.load("mesh.msh")
+    scale = 1e0
+    mesh = Mesh.load("mesh.msh").scaled(scale)
     basis = Basis(mesh, ElementTriN2() * ElementTriP2())
     basis0 = basis.with_element(ElementTriP0())
     epsilon = basis0.zeros(dtype=complex)
     epsilon[basis0.get_dofs(elements="core")] = 3.4777**2
     epsilon[basis0.get_dofs(elements="clad")] = 1.444**2
     epsilon[basis0.get_dofs(elements="box")] = 1.444**2
     # basis0.plot(epsilon, colorbar=True).show()
 
-    lams, basis, xs = compute_modes(
-        basis0, epsilon, wavelength=1.55, mu_r=1, num_modes=6, order=2, radius=3
+    modes = compute_modes(
+        basis0,
+        epsilon,
+        wavelength=1.55 * scale,
+        mu_r=1,
+        num_modes=6,
+        order=2,
+        radius=3 * scale,
     )
+    print(modes)
+    print(modes[0].te_fraction)
 
-    print(lams)
+    modes[0].show(np.real(modes[0].E))
+    modes[0].show(np.imag(modes[0].E))
 
-    plot_mode(basis, np.real(xs[0]))
-    plt.show()
-    plot_mode(basis, np.imag(xs[0]))
-    plt.show()
-
-    xbs = calculate_hfield(basis, xs[0], lams[0] * (2 * np.pi / 1.55))
+    modes[0].show(np.real(modes[0].H))
+    modes[0].show(np.imag(modes[0].H))
 
-    plot_mode(basis, np.real(xbs))
-    plt.show()
-    plot_mode(basis, np.imag(xbs))
-    plt.show()
+    integrals = np.zeros((len(modes),) * 2, dtype=complex)
 
-    integrals = np.zeros((len(lams),) * 2, dtype=complex)
-    for i in range(len(lams)):
-        for j in range(len(lams)):
-            E_i = xs[i]
-            E_j = xs[j]
-            H_i = calculate_hfield(basis, E_i, lams[i] * (2 * np.pi / 1.55))
-            H_j = calculate_hfield(basis, E_j, lams[j] * (2 * np.pi / 1.55))
-            integrals[i, j] = calculate_overlap(basis, E_i, H_i, basis, E_j, H_j)
+    for i in range(len(modes)):
+        for j in range(len(modes)):
+            integrals[i, j] = modes[i].calculate_overlap(modes[j])
 
     plt.imshow(np.real(integrals))
     plt.colorbar()
     plt.show()
+
+    # Create basis to select a certain simulation extent
+    def sel_fun(x):
+        return (x[0] < 0) * (x[0] > -1) * (x[1] > 0) * (x[1] < 0.5)
+
+    print(modes.sorted(lambda mode: mode.calculate_power(elements=sel_fun)))
```

### Comparing `femwell-0.0.9/femwell/mode_solver_1d.py` & `femwell-0.1.0/femwell/mode_solver_1d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/mode_solver_2d_periodic.py` & `femwell-0.1.0/femwell/mode_solver_2d_periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # implementing https://opg.optica.org/ol/fulltext.cfm?uri=ol-40-6-1053&id=312806
 
 import numpy as np
 from skfem import Basis, BilinearForm, ElementTriP1, FacetBasis, solve
 from skfem.helpers import d, grad
-from skfem.utils import mpc
 
 from femwell.solver import solver_dense, solver_eigen_scipy_invert, solver_eigen_slepc
+from femwell.utils import mpc_symmetric
 
 
 def solve_periodic(basis_epsilon_r, epsilon_r, k0):
     fbases = [
         FacetBasis(basis_epsilon_r.mesh, ElementTriP1(), facets="left"),
         FacetBasis(basis_epsilon_r.mesh, ElementTriP1(), facets="right"),
     ]
@@ -49,15 +49,15 @@
     top = basis_vec.get_dofs(facets="top")
     bottom = basis_vec.get_dofs(facets="bottom")
 
     left = np.setdiff1d(left, top + bottom)
     right = np.setdiff1d(right, top + bottom)
 
     ks, xs = solve(
-        *mpc(A, f, M=left, S=np.concatenate((right, top, bottom))),
+        *mpc_symmetric(A, f, M=left, S=np.concatenate((right, top, bottom))),
         solver=solver_eigen_scipy_invert(
             k=20, which="LM", sigma=k0 * np.sqrt(epsilon_r.real.max())
         ),
     )
     (phis, basis_phi), (k_phis, basis_k_phi) = basis_vec.split(xs)
 
     return ks, basis_phi, phis
```

### Comparing `femwell-0.0.9/femwell/mode_solver_2d_periodic_quadratic.py` & `femwell-0.1.0/femwell/mode_solver_2d_periodic_quadratic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/mode_solver_inplane.py` & `femwell-0.1.0/femwell/mode_solver_inplane.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/solver.py` & `femwell-0.1.0/femwell/solver.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
         ks, xs = scipy.linalg.eig(A.todense(), B.todense())
 
         if kwargs["which"] == "LM":
             idx = np.abs(ks - kwargs["sigma"]).argsort()
             ks = ks[idx]
             xs = xs[:, idx]
+
+        if kwargs["which"] == "LR":
+            idx = np.real(ks - kwargs["sigma"]).argsort()
+            ks = ks[idx]
+            xs = xs[:, idx]
         return ks, xs
 
     return solver
 
 
 def solver_eigen_scipy_operator(**kwargs):
     """Solve generalized eigenproblem using SciPy (ARPACK).
@@ -133,14 +138,59 @@
             xs.append(np.array(xr) + 1j * np.array(xi))
 
         return np.array(lams), np.array(xs).T
 
     return solver
 
 
+def solver_cached(solver_orig, cache_path):
+    import hashlib
+    import json
+    import os
+
+    import scipy
+
+    def solver_generator(**kwargs):
+        def solver(*matrices):
+            hashkey = hashlib.md5(
+                matrices[0].data.tobytes()
+                + matrices[1].data.tobytes()
+                + bytes(str(kwargs), encoding="utf-8")
+            ).digest()
+            cachepath = f"{cache_path}/{hashkey}"
+            os.makedirs(f"{cachepath}", exist_ok=True)
+            folders = os.listdir(cachepath)
+
+            for folder in folders:
+                try:
+                    for i, matrix in enumerate(matrices):
+                        if (scipy.sparse.load_npz(f"{cachepath}/{folder}/{i}.npz") != matrix).nnz:
+                            break
+                    else:
+                        if np.load(f"{cachepath}/{folder}/params.npz") != kwargs:
+                            continue
+                        result = np.load(f"{cachepath}/{folder}/result.npz")
+                        return result.values()
+                except:
+                    pass
+
+            cachepath = f"{cachepath}/{len(folders)}"
+            os.makedirs(cachepath, exist_ok=True)
+            result = solver_orig(**kwargs)(*matrices)
+            for i, matrix in enumerate(matrices):
+                scipy.sparse.save_npz(f"{cachepath}/{i}.npz", matrix)
+            np.savez_compressed(f"{cachepath}/params.npz", **kwargs)
+            np.savez_compressed(f"{cachepath}/result.npz", *result)
+            return result
+
+        return solver
+
+    return solver_generator
+
+
 if __name__ == "__main__":
     import scipy.sparse
     from petsc4py import PETSc
     from slepc4py import SLEPc
 
     pep = SLEPc.PEP().create()
```

### Comparing `femwell-0.0.9/femwell/tcad.py` & `femwell-0.1.0/femwell/tcad.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/tests/test_mesh.py` & `femwell-0.1.0/femwell/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.0.9/femwell/thermal.py` & `femwell-0.1.0/femwell/thermal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Dict
 
 import numpy as np
 from skfem import (
     Basis,
     BilinearForm,
-    ElementTetP0,
     ElementTetP1,
+    ElementTetP2,
+    ElementTriP0,
     ElementTriP1,
+    ElementTriP2,
+    ElementTriP3,
     LinearForm,
     Mesh,
     asm,
     condense,
     solve,
 )
 from skfem.helpers import dot
@@ -18,33 +21,42 @@
 
 def solve_thermal(
     basis0,
     thermal_conductivity,
     specific_conductivity: Dict[str, float],
     current_densities,
     fixed_boundaries,
+    order=1,
 ):
     """Thermal simulation.
 
     Args:
         basis0: Basis of the thermal_conductivity
         thermal_conductivity: thermal conductivity in W/m‧K.
         specific_conductivity: specific conductivity in S/m.
         current_densities: current densities flowing through the layer in A.
 
     Returns:
         basis, temperature profile
     """
 
+    if order == 1:
+        element = ElementTriP1() if basis0.mesh.dim() == 2 else ElementTetP1()
+    elif order == 2:
+        element = ElementTriP2() if basis0.mesh.dim() == 2 else ElementTetP2()
+    elif order == 3:
+        if basis0.mesh.dim() == 2:
+            element = ElementTriP3()
+        else:
+            raise NotImplementedError()
+
     @BilinearForm
     def conduction(u, v, w):
         return dot(w["thermal_conductivity"] * u.grad, v.grad)
 
-    element = ElementTriP1() if basis0.mesh.dim() == 2 else ElementTetP1()
-
     basis = basis0.with_element(element)
 
     @LinearForm
     def unit_load(v, _):
         return v
 
     joule_heating_rhs = basis.zeros()
@@ -140,23 +152,22 @@
         box={"resolution": 0.4, "distance": 1},
         heater={"resolution": 0.05, "distance": 1},
     )
 
     mesh_from_OrderedDict(polygons, resolutions, filename="mesh.msh", default_resolution_max=0.4)
 
     mesh = Mesh.load("mesh.msh")
-    print(mesh.boundaries)
 
     currents = np.linspace(0.007, 10e-3, 10) / polygons["heater"].area
     neffs = []
 
     from tqdm.auto import tqdm
 
     for current in tqdm(currents):
-        basis0 = Basis(mesh, ElementTetP0(), intorder=4)
+        basis0 = Basis(mesh, ElementTriP0(), intorder=4)
         thermal_conductivity_p0 = basis0.zeros()
         for domain, value in {
             "core": 148,
             "box": 1.38,
             "clad": 1.38,
             "heater": 28,
         }.items():
@@ -169,30 +180,27 @@
             specific_conductivity={"heater": 2.3e6},
             current_densities={"heater": current},
             fixed_boundaries={"bottom": 0},
         )
         # basis.plot(temperature, colorbar=True)
         # plt.show()
 
-        from femwell.mode_solver import compute_modes, plot_mode
+        from femwell.maxwell.waveguide import compute_modes
 
         temperature0 = basis0.project(basis.interpolate(temperature))
         epsilon = basis0.zeros() + (1.444 + 1.00e-5 * temperature0) ** 2
         epsilon[basis0.get_dofs(elements="core")] = (
             3.4777 + 1.86e-4 * temperature0[basis0.get_dofs(elements="core")]
         ) ** 2
         # basis0.plot(epsilon, colorbar=True).show()
 
-        lams, basis, xs = compute_modes(basis0, epsilon, wavelength=1.55, mu_r=1, num_modes=5)
+        modes = compute_modes(basis0, epsilon, wavelength=1.55, num_modes=5)
 
-        print(lams)
-
-        # plot_mode(basis, xs[0])
-        # plt.show()
+        # modes[0].show(modes[0].E)
 
-        neffs.append(np.real(lams[0]))
+        neffs.append(np.real(modes[0].n_eff))
 
     print(f"Phase shift: {2 * np.pi / 1.55 * (neffs[-1] - neffs[0]) * 320}")
     plt.xlabel("Power")
     plt.ylabel("$n_{eff}$")
     plt.plot(currents, neffs)
     plt.show()
```

### Comparing `femwell-0.0.9/femwell/thermal_transient.py` & `femwell-0.1.0/femwell/thermal_transient.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 
 
 def solve_thermal_transient(
     basis0,
     thermal_conductivity_p0,
     thermal_diffusivity_p0,
     specific_conductivity: Dict[str, float],
+    current_densities_0,
     current_densities,
     fixed_boundaries,
     dt,
     steps,
 ):
     basis, temperature = solve_thermal(
         basis0,
         thermal_conductivity_p0,
         specific_conductivity,
-        {domain: current(0) for domain, current in current_densities.items()},
+        {domain: current for domain, current in current_densities_0.items()},
         fixed_boundaries=fixed_boundaries,
     )
 
     @BilinearForm
     def diffusivity_laplace(u, v, w):
         return w["thermal_conductivity"] * dot(u.grad, v.grad)
 
@@ -49,19 +50,19 @@
     )
 
     theta = 0.5  # Crank–Nicolson
 
     x = basis.zeros()
     for key, value in fixed_boundaries.items():
         x[basis.get_dofs(key)] = value
-    L0, M0 = enforce(L, M, D=basis.get_dofs(set(fixed_boundaries.keys())), x=x)
+    M0, L0 = enforce(M, L, D=basis.get_dofs(set(fixed_boundaries.keys())))
     A = M0 + theta * L0 * dt
     B = M0 - (1 - theta) * L0 * dt
 
-    backsolve = splu(A.T).solve  # .T as splu prefers CSC
+    backsolve = splu(A).solve  # .T as splu prefers CSC
 
     t = 0
     temperatures = [temperature]
     for i in range(steps):
         joule_heating_rhs = basis.zeros()
         for (
             domain,
@@ -86,14 +87,15 @@
     return basis, temperatures
 
 
 if __name__ == "__main__":
     from collections import OrderedDict
 
     import matplotlib.pyplot as plt
+    import scipy.constants
     from shapely.geometry import LineString, Polygon
     from skfem.io import from_meshio
 
     from femwell.mesh import mesh_from_OrderedDict
 
     # Simulating the TiN TOPS heater in https://doi.org/10.1364/OE.27.010456
 
@@ -103,14 +105,16 @@
     w_core = 0.5
     h_core = 0.22
     offset_heater = 2.2
     h_heater = 0.14
     w_heater = 2
     h_silicon = 3
 
+    wavelength = 1.55
+
     polygons = OrderedDict(
         bottom=LineString([(-w_sim / 2, -h_box), (w_sim / 2, -h_box)]),
         core=Polygon(
             [
                 (-w_core / 2, 0),
                 (-w_core / 2, h_core),
                 (w_core / 2, h_core),
@@ -187,14 +191,15 @@
         lambda t: 0.007 / polygons["heater"].area * ((t < dt * steps / 10) + (t > dt * steps / 2))
     )
     basis, temperatures = solve_thermal_transient(
         basis0,
         thermal_conductivity_p0,
         thermal_diffusivity_p0,
         specific_conductivity={"heater": 2.3e6},
+        current_densities_0={"heater": current(0)},
         current_densities={"heater": current},
         fixed_boundaries={"bottom": 0},
         dt=dt,
         steps=steps,
     )
 
     @LinearForm
@@ -215,37 +220,69 @@
     #         mesh.restrict(subdomain).draw(ax=ax, boundaries_only=True)
     #     basis.plot(temperatures[i], ax=ax, vmin=0, vmax=np.max(temperatures), shading='gouraud').show()
 
     # Calculate modes
 
     from tqdm.auto import tqdm
 
+    from femwell.mode_solver import (
+        calculate_coupling_coefficient,
+        compute_modes,
+        plot_mode,
+    )
+
+    epsilon_0 = basis0.zeros() + 1.444**2
+    epsilon_0[basis0.get_dofs(elements="core")] = 3.4777**2
+    lams_0, basis_modes_0, xs_0 = compute_modes(
+        basis0, epsilon_0, wavelength=wavelength, mu_r=1, num_modes=1
+    )
+
     neffs = []
+    neffs_approximated = []
     for i, temperature in enumerate(tqdm(temperatures)):
         # basis.plot(temperature, vmin=0, vmax=np.max(temperatures))
         # plt.show()
 
-        from femwell.mode_solver import compute_modes, plot_mode
-
         temperature0 = basis0.project(basis.interpolate(temperature))
         epsilon = basis0.zeros() + (1.444 + 1.00e-5 * temperature0) ** 2
         epsilon[basis0.get_dofs(elements="core")] = (
             3.4777 + 1.86e-4 * temperature0[basis0.get_dofs(elements="core")]
         ) ** 2
         # basis0.plot(epsilon, colorbar=True).show()
 
-        lams, basis_modes, xs = compute_modes(basis0, epsilon, wavelength=1.55, mu_r=1, num_modes=1)
+        lams, basis_modes, xs = compute_modes(basis0, epsilon, wavelength=wavelength, num_modes=1)
 
         # plot_mode(basis_modes, xs[0])
         # plt.show()
 
         neffs.append(np.real(lams[0]))
+        neffs_approximated.append(
+            np.real(
+                lams_0[0]
+                + calculate_coupling_coefficient(
+                    basis0,
+                    (epsilon - epsilon_0) * scipy.constants.epsilon_0,
+                    basis_modes_0,
+                    xs_0[0],
+                    xs_0[0],
+                )
+                * scipy.constants.speed_of_light
+                * 2e-3
+            )
+        )
 
     fig = plt.figure()
     ax = fig.add_subplot(111)
     ax.set_xlabel("Time [us]")
     ax.set_ylabel("Current [mA]")
     ax.plot(times * 1e6, current(times), "b-o")
     ax2 = ax.twinx()
     ax2.set_ylabel("Phase shift")
-    ax2.plot(times * 1e6, 2 * np.pi / 1.55 * (neffs - neffs[0]) * 320, "r-o")
+    ax2.plot(times * 1e6, 2 * np.pi / 1.55 * (neffs - lams_0[0]) * 320, "r-o", label="Exact")
+    ax2.plot(
+        times * 1e6,
+        2 * np.pi / 1.55 * (neffs_approximated - lams_0[0]) * 320,
+        "g-o",
+        label="Approximation",
+    )
+    plt.legend()
     plt.show()
```

### Comparing `femwell-0.0.9/femwell/waveguide.py` & `femwell-0.1.0/femwell/waveguide.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import skfem
 from shapely.geometry import Polygon
 from skfem import Basis, ElementTriP0, ElementVector, Mesh
 from skfem.io.meshio import from_meshio
 
+from femwell.maxwell.waveguide import compute_modes
 from femwell.mesh import mesh_from_OrderedDict
-from femwell.mode_solver import compute_modes, plot_mode
 
 
 def mesh_waveguide(filename, wsim, hclad, hbox, wcore, hcore):
     polygons = OrderedDict(
         core=Polygon(
             [
                 (-wcore / 2, -hcore / 2),
@@ -62,11 +62,10 @@
     basis0 = Basis(mesh, ElementTriP0(), intorder=4)
     epsilon = basis0.zeros()
     epsilon[basis0.get_dofs(elements="core")] = 3.4777**2
     epsilon[basis0.get_dofs(elements="clad")] = 1.444**2
     epsilon[basis0.get_dofs(elements="box")] = 1.444**2
     basis0.plot(epsilon, colorbar=True).show()
 
-    lams, basis, xs = compute_modes(basis0, epsilon, wavelength=1.55, mu_r=1, num_modes=5)
+    modes = compute_modes(basis0, epsilon, wavelength=1.55, mu_r=1, num_modes=5)
 
-    fig, axs = plot_mode(basis, xs[0], colorbar=False)
-    plt.show()
+    modes[0].show(modes[0].E.real)
```

### Comparing `femwell-0.0.9/pyproject.toml` & `femwell-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "femwell"
-version = "0.0.9"
+version = "0.1.0"
 authors = ["Helge Gehring"]
 description = "Mode solver for photonic and electric waveguides based on FEM"
 homepage = "https://github.com/HelgeGehring/femwell"
 keywords = [
     "integrated photonics",
     "silicon photonics",
     "mode solving",
@@ -15,27 +15,31 @@
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering"
 ]
 license = "GPLv3"
 readme = "README.md"
 
+[tool.poetry.urls]
+Documentation = "https://HelgeGehring.github.io/femwell/"
+
 [tool.poetry.dependencies]
 python = ">=3.8"
 scikit-fem = ">=8.0.0"
 gmsh = "*"
 pygmsh = "*"
 matplotlib = "*"
 shapely = ">=2.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 flake8 = "*"
 
 [tool.poetry.group.docs.dependencies]
 tqdm = "*"
-sphinx-book-theme = "*"
+# sphinx-book-theme = "*"
 jupytext = "*"
-myst-parser = "*"
+# myst-parser = "*"
+pandas = "*"
 
 [tool.black]
 line-length = 100
```

### Comparing `femwell-0.0.9/PKG-INFO` & `femwell-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femwell
-Version: 0.0.9
+Version: 0.1.0
 Summary: Mode solver for photonic and electric waveguides based on FEM
 Home-page: https://github.com/HelgeGehring/femwell
 License: GPLv3
 Keywords: integrated photonics,silicon photonics,mode solving,finite element analysis
 Author: Helge Gehring
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
@@ -18,53 +18,70 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: gmsh
 Requires-Dist: matplotlib
 Requires-Dist: pygmsh
 Requires-Dist: scikit-fem (>=8.0.0)
 Requires-Dist: shapely (>=2.0.0)
+Project-URL: Documentation, https://HelgeGehring.github.io/femwell/
 Description-Content-Type: text/markdown
 
 # Femwell
 
 ![logo](https://raw.githubusercontent.com/HelgeGehring/femwell/main/logo_inline.svg)
 
 [![Docs](https://github.com/helgegehring/femwell/actions/workflows/docs.yml/badge.svg)](https://HelgeGehring.github.io/femwell/)
 [![Build](https://github.com/helgegehring/femwell/actions/workflows/build.yml/badge.svg)](https://github.com/HelgeGehring/femwell/actions/workflows/build.yml)
 [![PiPy](https://img.shields.io/pypi/v/femwell)](https://pypi.org/project/femwell/)
 [![Downloads](https://static.pepy.tech/badge/femwell/month)](https://pepy.tech/project/femwell)
 
 Finite element based simulation tool for integrated circuits, electric and photonic!
-The documentation is lagging behind the state of code, so there's several features for which there are only examples in the code.
+The documentation is lagging behind the state of code,
+so there's several features for which there are only examples in the code.
 
-**You can try out the examples in the browser! Hover the rocket at the top on the example pages and click live code!**
+**You can try out the examples in the browser!**
+**Hover the rocket at the top on the example pages and click live code!**
 (Might take some time to load)
 
-# Working Features
+## Features
+
 - Photonic eigenmode solver
 - Periodic photonic eigenmode solver
 - Electric eigenmode solver
 - Thermal mode solver (static and transient)
 - Coulomb solver
 
-# Possible Simulations
+## Possible Simulations
+
 - Eigenmodes of waveguides and determining their effective refractive index
+- Coupling between neighboring waveguides
+- Eigenmodes of bent waveguides
+- Propagation loss of circular bends and mode mismatch loss with straight waveguides
+- Calculation of the group velocity and its dispersion
+- Calculation of overlap-integrals and confinement-factors
 - Bragg grating cells
 - Grating coupler cells
 - Eigenmode of a coaxial cable and its specific impedance
-- Eigenmodes of electric transmission lines and determining their propagation constant (in work)
+- Eigenmodes of electric transmission lines
+  and determining their propagation constant (in work)
 - Static thermal profiles
 - Transient thermal behavior
 - Static electric fields
 - Overlap integrals between waveguide modes
 - Overlap integral between a waveguide mode and a fiber mode
 - Coupled mode theory - coupling between adjacent waveguides
 - Heat based photonic phase shifters
 - Pockels based photonic phase shifters
+- PN junction depletion modulator (analytical)
+
+Something missing? Feel free to open an [issue](https://github.com/HelgeGehring/femwell/issues) :)
+
+## Contributors
 
-# Contributors
 - Helge Gehring (Google): Maintainer
-- Simon Bilodeau (Google): Meshes everything
+- Simon Bilodeau (Google): Meshes everything, Analytical PN model
 - Joaquin Matres (Google): Code simplifications
+- Marc de Cea Falco (Google): Documentation improvements
 
-Happy about every form of contribution - pull requests, feature requests, issues, questions, ... :)
+Happy about every form of contribution -
+pull requests, feature requests, issues, questions, ... :)
```

