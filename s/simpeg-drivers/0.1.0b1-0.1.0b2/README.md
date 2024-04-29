# Comparing `tmp/simpeg_drivers-0.1.0b1.tar.gz` & `tmp/simpeg_drivers-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpeg_drivers-0.1.0b1.tar", max compression
+gzip compressed data, was "simpeg_drivers-0.1.0b2.tar", max compression
```

## Comparing `simpeg_drivers-0.1.0b1.tar` & `simpeg_drivers-0.1.0b2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 simpeg_drivers-0.1.0b1/LICENSE
--rw-r--r--   0        0        0     4938 2024-04-29 02:52:45.702104 simpeg_drivers-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     5466 2024-04-29 02:02:58.449338 simpeg_drivers-0.1.0b1/README.rst
--rw-r--r--   0        0        0     3604 2024-04-29 02:52:45.703111 simpeg_drivers-0.1.0b1/simpeg_drivers/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-29 02:02:58.454666 simpeg_drivers-0.1.0b1/simpeg_drivers/components/__init__.py
--rw-r--r--   0        0        0    20280 2024-04-26 14:45:23.742914 simpeg_drivers-0.1.0b1/simpeg_drivers/components/data.py
--rw-r--r--   0        0        0     1231 2024-04-29 02:14:00.711152 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/__init__.py
--rw-r--r--   0        0        0     1462 2024-04-26 14:45:23.744035 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/abstract_factory.py
--rw-r--r--   0        0        0    21970 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/directives_factory.py
--rw-r--r--   0        0        0     4382 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/entity_factory.py
--rw-r--r--   0        0        0     5003 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/misfit_factory.py
--rw-r--r--   0        0        0     7519 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/receiver_factory.py
--rw-r--r--   0        0        0     3521 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/simpeg_factory.py
--rw-r--r--   0        0        0     8146 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/simulation_factory.py
--rw-r--r--   0        0        0     6142 2024-04-26 14:45:23.748321 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/source_factory.py
--rw-r--r--   0        0        0    17787 2024-04-29 01:48:58.170502 simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/survey_factory.py
--rw-r--r--   0        0        0     6476 2024-04-26 14:45:23.750330 simpeg_drivers-0.1.0b1/simpeg_drivers/components/locations.py
--rw-r--r--   0        0        0     4799 2024-04-26 14:45:23.751485 simpeg_drivers-0.1.0b1/simpeg_drivers/components/meshes.py
--rw-r--r--   0        0        0    16897 2024-04-26 14:45:23.751584 simpeg_drivers-0.1.0b1/simpeg_drivers/components/models.py
--rw-r--r--   0        0        0     6135 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b1/simpeg_drivers/components/topography.py
--rw-r--r--   0        0        0     1846 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b1/simpeg_drivers/components/utils.py
--rw-r--r--   0        0        0     4179 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b1/simpeg_drivers/components/windows.py
--rw-r--r--   0        0        0    14591 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b1/simpeg_drivers/constants.py
--rw-r--r--   0        0        0    18654 2024-04-26 14:45:23.754889 simpeg_drivers-0.1.0b1/simpeg_drivers/driver.py
--rw-r--r--   0        0        0     1112 2024-04-29 02:14:00.696694 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/__init__.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.755992 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/__init__.py
--rw-r--r--   0        0        0    10334 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py
--rw-r--r--   0        0        0     1506 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py
--rw-r--r--   0        0        0     2680 2024-04-26 14:45:23.758085 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py
--rw-r--r--   0        0        0      962 2024-04-29 02:14:00.601072 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py
--rw-r--r--   0        0        0     9075 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py
--rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py
--rw-r--r--   0        0        0     2808 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/three_dimensions/params.py
--rw-r--r--   0        0        0      911 2024-04-26 14:45:23.761252 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py
--rw-r--r--   0        0        0    10879 2024-04-26 14:45:23.762303 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py
--rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py
--rw-r--r--   0        0        0     2646 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/two_dimensions/params.py
--rw-r--r--   0        0        0     6721 2024-04-29 01:48:52.896367 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/driver.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.763466 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/__init__.py
--rw-r--r--   0        0        0    10754 2024-04-26 14:45:23.764555 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py
--rw-r--r--   0        0        0     1596 2024-04-26 14:45:23.765703 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py
--rw-r--r--   0        0        0     3031 2024-04-26 14:45:23.766703 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py
--rw-r--r--   0        0        0      968 2024-04-29 02:14:00.644863 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py
--rw-r--r--   0        0        0     9362 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py
--rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py
--rw-r--r--   0        0        0     3529 2024-04-26 14:45:23.768920 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py
--rw-r--r--   0        0        0      968 2024-04-29 02:14:00.616156 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py
--rw-r--r--   0        0        0    11193 2024-04-26 14:45:23.770003 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py
--rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.771008 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py
--rw-r--r--   0        0        0     3368 2024-04-26 14:45:23.771078 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py
--rw-r--r--   0        0        0     5508 2024-04-26 14:45:23.772174 simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/params.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.773241 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/__init__.py
--rw-r--r--   0        0        0      978 2024-04-29 02:14:00.679279 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/frequency_domain/__init__.py
--rw-r--r--   0        0        0     8022 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/frequency_domain/constants.py
--rw-r--r--   0        0        0     1320 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/frequency_domain/driver.py
--rw-r--r--   0        0        0     5676 2024-04-26 14:45:23.775408 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/frequency_domain/params.py
--rw-r--r--   0        0        0      973 2024-04-29 02:14:00.668402 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/time_domain/__init__.py
--rw-r--r--   0        0        0     9507 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/time_domain/constants.py
--rw-r--r--   0        0        0     1300 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/time_domain/driver.py
--rw-r--r--   0        0        0     6307 2024-04-26 14:45:23.777654 simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/time_domain/params.py
--rw-r--r--   0        0        0     3121 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/constants.py
--rw-r--r--   0        0        0     8448 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/driver.py
--rw-r--r--   0        0        0      965 2024-04-29 02:14:00.630255 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_cross_gradient/__init__.py
--rw-r--r--   0        0        0     6884 2024-04-26 14:45:23.780891 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_cross_gradient/constants.py
--rw-r--r--   0        0        0     9514 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_cross_gradient/driver.py
--rw-r--r--   0        0        0     2789 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_cross_gradient/params.py
--rw-r--r--   0        0        0      959 2024-04-29 02:14:00.702198 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_surveys/__init__.py
--rw-r--r--   0        0        0     4669 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_surveys/constants.py
--rw-r--r--   0        0        0     4940 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_surveys/driver.py
--rw-r--r--   0        0        0     2126 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_surveys/params.py
--rw-r--r--   0        0        0     3644 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b1/simpeg_drivers/joint/params.py
--rw-r--r--   0        0        0     8892 2024-04-26 14:45:23.786252 simpeg_drivers-0.1.0b1/simpeg_drivers/line_sweep/driver.py
--rw-r--r--   0        0        0     1007 2024-04-29 02:14:00.690154 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/__init__.py
--rw-r--r--   0        0        0      963 2024-04-29 02:14:00.673785 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/magnetotellurics/__init__.py
--rw-r--r--   0        0        0    17280 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/magnetotellurics/constants.py
--rw-r--r--   0        0        0     1260 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/magnetotellurics/driver.py
--rw-r--r--   0        0        0    10843 2024-04-26 14:45:23.789513 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/magnetotellurics/params.py
--rw-r--r--   0        0        0      953 2024-04-29 02:14:00.684640 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/tipper/__init__.py
--rw-r--r--   0        0        0    10148 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/tipper/constants.py
--rw-r--r--   0        0        0     1220 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/tipper/driver.py
--rw-r--r--   0        0        0     7359 2024-04-26 14:45:23.791658 simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/tipper/params.py
--rw-r--r--   0        0        0    20664 2024-04-26 14:45:23.792706 simpeg_drivers-0.1.0b1/simpeg_drivers/params.py
--rw-r--r--   0        0        0     1078 2024-04-29 02:14:00.706667 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/__init__.py
--rw-r--r--   0        0        0      954 2024-04-29 02:14:00.716496 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/gravity/__init__.py
--rw-r--r--   0        0        0    18355 2024-04-26 14:45:23.793880 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/gravity/constants.py
--rw-r--r--   0        0        0     1224 2024-04-26 14:45:23.795051 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/gravity/driver.py
--rw-r--r--   0        0        0     9715 2024-04-26 14:45:23.796179 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/gravity/params.py
--rw-r--r--   0        0        0      961 2024-04-29 02:14:00.586879 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py
--rw-r--r--   0        0        0    19126 2024-04-26 14:45:23.797274 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_scalar/constants.py
--rw-r--r--   0        0        0     1252 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_scalar/driver.py
--rw-r--r--   0        0        0    11229 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_scalar/params.py
--rw-r--r--   0        0        0      961 2024-04-29 02:14:00.658721 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_vector/__init__.py
--rw-r--r--   0        0        0    21697 2024-04-26 14:45:23.800544 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_vector/constants.py
--rw-r--r--   0        0        0     2522 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_vector/driver.py
--rw-r--r--   0        0        0    12279 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_vector/params.py
--rw-r--r--   0        0        0      864 2024-04-26 14:45:23.802683 simpeg_drivers-0.1.0b1/simpeg_drivers/utils/__init__.py
--rw-r--r--   0        0        0     6760 2024-04-29 01:49:04.877716 simpeg_drivers-0.1.0b1/simpeg_drivers/utils/surveys.py
--rw-r--r--   0        0        0    17509 2024-04-26 14:45:23.804857 simpeg_drivers-0.1.0b1/simpeg_drivers/utils/testing.py
--rw-r--r--   0        0        0    27897 2024-04-29 01:49:00.210738 simpeg_drivers-0.1.0b1/simpeg_drivers/utils/utils.py
--rw-r--r--   0        0        0      944 2024-04-26 14:45:23.726759 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/__init__.py
--rw-r--r--   0        0        0      216 2024-04-24 21:13:56.506158 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/colortable.csv
--rw-r--r--   0        0        0  3108380 2024-04-24 21:13:58.874200 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/inversion_demo.geoh5
--rw-r--r--   0        0        0      109 2024-04-24 21:13:57.168793 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/time_channels.txt
--rw-r--r--   0        0        0     6004 2024-04-26 14:45:23.727858 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json
--rw-r--r--   0        0        0     4504 2024-04-26 14:45:23.727858 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json
--rw-r--r--   0        0        0     6052 2024-04-26 14:45:23.728954 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json
--rw-r--r--   0        0        0    14041 2024-04-26 14:45:23.728954 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json
--rw-r--r--   0        0        0    13494 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json
--rw-r--r--   0        0        0    14265 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json
--rw-r--r--   0        0        0     3788 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/fem_forward.ui.json
--rw-r--r--   0        0        0    13429 2024-04-26 14:45:23.731042 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/fem_inversion.ui.json
--rw-r--r--   0        0        0     6267 2024-04-26 14:45:23.731042 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/gravity_forward.ui.json
--rw-r--r--   0        0        0    20665 2024-04-26 14:45:23.732150 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/gravity_inversion.ui.json
--rw-r--r--   0        0        0     6083 2024-04-26 14:45:23.732150 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json
--rw-r--r--   0        0        0     4915 2024-04-26 14:45:23.733154 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json
--rw-r--r--   0        0        0     6370 2024-04-26 14:45:23.733921 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json
--rw-r--r--   0        0        0    14301 2024-04-26 14:45:23.734093 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json
--rw-r--r--   0        0        0    13912 2024-04-26 14:45:23.734093 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json
--rw-r--r--   0        0        0    14596 2024-04-26 14:45:23.735158 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json
--rw-r--r--   0        0        0    12638 2024-04-26 14:45:23.735158 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json
--rw-r--r--   0        0        0    12715 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json
--rw-r--r--   0        0        0     7075 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json
--rw-r--r--   0        0        0    21473 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json
--rw-r--r--   0        0        0     7896 2024-04-26 14:45:23.737413 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json
--rw-r--r--   0        0        0    23135 2024-04-26 14:45:23.737413 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json
--rw-r--r--   0        0        0     5966 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json
--rw-r--r--   0        0        0    19475 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json
--rw-r--r--   0        0        0     4262 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/tdem_forward.ui.json
--rw-r--r--   0        0        0    14381 2024-04-26 14:45:23.739597 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/tdem_inversion.ui.json
--rw-r--r--   0        0        0     5343 2024-04-26 14:45:23.739597 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/tipper_forward.ui.json
--rw-r--r--   0        0        0    16280 2024-04-26 14:45:23.740599 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/tipper_inversion.ui.json
--rw-r--r--   0        0        0      175 2024-04-24 21:13:57.169304 simpeg_drivers-0.1.0b1/simpeg_drivers-assets/waveform.txt
--rw-r--r--   0        0        0      800 2024-04-23 22:37:27.593550 simpeg_drivers-0.1.0b1/THIRD_PARTY_SOFTWARE.rst
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 simpeg_drivers-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-23 22:39:23.612815 simpeg_drivers-0.1.0b2/LICENSE
+-rw-r--r--   0        0        0     5102 2024-04-29 03:46:09.152350 simpeg_drivers-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     5466 2024-04-29 02:02:58.449338 simpeg_drivers-0.1.0b2/README.rst
+-rw-r--r--   0        0        0     3604 2024-04-29 03:35:10.574892 simpeg_drivers-0.1.0b2/simpeg_drivers/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-29 02:02:58.454666 simpeg_drivers-0.1.0b2/simpeg_drivers/components/__init__.py
+-rw-r--r--   0        0        0    20280 2024-04-26 14:45:23.742914 simpeg_drivers-0.1.0b2/simpeg_drivers/components/data.py
+-rw-r--r--   0        0        0     1231 2024-04-29 02:14:00.711152 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/__init__.py
+-rw-r--r--   0        0        0     1462 2024-04-26 14:45:23.744035 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/abstract_factory.py
+-rw-r--r--   0        0        0    21970 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/directives_factory.py
+-rw-r--r--   0        0        0     4382 2024-04-26 14:45:23.745132 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/entity_factory.py
+-rw-r--r--   0        0        0     5003 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/misfit_factory.py
+-rw-r--r--   0        0        0     7519 2024-04-26 14:45:23.746226 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/receiver_factory.py
+-rw-r--r--   0        0        0     3521 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/simpeg_factory.py
+-rw-r--r--   0        0        0     8146 2024-04-26 14:45:23.747226 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/simulation_factory.py
+-rw-r--r--   0        0        0     6142 2024-04-26 14:45:23.748321 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/source_factory.py
+-rw-r--r--   0        0        0    17787 2024-04-29 01:48:58.170502 simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/survey_factory.py
+-rw-r--r--   0        0        0     6476 2024-04-26 14:45:23.750330 simpeg_drivers-0.1.0b2/simpeg_drivers/components/locations.py
+-rw-r--r--   0        0        0     4799 2024-04-26 14:45:23.751485 simpeg_drivers-0.1.0b2/simpeg_drivers/components/meshes.py
+-rw-r--r--   0        0        0    16897 2024-04-26 14:45:23.751584 simpeg_drivers-0.1.0b2/simpeg_drivers/components/models.py
+-rw-r--r--   0        0        0     6135 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b2/simpeg_drivers/components/topography.py
+-rw-r--r--   0        0        0     1846 2024-04-26 14:45:23.752688 simpeg_drivers-0.1.0b2/simpeg_drivers/components/utils.py
+-rw-r--r--   0        0        0     4179 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b2/simpeg_drivers/components/windows.py
+-rw-r--r--   0        0        0    14591 2024-04-26 14:45:23.753785 simpeg_drivers-0.1.0b2/simpeg_drivers/constants.py
+-rw-r--r--   0        0        0    18654 2024-04-26 14:45:23.754889 simpeg_drivers-0.1.0b2/simpeg_drivers/driver.py
+-rw-r--r--   0        0        0     1112 2024-04-29 02:14:00.696694 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.755992 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/__init__.py
+-rw-r--r--   0        0        0    10334 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py
+-rw-r--r--   0        0        0     1506 2024-04-26 14:45:23.756990 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py
+-rw-r--r--   0        0        0     2680 2024-04-26 14:45:23.758085 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py
+-rw-r--r--   0        0        0      962 2024-04-29 02:14:00.601072 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py
+-rw-r--r--   0        0        0     9075 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py
+-rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py
+-rw-r--r--   0        0        0     2808 2024-04-26 14:45:23.760200 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/three_dimensions/params.py
+-rw-r--r--   0        0        0      911 2024-04-26 14:45:23.761252 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py
+-rw-r--r--   0        0        0    10879 2024-04-26 14:45:23.762303 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py
+-rw-r--r--   0        0        0     1256 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py
+-rw-r--r--   0        0        0     2646 2024-04-26 14:45:23.762376 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/two_dimensions/params.py
+-rw-r--r--   0        0        0     6721 2024-04-29 01:48:52.896367 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/driver.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.763466 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/__init__.py
+-rw-r--r--   0        0        0    10754 2024-04-26 14:45:23.764555 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py
+-rw-r--r--   0        0        0     1596 2024-04-26 14:45:23.765703 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py
+-rw-r--r--   0        0        0     3031 2024-04-26 14:45:23.766703 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py
+-rw-r--r--   0        0        0      968 2024-04-29 02:14:00.644863 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py
+-rw-r--r--   0        0        0     9362 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py
+-rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.767812 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py
+-rw-r--r--   0        0        0     3529 2024-04-26 14:45:23.768920 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py
+-rw-r--r--   0        0        0      968 2024-04-29 02:14:00.616156 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py
+-rw-r--r--   0        0        0    11193 2024-04-26 14:45:23.770003 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py
+-rw-r--r--   0        0        0     1280 2024-04-26 14:45:23.771008 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py
+-rw-r--r--   0        0        0     3368 2024-04-26 14:45:23.771078 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py
+-rw-r--r--   0        0        0     5508 2024-04-26 14:45:23.772174 simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/params.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.773241 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/__init__.py
+-rw-r--r--   0        0        0      978 2024-04-29 02:14:00.679279 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/frequency_domain/__init__.py
+-rw-r--r--   0        0        0     8022 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/frequency_domain/constants.py
+-rw-r--r--   0        0        0     1320 2024-04-26 14:45:23.774328 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/frequency_domain/driver.py
+-rw-r--r--   0        0        0     5676 2024-04-26 14:45:23.775408 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/frequency_domain/params.py
+-rw-r--r--   0        0        0      973 2024-04-29 02:14:00.668402 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/time_domain/__init__.py
+-rw-r--r--   0        0        0     9507 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/time_domain/constants.py
+-rw-r--r--   0        0        0     1300 2024-04-26 14:45:23.776468 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/time_domain/driver.py
+-rw-r--r--   0        0        0     6307 2024-04-26 14:45:23.777654 simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/time_domain/params.py
+-rw-r--r--   0        0        0     3121 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/constants.py
+-rw-r--r--   0        0        0     8448 2024-04-26 14:45:23.778652 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/driver.py
+-rw-r--r--   0        0        0      965 2024-04-29 02:14:00.630255 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_cross_gradient/__init__.py
+-rw-r--r--   0        0        0     6884 2024-04-26 14:45:23.780891 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_cross_gradient/constants.py
+-rw-r--r--   0        0        0     9514 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_cross_gradient/driver.py
+-rw-r--r--   0        0        0     2789 2024-04-26 14:45:23.781891 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_cross_gradient/params.py
+-rw-r--r--   0        0        0      959 2024-04-29 02:14:00.702198 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_surveys/__init__.py
+-rw-r--r--   0        0        0     4669 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_surveys/constants.py
+-rw-r--r--   0        0        0     4940 2024-04-26 14:45:23.784105 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_surveys/driver.py
+-rw-r--r--   0        0        0     2126 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_surveys/params.py
+-rw-r--r--   0        0        0     3644 2024-04-26 14:45:23.785104 simpeg_drivers-0.1.0b2/simpeg_drivers/joint/params.py
+-rw-r--r--   0        0        0     8892 2024-04-26 14:45:23.786252 simpeg_drivers-0.1.0b2/simpeg_drivers/line_sweep/driver.py
+-rw-r--r--   0        0        0     1007 2024-04-29 02:14:00.690154 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-29 02:14:00.673785 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/magnetotellurics/__init__.py
+-rw-r--r--   0        0        0    17280 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/magnetotellurics/constants.py
+-rw-r--r--   0        0        0     1260 2024-04-26 14:45:23.788410 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/magnetotellurics/driver.py
+-rw-r--r--   0        0        0    10843 2024-04-26 14:45:23.789513 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/magnetotellurics/params.py
+-rw-r--r--   0        0        0      953 2024-04-29 02:14:00.684640 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/tipper/__init__.py
+-rw-r--r--   0        0        0    10148 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/tipper/constants.py
+-rw-r--r--   0        0        0     1220 2024-04-26 14:45:23.790601 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/tipper/driver.py
+-rw-r--r--   0        0        0     7359 2024-04-26 14:45:23.791658 simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/tipper/params.py
+-rw-r--r--   0        0        0    20664 2024-04-26 14:45:23.792706 simpeg_drivers-0.1.0b2/simpeg_drivers/params.py
+-rw-r--r--   0        0        0     1078 2024-04-29 02:14:00.706667 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/__init__.py
+-rw-r--r--   0        0        0      954 2024-04-29 02:14:00.716496 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/gravity/__init__.py
+-rw-r--r--   0        0        0    18355 2024-04-26 14:45:23.793880 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/gravity/constants.py
+-rw-r--r--   0        0        0     1224 2024-04-26 14:45:23.795051 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/gravity/driver.py
+-rw-r--r--   0        0        0     9715 2024-04-26 14:45:23.796179 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/gravity/params.py
+-rw-r--r--   0        0        0      961 2024-04-29 02:14:00.586879 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py
+-rw-r--r--   0        0        0    19126 2024-04-26 14:45:23.797274 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_scalar/constants.py
+-rw-r--r--   0        0        0     1252 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_scalar/driver.py
+-rw-r--r--   0        0        0    11229 2024-04-26 14:45:23.798365 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_scalar/params.py
+-rw-r--r--   0        0        0      961 2024-04-29 02:14:00.658721 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_vector/__init__.py
+-rw-r--r--   0        0        0    21697 2024-04-26 14:45:23.800544 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_vector/constants.py
+-rw-r--r--   0        0        0     2522 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_vector/driver.py
+-rw-r--r--   0        0        0    12279 2024-04-26 14:45:23.801620 simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_vector/params.py
+-rw-r--r--   0        0        0      864 2024-04-26 14:45:23.802683 simpeg_drivers-0.1.0b2/simpeg_drivers/utils/__init__.py
+-rw-r--r--   0        0        0     6760 2024-04-29 01:49:04.877716 simpeg_drivers-0.1.0b2/simpeg_drivers/utils/surveys.py
+-rw-r--r--   0        0        0    17509 2024-04-26 14:45:23.804857 simpeg_drivers-0.1.0b2/simpeg_drivers/utils/testing.py
+-rw-r--r--   0        0        0    27897 2024-04-29 01:49:00.210738 simpeg_drivers-0.1.0b2/simpeg_drivers/utils/utils.py
+-rw-r--r--   0        0        0      944 2024-04-26 14:45:23.726759 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-24 21:13:56.506158 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/colortable.csv
+-rw-r--r--   0        0        0  3108380 2024-04-24 21:13:58.874200 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/inversion_demo.geoh5
+-rw-r--r--   0        0        0      109 2024-04-24 21:13:57.168793 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/time_channels.txt
+-rw-r--r--   0        0        0     6004 2024-04-26 14:45:23.727858 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json
+-rw-r--r--   0        0        0     4504 2024-04-26 14:45:23.727858 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json
+-rw-r--r--   0        0        0     6052 2024-04-26 14:45:23.728954 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json
+-rw-r--r--   0        0        0    14041 2024-04-26 14:45:23.728954 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json
+-rw-r--r--   0        0        0    13494 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json
+-rw-r--r--   0        0        0    14265 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json
+-rw-r--r--   0        0        0     3788 2024-04-26 14:45:23.729954 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/fem_forward.ui.json
+-rw-r--r--   0        0        0    13429 2024-04-26 14:45:23.731042 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/fem_inversion.ui.json
+-rw-r--r--   0        0        0     6267 2024-04-26 14:45:23.731042 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/gravity_forward.ui.json
+-rw-r--r--   0        0        0    20665 2024-04-26 14:45:23.732150 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/gravity_inversion.ui.json
+-rw-r--r--   0        0        0     6083 2024-04-26 14:45:23.732150 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json
+-rw-r--r--   0        0        0     4915 2024-04-26 14:45:23.733154 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json
+-rw-r--r--   0        0        0     6370 2024-04-26 14:45:23.733921 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json
+-rw-r--r--   0        0        0    14301 2024-04-26 14:45:23.734093 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json
+-rw-r--r--   0        0        0    13912 2024-04-26 14:45:23.734093 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json
+-rw-r--r--   0        0        0    14596 2024-04-26 14:45:23.735158 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json
+-rw-r--r--   0        0        0    12638 2024-04-26 14:45:23.735158 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json
+-rw-r--r--   0        0        0    12715 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json
+-rw-r--r--   0        0        0     7075 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json
+-rw-r--r--   0        0        0    21473 2024-04-26 14:45:23.736318 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json
+-rw-r--r--   0        0        0     7896 2024-04-26 14:45:23.737413 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json
+-rw-r--r--   0        0        0    23135 2024-04-26 14:45:23.737413 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json
+-rw-r--r--   0        0        0     5966 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json
+-rw-r--r--   0        0        0    19475 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json
+-rw-r--r--   0        0        0     4262 2024-04-26 14:45:23.738495 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/tdem_forward.ui.json
+-rw-r--r--   0        0        0    14381 2024-04-26 14:45:23.739597 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/tdem_inversion.ui.json
+-rw-r--r--   0        0        0     5343 2024-04-26 14:45:23.739597 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/tipper_forward.ui.json
+-rw-r--r--   0        0        0    16280 2024-04-26 14:45:23.740599 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/tipper_inversion.ui.json
+-rw-r--r--   0        0        0      175 2024-04-24 21:13:57.169304 simpeg_drivers-0.1.0b2/simpeg_drivers-assets/waveform.txt
+-rw-r--r--   0        0        0      800 2024-04-23 22:37:27.593550 simpeg_drivers-0.1.0b2/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 simpeg_drivers-0.1.0b2/PKG-INFO
```

### Comparing `simpeg_drivers-0.1.0b1/LICENSE` & `simpeg_drivers-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/pyproject.toml` & `simpeg_drivers-0.1.0b2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simpeg-drivers"
-version = "0.1.0-beta.1"
+version = "0.1.0-beta.2"
 description = "Application to run SimPEG inversions with geoh5 files from Geoscience Analyst."
 license = "MIT"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 maintainers = [
     "Benjamin Kary <benjamink@mirageoscience.com>",
     "Dominique Fournier <dominiquef@mirageoscience.com>",
 ]
@@ -36,15 +36,15 @@
 
 ## Pip dependencies from Git repositories
 #----------------------------------------
 geoh5py = {version = "~0.9.0rc1", source = "pypi", allow-prereleases = true}
 #geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
 #geoh5py = {url = "http://localhost:8888/geoh5py.tar.gz#sha256="}
 
-octree-creation-app = {version = "~0.1.0rc1", source = "pypi", allow-prereleases = true}
+octree-creation-app = {version = "~0.1.0rc2", source = "pypi", allow-prereleases = true}
 #octree-creation-app = {url = "https://github.com/MiraGeoscience/octree-creation-app/archive/refs/heads/release/0.1.0.zip#sha256="}
 #octree-creation-app = {url = "http://localhost:8888/octree-creation-app.tar.gz#sha256="}
 
 geoapps-utils = {version = "~0.3.0rc1", source = "pypi", allow-prereleases = true}
 #geoapps-utils = {url = "https://github.com/MiraGeoscience/geoapps-utils/archive/refs/heads/release/0.3.0.zip#sha256="}
 #geoapps-utils = {url = "http://localhost:8888/geoapps-utils.tar.gz#sha256="}
 
@@ -58,17 +58,19 @@
 
 ## indirect dependencies, forcing them here for installation through Conda not pip
 #---------------------------------------------------------------------------------
 Pillow = "~10.1.0"  # from geoh5py
 geoana = "~0.4.0"  # from simpeg
 h5py = "^3.2.1"  # from geoh5py
 mkl = "2022.1.*"  # from simpeg
+pandas = "~2.2.1"  # from SimPEG, also used by targeting-workflow, petro-lingo
 pydantic = "~2.5.2"  # from geoapps-utils
 pydiso = "~0.0.3"  # from simpeg
 pymatsolver = "~0.2.0"  # from simpeg
+scikit-learn = "~1.4.0"  # from SimPEG, also used by geo-unsup-mapper, petro-lingo
 tqdm = "^4.66.1"  # from simpeg
 zarr = "~2.14.2"  # from simpeg using Dask
 
 # force some versions to resolve incompatible resolution between PyPI and Conda
 tzdata = "2023.4"  # through pandas from SimPEG
 
 ## about pip dependencies
```

### Comparing `simpeg_drivers-0.1.0b1/README.rst` & `simpeg_drivers-0.1.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 # pylint: disable=unused-import
 # flake8: noqa
 
 from __future__ import annotations
 
-__version__ = "0.1.0-beta.1"
+__version__ = "0.1.0-beta.2"
 
 from pathlib import Path
 
 from SimPEG import dask
 
 from simpeg_drivers.constants import default_ui_json
 from simpeg_drivers.params import InversionBaseParams
```

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/data.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/data.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/abstract_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/abstract_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/directives_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/directives_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/entity_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/entity_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/misfit_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/misfit_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/receiver_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/receiver_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/simpeg_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/simpeg_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/simulation_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/simulation_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/source_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/factories/survey_factory.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/factories/survey_factory.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/locations.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/locations.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/meshes.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/meshes.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/models.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/models.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/topography.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/topography.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/utils.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/utils.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/components/windows.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/components/windows.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/pseudo_three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/three_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/three_dimensions/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/two_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/two_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/two_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/direct_current/two_dimensions/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/direct_current/two_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/pseudo_three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/three_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/three_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/three_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/three_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/two_dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/two_dimensions/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/two_dimensions/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/induced_polarization/two_dimensions/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electricals/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electricals/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/frequency_domain/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/frequency_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/frequency_domain/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/frequency_domain/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/frequency_domain/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/frequency_domain/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/frequency_domain/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/frequency_domain/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/time_domain/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/time_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/time_domain/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/time_domain/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/time_domain/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/time_domain/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/electromagnetics/time_domain/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/electromagnetics/time_domain/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_cross_gradient/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_cross_gradient/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_cross_gradient/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_cross_gradient/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_cross_gradient/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_cross_gradient/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_cross_gradient/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_cross_gradient/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_surveys/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_surveys/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_surveys/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_surveys/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_surveys/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/joint_surveys/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/joint_surveys/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/joint/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/joint/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/line_sweep/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/line_sweep/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/magnetotellurics/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/magnetotellurics/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/magnetotellurics/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/magnetotellurics/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/magnetotellurics/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/magnetotellurics/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/magnetotellurics/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/magnetotellurics/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/tipper/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/tipper/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/tipper/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/tipper/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/tipper/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/tipper/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/natural_sources/tipper/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/natural_sources/tipper/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/gravity/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/gravity/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/gravity/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/gravity/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/gravity/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/gravity/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/gravity/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/gravity/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_scalar/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_scalar/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_scalar/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_scalar/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_scalar/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_scalar/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_scalar/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_vector/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_vector/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_vector/constants.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_vector/constants.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_vector/driver.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_vector/driver.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/potential_fields/magnetic_vector/params.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/potential_fields/magnetic_vector/params.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/utils/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/utils/surveys.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/utils/surveys.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/utils/testing.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/utils/testing.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers/utils/utils.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers/utils/utils.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/__init__.py` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/inversion_demo.geoh5` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/inversion_demo.geoh5`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_forward_2d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_forward_3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_forward_pseudo3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_inversion_2d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_inversion_3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/direct_current_inversion_pseudo3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/fem_forward.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/fem_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/fem_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/fem_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/gravity_forward.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/gravity_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/gravity_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/gravity_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_forward_2d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_forward_3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_forward_pseudo3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_inversion_2d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_inversion_3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/induced_polarization_inversion_pseudo3d.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/joint_cross_gradient_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/joint_surveys_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetic_scalar_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetic_scalar_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetic_vector_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetic_vector_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetotellurics_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/magnetotellurics_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/tdem_forward.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/tdem_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/tdem_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/tdem_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/tipper_forward.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/tipper_forward.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/simpeg_drivers-assets/uijson/tipper_inversion.ui.json` & `simpeg_drivers-0.1.0b2/simpeg_drivers-assets/uijson/tipper_inversion.ui.json`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/THIRD_PARTY_SOFTWARE.rst` & `simpeg_drivers-0.1.0b2/THIRD_PARTY_SOFTWARE.rst`

 * *Files identical despite different names*

### Comparing `simpeg_drivers-0.1.0b1/PKG-INFO` & `simpeg_drivers-0.1.0b2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpeg-drivers
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Application to run SimPEG inversions with geoh5 files from Geoscience Analyst.
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: MIT
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Benjamin Kary
 Maintainer-email: benjamink@mirageoscience.com
@@ -19,18 +19,20 @@
 Requires-Dist: geoana (>=0.4.0,<0.5.0)
 Requires-Dist: geoapps-utils (>=0.3.0rc1,<0.4.0)
 Requires-Dist: geoh5py (>=0.9.0rc1,<0.10.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: mira-simpeg (>=0.19.0.8a3,<0.20.0.0)
 Requires-Dist: mkl (==2022.1.*)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
-Requires-Dist: octree-creation-app (>=0.1.0rc1,<0.2.0)
+Requires-Dist: octree-creation-app (>=0.1.0rc2,<0.2.0)
+Requires-Dist: pandas (>=2.2.1,<2.3.0)
 Requires-Dist: param-sweeps (>=0.1.7rc1,<0.2.0)
 Requires-Dist: pydantic (>=2.5.2,<2.6.0)
 Requires-Dist: pydiso (>=0.0.3,<0.1.0)
 Requires-Dist: pymatsolver (>=0.2.0,<0.3.0)
+Requires-Dist: scikit-learn (>=1.4.0,<1.5.0)
 Requires-Dist: scipy (>=1.10.1,<1.11.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: tzdata (==2023.4)
 Requires-Dist: zarr (>=2.14.2,<2.15.0)
 Project-URL: Documentation, https://mirageoscience-simpeg-drivers.readthedocs-hosted.com/
 Project-URL: Repository, https://github.com/MiraGeoscience/simpeg-drivers
```

