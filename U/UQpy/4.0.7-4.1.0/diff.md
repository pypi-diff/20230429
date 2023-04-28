# Comparing `tmp/UQpy-4.0.7.tar.gz` & `tmp/UQpy-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UQpy-4.0.7.tar", last modified: Thu Feb 23 23:58:35 2023, max compression
+gzip compressed data, was "UQpy-4.1.0.tar", last modified: Fri Apr 28 22:56:36 2023, max compression
```

## Comparing `UQpy-4.0.7.tar` & `UQpy-4.1.0.tar`

### file list

```diff
@@ -1,321 +1,330 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.533133 UQpy-4.0.7/
--rw-r--r--   0 runner     (501) staff       (20)     1075 2023-02-23 23:18:44.000000 UQpy-4.0.7/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-02-23 23:58:35.532731 UQpy-4.0.7/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     5526 2023-02-23 23:18:44.000000 UQpy-4.0.7/README.rst
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-02-23 23:58:35.533265 UQpy-4.0.7/setup.cfg
--rwxr-xr-x   0 runner     (501) staff       (20)     1046 2023-02-23 23:18:44.000000 UQpy-4.0.7/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.366950 UQpy-4.0.7/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.395750 UQpy-4.0.7/src/UQpy/
--rw-r--r--   0 runner     (501) staff       (20)     1583 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.398711 UQpy-4.0.7/src/UQpy/dimension_reduction/
--rw-r--r--   0 runner     (501) staff       (20)      200 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.399855 UQpy-4.0.7/src/UQpy/dimension_reduction/diffusion_maps/
--rw-r--r--   0 runner     (501) staff       (20)    14135 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/diffusion_maps/DiffusionMaps.py
--rw-r--r--   0 runner     (501) staff       (20)       80 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/diffusion_maps/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.403403 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/
--rw-r--r--   0 runner     (501) staff       (20)     3926 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannInterpolation.py
--rw-r--r--   0 runner     (501) staff       (20)    12719 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannOperations.py
--rw-r--r--   0 runner     (501) staff       (20)      268 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.404951 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/projections/
--rw-r--r--   0 runner     (501) staff       (20)     3465 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/projections/SVDProjection.py
--rw-r--r--   0 runner     (501) staff       (20)      176 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/projections/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.406139 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      231 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/GrassmannProjection.py
--rw-r--r--   0 runner     (501) staff       (20)      127 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.407165 UQpy-4.0.7/src/UQpy/dimension_reduction/hosvd/
--rw-r--r--   0 runner     (501) staff       (20)     6969 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/hosvd/HigherOrderSVD.py
--rw-r--r--   0 runner     (501) staff       (20)       72 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/hosvd/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.408757 UQpy-4.0.7/src/UQpy/dimension_reduction/pod/
--rw-r--r--   0 runner     (501) staff       (20)     1206 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/pod/DirectPOD.py
--rw-r--r--   0 runner     (501) staff       (20)     1302 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/pod/SnapshotPOD.py
--rw-r--r--   0 runner     (501) staff       (20)      179 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/pod/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.410484 UQpy-4.0.7/src/UQpy/dimension_reduction/pod/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     6163 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/pod/baseclass/POD.py
--rw-r--r--   0 runner     (501) staff       (20)       56 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/dimension_reduction/pod/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.411132 UQpy-4.0.7/src/UQpy/distributions/
--rw-r--r--   0 runner     (501) staff       (20)      209 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.414974 UQpy-4.0.7/src/UQpy/distributions/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     2414 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/baseclass/Copula.py
--rw-r--r--   0 runner     (501) staff       (20)     4131 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/baseclass/Distribution.py
--rw-r--r--   0 runner     (501) staff       (20)     1326 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/baseclass/Distribution1D.py
--rw-r--r--   0 runner     (501) staff       (20)     1094 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/baseclass/DistributionContinuous1D.py
--rw-r--r--   0 runner     (501) staff       (20)      659 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/baseclass/DistributionDiscrete1D.py
--rw-r--r--   0 runner     (501) staff       (20)      680 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/baseclass/DistributionND.py
--rw-r--r--   0 runner     (501) staff       (20)      488 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.428624 UQpy-4.0.7/src/UQpy/distributions/collection/
--rw-r--r--   0 runner     (501) staff       (20)      822 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Beta.py
--rw-r--r--   0 runner     (501) staff       (20)      701 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Binomial.py
--rw-r--r--   0 runner     (501) staff       (20)      566 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Cauchy.py
--rw-r--r--   0 runner     (501) staff       (20)      740 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/ChiSquare.py
--rw-r--r--   0 runner     (501) staff       (20)      570 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Exponential.py
--rw-r--r--   0 runner     (501) staff       (20)      683 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Gamma.py
--rw-r--r--   0 runner     (501) staff       (20)      701 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/GeneralizedExtreme.py
--rw-r--r--   0 runner     (501) staff       (20)      710 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/InverseGaussian.py
--rw-r--r--   0 runner     (501) staff       (20)     6418 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/JointCopula.py
--rw-r--r--   0 runner     (501) staff       (20)     7362 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/JointIndependent.py
--rw-r--r--   0 runner     (501) staff       (20)      568 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Laplace.py
--rw-r--r--   0 runner     (501) staff       (20)      562 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Levy.py
--rw-r--r--   0 runner     (501) staff       (20)      570 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Logistic.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Lognormal.py
--rw-r--r--   0 runner     (501) staff       (20)      568 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Maxwell.py
--rw-r--r--   0 runner     (501) staff       (20)     1980 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Multinomial.py
--rw-r--r--   0 runner     (501) staff       (20)     2618 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/MultivariateNormal.py
--rw-r--r--   0 runner     (501) staff       (20)      562 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Normal.py
--rw-r--r--   0 runner     (501) staff       (20)      684 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Pareto.py
--rw-r--r--   0 runner     (501) staff       (20)      529 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Poisson.py
--rw-r--r--   0 runner     (501) staff       (20)      569 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Rayleigh.py
--rw-r--r--   0 runner     (501) staff       (20)      826 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/TruncatedNormal.py
--rw-r--r--   0 runner     (501) staff       (20)      550 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/Uniform.py
--rw-r--r--   0 runner     (501) staff       (20)     1469 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/collection/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.430730 UQpy-4.0.7/src/UQpy/distributions/copulas/
--rw-r--r--   0 runner     (501) staff       (20)     1527 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/copulas/Clayton.py
--rw-r--r--   0 runner     (501) staff       (20)     1583 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/copulas/Frank.py
--rw-r--r--   0 runner     (501) staff       (20)     2939 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/copulas/Gumbel.py
--rw-r--r--   0 runner     (501) staff       (20)      159 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/distributions/copulas/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.433311 UQpy-4.0.7/src/UQpy/inference/
--rw-r--r--   0 runner     (501) staff       (20)     7270 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/BayesModelSelection.py
--rw-r--r--   0 runner     (501) staff       (20)     5220 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/BayesParameterEstimation.py
--rw-r--r--   0 runner     (501) staff       (20)     7269 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/InformationModelSelection.py
--rw-r--r--   0 runner     (501) staff       (20)     8194 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/MLE.py
--rw-r--r--   0 runner     (501) staff       (20)      593 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.434364 UQpy-4.0.7/src/UQpy/inference/evidence_methods/
--rw-r--r--   0 runner     (501) staff       (20)      527 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/evidence_methods/HarmonicMean.py
--rw-r--r--   0 runner     (501) staff       (20)      126 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/evidence_methods/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.435550 UQpy-4.0.7/src/UQpy/inference/evidence_methods/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      908 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/evidence_methods/baseclass/EvidenceMethod.py
--rw-r--r--   0 runner     (501) staff       (20)       84 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/evidence_methods/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.437763 UQpy-4.0.7/src/UQpy/inference/inference_models/
--rw-r--r--   0 runner     (501) staff       (20)     4003 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/inference_models/ComputationalModel.py
--rw-r--r--   0 runner     (501) staff       (20)     2903 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/inference_models/DistributionModel.py
--rw-r--r--   0 runner     (501) staff       (20)     1301 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/inference_models/LogLikelihoodModel.py
--rw-r--r--   0 runner     (501) staff       (20)      302 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/inference_models/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.439226 UQpy-4.0.7/src/UQpy/inference/inference_models/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     3496 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/inference_models/baseclass/InferenceModel.py
--rw-r--r--   0 runner     (501) staff       (20)       84 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/inference_models/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.441625 UQpy-4.0.7/src/UQpy/inference/information_criteria/
--rw-r--r--   0 runner     (501) staff       (20)      883 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/information_criteria/AIC.py
--rw-r--r--   0 runner     (501) staff       (20)     1004 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/information_criteria/AICc.py
--rw-r--r--   0 runner     (501) staff       (20)      959 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/information_criteria/BIC.py
--rw-r--r--   0 runner     (501) staff       (20)      230 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/information_criteria/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.442625 UQpy-4.0.7/src/UQpy/inference/information_criteria/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      649 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/information_criteria/baseclass/InformationCriterion.py
--rw-r--r--   0 runner     (501) staff       (20)      100 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/inference/information_criteria/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.443844 UQpy-4.0.7/src/UQpy/reliability/
--rw-r--r--   0 runner     (501) staff       (20)    13794 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/reliability/SubsetSimulation.py
--rw-r--r--   0 runner     (501) staff       (20)      136 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/reliability/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.445506 UQpy-4.0.7/src/UQpy/reliability/taylor_series/
--rw-r--r--   0 runner     (501) staff       (20)    16596 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/reliability/taylor_series/FORM.py
--rw-r--r--   0 runner     (501) staff       (20)     6843 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/reliability/taylor_series/SORM.py
--rw-r--r--   0 runner     (501) staff       (20)      185 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/reliability/taylor_series/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.446627 UQpy-4.0.7/src/UQpy/reliability/taylor_series/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     6400 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py
--rw-r--r--   0 runner     (501) staff       (20)       68 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/reliability/taylor_series/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.447916 UQpy-4.0.7/src/UQpy/run_model/
--rwxr-xr-x   0 runner     (501) staff       (20)    10530 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/run_model/RunModel.py
--rw-r--r--   0 runner     (501) staff       (20)       91 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/run_model/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.450976 UQpy-4.0.7/src/UQpy/run_model/model_execution/
--rw-r--r--   0 runner     (501) staff       (20)     2632 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/run_model/model_execution/ParallelExecution.py
--rw-r--r--   0 runner     (501) staff       (20)     6848 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/run_model/model_execution/PythonModel.py
--rw-r--r--   0 runner     (501) staff       (20)      650 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/run_model/model_execution/SerialExecution.py
--rw-r--r--   0 runner     (501) staff       (20)    23075 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/run_model/model_execution/ThirdPartyModel.py
--rw-r--r--   0 runner     (501) staff       (20)      244 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/run_model/model_execution/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.454080 UQpy-4.0.7/src/UQpy/sampling/
--rw-r--r--   0 runner     (501) staff       (20)    11872 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/AdaptiveKriging.py
--rw-r--r--   0 runner     (501) staff       (20)     8359 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/ImportanceSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     9204 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/MonteCarloSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     3835 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/SimplexSampling.py
--rw-r--r--   0 runner     (501) staff       (20)      382 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.457390 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/
--rw-r--r--   0 runner     (501) staff       (20)     1908 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py
--rw-r--r--   0 runner     (501) staff       (20)     1330 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py
--rw-r--r--   0 runner     (501) staff       (20)     1535 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py
--rw-r--r--   0 runner     (501) staff       (20)     1062 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/UFunction.py
--rw-r--r--   0 runner     (501) staff       (20)     1627 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py
--rw-r--r--   0 runner     (501) staff       (20)      437 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.458580 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      717 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/baseclass/LearningFunction.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.462204 UQpy-4.0.7/src/UQpy/sampling/mcmc/
--rw-r--r--   0 runner     (501) staff       (20)    14747 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/mcmc/DRAM.py
--rw-r--r--   0 runner     (501) staff       (20)    13883 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/mcmc/DREAM.py
--rw-r--r--   0 runner     (501) staff       (20)     7813 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/mcmc/MetropolisHastings.py
--rw-r--r--   0 runner     (501) staff       (20)    12556 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py
--rw-r--r--   0 runner     (501) staff       (20)     8369 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/mcmc/Stretch.py
--rw-r--r--   0 runner     (501) staff       (20)      336 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/mcmc/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.463482 UQpy-4.0.7/src/UQpy/sampling/mcmc/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)    18314 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/mcmc/baseclass/MCMC.py
--rw-r--r--   0 runner     (501) staff       (20)       51 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/mcmc/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.465609 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/
--rw-r--r--   0 runner     (501) staff       (20)     5475 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     4839 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py
--rw-r--r--   0 runner     (501) staff       (20)     8527 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py
--rw-r--r--   0 runner     (501) staff       (20)      530 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.466781 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)       62 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/baseclass/StratifiedSampling.py
--rw-r--r--   0 runner     (501) staff       (20)       94 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.469954 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py
--rw-r--r--   0 runner     (501) staff       (20)     2125 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MaxiMin.py
--rw-r--r--   0 runner     (501) staff       (20)     1587 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MinCorrelation.py
--rw-r--r--   0 runner     (501) staff       (20)      933 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Random.py
--rw-r--r--   0 runner     (501) staff       (20)      588 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.471057 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     1069 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/Criterion.py
--rw-r--r--   0 runner     (501) staff       (20)       93 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.472682 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/
--rw-r--r--   0 runner     (501) staff       (20)     5703 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/GradientEnhancedRefinement.py
--rw-r--r--   0 runner     (501) staff       (20)     1648 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/RandomRefinement.py
--rw-r--r--   0 runner     (501) staff       (20)      231 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.473695 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     2517 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/baseclass/Refinement.py
--rw-r--r--   0 runner     (501) staff       (20)       80 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.476477 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/
--rw-r--r--   0 runner     (501) staff       (20)     4785 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/DelaunayStrata.py
--rw-r--r--   0 runner     (501) staff       (20)    12238 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/RectangularStrata.py
--rw-r--r--   0 runner     (501) staff       (20)       87 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/SamplingCriterion.py
--rw-r--r--   0 runner     (501) staff       (20)    19271 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/VoronoiStrata.py
--rw-r--r--   0 runner     (501) staff       (20)      407 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.477410 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     3383 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/baseclass/Strata.py
--rw-r--r--   0 runner     (501) staff       (20)       77 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.481922 UQpy-4.0.7/src/UQpy/sensitivity/
--rw-r--r--   0 runner     (501) staff       (20)    15373 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/ChatterjeeSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)    10943 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/CramerVonMisesSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)    14008 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/GeneralisedSobolSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)    12705 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/MorrisSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)     5812 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/PceSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)     9026 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/PostProcess.py
--rw-r--r--   0 runner     (501) staff       (20)    33267 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/SobolSensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)      637 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.483476 UQpy-4.0.7/src/UQpy/sensitivity/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     2577 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/baseclass/PickFreeze.py
--rw-r--r--   0 runner     (501) staff       (20)     9919 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/baseclass/Sensitivity.py
--rw-r--r--   0 runner     (501) staff       (20)      105 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/sensitivity/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.487391 UQpy-4.0.7/src/UQpy/stochastic_process/
--rw-r--r--   0 runner     (501) staff       (20)    12136 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/BispectralRepresentation.py
--rw-r--r--   0 runner     (501) staff       (20)     7111 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/InverseTranslation.py
--rw-r--r--   0 runner     (501) staff       (20)     5317 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/KarhunenLoeveExpansion.py
--rw-r--r--   0 runner     (501) staff       (20)     6802 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/KarhunenLoeveExpansion2D.py
--rw-r--r--   0 runner     (501) staff       (20)     9744 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/SpectralRepresentation.py
--rw-r--r--   0 runner     (501) staff       (20)     7111 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/Translation.py
--rw-r--r--   0 runner     (501) staff       (20)      523 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.489396 UQpy-4.0.7/src/UQpy/stochastic_process/supportive/
--rw-r--r--   0 runner     (501) staff       (20)      378 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/supportive/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1159 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/supportive/inverse_wiener_khinchin_transform.py
--rw-r--r--   0 runner     (501) staff       (20)      579 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/supportive/scaling_correlation_function.py
--rw-r--r--   0 runner     (501) staff       (20)     1087 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/stochastic_process/supportive/wiener_khinchin_transform.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.489874 UQpy-4.0.7/src/UQpy/surrogates/
--rw-r--r--   0 runner     (501) staff       (20)      290 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.490874 UQpy-4.0.7/src/UQpy/surrogates/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      212 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/baseclass/Surrogate.py
--rw-r--r--   0 runner     (501) staff       (20)       58 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.491893 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/
--rwxr-xr-x   0 runner     (501) staff       (20)    16575 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      277 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.492920 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/constraints/
--rw-r--r--   0 runner     (501) staff       (20)     2363 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py
--rw-r--r--   0 runner     (501) staff       (20)      150 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/constraints/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.493853 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/constraints/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      708 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py
--rw-r--r--   0 runner     (501) staff       (20)       94 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/constraints/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.495301 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/
--rw-r--r--   0 runner     (501) staff       (20)     1279 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/Matern.py
--rw-r--r--   0 runner     (501) staff       (20)      612 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/RBF.py
--rw-r--r--   0 runner     (501) staff       (20)      193 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.496248 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     2135 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/baseclass/Kernel.py
--rw-r--r--   0 runner     (501) staff       (20)       77 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.498245 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/
--rw-r--r--   0 runner     (501) staff       (20)      305 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/ConstantRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      487 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/LinearRegression.py
--rw-r--r--   0 runner     (501) staff       (20)     1323 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      376 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.499225 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      385 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/Regression.py
--rw-r--r--   0 runner     (501) staff       (20)       95 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.500162 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/
--rw-r--r--   0 runner     (501) staff       (20)    12979 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py
--rw-r--r--   0 runner     (501) staff       (20)      584 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.503715 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/
--rw-r--r--   0 runner     (501) staff       (20)     2608 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/Hermite.py
--rw-r--r--   0 runner     (501) staff       (20)     1528 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/HyperbolicBasis.py
--rw-r--r--   0 runner     (501) staff       (20)     3300 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/Legendre.py
--rw-r--r--   0 runner     (501) staff       (20)     1868 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/PolynomialsND.py
--rw-r--r--   0 runner     (501) staff       (20)     1252 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/TensorProductBasis.py
--rw-r--r--   0 runner     (501) staff       (20)     1599 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/TotalDegreeBasis.py
--rw-r--r--   0 runner     (501) staff       (20)      580 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.505209 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     5969 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/PolynomialBasis.py
--rw-r--r--   0 runner     (501) staff       (20)     3856 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/Polynomials.py
--rw-r--r--   0 runner     (501) staff       (20)      190 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.507665 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/
--rw-r--r--   0 runner     (501) staff       (20)     3015 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/LassoRegression.py
--rw-r--r--   0 runner     (501) staff       (20)     5634 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/LeastAngleRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      951 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/LeastSquareRegression.py
--rw-r--r--   0 runner     (501) staff       (20)     2687 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/RidgeRegression.py
--rw-r--r--   0 runner     (501) staff       (20)      378 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.508620 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)      229 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/Regression.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.509693 UQpy-4.0.7/src/UQpy/surrogates/stochastic_reduced_order_models/
--rw-r--r--   0 runner     (501) staff       (20)    17080 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/stochastic_reduced_order_models/SROM.py
--rw-r--r--   0 runner     (501) staff       (20)       23 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/surrogates/stochastic_reduced_order_models/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.511798 UQpy-4.0.7/src/UQpy/transformations/
--rw-r--r--   0 runner     (501) staff       (20)      988 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/transformations/Correlate.py
--rw-r--r--   0 runner     (501) staff       (20)     1027 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/transformations/Decorrelate.py
--rw-r--r--   0 runner     (501) staff       (20)    20420 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/transformations/Nataf.py
--rw-r--r--   0 runner     (501) staff       (20)       95 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/transformations/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.516544 UQpy-4.0.7/src/UQpy/utilities/
--rw-r--r--   0 runner     (501) staff       (20)       84 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/Constants.py
--rw-r--r--   0 runner     (501) staff       (20)      429 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/DistanceMetric.py
--rw-r--r--   0 runner     (501) staff       (20)     1324 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/FminCobyla.py
--rw-r--r--   0 runner     (501) staff       (20)      563 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/GrassmannPoint.py
--rw-r--r--   0 runner     (501) staff       (20)     1920 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/MinimizeOptimizer.py
--rw-r--r--   0 runner     (501) staff       (20)      772 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/NoPublicConstructor.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/UQpyLoggingFormatter.py
--rwxr-xr-x   0 runner     (501) staff       (20)    11339 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/Utilities.py
--rw-r--r--   0 runner     (501) staff       (20)      826 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/ValidationTypes.py
--rw-r--r--   0 runner     (501) staff       (20)      399 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.517014 UQpy-4.0.7/src/UQpy/utilities/distances/
--rw-r--r--   0 runner     (501) staff       (20)      170 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.518947 UQpy-4.0.7/src/UQpy/utilities/distances/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     1244 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/baseclass/Distance.py
--rw-r--r--   0 runner     (501) staff       (20)     1270 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/baseclass/EuclideanDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     2053 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/baseclass/GrassmannianDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      237 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.523437 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/
--rw-r--r--   0 runner     (501) staff       (20)      642 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/BrayCurtisDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      618 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/CanberraDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      620 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/ChebyshevDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      634 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/CityBlockDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      626 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/CorrelationDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      612 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/CosineDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      590 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/L2Distance.py
--rw-r--r--   0 runner     (501) staff       (20)      767 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/MinkowskiDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.527960 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/
--rw-r--r--   0 runner     (501) staff       (20)      954 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/AsimovDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      979 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/BinetCauchyDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      991 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     1085 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     1128 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     1068 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py
--rw-r--r--   0 runner     (501) staff       (20)     1037 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      932 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py
--rw-r--r--   0 runner     (501) staff       (20)      764 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.530092 UQpy-4.0.7/src/UQpy/utilities/kernels/
--rw-r--r--   0 runner     (501) staff       (20)      772 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/kernels/BinetCauchyKernel.py
--rw-r--r--   0 runner     (501) staff       (20)     2939 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/kernels/GaussianKernel.py
--rw-r--r--   0 runner     (501) staff       (20)      785 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/kernels/ProjectionKernel.py
--rw-r--r--   0 runner     (501) staff       (20)      254 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/kernels/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.532118 UQpy-4.0.7/src/UQpy/utilities/kernels/baseclass/
--rw-r--r--   0 runner     (501) staff       (20)     1255 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/kernels/baseclass/EuclideanKernel.py
--rw-r--r--   0 runner     (501) staff       (20)     1592 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/kernels/baseclass/GrassmannianKernel.py
--rw-r--r--   0 runner     (501) staff       (20)     2090 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/kernels/baseclass/Kernel.py
--rw-r--r--   0 runner     (501) staff       (20)      219 2023-02-23 23:18:44.000000 UQpy-4.0.7/src/UQpy/utilities/kernels/baseclass/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-02-23 23:58:35.398230 UQpy-4.0.7/src/UQpy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      677 2023-02-23 23:58:35.000000 UQpy-4.0.7/src/UQpy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    13607 2023-02-23 23:58:35.000000 UQpy-4.0.7/src/UQpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-02-23 23:58:35.000000 UQpy-4.0.7/src/UQpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       57 2023-02-23 23:58:35.000000 UQpy-4.0.7/src/UQpy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        5 2023-02-23 23:58:35.000000 UQpy-4.0.7/src/UQpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.952403 UQpy-4.1.0/
+-rw-r--r--   0 runner     (501) staff       (20)     1075 2023-04-28 22:03:53.000000 UQpy-4.1.0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-28 22:56:36.952019 UQpy-4.1.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     5526 2023-04-28 22:03:53.000000 UQpy-4.1.0/README.rst
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-28 22:56:36.952514 UQpy-4.1.0/setup.cfg
+-rwxr-xr-x   0 runner     (501) staff       (20)     1046 2023-04-28 22:03:54.000000 UQpy-4.1.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.753139 UQpy-4.1.0/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.770341 UQpy-4.1.0/src/UQpy/
+-rw-r--r--   0 runner     (501) staff       (20)     1583 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.773424 UQpy-4.1.0/src/UQpy/dimension_reduction/
+-rw-r--r--   0 runner     (501) staff       (20)      200 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.774475 UQpy-4.1.0/src/UQpy/dimension_reduction/diffusion_maps/
+-rw-r--r--   0 runner     (501) staff       (20)    14135 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/diffusion_maps/DiffusionMaps.py
+-rw-r--r--   0 runner     (501) staff       (20)       80 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/diffusion_maps/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.775867 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/
+-rw-r--r--   0 runner     (501) staff       (20)     3926 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannInterpolation.py
+-rw-r--r--   0 runner     (501) staff       (20)    12719 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannOperations.py
+-rw-r--r--   0 runner     (501) staff       (20)      268 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.776931 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/
+-rw-r--r--   0 runner     (501) staff       (20)     3465 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/SVDProjection.py
+-rw-r--r--   0 runner     (501) staff       (20)      176 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.777995 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      231 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/GrassmannProjection.py
+-rw-r--r--   0 runner     (501) staff       (20)      127 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.779024 UQpy-4.1.0/src/UQpy/dimension_reduction/hosvd/
+-rw-r--r--   0 runner     (501) staff       (20)     6969 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/hosvd/HigherOrderSVD.py
+-rw-r--r--   0 runner     (501) staff       (20)       72 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/hosvd/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.780313 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/
+-rw-r--r--   0 runner     (501) staff       (20)     1206 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/DirectPOD.py
+-rw-r--r--   0 runner     (501) staff       (20)     1302 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/SnapshotPOD.py
+-rw-r--r--   0 runner     (501) staff       (20)      179 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.781191 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     6163 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/baseclass/POD.py
+-rw-r--r--   0 runner     (501) staff       (20)       56 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/dimension_reduction/pod/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.781611 UQpy-4.1.0/src/UQpy/distributions/
+-rw-r--r--   0 runner     (501) staff       (20)      209 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.785452 UQpy-4.1.0/src/UQpy/distributions/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     2414 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/Copula.py
+-rw-r--r--   0 runner     (501) staff       (20)     4131 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/Distribution.py
+-rw-r--r--   0 runner     (501) staff       (20)     1326 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/Distribution1D.py
+-rw-r--r--   0 runner     (501) staff       (20)     1094 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionContinuous1D.py
+-rw-r--r--   0 runner     (501) staff       (20)      659 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionDiscrete1D.py
+-rw-r--r--   0 runner     (501) staff       (20)      680 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionND.py
+-rw-r--r--   0 runner     (501) staff       (20)      488 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.834528 UQpy-4.1.0/src/UQpy/distributions/collection/
+-rw-r--r--   0 runner     (501) staff       (20)      822 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Beta.py
+-rw-r--r--   0 runner     (501) staff       (20)      701 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Binomial.py
+-rw-r--r--   0 runner     (501) staff       (20)      566 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Cauchy.py
+-rw-r--r--   0 runner     (501) staff       (20)      740 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/ChiSquare.py
+-rw-r--r--   0 runner     (501) staff       (20)      570 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Exponential.py
+-rw-r--r--   0 runner     (501) staff       (20)      683 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Gamma.py
+-rw-r--r--   0 runner     (501) staff       (20)      701 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/GeneralizedExtreme.py
+-rw-r--r--   0 runner     (501) staff       (20)      710 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/InverseGaussian.py
+-rw-r--r--   0 runner     (501) staff       (20)     6418 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/JointCopula.py
+-rw-r--r--   0 runner     (501) staff       (20)     7362 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/JointIndependent.py
+-rw-r--r--   0 runner     (501) staff       (20)      568 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Laplace.py
+-rw-r--r--   0 runner     (501) staff       (20)      562 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Levy.py
+-rw-r--r--   0 runner     (501) staff       (20)      570 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Logistic.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Lognormal.py
+-rw-r--r--   0 runner     (501) staff       (20)      568 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Maxwell.py
+-rw-r--r--   0 runner     (501) staff       (20)     1980 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Multinomial.py
+-rw-r--r--   0 runner     (501) staff       (20)     2618 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/MultivariateNormal.py
+-rw-r--r--   0 runner     (501) staff       (20)      562 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Normal.py
+-rw-r--r--   0 runner     (501) staff       (20)      684 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Pareto.py
+-rw-r--r--   0 runner     (501) staff       (20)      529 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Poisson.py
+-rw-r--r--   0 runner     (501) staff       (20)      569 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Rayleigh.py
+-rw-r--r--   0 runner     (501) staff       (20)      826 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/TruncatedNormal.py
+-rw-r--r--   0 runner     (501) staff       (20)      550 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/Uniform.py
+-rw-r--r--   0 runner     (501) staff       (20)     1469 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/collection/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.836303 UQpy-4.1.0/src/UQpy/distributions/copulas/
+-rw-r--r--   0 runner     (501) staff       (20)     1527 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/copulas/Clayton.py
+-rw-r--r--   0 runner     (501) staff       (20)     1583 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/copulas/Frank.py
+-rw-r--r--   0 runner     (501) staff       (20)     2939 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/copulas/Gumbel.py
+-rw-r--r--   0 runner     (501) staff       (20)      159 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/distributions/copulas/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.838656 UQpy-4.1.0/src/UQpy/inference/
+-rw-r--r--   0 runner     (501) staff       (20)     7270 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/BayesModelSelection.py
+-rw-r--r--   0 runner     (501) staff       (20)     5220 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/BayesParameterEstimation.py
+-rw-r--r--   0 runner     (501) staff       (20)     7269 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/InformationModelSelection.py
+-rw-r--r--   0 runner     (501) staff       (20)     8194 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/MLE.py
+-rw-r--r--   0 runner     (501) staff       (20)      593 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.839702 UQpy-4.1.0/src/UQpy/inference/evidence_methods/
+-rw-r--r--   0 runner     (501) staff       (20)      527 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/evidence_methods/HarmonicMean.py
+-rw-r--r--   0 runner     (501) staff       (20)      126 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/evidence_methods/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.840687 UQpy-4.1.0/src/UQpy/inference/evidence_methods/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      908 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/evidence_methods/baseclass/EvidenceMethod.py
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/evidence_methods/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.842585 UQpy-4.1.0/src/UQpy/inference/inference_models/
+-rw-r--r--   0 runner     (501) staff       (20)     4003 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/ComputationalModel.py
+-rw-r--r--   0 runner     (501) staff       (20)     2903 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/DistributionModel.py
+-rw-r--r--   0 runner     (501) staff       (20)     1301 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/LogLikelihoodModel.py
+-rw-r--r--   0 runner     (501) staff       (20)      302 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.843544 UQpy-4.1.0/src/UQpy/inference/inference_models/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/baseclass/InferenceModel.py
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/inference_models/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.845336 UQpy-4.1.0/src/UQpy/inference/information_criteria/
+-rw-r--r--   0 runner     (501) staff       (20)      883 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/AIC.py
+-rw-r--r--   0 runner     (501) staff       (20)     1004 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/AICc.py
+-rw-r--r--   0 runner     (501) staff       (20)      959 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/BIC.py
+-rw-r--r--   0 runner     (501) staff       (20)      230 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.846272 UQpy-4.1.0/src/UQpy/inference/information_criteria/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      649 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/baseclass/InformationCriterion.py
+-rw-r--r--   0 runner     (501) staff       (20)      100 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/inference/information_criteria/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.847234 UQpy-4.1.0/src/UQpy/reliability/
+-rw-r--r--   0 runner     (501) staff       (20)    13794 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/SubsetSimulation.py
+-rw-r--r--   0 runner     (501) staff       (20)      136 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.849007 UQpy-4.1.0/src/UQpy/reliability/taylor_series/
+-rw-r--r--   0 runner     (501) staff       (20)    16597 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/FORM.py
+-rw-r--r--   0 runner     (501) staff       (20)     6843 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/SORM.py
+-rw-r--r--   0 runner     (501) staff       (20)      185 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.850250 UQpy-4.1.0/src/UQpy/reliability/taylor_series/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     6400 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py
+-rw-r--r--   0 runner     (501) staff       (20)       68 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/reliability/taylor_series/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.851329 UQpy-4.1.0/src/UQpy/run_model/
+-rwxr-xr-x   0 runner     (501) staff       (20)    11467 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/RunModel.py
+-rw-r--r--   0 runner     (501) staff       (20)       91 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.855294 UQpy-4.1.0/src/UQpy/run_model/model_execution/
+-rw-r--r--   0 runner     (501) staff       (20)     2410 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/ClusterExecution.py
+-rw-r--r--   0 runner     (501) staff       (20)     2632 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/ParallelExecution.py
+-rw-r--r--   0 runner     (501) staff       (20)     6848 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/PythonModel.py
+-rw-r--r--   0 runner     (501) staff       (20)      650 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/SerialExecution.py
+-rw-r--r--   0 runner     (501) staff       (20)    23079 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/ThirdPartyModel.py
+-rw-r--r--   0 runner     (501) staff       (20)      244 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/run_model/model_execution/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.859203 UQpy-4.1.0/src/UQpy/sampling/
+-rw-r--r--   0 runner     (501) staff       (20)    11872 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/AdaptiveKriging.py
+-rw-r--r--   0 runner     (501) staff       (20)     8359 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/ImportanceSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     9204 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/MonteCarloSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     3835 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/SimplexSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     5079 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/ThetaCriterionPCE.py
+-rw-r--r--   0 runner     (501) staff       (20)      492 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.862714 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py
+-rw-r--r--   0 runner     (501) staff       (20)     1330 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py
+-rw-r--r--   0 runner     (501) staff       (20)     1535 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py
+-rw-r--r--   0 runner     (501) staff       (20)     1062 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/UFunction.py
+-rw-r--r--   0 runner     (501) staff       (20)     1627 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py
+-rw-r--r--   0 runner     (501) staff       (20)      437 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.863683 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      717 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/baseclass/LearningFunction.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.867054 UQpy-4.1.0/src/UQpy/sampling/mcmc/
+-rw-r--r--   0 runner     (501) staff       (20)    14747 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/DRAM.py
+-rw-r--r--   0 runner     (501) staff       (20)    13883 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/DREAM.py
+-rw-r--r--   0 runner     (501) staff       (20)     7890 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/MetropolisHastings.py
+-rw-r--r--   0 runner     (501) staff       (20)    12556 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py
+-rw-r--r--   0 runner     (501) staff       (20)     8369 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/Stretch.py
+-rw-r--r--   0 runner     (501) staff       (20)      385 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.868092 UQpy-4.1.0/src/UQpy/sampling/mcmc/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)    18931 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/baseclass/MCMC.py
+-rw-r--r--   0 runner     (501) staff       (20)       51 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.869758 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/
+-rw-r--r--   0 runner     (501) staff       (20)    13557 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/ParallelTemperingMCMC.py
+-rw-r--r--   0 runner     (501) staff       (20)    17860 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/SequentialTemperingMCMC.py
+-rw-r--r--   0 runner     (501) staff       (20)      243 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.870728 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     5548 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/TemperingMCMC.py
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.872757 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/
+-rw-r--r--   0 runner     (501) staff       (20)     5475 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     4839 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)     8527 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)      530 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.873772 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)       62 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/baseclass/StratifiedSampling.py
+-rw-r--r--   0 runner     (501) staff       (20)       94 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.876087 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/
+-rw-r--r--   0 runner     (501) staff       (20)      728 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py
+-rw-r--r--   0 runner     (501) staff       (20)     2125 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MaxiMin.py
+-rw-r--r--   0 runner     (501) staff       (20)     1587 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MinCorrelation.py
+-rw-r--r--   0 runner     (501) staff       (20)      933 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Random.py
+-rw-r--r--   0 runner     (501) staff       (20)      588 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.877093 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/Criterion.py
+-rw-r--r--   0 runner     (501) staff       (20)       93 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.878530 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/
+-rw-r--r--   0 runner     (501) staff       (20)     5703 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/GradientEnhancedRefinement.py
+-rw-r--r--   0 runner     (501) staff       (20)     1648 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/RandomRefinement.py
+-rw-r--r--   0 runner     (501) staff       (20)      231 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.879754 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     2517 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/baseclass/Refinement.py
+-rw-r--r--   0 runner     (501) staff       (20)       80 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.882694 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/
+-rw-r--r--   0 runner     (501) staff       (20)     4785 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/DelaunayStrata.py
+-rw-r--r--   0 runner     (501) staff       (20)    12238 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/RectangularStrata.py
+-rw-r--r--   0 runner     (501) staff       (20)       87 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/SamplingCriterion.py
+-rw-r--r--   0 runner     (501) staff       (20)    19271 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/VoronoiStrata.py
+-rw-r--r--   0 runner     (501) staff       (20)      407 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.884951 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     3383 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/baseclass/Strata.py
+-rw-r--r--   0 runner     (501) staff       (20)       77 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.893751 UQpy-4.1.0/src/UQpy/sensitivity/
+-rw-r--r--   0 runner     (501) staff       (20)    15373 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/ChatterjeeSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)    10943 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/CramerVonMisesSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)    14008 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/GeneralisedSobolSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)    12705 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/MorrisSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)     5812 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/PceSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)     9026 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/PostProcess.py
+-rw-r--r--   0 runner     (501) staff       (20)    33267 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/SobolSensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)      637 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.895153 UQpy-4.1.0/src/UQpy/sensitivity/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     2577 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/baseclass/PickFreeze.py
+-rw-r--r--   0 runner     (501) staff       (20)     9919 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/baseclass/Sensitivity.py
+-rw-r--r--   0 runner     (501) staff       (20)      105 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/sensitivity/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.899557 UQpy-4.1.0/src/UQpy/stochastic_process/
+-rw-r--r--   0 runner     (501) staff       (20)    12136 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/BispectralRepresentation.py
+-rw-r--r--   0 runner     (501) staff       (20)     7111 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/InverseTranslation.py
+-rw-r--r--   0 runner     (501) staff       (20)     5317 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/KarhunenLoeveExpansion.py
+-rw-r--r--   0 runner     (501) staff       (20)     6802 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/KarhunenLoeveExpansion2D.py
+-rw-r--r--   0 runner     (501) staff       (20)     9744 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/SpectralRepresentation.py
+-rw-r--r--   0 runner     (501) staff       (20)     7111 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/Translation.py
+-rw-r--r--   0 runner     (501) staff       (20)      523 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.902293 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/
+-rw-r--r--   0 runner     (501) staff       (20)      378 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1159 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/inverse_wiener_khinchin_transform.py
+-rw-r--r--   0 runner     (501) staff       (20)      579 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/scaling_correlation_function.py
+-rw-r--r--   0 runner     (501) staff       (20)     1087 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/stochastic_process/supportive/wiener_khinchin_transform.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.902799 UQpy-4.1.0/src/UQpy/surrogates/
+-rw-r--r--   0 runner     (501) staff       (20)      290 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.903841 UQpy-4.1.0/src/UQpy/surrogates/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      212 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/baseclass/Surrogate.py
+-rw-r--r--   0 runner     (501) staff       (20)       58 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.904917 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/
+-rwxr-xr-x   0 runner     (501) staff       (20)    16575 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      277 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.905867 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/
+-rw-r--r--   0 runner     (501) staff       (20)     2363 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py
+-rw-r--r--   0 runner     (501) staff       (20)      150 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.906871 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      708 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py
+-rw-r--r--   0 runner     (501) staff       (20)       94 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.908379 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/
+-rw-r--r--   0 runner     (501) staff       (20)     1279 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/Matern.py
+-rw-r--r--   0 runner     (501) staff       (20)      612 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/RBF.py
+-rw-r--r--   0 runner     (501) staff       (20)      193 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.909291 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     2135 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/baseclass/Kernel.py
+-rw-r--r--   0 runner     (501) staff       (20)       77 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.911178 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/
+-rw-r--r--   0 runner     (501) staff       (20)      305 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/ConstantRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      487 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/LinearRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)     1323 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      376 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.912133 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      385 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/Regression.py
+-rw-r--r--   0 runner     (501) staff       (20)       95 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.913029 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/
+-rw-r--r--   0 runner     (501) staff       (20)    12979 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py
+-rw-r--r--   0 runner     (501) staff       (20)      584 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.916252 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/
+-rw-r--r--   0 runner     (501) staff       (20)     2608 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/Hermite.py
+-rw-r--r--   0 runner     (501) staff       (20)     1528 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/HyperbolicBasis.py
+-rw-r--r--   0 runner     (501) staff       (20)     3300 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/Legendre.py
+-rw-r--r--   0 runner     (501) staff       (20)     1868 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/PolynomialsND.py
+-rw-r--r--   0 runner     (501) staff       (20)     1252 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/TensorProductBasis.py
+-rw-r--r--   0 runner     (501) staff       (20)     1599 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/TotalDegreeBasis.py
+-rw-r--r--   0 runner     (501) staff       (20)      580 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.917831 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     5969 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/PolynomialBasis.py
+-rw-r--r--   0 runner     (501) staff       (20)     6186 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/Polynomials.py
+-rw-r--r--   0 runner     (501) staff       (20)      190 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.920244 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/
+-rw-r--r--   0 runner     (501) staff       (20)     3015 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LassoRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)     5634 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LeastAngleRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      951 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LeastSquareRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)     2687 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/RidgeRegression.py
+-rw-r--r--   0 runner     (501) staff       (20)      378 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.921302 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)      229 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/Regression.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.922113 UQpy-4.1.0/src/UQpy/surrogates/stochastic_reduced_order_models/
+-rw-r--r--   0 runner     (501) staff       (20)    17080 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/stochastic_reduced_order_models/SROM.py
+-rw-r--r--   0 runner     (501) staff       (20)       23 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/surrogates/stochastic_reduced_order_models/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.923937 UQpy-4.1.0/src/UQpy/transformations/
+-rw-r--r--   0 runner     (501) staff       (20)      988 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/transformations/Correlate.py
+-rw-r--r--   0 runner     (501) staff       (20)     1027 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/transformations/Decorrelate.py
+-rw-r--r--   0 runner     (501) staff       (20)    20420 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/transformations/Nataf.py
+-rw-r--r--   0 runner     (501) staff       (20)       95 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/transformations/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.929320 UQpy-4.1.0/src/UQpy/utilities/
+-rw-r--r--   0 runner     (501) staff       (20)       84 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/Constants.py
+-rw-r--r--   0 runner     (501) staff       (20)      429 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/DistanceMetric.py
+-rw-r--r--   0 runner     (501) staff       (20)     1324 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/FminCobyla.py
+-rw-r--r--   0 runner     (501) staff       (20)      563 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/GrassmannPoint.py
+-rw-r--r--   0 runner     (501) staff       (20)     1920 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/MinimizeOptimizer.py
+-rw-r--r--   0 runner     (501) staff       (20)      772 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/NoPublicConstructor.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/UQpyLoggingFormatter.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    11339 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/Utilities.py
+-rw-r--r--   0 runner     (501) staff       (20)      826 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/ValidationTypes.py
+-rw-r--r--   0 runner     (501) staff       (20)      399 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.930918 UQpy-4.1.0/src/UQpy/utilities/distances/
+-rw-r--r--   0 runner     (501) staff       (20)      170 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.934037 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     1244 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/Distance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1270 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/EuclideanDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     2053 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/GrassmannianDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      237 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.940410 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/
+-rw-r--r--   0 runner     (501) staff       (20)      642 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/BrayCurtisDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      618 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CanberraDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      620 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/ChebyshevDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      634 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CityBlockDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      626 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CorrelationDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      612 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CosineDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      590 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/L2Distance.py
+-rw-r--r--   0 runner     (501) staff       (20)      767 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/MinkowskiDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      728 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.946910 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/
+-rw-r--r--   0 runner     (501) staff       (20)      954 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/AsimovDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      979 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/BinetCauchyDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      991 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1085 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1128 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1068 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1037 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      932 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py
+-rw-r--r--   0 runner     (501) staff       (20)      764 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.948775 UQpy-4.1.0/src/UQpy/utilities/kernels/
+-rw-r--r--   0 runner     (501) staff       (20)      772 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/BinetCauchyKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)     2939 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/GaussianKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)      785 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/ProjectionKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)      254 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.951368 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/
+-rw-r--r--   0 runner     (501) staff       (20)     1255 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/EuclideanKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)     1592 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/GrassmannianKernel.py
+-rw-r--r--   0 runner     (501) staff       (20)     2090 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/Kernel.py
+-rw-r--r--   0 runner     (501) staff       (20)      219 2023-04-28 22:03:54.000000 UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-28 22:56:36.772963 UQpy-4.1.0/src/UQpy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      677 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    14004 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       57 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        5 2023-04-28 22:56:36.000000 UQpy-4.1.0/src/UQpy.egg-info/top_level.txt
```

### Comparing `UQpy-4.0.7/LICENSE` & `UQpy-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/PKG-INFO` & `UQpy-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UQpy
-Version: 4.0.7
+Version: 4.1.0
 Summary: UQpy is a general purpose toolbox for Uncertainty Quantification
 Home-page: https://github.com/SURGroup/UQpy
 Author: Michael D. Shields, Dimitris G. Giovanis, Audrey Olivier, Aakash Bangalore-Satish, Mohit Chauhan, Lohit Vandanapu, Ketson R.M. dos Santos
 Author-email: UQpy.info@gmail.com
 License: MIT
 Platform: OSX
 Platform: Windows
```

### Comparing `UQpy-4.0.7/README.rst` & `UQpy-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/setup.py` & `UQpy-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/__init__.py` & `UQpy-4.1.0/src/UQpy/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/dimension_reduction/diffusion_maps/DiffusionMaps.py` & `UQpy-4.1.0/src/UQpy/dimension_reduction/diffusion_maps/DiffusionMaps.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannInterpolation.py` & `UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannInterpolation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannOperations.py` & `UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/GrassmannOperations.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/dimension_reduction/grassmann_manifold/projections/SVDProjection.py` & `UQpy-4.1.0/src/UQpy/dimension_reduction/grassmann_manifold/projections/SVDProjection.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/dimension_reduction/hosvd/HigherOrderSVD.py` & `UQpy-4.1.0/src/UQpy/dimension_reduction/hosvd/HigherOrderSVD.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/dimension_reduction/pod/DirectPOD.py` & `UQpy-4.1.0/src/UQpy/dimension_reduction/pod/DirectPOD.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/dimension_reduction/pod/SnapshotPOD.py` & `UQpy-4.1.0/src/UQpy/dimension_reduction/pod/SnapshotPOD.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/dimension_reduction/pod/baseclass/POD.py` & `UQpy-4.1.0/src/UQpy/dimension_reduction/pod/baseclass/POD.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/baseclass/Copula.py` & `UQpy-4.1.0/src/UQpy/distributions/baseclass/Copula.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/baseclass/Distribution.py` & `UQpy-4.1.0/src/UQpy/distributions/baseclass/Distribution.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/baseclass/Distribution1D.py` & `UQpy-4.1.0/src/UQpy/distributions/baseclass/Distribution1D.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/baseclass/DistributionContinuous1D.py` & `UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionContinuous1D.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/baseclass/DistributionDiscrete1D.py` & `UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionDiscrete1D.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/baseclass/DistributionND.py` & `UQpy-4.1.0/src/UQpy/distributions/baseclass/DistributionND.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Beta.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Beta.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Binomial.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Binomial.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Cauchy.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Cauchy.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/ChiSquare.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/ChiSquare.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Exponential.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Exponential.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Gamma.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Gamma.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/GeneralizedExtreme.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/GeneralizedExtreme.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/InverseGaussian.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/InverseGaussian.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/JointCopula.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/JointCopula.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/JointIndependent.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/JointIndependent.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Laplace.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Laplace.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Levy.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Levy.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Logistic.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Logistic.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Lognormal.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Lognormal.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Maxwell.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Maxwell.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Multinomial.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Multinomial.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/MultivariateNormal.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/MultivariateNormal.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Normal.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Normal.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Pareto.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Pareto.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Poisson.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Poisson.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Rayleigh.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Rayleigh.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/TruncatedNormal.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/TruncatedNormal.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/Uniform.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/Uniform.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/collection/__init__.py` & `UQpy-4.1.0/src/UQpy/distributions/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/copulas/Clayton.py` & `UQpy-4.1.0/src/UQpy/distributions/copulas/Clayton.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/copulas/Frank.py` & `UQpy-4.1.0/src/UQpy/distributions/copulas/Frank.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/distributions/copulas/Gumbel.py` & `UQpy-4.1.0/src/UQpy/distributions/copulas/Gumbel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/BayesModelSelection.py` & `UQpy-4.1.0/src/UQpy/inference/BayesModelSelection.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/BayesParameterEstimation.py` & `UQpy-4.1.0/src/UQpy/inference/BayesParameterEstimation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/InformationModelSelection.py` & `UQpy-4.1.0/src/UQpy/inference/InformationModelSelection.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/MLE.py` & `UQpy-4.1.0/src/UQpy/inference/MLE.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/__init__.py` & `UQpy-4.1.0/src/UQpy/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/evidence_methods/HarmonicMean.py` & `UQpy-4.1.0/src/UQpy/inference/evidence_methods/HarmonicMean.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/evidence_methods/baseclass/EvidenceMethod.py` & `UQpy-4.1.0/src/UQpy/inference/evidence_methods/baseclass/EvidenceMethod.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/inference_models/ComputationalModel.py` & `UQpy-4.1.0/src/UQpy/inference/inference_models/ComputationalModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/inference_models/DistributionModel.py` & `UQpy-4.1.0/src/UQpy/inference/inference_models/DistributionModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/inference_models/LogLikelihoodModel.py` & `UQpy-4.1.0/src/UQpy/inference/inference_models/LogLikelihoodModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/inference_models/baseclass/InferenceModel.py` & `UQpy-4.1.0/src/UQpy/inference/inference_models/baseclass/InferenceModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/information_criteria/AIC.py` & `UQpy-4.1.0/src/UQpy/inference/information_criteria/AIC.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/information_criteria/AICc.py` & `UQpy-4.1.0/src/UQpy/inference/information_criteria/AICc.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/information_criteria/BIC.py` & `UQpy-4.1.0/src/UQpy/inference/information_criteria/BIC.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/inference/information_criteria/baseclass/InformationCriterion.py` & `UQpy-4.1.0/src/UQpy/inference/information_criteria/baseclass/InformationCriterion.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/reliability/SubsetSimulation.py` & `UQpy-4.1.0/src/UQpy/reliability/SubsetSimulation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/reliability/taylor_series/FORM.py` & `UQpy-4.1.0/src/UQpy/reliability/taylor_series/FORM.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,14 +299,15 @@
                 error3 = np.linalg.norm(dg_u_record[k + 1, :] - dg_u_record[k, :])
                 error_record.append([error1, error3])
                 if error1 <= self.tol1 and error3 < self.tol3:
                     converged = True
                 else:
                     k = k + 1
 
+
             elif (self.tol1 is None) and (self.tol2 is not None) and (self.tol3 is not None):
                 error2 = np.linalg.norm(beta[k + 1] - beta[k])
                 error3 = np.linalg.norm(dg_u_record[k + 1, :] - dg_u_record[k, :])
                 error_record.append([error2, error3])
                 if error2 <= self.tol2 and error3 < self.tol3:
                     converged = True
                 else:
```

### Comparing `UQpy-4.0.7/src/UQpy/reliability/taylor_series/SORM.py` & `UQpy-4.1.0/src/UQpy/reliability/taylor_series/SORM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py` & `UQpy-4.1.0/src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/run_model/RunModel.py` & `UQpy-4.1.0/src/UQpy/run_model/RunModel.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,33 +18,40 @@
 import logging
 import os
 import pickle
 from typing import Union
 
 import numpy as np
 from beartype import beartype
+from enum import Enum, auto
 
 from UQpy.utilities.ValidationTypes import NumpyFloatArray
 
+class RunType(Enum):
+    LOCAL = auto()
+    CLUSTER = auto()
+
 
 class RunModel:
     # Authors:
-    # B.S. Aakash, Lohit Vandanapu, Michael D.Shields
+    # B.S. Aakash, Lohit Vandanapu, Michael D.Shields, Michael H. Gardner
     #
     # Last
-    # modified: 5 / 8 / 2020 by Michael D.Shields
+    # modified: 8 / 31 / 2022 by Michael H. Gardner
     @beartype
     def __init__(
             self,
             model,
             samples: Union[list, NumpyFloatArray] = None,
             ntasks: int = 1,
             cores_per_task: int = 1,
             nodes: int = 1,
             resume: bool = False,
+            run_type: str = 'LOCAL',
+            cluster_script: str = None
     ):
         """
         Run a computational model at specified sample points.
 
         This class is the interface between :py:mod:`UQpy` and computational models. The model is called in a Python script whose
         name must be passed as one the arguments to the :class:`.RunModel` call. If the model is in Python, :py:mod:`UQpy` import the
         model and executes it directly. If the model is not in Python, :class:`.RunModel` must be provided the name of a template
@@ -81,14 +88,17 @@
          model workflow. If more than one compute node is necessary to execute individual runs in parallel, `nodes` must
          be specified.
         """
         self.logger = logging.getLogger(__name__)
         self.model = model
         # Save option for resuming parallel execution
         self.resume = resume
+        # Set location for model runs
+        self.run_type = RunType[run_type]
+        self.cluster_script = cluster_script
 
         self.nodes = nodes
         self.ntasks = ntasks
         self.cores_per_task = cores_per_task
 
         self.is_serial = ntasks <= 1 and cores_per_task <= 1 and nodes <= 1
 
@@ -185,17 +195,28 @@
 
     def parallel_execution(self):
         # TODO: Check if files with the names used below already exist and raise error
         with open('model.pkl', 'wb') as filehandle:
             pickle.dump(self.model, filehandle)
         with open('samples.pkl', 'wb') as filehandle:
             pickle.dump(self.samples, filehandle)
-        os.system(f"mpirun python -m "
-                  f"UQpy.run_model.model_execution.ParallelExecution {self.n_existing_simulations} "
-                  f"{self.n_new_simulations}")
+            
+        if self.run_type is RunType.LOCAL:        
+            os.system(f"mpirun python -m "
+                      f"UQpy.run_model.model_execution.ParallelExecution {self.n_existing_simulations} "
+                      f"{self.n_new_simulations}")
+
+        elif self.run_type is RunType.CLUSTER:
+            if self.cluster_script is None:
+                raise ValueError("\nUQpy: User-provided slurm script not input, please provide this input\n")
+            os.system(f"python -m UQpy.run_model.model_execution.ClusterExecution {self.cores_per_task} "
+                      f"{self.n_new_simulations} {self.n_existing_simulations} {self.cluster_script}")
+        else:
+            raise ValueError("\nUQpy: RunType is not in currently supported list of cluster types\n")            
+        
         with open('qoi.pkl', 'rb') as filehandle:
             results = pickle.load(filehandle)
 
         os.remove("model.pkl")
         os.remove("samples.pkl")
         os.remove("qoi.pkl")
```

### Comparing `UQpy-4.0.7/src/UQpy/run_model/model_execution/ParallelExecution.py` & `UQpy-4.1.0/src/UQpy/run_model/model_execution/ParallelExecution.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/run_model/model_execution/PythonModel.py` & `UQpy-4.1.0/src/UQpy/run_model/model_execution/PythonModel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/run_model/model_execution/SerialExecution.py` & `UQpy-4.1.0/src/UQpy/run_model/model_execution/SerialExecution.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/run_model/model_execution/ThirdPartyModel.py` & `UQpy-4.1.0/src/UQpy/run_model/model_execution/ThirdPartyModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                     temp = string[1:-1].replace(var_names[j], "sample[" + str(j) + "]")
                     try:
                         temp = eval(temp)
                     except IndexError as err:
                         print("\nUQpy: Index Error: {0}\n".format(err))
                         raise IndexError("{0}".format(err))
 
-                    if isinstance(temp, collections.Iterable):
+                    if isinstance(temp, collections.abc.Iterable):
                         # If it is iterable, flatten and write as text file with designated separator
                         temp = np.array(temp).flatten()
                         to_add = ""
                         for i in range(len(temp) - 1):
                             if self.fmt is None:
                                 to_add += str(temp[i]) + self.separator
                             else:
```

### Comparing `UQpy-4.0.7/src/UQpy/sampling/AdaptiveKriging.py` & `UQpy-4.1.0/src/UQpy/sampling/AdaptiveKriging.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/ImportanceSampling.py` & `UQpy-4.1.0/src/UQpy/sampling/ImportanceSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/MonteCarloSampling.py` & `UQpy-4.1.0/src/UQpy/sampling/MonteCarloSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/SimplexSampling.py` & `UQpy-4.1.0/src/UQpy/sampling/SimplexSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py` & `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py` & `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py` & `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/UFunction.py` & `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/UFunction.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py` & `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/adaptive_kriging_functions/baseclass/LearningFunction.py` & `UQpy-4.1.0/src/UQpy/sampling/adaptive_kriging_functions/baseclass/LearningFunction.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/mcmc/DRAM.py` & `UQpy-4.1.0/src/UQpy/sampling/mcmc/DRAM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/mcmc/DREAM.py` & `UQpy-4.1.0/src/UQpy/sampling/mcmc/DREAM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/mcmc/MetropolisHastings.py` & `UQpy-4.1.0/src/UQpy/sampling/mcmc/MetropolisHastings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 warnings.filterwarnings('ignore')
 
 
 class MetropolisHastings(MCMC):
 
     @beartype
     def __init__(
-        self,
-        pdf_target: Union[Callable, list[Callable]] = None,
-        log_pdf_target: Union[Callable, list[Callable]] = None,
-        args_target: tuple = None,
-        burn_length: Annotated[int, Is[lambda x: x >= 0]] = 0,
-        jump: int = 1,
-        dimension: int = None,
-        seed: list = None,
-        save_log_pdf: bool = False,
-        concatenate_chains: bool = True,
-        n_chains: int = None,
-        proposal: Distribution = None,
-        proposal_is_symmetric: bool = False,
-        random_state: RandomStateType = None,
-        nsamples: PositiveInteger = None,
-        nsamples_per_chain: PositiveInteger = None,
+            self,
+            pdf_target: Union[Callable, list[Callable]] = None,
+            log_pdf_target: Union[Callable, list[Callable]] = None,
+            args_target: tuple = None,
+            burn_length: Annotated[int, Is[lambda x: x >= 0]] = 0,
+            jump: int = 1,
+            dimension: int = None,
+            seed: list = None,
+            save_log_pdf: bool = False,
+            concatenate_chains: bool = True,
+            n_chains: int = None,
+            proposal: Distribution = None,
+            proposal_is_symmetric: bool = False,
+            random_state: RandomStateType = None,
+            nsamples: PositiveInteger = None,
+            nsamples_per_chain: PositiveInteger = None,
     ):
         """
         Metropolis-Hastings algorithm :cite:`MCMC1` :cite:`MCMC2`
 
         :param pdf_target: Target density function from which to draw random samples. Either `pdf_target` or
          `log_pdf_target` must be provided (the latter should be preferred for better numerical stability).
 
@@ -111,15 +111,15 @@
             self.proposal_is_symmetric = True
         else:
             self._check_methods_proposal(self.proposal)
 
         self.logger.info("\nUQpy: Initialization of " + self.__class__.__name__ + " algorithm complete.")
 
         if (nsamples is not None) or (nsamples_per_chain is not None):
-            self.run(nsamples=nsamples, nsamples_per_chain=nsamples_per_chain,)
+            self.run(nsamples=nsamples, nsamples_per_chain=nsamples_per_chain, )
 
     def run_one_iteration(self, current_state: np.ndarray, current_log_pdf: np.ndarray):
         """
         Run one iteration of the mcmc chain for MH algorithm, starting at current state -
         see :class:`MCMC` class.
         """
         # Sample candidate
@@ -140,19 +140,19 @@
 
         # Compare candidate with current sample and decide or not to keep the candidate (loop over nc chains)
         accept_vec = np.zeros(
             (self.n_chains,)
         )  # this vector will be used to compute accept_ratio of each chain
         unif_rvs = (
             Uniform()
-            .rvs(nsamples=self.n_chains, random_state=self.random_state)
-            .reshape((-1,))
+                .rvs(nsamples=self.n_chains, random_state=self.random_state)
+                .reshape((-1,))
         )
         for nc, (cand, log_p_cand, r_) in enumerate(
-            zip(candidate, log_p_candidate, log_ratios)
+                zip(candidate, log_p_candidate, log_ratios)
         ):
             accept = np.log(unif_rvs[nc]) < r_
             if accept:
                 current_state[nc, :] = cand
                 current_log_pdf[nc] = log_p_cand
                 accept_vec[nc] = 1.0
         # Update the acceptance rate
```

### Comparing `UQpy-4.0.7/src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py` & `UQpy-4.1.0/src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/mcmc/Stretch.py` & `UQpy-4.1.0/src/UQpy/sampling/mcmc/Stretch.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/mcmc/baseclass/MCMC.py` & `UQpy-4.1.0/src/UQpy/sampling/mcmc/baseclass/MCMC.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 warnings.filterwarnings('ignore')
 
 import numpy as np
 from beartype import beartype
 from UQpy.distributions import Distribution
 from UQpy.utilities.ValidationTypes import *
 from UQpy.utilities.Utilities import process_random_state
-from abc import ABC
+from abc import ABC, abstractmethod
 
 
 class MCMC(ABC):
     @beartype
     def __init__(
             self,
             dimension: Union[None, int] = None,
@@ -173,37 +173,30 @@
     def _concatenate_chains(self):
         self.samples = self.samples.reshape((-1, self.dimension), order="C")
         if self.save_log_pdf:
             self.log_pdf_values = self.log_pdf_values.reshape((-1,), order="C")
         return None
 
     def _unconcatenate_chains(self):
-        self.samples = self.samples.reshape(
-            (-1, self.n_chains, self.dimension), order="C"
-        )
+        self.samples = self.samples.reshape((-1, self.n_chains, self.dimension), order="C")
         if self.save_log_pdf:
-            self.log_pdf_values = self.log_pdf_values.reshape(
-                (-1, self.n_chains), order="C"
-            )
+            self.log_pdf_values = self.log_pdf_values.reshape((-1, self.n_chains), order="C")
         return None
 
     def _initialize_samples(self, nsamples, nsamples_per_chain):
         if ((nsamples is not None) and (nsamples_per_chain is not None)) \
                 or (nsamples is None and nsamples_per_chain is None):
             raise ValueError("UQpy: Either nsamples or nsamples_per_chain must be provided (not both)")
-        if nsamples_per_chain is not None:
-            if not (isinstance(nsamples_per_chain, int) and nsamples_per_chain >= 0):
-                raise TypeError("UQpy: nsamples_per_chain must be an integer >= 0.")
-            nsamples = int(nsamples_per_chain * self.n_chains)
-        else:
+        if nsamples_per_chain is None:
             if not (isinstance(nsamples, int) and nsamples >= 0):
                 raise TypeError("UQpy: nsamples must be an integer >= 0.")
             nsamples_per_chain = int(np.ceil(nsamples / self.n_chains))
-            nsamples = int(nsamples_per_chain * self.n_chains)
-
+        elif not (isinstance(nsamples_per_chain, int) and nsamples_per_chain >= 0):
+            raise TypeError("UQpy: nsamples_per_chain must be an integer >= 0.")
+        nsamples = int(nsamples_per_chain * self.n_chains)
         if self.samples is None:  # very first call of run, set current_state as the seed and initialize self.samples
             self.samples = np.zeros((nsamples_per_chain, self.n_chains, self.dimension))
             if self.save_log_pdf:
                 self.log_pdf_values = np.zeros((nsamples_per_chain, self.n_chains))
             current_state = np.zeros_like(self.seed)
             np.copyto(current_state, self.seed)
             current_log_pdf = self.evaluate_log_target(current_state)
@@ -312,7 +305,27 @@
         if not hasattr(proposal_distribution, "rvs"):
             raise AttributeError("UQpy: The proposal should have an rvs method")
         if not hasattr(proposal_distribution, "log_pdf"):
             if not hasattr(proposal_distribution, "pdf"):
                 raise AttributeError("UQpy: The proposal should have a log_pdf or pdf method")
             proposal_distribution.log_pdf = lambda x: np.log(
                 np.maximum(proposal_distribution.pdf(x), 10 ** (-320) * np.ones((x.shape[0],))))
+
+    def __copy__(self, **kwargs):
+        keys = kwargs.keys()
+        attributes = self.__dict__
+        import inspect
+        initializer_parameters = inspect.signature(self.__class__.__init__).parameters.keys()
+
+        for key in attributes.keys():
+            if key not in initializer_parameters:
+                continue
+            new_value = attributes[key] if key not in keys else kwargs[key]
+            if new_value is not None:
+                kwargs[key] = new_value
+
+        if 'seed' in kwargs.keys():
+            kwargs['seed'] = list(kwargs['seed'])
+        if 'nsamples_per_chain' in kwargs.keys() and kwargs['nsamples_per_chain'] == 0:
+            del kwargs['nsamples_per_chain']
+
+        return self.__class__(**kwargs)
```

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/__init__.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MaxiMin.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MaxiMin.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MinCorrelation.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/MinCorrelation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Random.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Random.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/__init__.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/Criterion.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/baseclass/Criterion.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/GradientEnhancedRefinement.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/GradientEnhancedRefinement.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/RandomRefinement.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/RandomRefinement.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/refinement/baseclass/Refinement.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/refinement/baseclass/Refinement.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/DelaunayStrata.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/DelaunayStrata.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/RectangularStrata.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/RectangularStrata.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/VoronoiStrata.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/VoronoiStrata.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sampling/stratified_sampling/strata/baseclass/Strata.py` & `UQpy-4.1.0/src/UQpy/sampling/stratified_sampling/strata/baseclass/Strata.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/ChatterjeeSensitivity.py` & `UQpy-4.1.0/src/UQpy/sensitivity/ChatterjeeSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/CramerVonMisesSensitivity.py` & `UQpy-4.1.0/src/UQpy/sensitivity/CramerVonMisesSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/GeneralisedSobolSensitivity.py` & `UQpy-4.1.0/src/UQpy/sensitivity/GeneralisedSobolSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/MorrisSensitivity.py` & `UQpy-4.1.0/src/UQpy/sensitivity/MorrisSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/PceSensitivity.py` & `UQpy-4.1.0/src/UQpy/sensitivity/PceSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/PostProcess.py` & `UQpy-4.1.0/src/UQpy/sensitivity/PostProcess.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/SobolSensitivity.py` & `UQpy-4.1.0/src/UQpy/sensitivity/SobolSensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/__init__.py` & `UQpy-4.1.0/src/UQpy/sensitivity/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/baseclass/PickFreeze.py` & `UQpy-4.1.0/src/UQpy/sensitivity/baseclass/PickFreeze.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/sensitivity/baseclass/Sensitivity.py` & `UQpy-4.1.0/src/UQpy/sensitivity/baseclass/Sensitivity.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/BispectralRepresentation.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/BispectralRepresentation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/InverseTranslation.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/InverseTranslation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/KarhunenLoeveExpansion.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/KarhunenLoeveExpansion.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/KarhunenLoeveExpansion2D.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/KarhunenLoeveExpansion2D.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/SpectralRepresentation.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/SpectralRepresentation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/Translation.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/Translation.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/__init__.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/supportive/inverse_wiener_khinchin_transform.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/supportive/inverse_wiener_khinchin_transform.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/supportive/scaling_correlation_function.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/supportive/scaling_correlation_function.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/stochastic_process/supportive/wiener_khinchin_transform.py` & `UQpy-4.1.0/src/UQpy/stochastic_process/supportive/wiener_khinchin_transform.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py` & `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/GaussianProcessRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py` & `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/NonNegative.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py` & `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/constraints/baseclass/Constraints.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/Matern.py` & `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/Matern.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/RBF.py` & `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/RBF.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/kernels/baseclass/Kernel.py` & `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/kernels/baseclass/Kernel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py` & `UQpy-4.1.0/src/UQpy/surrogates/gaussian_process/regression_models/QuadraticRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/PolynomialChaosExpansion.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/__init__.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/Hermite.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/Hermite.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/HyperbolicBasis.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/HyperbolicBasis.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/Legendre.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/Legendre.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/PolynomialsND.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/PolynomialsND.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/TensorProductBasis.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/TensorProductBasis.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/TotalDegreeBasis.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/TotalDegreeBasis.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/__init__.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/PolynomialBasis.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/polynomials/baseclass/PolynomialBasis.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/LassoRegression.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LassoRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/LeastAngleRegression.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LeastAngleRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/LeastSquareRegression.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/LeastSquareRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/polynomial_chaos/regressions/RidgeRegression.py` & `UQpy-4.1.0/src/UQpy/surrogates/polynomial_chaos/regressions/RidgeRegression.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/surrogates/stochastic_reduced_order_models/SROM.py` & `UQpy-4.1.0/src/UQpy/surrogates/stochastic_reduced_order_models/SROM.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/transformations/Correlate.py` & `UQpy-4.1.0/src/UQpy/transformations/Correlate.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/transformations/Decorrelate.py` & `UQpy-4.1.0/src/UQpy/transformations/Decorrelate.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/transformations/Nataf.py` & `UQpy-4.1.0/src/UQpy/transformations/Nataf.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/FminCobyla.py` & `UQpy-4.1.0/src/UQpy/utilities/FminCobyla.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/GrassmannPoint.py` & `UQpy-4.1.0/src/UQpy/utilities/GrassmannPoint.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/MinimizeOptimizer.py` & `UQpy-4.1.0/src/UQpy/utilities/MinimizeOptimizer.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/NoPublicConstructor.py` & `UQpy-4.1.0/src/UQpy/utilities/NoPublicConstructor.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/UQpyLoggingFormatter.py` & `UQpy-4.1.0/src/UQpy/utilities/UQpyLoggingFormatter.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/Utilities.py` & `UQpy-4.1.0/src/UQpy/utilities/Utilities.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/ValidationTypes.py` & `UQpy-4.1.0/src/UQpy/utilities/ValidationTypes.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/baseclass/Distance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/Distance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/baseclass/EuclideanDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/EuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/baseclass/GrassmannianDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/baseclass/GrassmannianDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/BrayCurtisDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/BrayCurtisDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/CanberraDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CanberraDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/ChebyshevDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/ChebyshevDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/CityBlockDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CityBlockDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/CorrelationDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CorrelationDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/CosineDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/CosineDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/L2Distance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/L2Distance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/MinkowskiDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/MinkowskiDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/euclidean_distances/__init__.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/euclidean_distances/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/AsimovDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/AsimovDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/BinetCauchyDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/BinetCauchyDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/FubiniStudyDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/GeodesicDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/MartinDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/ProcrustesDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/ProjectionDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/SpectralDistance.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/distances/grassmannian_distances/__init__.py` & `UQpy-4.1.0/src/UQpy/utilities/distances/grassmannian_distances/__init__.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/kernels/BinetCauchyKernel.py` & `UQpy-4.1.0/src/UQpy/utilities/kernels/BinetCauchyKernel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/kernels/GaussianKernel.py` & `UQpy-4.1.0/src/UQpy/utilities/kernels/GaussianKernel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/kernels/ProjectionKernel.py` & `UQpy-4.1.0/src/UQpy/utilities/kernels/ProjectionKernel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/kernels/baseclass/EuclideanKernel.py` & `UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/EuclideanKernel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/kernels/baseclass/GrassmannianKernel.py` & `UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/GrassmannianKernel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy/utilities/kernels/baseclass/Kernel.py` & `UQpy-4.1.0/src/UQpy/utilities/kernels/baseclass/Kernel.py`

 * *Files identical despite different names*

### Comparing `UQpy-4.0.7/src/UQpy.egg-info/PKG-INFO` & `UQpy-4.1.0/src/UQpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UQpy
-Version: 4.0.7
+Version: 4.1.0
 Summary: UQpy is a general purpose toolbox for Uncertainty Quantification
 Home-page: https://github.com/SURGroup/UQpy
 Author: Michael D. Shields, Dimitris G. Giovanis, Audrey Olivier, Aakash Bangalore-Satish, Mohit Chauhan, Lohit Vandanapu, Ketson R.M. dos Santos
 Author-email: UQpy.info@gmail.com
 License: MIT
 Platform: OSX
 Platform: Windows
```

### Comparing `UQpy-4.0.7/src/UQpy.egg-info/SOURCES.txt` & `UQpy-4.1.0/src/UQpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -86,23 +86,25 @@
 src/UQpy/reliability/taylor_series/FORM.py
 src/UQpy/reliability/taylor_series/SORM.py
 src/UQpy/reliability/taylor_series/__init__.py
 src/UQpy/reliability/taylor_series/baseclass/TaylorSeries.py
 src/UQpy/reliability/taylor_series/baseclass/__init__.py
 src/UQpy/run_model/RunModel.py
 src/UQpy/run_model/__init__.py
+src/UQpy/run_model/model_execution/ClusterExecution.py
 src/UQpy/run_model/model_execution/ParallelExecution.py
 src/UQpy/run_model/model_execution/PythonModel.py
 src/UQpy/run_model/model_execution/SerialExecution.py
 src/UQpy/run_model/model_execution/ThirdPartyModel.py
 src/UQpy/run_model/model_execution/__init__.py
 src/UQpy/sampling/AdaptiveKriging.py
 src/UQpy/sampling/ImportanceSampling.py
 src/UQpy/sampling/MonteCarloSampling.py
 src/UQpy/sampling/SimplexSampling.py
+src/UQpy/sampling/ThetaCriterionPCE.py
 src/UQpy/sampling/__init__.py
 src/UQpy/sampling/adaptive_kriging_functions/ExpectedFeasibility.py
 src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovement.py
 src/UQpy/sampling/adaptive_kriging_functions/ExpectedImprovementGlobalFit.py
 src/UQpy/sampling/adaptive_kriging_functions/UFunction.py
 src/UQpy/sampling/adaptive_kriging_functions/WeightedUFunction.py
 src/UQpy/sampling/adaptive_kriging_functions/__init__.py
@@ -112,14 +114,19 @@
 src/UQpy/sampling/mcmc/DREAM.py
 src/UQpy/sampling/mcmc/MetropolisHastings.py
 src/UQpy/sampling/mcmc/ModifiedMetropolisHastings.py
 src/UQpy/sampling/mcmc/Stretch.py
 src/UQpy/sampling/mcmc/__init__.py
 src/UQpy/sampling/mcmc/baseclass/MCMC.py
 src/UQpy/sampling/mcmc/baseclass/__init__.py
+src/UQpy/sampling/mcmc/tempering_mcmc/ParallelTemperingMCMC.py
+src/UQpy/sampling/mcmc/tempering_mcmc/SequentialTemperingMCMC.py
+src/UQpy/sampling/mcmc/tempering_mcmc/__init__.py
+src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/TemperingMCMC.py
+src/UQpy/sampling/mcmc/tempering_mcmc/baseclass/__init__.py
 src/UQpy/sampling/stratified_sampling/LatinHypercubeSampling.py
 src/UQpy/sampling/stratified_sampling/RefinedStratifiedSampling.py
 src/UQpy/sampling/stratified_sampling/TrueStratifiedSampling.py
 src/UQpy/sampling/stratified_sampling/__init__.py
 src/UQpy/sampling/stratified_sampling/baseclass/StratifiedSampling.py
 src/UQpy/sampling/stratified_sampling/baseclass/__init__.py
 src/UQpy/sampling/stratified_sampling/latin_hypercube_criteria/Centered.py
```

