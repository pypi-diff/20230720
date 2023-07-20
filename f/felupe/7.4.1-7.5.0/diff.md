# Comparing `tmp/felupe-7.4.1.tar.gz` & `tmp/felupe-7.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-7.4.1.tar", last modified: Tue May  2 21:52:01 2023, max compression
+gzip compressed data, was "felupe-7.5.0.tar", last modified: Thu Jul 20 20:19:39 2023, max compression
```

## Comparing `felupe-7.4.1.tar` & `felupe-7.5.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.849577 felupe-7.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-05-02 21:51:49.000000 felupe-7.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50264 2023-05-02 21:52:01.849577 felupe-7.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-05-02 21:51:49.000000 felupe-7.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-02 21:51:49.000000 felupe-7.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:52:01.849577 felupe-7.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.833577 felupe-7.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/_assembly/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_assembly/_mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/_basis/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_basis/_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/_field/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/_field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    17201 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/constitution/_user_materials_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_dual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_line_rectangle_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.841577 felupe-7.4.1/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.845577 felupe-7.4.1/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.845577 felupe-7.4.1/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.845577 felupe-7.4.1/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-02 21:51:49.000000 felupe-7.4.1/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.837577 felupe-7.4.1/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50264 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 21:52:01.000000 felupe-7.4.1/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:01.845577 felupe-7.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-05-02 21:51:49.000000 felupe-7.4.1/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.676153 felupe-7.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-07-20 20:19:30.000000 felupe-7.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50402 2023-07-20 20:19:39.676153 felupe-7.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-07-20 20:19:30.000000 felupe-7.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-20 20:19:30.000000 felupe-7.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:19:39.676153 felupe-7.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.660153 felupe-7.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.660153 felupe-7.5.0/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.664153 felupe-7.5.0/src/felupe/_assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23227 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_assembly/_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_assembly/_integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_assembly/_weak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.664153 felupe-7.5.0/src/felupe/_basis/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_basis/_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.664153 felupe-7.5.0/src/felupe/_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/_field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.664153 felupe-7.5.0/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/constitution/_user_materials_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.664153 felupe-7.5.0/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.668153 felupe-7.5.0/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.668153 felupe-7.5.0/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.668153 felupe-7.5.0/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.668153 felupe-7.5.0/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_line_rectangle_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.672153 felupe-7.5.0/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/quadrature/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.672153 felupe-7.5.0/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.672153 felupe-7.5.0/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.672153 felupe-7.5.0/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/tools/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 20:19:30.000000 felupe-7.5.0/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.660153 felupe-7.5.0/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50402 2023-07-20 20:19:39.000000 felupe-7.5.0/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-20 20:19:39.000000 felupe-7.5.0/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:19:39.000000 felupe-7.5.0/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 20:19:39.000000 felupe-7.5.0/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 20:19:39.000000 felupe-7.5.0/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:19:39.676153 felupe-7.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-20 20:19:30.000000 felupe-7.5.0/tests/test_tools.py
```

### Comparing `felupe-7.4.1/LICENSE` & `felupe-7.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/PKG-INFO` & `felupe-7.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.4.1
+Version: 7.5.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -791,19 +791,20 @@
 
 # Documentation
 The documentation is located [here](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 # Extension Packages
 The capabilities of FElupe may be enhanced with extension packages created by the community.
 
-| **Package** |                     **Description**                     |                **Link**               |
-|:-----------:|:-------------------------------------------------------:|:-------------------------------------:|
-|  tensortrax |     Math on (Hyper-Dual) Tensors with Trailing Axes     |  https://github.com/adtzlr/tensortrax |
-|    matADi   | Material Definition with Automatic Differentiation (AD) |    https://github.com/adtzlr/matadi   |
-|    FEplot   |             A visualization tool for FElupe             | https://github.com/ZAARAOUI999/feplot |
+|                    **Package**                          |                     **Description**                     |
+|:-------------------------------------------------------:|:-------------------------------------------------------:|
+|  [hyperelastic](https://github.com/adtzlr/hyperelastic) |     Constitutive hyperelastic material formulations     |
+|    [matadi](https://github.com/adtzlr/matadi)           | Material Definition with Automatic Differentiation (AD) |
+|  [tensortrax](https://github.com/adtzlr/tensortrax)     |     Math on (Hyper-Dual) Tensors with Trailing Axes     |
+|    [feplot](https://github.com/ZAARAOUI999/feplot)      |             A visualization tool for FElupe             |
 
 # Changelog
 All notable changes to this project will be documented in [this file](CHANGELOG.md). The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 # License
 FElupe - finite element analysis (C) 2023 Andreas Dutzler, Graz (Austria).
```

### Comparing `felupe-7.4.1/README.md` & `felupe-7.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -85,19 +85,20 @@
 
 # Documentation
 The documentation is located [here](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 # Extension Packages
 The capabilities of FElupe may be enhanced with extension packages created by the community.
 
-| **Package** |                     **Description**                     |                **Link**               |
-|:-----------:|:-------------------------------------------------------:|:-------------------------------------:|
-|  tensortrax |     Math on (Hyper-Dual) Tensors with Trailing Axes     |  https://github.com/adtzlr/tensortrax |
-|    matADi   | Material Definition with Automatic Differentiation (AD) |    https://github.com/adtzlr/matadi   |
-|    FEplot   |             A visualization tool for FElupe             | https://github.com/ZAARAOUI999/feplot |
+|                    **Package**                          |                     **Description**                     |
+|:-------------------------------------------------------:|:-------------------------------------------------------:|
+|  [hyperelastic](https://github.com/adtzlr/hyperelastic) |     Constitutive hyperelastic material formulations     |
+|    [matadi](https://github.com/adtzlr/matadi)           | Material Definition with Automatic Differentiation (AD) |
+|  [tensortrax](https://github.com/adtzlr/tensortrax)     |     Math on (Hyper-Dual) Tensors with Trailing Axes     |
+|    [feplot](https://github.com/ZAARAOUI999/feplot)      |             A visualization tool for FElupe             |
 
 # Changelog
 All notable changes to this project will be documented in [this file](CHANGELOG.md). The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 # License
 FElupe - finite element analysis (C) 2023 Andreas Dutzler, Graz (Austria).
```

#### html2text {}

```diff
@@ -79,26 +79,28 @@
 view.plot("Principal Values of Logarithmic Strain").show() ``` ![curve](https:/
 /user-images.githubusercontent.com/5793153/234382805-d9a56108-9dd7-4f57-a029-
 571a5a2486a4.svg) ![cube](https://user-images.githubusercontent.com/5793153/
 234405093-2f5201c1-3bba-46ee-bd91-af87813609d9.png) # Documentation The
 documentation is located [here](https://felupe.readthedocs.io/en/latest/
 ?badge=latest). # Extension Packages The capabilities of FElupe may be enhanced
 with extension packages created by the community. | **Package** |
-**Description** | **Link** | |:-----------:|:----------------------------------
----------------------:|:-------------------------------------:| | tensortrax |
-Math on (Hyper-Dual) Tensors with Trailing Axes | https://github.com/adtzlr/
-tensortrax | | matADi | Material Definition with Automatic Differentiation (AD)
-| https://github.com/adtzlr/matadi | | FEplot | A visualization tool for FElupe
-| https://github.com/ZAARAOUI999/feplot | # Changelog All notable changes to
-this project will be documented in [this file](CHANGELOG.md). The format is
-based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
-project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-# License FElupe - finite element analysis (C) 2023 Andreas Dutzler, Graz
-(Austria). This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by the Free
-Software Foundation, either version 3 of the License, or (at your option) any
-later version. This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
-or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for
-more details. You should have received a copy of the GNU General Public License
-along with this program. If not, see
+**Description** | |:-------------------------------------------------------:|:-
+------------------------------------------------------:| | [hyperelastic]
+(https://github.com/adtzlr/hyperelastic) | Constitutive hyperelastic material
+formulations | | [matadi](https://github.com/adtzlr/matadi) | Material
+Definition with Automatic Differentiation (AD) | | [tensortrax](https://
+github.com/adtzlr/tensortrax) | Math on (Hyper-Dual) Tensors with Trailing Axes
+| | [feplot](https://github.com/ZAARAOUI999/feplot) | A visualization tool for
+FElupe | # Changelog All notable changes to this project will be documented in
+[this file](CHANGELOG.md). The format is based on [Keep a Changelog](https://
+keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
+Versioning](https://semver.org/spec/v2.0.0.html). # License FElupe - finite
+element analysis (C) 2023 Andreas Dutzler, Graz (Austria). This program is free
+software: you can redistribute it and/or modify it under the terms of the GNU
+General Public License as published by the Free Software Foundation, either
+version 3 of the License, or (at your option) any later version. This program
+is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
+without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+PARTICULAR PURPOSE. See the GNU General Public License for more details. You
+should have received a copy of the GNU General Public License along with this
+program. If not, see
 www.gnu.org/licenses/>.
```

### Comparing `felupe-7.4.1/pyproject.toml` & `felupe-7.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/_assembly/_axi.py` & `felupe-7.5.0/src/felupe/_assembly/_axi.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,114 +16,100 @@
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from .._field._axi import FieldAxisymmetric
 from .._field._base import Field
-from ._base import IntegralForm
+from ._weak import WeakForm
 
 
-class IntegralFormAxisymmetric(IntegralForm):
+class IntegralFormAxisymmetric(WeakForm):
     def __init__(self, fun, v, dV, u=None, grad_v=True, grad_u=True):
-
         R = v.radius
         self.dV = 2 * np.pi * R * dV
 
         if u is None:
-
             if isinstance(v, FieldAxisymmetric):
-
                 self.mode = 1
 
                 if grad_v:
                     fun_2d = fun[:-1, :-1]
                     fun_zz = fun[(-1,), (-1,)] / R
                 else:
                     fun_2d = fun[:-1]
                     fun_zz = fun[-1].reshape(1, *fun[-1].shape) / R
 
-                form_a = IntegralForm(fun_2d, v, self.dV, grad_v=grad_v)
-                form_b = IntegralForm(fun_zz, v.scalar, self.dV)
+                form_a = WeakForm(fun_2d, v, self.dV, grad_v=grad_v)
+                form_b = WeakForm(fun_zz, v.scalar, self.dV)
 
                 self.forms = [form_a, form_b]
 
             else:
-
                 self.mode = 10
 
-                form_a = IntegralForm(fun, v, self.dV, grad_v=False)
+                form_a = WeakForm(fun, v, self.dV, grad_v=False)
                 self.forms = [
                     form_a,
                 ]
 
         else:
-
             if isinstance(v, FieldAxisymmetric) and isinstance(u, FieldAxisymmetric):
-
                 self.mode = 2
 
                 if grad_v and grad_u:
-
-                    form_aa = IntegralForm(
+                    form_aa = WeakForm(
                         fun[:-1, :-1, :-1, :-1], v, self.dV, u, True, True
                     )
-                    form_bb = IntegralForm(
+                    form_bb = WeakForm(
                         fun[-1, -1, -1, -1] / R**2,
                         v.scalar,
                         self.dV,
                         u.scalar,
                         False,
                         False,
                     )
-                    form_ba = IntegralForm(
+                    form_ba = WeakForm(
                         fun[-1, -1, :-1, :-1] / R, v.scalar, self.dV, u, False, True
                     )
-                    form_ab = IntegralForm(
+                    form_ab = WeakForm(
                         fun[:-1, :-1, -1, -1] / R, v, self.dV, u.scalar, True, False
                     )
 
                 if not grad_v and grad_u:
-
-                    form_aa = IntegralForm(
-                        fun[:-1, :-1, :-1], v, self.dV, u, False, True
-                    )
-                    form_bb = IntegralForm(
+                    form_aa = WeakForm(fun[:-1, :-1, :-1], v, self.dV, u, False, True)
+                    form_bb = WeakForm(
                         fun[-1, -1, -1] / R**2,
                         v.scalar,
                         self.dV,
                         u.scalar,
                         False,
                         False,
                     )
-                    form_ba = IntegralForm(
+                    form_ba = WeakForm(
                         fun[-1, :-1, :-1] / R, v.scalar, self.dV, u, False, True
                     )
-                    form_ab = IntegralForm(
+                    form_ab = WeakForm(
                         fun[:-1, -1, -1] / R, v, self.dV, u.scalar, False, False
                     )
 
                 self.forms = [form_aa, form_bb, form_ba, form_ab]
 
             elif isinstance(v, FieldAxisymmetric) and isinstance(u, Field):
-
                 self.mode = 30
 
-                form_a = IntegralForm(fun[:-1, :-1], v, self.dV, u, True, False)
-                form_b = IntegralForm(
-                    fun[-1, -1] / R, v.scalar, self.dV, u, False, False
-                )
+                form_a = WeakForm(fun[:-1, :-1], v, self.dV, u, True, False)
+                form_b = WeakForm(fun[-1, -1] / R, v.scalar, self.dV, u, False, False)
 
                 self.forms = [form_a, form_b]
 
             elif isinstance(v, Field) and isinstance(u, Field):
-
                 self.mode = 40
 
-                form_a = IntegralForm(fun, v, self.dV, u, False, False)
+                form_a = WeakForm(fun, v, self.dV, u, False, False)
 
                 self.forms = [
                     form_a,
                 ]
 
     def integrate(self, parallel=False):
         values = [form.integrate(parallel=parallel) for form in self.forms]
```

### Comparing `felupe-7.4.1/src/felupe/_assembly/_base.py` & `felupe-7.5.0/src/felupe/_assembly/_weak.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     from einsumt import einsumt
 except ModuleNotFoundError:
     from numpy import einsum as einsumt
 
 from scipy.sparse import csr_matrix as sparsematrix
 
 
-class IntegralForm:
-    r"""Integral Form constructed by a function result ``fun``,
+class WeakForm:
+    r"""Single-Field Integral-Form constructed by a function result ``fun``,
     a virtual field ``v``, differential volumes ``dV`` and optionally a
     field ``u``. For both fields ``v`` and ``u`` gradients may be passed by
     setting ``grad_v`` and ``grad_u`` to True (default is False for both).
 
     **Linearform**
 
     without gradient of ``v``
@@ -117,21 +117,21 @@
         # # linear form
         if not self.u:
             self.indices = self.v.indices.ai
             self.shape = self.v.indices.shape
 
         # # bilinear form
         else:
-            eai = self.v.indices.eai
-            ebk = self.u.indices.eai
+            cai = self.v.indices.cai
+            cbk = self.u.indices.cai
 
-            eaibk0 = np.repeat(eai, ebk.shape[1] * self.u.dim)
-            eaibk1 = np.tile(ebk, (1, eai.shape[1] * self.v.dim, 1)).ravel()
+            caibk0 = np.repeat(cai, cbk.shape[1] * self.u.dim)
+            caibk1 = np.tile(cbk, (1, cai.shape[1] * self.v.dim, 1)).ravel()
 
-            self.indices = (eaibk0, eaibk1)
+            self.indices = (caibk0, caibk1)
             self.shape = (self.v.indices.shape[0], self.u.indices.shape[0])
 
     def assemble(self, values=None, parallel=False):
         "Assembly of sparse region vectors or matrices."
 
         if values is None:
             values = self.integrate(parallel=parallel)
@@ -177,38 +177,36 @@
         if u is not None:
             if not grad_u:
                 ub = u.region.h
             else:
                 ub = u.region.dhdX
 
         if u is None:
-
             if not grad_v:
-                return einsum("ape,...pe,pe->a...e", vb, fun, dV, optimize=True)
+                return einsum("aqc,...qc,qc->a...c", vb, fun, dV, optimize=True)
             else:
-                return einsum("aJpe,...Jpe,pe->a...e", vb, fun, dV, optimize=True)
+                return einsum("aJqc,...Jqc,qc->a...c", vb, fun, dV, optimize=True)
 
         else:
-
             if not grad_v and not grad_u:
-                out = einsum("ape,...pe,bpe,pe->a...be", vb, fun, ub, dV, optimize=True)
+                out = einsum("aqc,...qc,bqc,qc->a...bc", vb, fun, ub, dV, optimize=True)
                 if len(out.shape) == 5:
-                    return einsum("aijbe->aibje", out)
+                    return einsum("aijbc->aibjc", out)
                 else:
                     return out
             elif grad_v and not grad_u:
                 return einsum(
-                    "aJpe,iJ...pe,bpe,pe->aib...e", vb, fun, ub, dV, optimize=True
+                    "aJqc,iJ...qc,bqc,qc->aib...c", vb, fun, ub, dV, optimize=True
                 )
             elif not grad_v and grad_u:
                 return einsum(
-                    "a...pe,...kLpe,bLpe,pe->a...bke",
+                    "a...qc,...kLqc,bLqc,qc->a...bkc",
                     vb,
                     fun,
                     ub,
                     dV,
                     optimize=True,
                 )
             else:  # grad_v and grad_u
                 return einsum(
-                    "aJpe,iJkLpe,bLpe,pe->aibke", vb, fun, ub, dV, optimize=True
+                    "aJqc,iJkLqc,bLqc,qc->aibkc", vb, fun, ub, dV, optimize=True
                 )
```

### Comparing `felupe-7.4.1/src/felupe/_assembly/_form.py` & `felupe-7.5.0/src/felupe/_assembly/_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 """
 
 from threading import Thread
 
 import numpy as np
 
 from .._basis import BasisMixed
-from ._base import IntegralForm
-from ._mixed import IntegralFormMixed
+from ._integral import IntegralForm
+from ._weak import WeakForm
 
 
 class LinearForm:
     r"""A linear form object with methods for integration and assembly of
     vectors.
 
     ..  math::
@@ -47,15 +47,15 @@
         self.v = v
         self.grad_v = grad_v
         if dx is None:
             self.dx = v.field.region.dV
         else:
             self.dx = dx
 
-        self._form = IntegralForm(fun=None, v=v.field, dV=self.dx, grad_v=grad_v)
+        self._form = WeakForm(fun=None, v=v.field, dV=self.dx, grad_v=grad_v)
 
     def integrate(self, weakform, args=(), kwargs={}, parallel=False):
         r"""Return evaluated (but not assembled) integrals.
 
         Parameters
         ----------
         weakform : callable
@@ -77,15 +77,14 @@
             v = self.v.grad
         else:
             v = self.v.basis
 
         values = np.zeros((len(v), *v.shape[-3:]))
 
         if not parallel:
-
             for a, vbasis in enumerate(v):
                 for i, vb in enumerate(vbasis):
                     values[a, i] = weakform(vb, *args, **kwargs) * self.dx
 
         else:
             idx_a, idx_i = np.indices(values.shape[:2])
             ai = zip(idx_a.ravel(), idx_i.ravel())
@@ -158,15 +157,15 @@
         self.u = u
         self.grad_u = grad_u
         if dx is None:
             self.dx = v.field.region.dV
         else:
             self.dx = dx
 
-        self._form = IntegralForm(None, v.field, self.dx, u.field, grad_v, grad_u)
+        self._form = WeakForm(None, v.field, self.dx, u.field, grad_v, grad_u)
 
     def integrate(self, weakform, args=(), kwargs={}, parallel=False, sym=False):
         r"""Return evaluated (but not assembled) integrals.
 
         Parameters
         ----------
         weakform : callable
@@ -195,55 +194,46 @@
             u = self.u.grad
         else:
             u = self.u.basis
 
         values = np.zeros((len(v), v.shape[-4], len(u), u.shape[-4], *u.shape[-2:]))
 
         if not parallel:
-
             for a, vbasis in enumerate(v):
                 for i, vb in enumerate(vbasis):
-
                     for b, ubasis in enumerate(u):
                         for j, ub in enumerate(ubasis):
-
                             if sym:
-
                                 if len(vbasis) * a + i <= len(ubasis) * b + j:
-
                                     values[a, i, b, j] = values[b, j, a, i] = (
                                         weakform(vb, ub, *args, **kwargs) * self.dx
                                     )
 
                             else:
-
                                 values[a, i, b, j] = (
                                     weakform(vb, ub, *args, **kwargs) * self.dx
                                 )
 
         else:
-
             idx_a, idx_i, idx_b, idx_j = np.indices(values.shape[:4])
             aibj = zip(idx_a.ravel(), idx_i.ravel(), idx_b.ravel(), idx_j.ravel())
 
             if sym:
-
                 len_vbasis = values.shape[1]
                 len_ubasis = values.shape[3]
 
                 mask = len_vbasis * idx_a + idx_i <= len_ubasis * idx_b + idx_j
                 idx_a, idx_i, idx_b, idx_j = (
                     idx_a[mask],
                     idx_i[mask],
                     idx_b[mask],
                     idx_j[mask],
                 )
 
             def contribution(values, a, i, b, j, sym, args, kwargs):
-
                 if sym:
                     values[a, i, b, j] = values[b, j, a, i] = (
                         weakform(v[a, i], u[b, j], *args, **kwargs) * self.dx
                     )
 
                 else:
                     values[a, i, b, j] = (
@@ -309,15 +299,15 @@
 
 
     """
 
     def __init__(self, v, grad_v=None):
         self.v = v
         self.dx = self.v.field[0].region.dV
-        self._form = IntegralFormMixed(
+        self._form = IntegralForm(
             np.zeros(len(v.field.fields)), self.v.field, self.dx, grad_v=grad_v
         )
 
         if grad_v is None:
             self.grad_v = np.zeros_like(self.v.field.fields, dtype=bool)
             self.grad_v[0] = True
         else:
@@ -412,27 +402,26 @@
                 grad = np.zeros_like(fields, dtype=bool)
                 grad[0] = True
             return grad
 
         self.grad_v = _set_first_grad_true(grad_v, self.v.field.fields)
         self.grad_u = _set_first_grad_true(grad_u, self.u.field.fields)
 
-        self._form = IntegralFormMixed(
+        self._form = IntegralForm(
             fun=np.zeros(len(self.i)),
             v=self.v.field,
             dV=self.dx,
             u=self.u.field,
             grad_v=self.grad_v,
             grad_u=self.grad_u,
         )
 
         self._bilinearform = []
 
         for a, (i, j) in enumerate(zip(self.i, self.j)):
-
             self._bilinearform.append(
                 BilinearForm(
                     v=self.v[i],
                     u=self.u[j],
                     grad_v=self.grad_v[i],
                     grad_u=self.grad_u[j],
                     dx=self.dx,
@@ -538,15 +527,14 @@
         grad_v=False,
         grad_u=False,
         dx=None,
         args=(),
         kwargs={},
         parallel=False,
     ):
-
         # set attributes
         self.form = None
         self.grad_u = grad_u
         self.grad_v = grad_v
         self.dx = dx
         self.weakform = weakform
 
@@ -554,15 +542,14 @@
         self._init_or_update_forms(v, u, args, kwargs, parallel)
 
     def _init_or_update_forms(self, v, u, args, kwargs, parallel):
         "Init or update the underlying form object."
 
         # update args and kwargs for weakform
         if args is not None or kwargs is not None:
-
             if args is not None:
                 self.args = args
             else:
                 self.args = ()
 
             if kwargs is not None:
                 self.kwargs = kwargs
@@ -572,30 +559,27 @@
         # get current form type
         if self.form is not None:
             form_type = type(self.form)
         else:
             form_type = None
 
         if v is not None:
-
             # linear form
             if u is None:
-
                 self.u = None
 
                 # mixed-field input
                 self.v = BasisMixed(v, parallel=parallel)
                 form = LinearFormMixed(self.v, self.grad_v)
 
                 # evaluate weakform to list of weakforms
                 if isinstance(self.weakform, type(lambda x: x)):
                     self.weakform = self.weakform()
 
             else:
-
                 self.v = BasisMixed(v, parallel=parallel)
                 self.u = BasisMixed(u, parallel=parallel)
                 form = BilinearFormMixed(self.v, self.u, self.grad_v, self.grad_u)
 
                 # evaluate weakform to list of weakforms
                 if isinstance(self.weakform, type(lambda x: x)):
                     self.weakform = self.weakform()
@@ -736,15 +720,14 @@
     BaseForm
         A form object based on LinearForm, LinearFormMixed, BilinearForm or
         BilinearFormMixed with methods for integration and assembly.
 
     """
 
     def form(weakform):
-
         return BaseForm(
             weakform=weakform,
             v=v,
             u=u,
             grad_v=grad_v,
             grad_u=grad_u,
             dx=dx,
```

### Comparing `felupe-7.4.1/src/felupe/_assembly/_mixed.py` & `felupe-7.5.0/src/felupe/_assembly/_integral.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,35 +19,34 @@
 import numpy as np
 from scipy.sparse import bmat, vstack
 
 from .._field._axi import FieldAxisymmetric
 from .._field._base import Field
 from .._field._planestrain import FieldPlaneStrain
 from ._axi import IntegralFormAxisymmetric
-from ._base import IntegralForm
+from ._weak import WeakForm
 
 
-class IntegralFormMixed:
+class IntegralForm:
     def __init__(self, fun, v, dV, u=None, grad_v=None, grad_u=None):
-
         self.fun = fun
         self.v = v.fields
         self.nv = len(self.v)
         self.dV = dV
 
         if u is not None:
             self.u = u.fields
             self.nu = len(self.u)
         else:
             self.u = None
             self.nu = None
 
         IntForm = {
-            Field: IntegralForm,
-            FieldPlaneStrain: IntegralForm,
+            Field: WeakForm,
+            FieldPlaneStrain: WeakForm,
             FieldAxisymmetric: IntegralFormAxisymmetric,
         }[type(self.v[0])]
 
         if isinstance(self.v[0], FieldAxisymmetric):
             for i in range(1, len(self.v)):
                 self.v[i].radius = self.v[0].radius
 
@@ -90,15 +89,14 @@
                     grad_u=self.grad_u[j],
                 )
                 self.forms.append(f)
         else:
             raise ValueError("Unknown input format.")
 
     def assemble(self, values=None, parallel=False, block=True):
-
         out = []
 
         if values is None:
             values = [None] * len(self.forms)
 
         for val, form in zip(values, self.forms):
             out.append(form.assemble(val, parallel=parallel))
@@ -115,13 +113,12 @@
         if block and self.mode == 1:
             return vstack(out).tocsr()
 
         else:
             return out
 
     def integrate(self, parallel=False):
-
         out = []
         for form in self.forms:
             out.append(form.integrate(parallel=parallel))
 
         return out
```

### Comparing `felupe-7.4.1/src/felupe/_basis/_basis.py` & `felupe-7.5.0/src/felupe/_basis/_basis.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 class Basis:
     r"""A basis and its gradient built on top of a scalar- or vector-valued
     field. *Basis* refers to the trial and test field, either values or
     gradients evaluated at quadrature points. The first two indices of a basis
     are used for looping over the element shape functions ``a`` and its
     components ``i``. The third index represents the vector component ``j`` of
-    the field. The two trailing axes ``(p, c)`` contain the evaluated element
-    shape functions at quadrature points ``p`` per cell ``c``.
+    the field. The two trailing axes ``(q, c)`` contain the evaluated element
+    shape functions at quadrature points ``q`` per cell ``c``.
 
     ..  math::
 
         \varphi_{aijpc} = \delta_{ij} \left( h_a \right)_{pc}
 
 
     For gradients, the fourth index is used for the vector component of the
@@ -59,42 +59,41 @@
         The evaluated basis functions at quadrature points.
     grad : ndarray
         The evaluated gradient of the basis (if provided by the region).
 
     """
 
     def __init__(self, field, parallel=False):
-
         self.field = field
 
         einsum = einsumt if parallel else np.einsum
 
         self.basis = einsum(
-            "ij,apc->aijpc",
+            "ij,aqc->aijqc",
             np.eye(self.field.dim),
             self.field.region.h,
         )
 
         if hasattr(self.field.region, "dhdX"):
             self.grad = einsum(
-                "ij,akpc->aijkpc", np.eye(self.field.dim), self.field.region.dhdX
+                "ij,akqc->aijkqc", np.eye(self.field.dim), self.field.region.dhdX
             )
 
         else:
             self.grad = None
 
 
 class BasisMixed:
     r"""A basis and its gradient built on top of a scalar- or vector-valued
     field container. *Basis* refers to the trial and test field, either values or
     gradients evaluated at quadrature points. The first two indices of a basis
     are used for looping over the element shape functions ``a`` and its
     components ``i``. The third index represents the vector component ``j`` of
-    the field. The two trailing axes ``(p, c)`` contain the evaluated element
-    shape functions at quadrature points ``p`` per cell ``c``.
+    the field. The two trailing axes ``(q, c)`` contain the evaluated element
+    shape functions at quadrature points ``q`` per cell ``c``.
 
     ..  math::
 
         \varphi_{aijpc} = \delta_{ij} \left( h_a \right)_{pc}
 
 
     For gradients, the fourth index is used for the vector component of the
@@ -116,15 +115,14 @@
         The evaluated basis functions at quadrature points.
     grad : ndarray
         The evaluated gradient of the basis (if provided by the region).
 
     """
 
     def __init__(self, field, parallel=False):
-
         self.field = field
         self.basis = [Basis(f, parallel=parallel) for f in self.field]
 
     def __getitem__(self, idx):
         "Slice-based access to underlying bases."
 
         return self.basis[idx]
```

### Comparing `felupe-7.4.1/src/felupe/_field/_axi.py` & `felupe-7.5.0/src/felupe/_field/_axi.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,18 @@
         self.radius = self.scalar.interpolate()
 
     def _interpolate_2d(self):
         """Interpolate 2D field values at points and evaluate them at the
         integration points of all cells in the region."""
 
         # interpolated field values "aI"
-        # evaluated at quadrature point "p"
+        # evaluated at quadrature point "q"
         # for cell "c"
         return np.einsum(
-            "ca...,apc->...pc", self.values[self.region.mesh.cells], self.region.h
+            "ca...,aqc->...qc", self.values[self.region.mesh.cells], self.region.h
         )
 
     def interpolate(self):
         # extend dimension of in-plane 2d-gradient
         return np.pad(self._interpolate_2d(), ((0, 1), (0, 0), (0, 0)))
 
     def _grad_2d(self, sym=False):
@@ -120,18 +120,18 @@
         array
             In-plane 2D-gradient as partial derivative of field values at points
             w.r.t. undeformed coordinates, evaluated at the integration points
             of all cells in the region.
         """
 
         # gradient as partial derivative of field component "I" at point "a"
-        # w.r.t. undeformed coordinate "J" evaluated at quadrature point "p"
+        # w.r.t. undeformed coordinate "J" evaluated at quadrature point "q"
         # for each cell "e"
         g = np.einsum(
-            "ca...,aJpc->...Jpc",
+            "ca...,aJqc->...Jqc",
             self.values[self.region.mesh.cells],
             self.region.dhdX,
         )
 
         if sym:
             return symmetric(g)
         else:
```

### Comparing `felupe-7.4.1/src/felupe/_field/_base.py` & `felupe-7.5.0/src/felupe/_field/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 class Field:
     r"""A Field on points of a `region` with dimension `dim`
     and initial point `values`. A slice of this field directly
     accesses the field values as 1d-array.
 
     The interpolation method returns the field values evaluated at the
-    numeric integration points ``p`` of all cells ``c`` in the region.
+    numeric integration points ``q`` of all cells ``c`` in the region.
 
     ..  math::
 
         u^i_{(pc)} = \hat{u}_a^i h_{a(pc)}
 
     The gradient method returns the gradient of the field values w.r.t. the
     undeformed mesh point coordinates, evaluated at the integration points of
@@ -58,15 +58,14 @@
         shape (region.mesh.npoints, dim)`.
     kwargs : dict, optional
         Optional keyword arguments of the field.
 
     """
 
     def __init__(self, region, dim=1, values=0, **kwargs):
-
         self.region = region
         self.dim = dim
         self.shape = self.region.quadrature.npoints, self.region.mesh.ncells
 
         # set optional user-defined attributes
         for key, value in kwargs.items():
             setattr(self, key, value)
@@ -86,15 +85,15 @@
 
         eai, ai = self._indices_per_cell(self.region.mesh.cells, dim)
         self.indices = Indices(eai, ai, region, dim)
 
     def _indices_per_cell(self, cells, dim):
         "Calculate pre-defined indices for sparse matrices."
 
-        # index of cell "e", point "a" and component "i"
+        # index of cell "c", point "a" and component "i"
         eai = (
             dim * np.repeat(cells, dim) + np.tile(np.arange(dim), cells.size)
         ).reshape(*cells.shape, dim)
         # store indices as (rows, cols) (note: sparse-matrices are always 2d)
         ai = (eai.ravel(), np.zeros_like(eai.ravel()))
 
         return eai, ai
@@ -115,36 +114,36 @@
         array
             Gradient as partial derivative of field values at points w.r.t.
             undeformed coordinates, evaluated at the integration points of
             all cells in the region.
         """
 
         # gradient dudX_IJpe as partial derivative of field values at points "aI"
-        # w.r.t. undeformed coordinates "J" evaluated at quadrature point "p"
+        # w.r.t. undeformed coordinates "J" evaluated at quadrature point "q"
         # for each cell "c"
         g = np.einsum(
-            "ca...,aJpc->...Jpc",
+            "ca...,aJqc->...Jqc",
             self.values[self.region.mesh.cells],
             self.region.dhdX,
         )
 
         if sym:
             return symmetric(g)
         else:
             return g
 
     def interpolate(self):
         """Interpolate field values at points and evaluate them at the
         integration points of all cells in the region."""
 
         # interpolated field values "aI"
-        # evaluated at quadrature point "p"
+        # evaluated at quadrature point "q"
         # for cell "c"
         return np.einsum(
-            "ca...,apc->...pc", self.values[self.region.mesh.cells], self.region.h
+            "ca...,aqc->...qc", self.values[self.region.mesh.cells], self.region.h
         )
 
     def extract(self, grad=True, sym=False, add_identity=True):
         """Generalized extraction method which evaluates either the gradient
         or the field values at the integration points of all cells
         in the region. Optionally, the symmetric part of the gradient is
         evaluated and/or the identity matrix is added to the gradient.
@@ -184,114 +183,106 @@
         return deepcopy(self)
 
     def fill(self, a):
         "Fill all field values with a scalar value."
         self.values.fill(a)
 
     def __add__(self, newvalues):
-
         if isinstance(newvalues, np.ndarray):
             field = deepcopy(self)
             field.values += newvalues.reshape(-1, field.dim)
             return field
 
         elif isinstance(newvalues, Field):
             field = deepcopy(self)
             field.values += newvalues.values
             return field
 
         else:
             raise TypeError("Unknown type.")
 
     def __sub__(self, newvalues):
-
         if isinstance(newvalues, np.ndarray):
             field = deepcopy(self)
             field.values -= newvalues.reshape(-1, field.dim)
             return field
 
         elif isinstance(newvalues, Field):
             field = deepcopy(self)
             field.values -= newvalues.values
             return field
 
         else:
             raise TypeError("Unknown type.")
 
     def __mul__(self, newvalues):
-
         if isinstance(newvalues, np.ndarray):
             field = deepcopy(self)
             field.values *= newvalues.reshape(-1, field.dim)
             return field
 
         elif isinstance(newvalues, Field):
             field = deepcopy(self)
             field.values *= newvalues.values
             return field
 
         else:
             raise TypeError("Unknown type.")
 
     def __truediv__(self, newvalues):
-
         if isinstance(newvalues, np.ndarray):
             field = deepcopy(self)
             field.values /= newvalues.reshape(-1, field.dim)
             return field
 
         elif isinstance(newvalues, Field):
             field = deepcopy(self)
             field.values /= newvalues.values
             return field
 
         else:
             raise TypeError("Unknown type.")
 
     def __iadd__(self, newvalues):
-
         if isinstance(newvalues, np.ndarray):
             self.values += newvalues.reshape(-1, self.dim)
             return self
 
         elif isinstance(newvalues, Field):
             self.values += newvalues.values
             return self
 
         else:
             raise TypeError("Unknown type.")
 
     def __isub__(self, newvalues):
-
         if isinstance(newvalues, np.ndarray):
             self.values -= newvalues.reshape(-1, self.dim)
             return self
 
         elif isinstance(newvalues, Field):
             self.values -= newvalues.values
             return self
 
         else:
             raise TypeError("Unknown type.")
 
     def __imul__(self, newvalues):
-
         if isinstance(newvalues, np.ndarray):
             self.values *= newvalues.reshape(-1, self.dim)
             return self
 
         elif isinstance(newvalues, Field):
             self.values *= newvalues.values
             return self
 
         else:
             raise TypeError("Unknown type.")
 
     def __itruediv__(self, newvalues):
-
         if isinstance(newvalues, np.ndarray):
             self.values /= newvalues.reshape(-1, self.dim)
             return self
 
         elif isinstance(newvalues, Field):
             self.values /= newvalues.values
             return self
```

### Comparing `felupe-7.4.1/src/felupe/_field/_container.py` & `felupe-7.5.0/src/felupe/_field/_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 
 class FieldContainer:
     """A container for fields based on a list or tuple of :class:`Field`
     instances."""
 
     def __init__(self, fields):
-
         self.fields = fields
         self.region = fields[0].region
 
         # get sizes of fields and calculate offsets
         self.fieldsizes = [f.indices.dof.size for f in self.fields]
         self.offsets = np.cumsum(self.fieldsizes)[:-1]
```

### Comparing `felupe-7.4.1/src/felupe/_field/_fields.py` & `felupe-7.5.0/src/felupe/_field/_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,66 +77,68 @@
             Offset for cell connectivity (default is 0).
         npoints : int or None, optional
             Specified number of mesh points (default is None).
         mesh: Mesh or None, optional
             A mesh for the dual region (default is None).
         """
 
-        regions = {
-            RegionHexahedron: RegionConstantHexahedron,
-            RegionQuad: RegionConstantQuad,
-            RegionQuadraticQuad: RegionConstantQuad,
-            RegionBiQuadraticQuad: RegionQuad,
-            RegionQuadraticHexahedron: RegionConstantHexahedron,
-            RegionTriQuadraticHexahedron: RegionHexahedron,
-            RegionQuadraticTetra: RegionTetra,
-            RegionQuadraticTriangle: RegionTriangle,
-            RegionTetraMINI: RegionTetra,
-            RegionTriangleMINI: RegionTriangle,
-            RegionLagrange: RegionLagrange,
-        }
-        points_per_cell = {
-            RegionConstantHexahedron: 1,
-            RegionConstantQuad: 1,
-            RegionQuad: 4,
-            RegionHexahedron: 8,
-            RegionTriangle: 3,
-            RegionTetra: 4,
-            RegionLagrange: None,
-        }
-
-        kwargs0 = {}
-
-        if isinstance(region, RegionLagrange):
-            kwargs0["order"] = region.order - 1
-            kwargs0["dim"] = region.mesh.dim
-            points_per_cell[RegionLagrange] = region.order**region.element.dim
-
-        RegionDual = regions[type(region)]
-
-        if mesh is None and points_per_cell[RegionDual] is not None:
-            mesh = region.mesh.dual(
-                points_per_cell=points_per_cell[RegionDual],
-                offset=offset,
-                npoints=npoints,
-            )
-
-        region_dual = RegionDual(
-            mesh,
-            quadrature=region.quadrature,
-            grad=False,
-            **{**kwargs0, **kwargs},
-        )
-
         if axisymmetric is False and planestrain is False:
             F = Field
         elif axisymmetric is True and planestrain is False:
             F = FieldAxisymmetric
         elif axisymmetric is False and planestrain is True:
             F = FieldPlaneStrain
 
         fields = [F(region, dim=region.mesh.dim, values=values[0])]
 
+        # create dual regions
+        if n > 1:
+            regions = {
+                RegionHexahedron: RegionConstantHexahedron,
+                RegionQuad: RegionConstantQuad,
+                RegionQuadraticQuad: RegionConstantQuad,
+                RegionBiQuadraticQuad: RegionQuad,
+                RegionQuadraticHexahedron: RegionConstantHexahedron,
+                RegionTriQuadraticHexahedron: RegionHexahedron,
+                RegionQuadraticTetra: RegionTetra,
+                RegionQuadraticTriangle: RegionTriangle,
+                RegionTetraMINI: RegionTetra,
+                RegionTriangleMINI: RegionTriangle,
+                RegionLagrange: RegionLagrange,
+            }
+            points_per_cell = {
+                RegionConstantHexahedron: 1,
+                RegionConstantQuad: 1,
+                RegionQuad: 4,
+                RegionHexahedron: 8,
+                RegionTriangle: 3,
+                RegionTetra: 4,
+                RegionLagrange: None,
+            }
+
+            kwargs0 = {}
+
+            if isinstance(region, RegionLagrange):
+                kwargs0["order"] = region.order - 1
+                kwargs0["dim"] = region.mesh.dim
+                points_per_cell[RegionLagrange] = region.order**region.element.dim
+
+            RegionDual = regions[type(region)]
+
+            if mesh is None and points_per_cell[RegionDual] is not None:
+                mesh = region.mesh.dual(
+                    points_per_cell=points_per_cell[RegionDual],
+                    offset=offset,
+                    npoints=npoints,
+                )
+
+            region_dual = RegionDual(
+                mesh,
+                quadrature=region.quadrature,
+                grad=False,
+                **{**kwargs0, **kwargs},
+            )
+
         for a in range(1, n):
             fields.append(Field(region_dual, values=values[a]))
 
         super().__init__(fields=tuple(fields))
```

### Comparing `felupe-7.4.1/src/felupe/_field/_indices.py` & `felupe-7.5.0/src/felupe/_field/_indices.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 
 class Indices:
-    def __init__(self, eai, ai, region, dim):
-        """Indices for cell "e", point "a" and component "i"."""
+    def __init__(self, cai, ai, region, dim):
+        """Indices for cell "c", point "a" and component "i"."""
 
-        self.eai = eai
+        self.cai = cai
         self.ai = ai
         self.dof = np.arange(region.mesh.npoints * dim).reshape(-1, dim)
         self.shape = (region.mesh.npoints * dim, 1)
```

### Comparing `felupe-7.4.1/src/felupe/_field/_planestrain.py` & `felupe-7.5.0/src/felupe/_field/_planestrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,18 +70,18 @@
         super().__init__(region, dim=dim, values=values)
 
     def _interpolate_2d(self):
         """Interpolate 2D field values at points and evaluate them at the
         integration points of all cells in the region."""
 
         # interpolated field values "aI"
-        # evaluated at quadrature point "p"
+        # evaluated at quadrature point "q"
         # for cell "c"
         return np.einsum(
-            "ca...,apc->...pc", self.values[self.region.mesh.cells], self.region.h
+            "ca...,aqc->...qc", self.values[self.region.mesh.cells], self.region.h
         )
 
     def interpolate(self):
         # extend dimension of in-plane 2d-gradient
         return np.pad(self._interpolate_2d(), ((0, 1), (0, 0), (0, 0)))
 
     def _grad_2d(self, sym=False):
@@ -100,18 +100,18 @@
         array
             In-plane 2D-gradient as partial derivative of field values at points
             w.r.t. undeformed coordinates, evaluated at the integration points
             of all cells in the region.
         """
 
         # gradient as partial derivative of field component "I" at point "a"
-        # w.r.t. undeformed coordinate "J" evaluated at quadrature point "p"
-        # for each cell "e"
+        # w.r.t. undeformed coordinate "J" evaluated at quadrature point "q"
+        # for each cell "c"
         g = np.einsum(
-            "ca...,aJpc->...Jpc",
+            "ca...,aJqc->...Jqc",
             self.values[self.region.mesh.cells],
             self.region.dhdX,
         )
 
         if sym:
             return symmetric(g)
         else:
```

### Comparing `felupe-7.4.1/src/felupe/constitution/__init__.py` & `felupe-7.5.0/src/felupe/constitution/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     LinearElasticPlaneStress,
     LinearElasticTensorNotation,
     lame_converter,
 )
 from ._models_pseudo_elasticity import OgdenRoxburgh
 from ._user_materials import (
     LinearElasticPlasticIsotropicHardening,
-    UserMaterial,
-    UserMaterialStrain,
+    Material,
+    MaterialStrain,
 )
-from ._user_materials_hyperelastic import UserMaterialHyperelastic
+from ._user_materials_hyperelastic import Hyperelastic, MaterialAD
 from ._user_materials_models import (
     linear_elastic,
     linear_elastic_plastic_isotropic_hardening,
 )
 
 __all__ = [
     "NeoHooke",
@@ -49,17 +49,18 @@
     "LinearElastic",
     "LinearElasticPlaneStrain",
     "LinearElasticPlaneStress",
     "LinearElasticTensorNotation",
     "lame_converter",
     "OgdenRoxburgh",
     "LinearElasticPlasticIsotropicHardening",
-    "UserMaterial",
-    "UserMaterialStrain",
-    "UserMaterialHyperelastic",
+    "Material",
+    "MaterialStrain",
+    "MaterialAD",
+    "Hyperelastic",
     "AreaChange",
     "LineChange",
     "VolumeChange",
     "ThreeFieldVariation",
     "linear_elastic",
     "linear_elastic_plastic_isotropic_hardening",
 ]
```

### Comparing `felupe-7.4.1/src/felupe/constitution/_kinematics.py` & `felupe-7.5.0/src/felupe/constitution/_kinematics.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/constitution/_mixed.py` & `felupe-7.5.0/src/felupe/constitution/_mixed.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
         Determinant-modification multiplied by ``Pb``
     PbbF : ndarray
         Double-dot product of ``Pb`` and the deformation gradient
 
     """
 
     def __init__(self, material, parallel=False):
-
         self.fun_P = material.gradient
         self.fun_A = material.hessian
 
         # initial variables for calling
         # ``self.gradient(self.x)`` and ``self.hessian(self.x)``
         self.x = [material.x[0], np.ones(1), np.ones(1), material.x[-1]]
```

### Comparing `felupe-7.4.1/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-7.5.0/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,14 @@
         Shear modulus
     bulk : float
         Bulk modulus
 
     """
 
     def __init__(self, mu=None, bulk=None, parallel=False):
-
         self.parallel = parallel
 
         self.mu = mu
         self.bulk = bulk
 
         # aliases for function, gradient and hessian
         self.energy = self.function
@@ -293,15 +292,14 @@
                 * ddot(F, F, parallel=self.parallel)
                 * cdya_il(iFT, iFT, parallel=self.parallel)
             )
             * J ** (-2 / 3)
         )
 
         if bulk is not None:
-
             p = bulk * (J - 1)
             q = p + bulk * J
 
             # "physical"-volumetric (not math-volumetric!) part of A4
             A4 += J * (
                 q * dya(iFT, iFT, parallel=self.parallel)
                 - p * cdya_il(iFT, iFT, parallel=self.parallel)
```

### Comparing `felupe-7.4.1/src/felupe/constitution/_models_hyperelasticity_ad.py` & `felupe-7.5.0/src/felupe/constitution/_models_hyperelasticity_ad.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,28 +51,28 @@
     return mu / 2 * (det(C) ** (-1 / 3) * trace(C) - 3)
 
 
 def mooney_rivlin(C, C10, C01):
     "Strain energy function of the Mooney-Rivlin material formulation."
     J3 = det(C) ** (-1 / 3)
     I1 = J3 * trace(C)
-    I2 = J3 * (I1**2 - trace(C @ C)) / 2
+    I2 = (I1**2 - J3**2 * trace(C @ C)) / 2
     return C10 * (I1 - 3) + C01 * (I2 - 3)
 
 
 def yeoh(C, C10, C20, C30):
     I1 = det(C) ** (-1 / 3) * trace(C)
     return C10 * (I1 - 3) + C20 * (I1 - 3) ** 2 + C30 * (I1 - 3) ** 3
 
 
 def third_order_deformation(C, C10, C01, C11, C20, C30):
     "Strain energy function of the Third-Order-Deformation material formulation."
     J3 = det(C) ** (-1 / 3)
     I1 = J3 * trace(C)
-    I2 = J3 * (I1**2 - trace(C @ C)) / 2
+    I2 = (I1**2 - J3**2 * trace(C @ C)) / 2
     return (
         C10 * (I1 - 3)
         + C01 * (I2 - 3)
         + C11 * (I1 - 3) * (I2 - 3)
         + C20 * (I1 - 3) ** 2
         + C30 * (I1 - 3) ** 3
     )
@@ -110,15 +110,15 @@
     return Wc + We
 
 
 def van_der_waals(C, mu, limit, a, beta):
     "Strain energy function of the Van der Waals material formulation."
     J3 = det(C) ** (-1 / 3)
     I1 = J3 * trace(C)
-    I2 = J3 * (trace(C) ** 2 - trace(C @ C)) / 2
+    I2 = (trace(C) ** 2 - J3**2 * trace(C @ C)) / 2
     Im = (1 - beta) * I1 + beta * I2
     Im.x[np.isclose(Im.x, 3)] += 1e-8
     eta = sqrt((Im - 3) / (limit**2 - 3))
     return mu * (
         -(limit**2 - 3) * (log(1 - eta) + eta) - 2 / 3 * a * ((Im - 3) / 2) ** (3 / 2)
     )
```

### Comparing `felupe-7.4.1/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-7.5.0/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,14 @@
         Young's modulus.
     nu : float
         Poisson ratio.
 
     """
 
     def __init__(self, E=None, nu=None):
-
         self.E = E
         self.nu = nu
 
         # aliases for gradient and hessian
         self.stress = self.gradient
         self.elasticity = self.hessian
 
@@ -227,15 +226,14 @@
         Young's modulus.
     nu : float
         Poisson ratio.
 
     """
 
     def __init__(self, E=None, nu=None, parallel=False):
-
         self.parallel = parallel
 
         self.E = E
         self.nu = nu
 
         # aliases for gradient and hessian
         self.stress = self.gradient
@@ -332,15 +330,14 @@
         Young's modulus.
     nu : float
         Poisson ratio.
 
     """
 
     def __init__(self, E, nu):
-
         self.E = E
         self.nu = nu
 
         self._umat = LinearElasticPlaneStress(*self._convert(self.E, self.nu))
 
         # initial variables for calling
         # ``self.gradient(self.x)`` and ``self.hessian(self.x)``
@@ -507,15 +504,14 @@
         Young's modulus.
     nu : float
         Poisson ratio.
 
     """
 
     def __init__(self, E, nu):
-
         self.E = E
         self.nu = nu
 
         # initial variables for calling
         # ``self.gradient(self.x)`` and ``self.hessian(self.x)``
         self.x = [np.eye(2), np.zeros(0)]
```

### Comparing `felupe-7.4.1/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-7.5.0/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,29 +35,27 @@
         \mathbb{A} &= \frac{\partial^2 \psi}{\partial \boldsymbol{F} \partial
         \boldsymbol{F}} + \frac{\partial \eta}{\partial \psi} \frac{\partial \psi}
         {\partial \boldsymbol{F}} \otimes \frac{\partial \psi}{\partial \boldsymbol{F}}
 
     """
 
     def __init__(self, material, r, m, beta):
-
         # isotropic hyperelastic material formulation
         self.material = material
 
         # ogden-roxburgh material parameters
         self.r = r
         self.m = m
         self.beta = beta
 
         # initial variables for calling
         # ``self.gradient(self.x)`` and ``self.hessian(self.x)``
         self.x = [np.eye(3), np.zeros(1)]
 
     def gradient(self, x):
-
         # unpack variables into deformation gradient and state variables
         F, statevars = x[0], x[-1]
 
         # material parameters alias
         r, m, beta = self.r, self.m, self.beta
 
         # isotropic material formulation: evaluate
@@ -76,15 +74,14 @@
         # update the state variables
         statevars_new = statevars.copy()
         statevars_new[0] = Wmax
 
         return [eta * P, statevars_new]
 
     def hessian(self, x):
-
         # unpack variables into deformation gradient and state variables
         F, statevars = x[0], x[-1]
 
         # material parameters alias
         r, m, beta = self.r, self.m, self.beta
 
         # isotropic material formulation: evaluate
```

### Comparing `felupe-7.4.1/src/felupe/constitution/_user_materials.py` & `felupe-7.5.0/src/felupe/constitution/_user_materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import numpy as np
 
 from ..math import identity, ravel, reshape, sym
 from ._models_linear_elasticity import lame_converter
 from ._user_materials_models import linear_elastic_plastic_isotropic_hardening
 
 
-class UserMaterial:
+class Material:
     """A user-defined material definition with given functions for the (first
     Piola-Kirchhoff) stress tensor and the according fourth-order elasticity
     tensor. Both functions take a list of the deformation gradient and optional
     state variables as the first input argument. The stress-function also
     returns the updated state variables.
 
     Take this code-block as template:
@@ -56,33 +56,32 @@
 
             # user code for fourth-order elasticity tensor
             # according to the (first Piola-Kirchhoff) stress tensor
             dPdF = None
 
             return [dPdF]
 
-        umat = UserMaterial(stress, elasticity, **kwargs)
+        umat = Material(stress, elasticity, **kwargs)
 
     """
 
     def __init__(self, stress, elasticity, nstatevars=0, **kwargs):
-
         self.umat = {"stress": stress, "elasticity": elasticity}
         self.kwargs = kwargs
         self.nstatevars = nstatevars
         self.x = [np.eye(3), np.zeros(nstatevars)]
 
     def gradient(self, x):
         return self.umat["stress"](x, **self.kwargs)
 
     def hessian(self, x):
         return self.umat["elasticity"](x, **self.kwargs)
 
 
-class UserMaterialStrain:
+class MaterialStrain:
     """A strain-based user-defined material definition with a given function
     for the stress tensor and the (fourth-order) elasticity tensor.
 
     Take this code-block from the linear-elastic material formulation
 
     ..  code-block::
 
@@ -116,29 +115,28 @@
             dσdε = 2 * μ * cdya(I, I) + λ * dya(I, I)
 
             # update state variables (not used here)
             ζ = ζn
 
             return dσdε, σ, ζ
 
-        umat = UserMaterialStrain(material=linear_elastic, μ=1, λ=2)
+        umat = MaterialStrain(material=linear_elastic, μ=1, λ=2)
 
     or this minimal header as template:
 
     ..  code-block::
 
         def fun(dε, εn, σn, ζn, **kwargs):
             return dσdε, σ, ζ
 
-        umat = UserMaterialStrain(material=fun, **kwargs)
+        umat = MaterialStrain(material=fun, **kwargs)
 
     """
 
     def __init__(self, material, dim=3, statevars=(0,), **kwargs):
-
         self.material = material
         self.statevars_shape = statevars
         self.statevars_size = [np.product(shape) for shape in statevars]
         self.statevars_offsets = np.cumsum(self.statevars_size)
         self.nstatevars = sum(self.statevars_size)
 
         self.kwargs = {**kwargs, "tangent": None}
@@ -178,15 +176,14 @@
 
         # change of strain
         dstrain = strain - strain_old
 
         return strain_old, dstrain, stress_old, statevars_old
 
     def gradient(self, x):
-
         strain_old, dstrain, stress_old, statevars_old = self.extract(x)
         self.kwargs["tangent"] = False
 
         dsde, stress_new, statevars_new_list = self.material(
             dstrain, strain_old, stress_old, statevars_old, **self.kwargs
         )
 
@@ -197,15 +194,14 @@
             [*[ravel(sv) for sv in statevars_new_list], strain_new_1d, stress_new_1d],
             axis=0,
         )
 
         return [stress_new, statevars_new]
 
     def hessian(self, x):
-
         strain_old, dstrain, stress_old, statevars_old = self.extract(x)
         self.kwargs["tangent"] = True
 
         dsde = self.material(
             dstrain, strain_old, stress_old, statevars_old, **self.kwargs
         )[0]
 
@@ -216,15 +212,15 @@
             + np.einsum("ijkl...->ijlk...", dsde)
             + np.einsum("ijkl...->jilk...", dsde)
         ) / 4
 
         return [dsde]
 
 
-class LinearElasticPlasticIsotropicHardening(UserMaterialStrain):
+class LinearElasticPlasticIsotropicHardening(MaterialStrain):
     """Linear-elastic-plastic material formulation with linear isotropic
     hardening (return mapping algorithm)."""
 
     def __init__(self, E, nu, sy, K):
         """Linear-elastic-plastic material formulation with linear isotropic
         hardening (return mapping algorithm).
```

### Comparing `felupe-7.4.1/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-7.5.0/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 import tensortrax as tr
 
 from ..math import cdya_ik, dot, transpose
-from ._user_materials import UserMaterial
+from ._user_materials import Material
 
 
-class UserMaterialHyperelastic(UserMaterial):
+class Hyperelastic(Material):
     """A user-defined hyperelastic material definition with a given function
     for the strain energy function with Automatic Differentiation provided by
     ``tensortrax``.
 
     Take this code-block as template
 
     ..  code-block::
 
         import tensortrax.math as tm
 
         def neo_hooke(C, mu):
             "Strain energy function of the Neo-Hookean material formulation."
             return mu / 2 * (tm.linalg.det(C) ** (-1/3) * tm.trace(C) - 3)
 
-        umat = fem.UserMaterialHyperelastic(neo_hooke, mu=1)
+        umat = fem.Hyperelastic(neo_hooke, mu=1)
 
     and this code-block for material formulations with state variables:
 
     ..  code-block::
 
         import tensortrax.math as tm
 
@@ -55,72 +55,176 @@
             # update of state variables by evolution equation
             Ci = tm.special.from_triu_1d(Cin, like=C) + mu / eta * dtime * Cu
             Ci = det(Ci) ** (-1 / 3) * Ci
 
             # first invariant of elastic part of right Cauchy-Green deformation tensor
             I1 = tm.trace(Cu @ inv(Ci))
 
-            # first Piola-Kirchhoff stress tensor and state variable
+            # strain energy function and state variable
             return mu / 2 * (I1 - 3), tm.special.triu_1d(Ci)
 
-        umat = fem.UserMaterialHyperelastic(
+        umat = fem.Hyperelastic(
             viscoelastic, mu=1, eta=1, dtime=1, nstatevars=6
         )
 
     See the `documentation of tensortrax <https://github.com/adtzlr/tensortrax>`_
     for further details.
 
     """
 
     def __init__(self, fun, nstatevars=0, parallel=False, **kwargs):
-
         if nstatevars > 0:
             # split the original function into two sub-functions
             self.fun = tr.take(fun, item=0)
             self.fun_statevars = tr.take(fun, item=1)
         else:
             self.fun = fun
 
         self.parallel = parallel
 
         super().__init__(
             stress=self._stress,
             elasticity=self._elasticity,
             nstatevars=nstatevars,
-            **kwargs
+            **kwargs,
         )
 
     def _stress(self, x, **kwargs):
-        F = x[0]
+        F = np.ascontiguousarray(x[0])
 
         if self.nstatevars > 0:
             statevars = (x[1],)
         else:
             statevars = ()
 
         C = dot(transpose(F), F)
-        S = tr.gradient(self.fun, wrt=0, ntrax=2, parallel=self.parallel, sym=True)(
+        dWdC = tr.gradient(self.fun, wrt=0, ntrax=2, parallel=self.parallel, sym=True)(
             C, *statevars, **kwargs
         )
         if self.nstatevars > 0:
             statevars_new = tr.function(
                 self.fun_statevars, wrt=0, ntrax=2, parallel=self.parallel
             )(C, *statevars, **kwargs)
         else:
             statevars_new = None
-        return [dot(F, 2 * S), statevars_new]
+        return [dot(F, 2 * dWdC), statevars_new]
 
     def _elasticity(self, x, **kwargs):
-        F = x[0]
+        F = np.ascontiguousarray(x[0])
 
         if self.nstatevars > 0:
             statevars = (x[1],)
         else:
             statevars = ()
 
         C = dot(transpose(F), F)
-        D, S, W = tr.hessian(
+        d2WdCdC, dWdC, W = tr.hessian(
             self.fun, wrt=0, ntrax=2, full_output=True, parallel=self.parallel, sym=True
         )(C, *statevars, **kwargs)
-        A = np.einsum("iI...,kK...,IJKL...->iJkL...", F, F, 4 * D)
-        B = cdya_ik(np.eye(3), 2 * S)
+        A = 4 * np.einsum(
+            "iI...,kK...,IJKL...->iJkL...", F, F, np.ascontiguousarray(d2WdCdC)
+        )
+        B = cdya_ik(np.eye(3), 2 * dWdC)
         return [np.sum(np.broadcast_arrays(A, B), axis=0)]
+
+
+class MaterialAD(Material):
+    """A user-defined material definition with a given function for the partial
+    derivative of the strain energy function w.r.t. the deformation gradient tensor
+    with Automatic Differentiation provided by ``tensortrax``.
+
+    Take this code-block as template
+
+    ..  code-block::
+
+        import tensortrax.math as tm
+
+        def neo_hooke(F, mu):
+            "First Piola-Kirchhoff stress of the Neo-Hookean material formulation."
+
+            C = tm.dot(tm.transpose(F), F)
+            Cu = tm.linalg.det(C) ** (-1/3) * C
+
+            return mu * F @ tm.special.dev(Cu) @ tm.linalg.inv(C)
+
+        umat = fem.MaterialAD(neo_hooke, mu=1)
+
+    and this code-block for material formulations with state variables:
+
+    ..  code-block::
+
+        import tensortrax.math as tm
+
+        def viscoelastic(F, Cin, mu, eta, dtime):
+            "Finite strain viscoelastic material formulation."
+
+            # unimodular part of the right Cauchy-Green deformation tensor
+            C = tm.dot(tm.transpose(F), F)
+            Cu = tm.linalg.det(C) ** (-1 / 3) * C
+
+            # update of state variables by evolution equation
+            Ci = tm.special.from_triu_1d(Cin, like=C) + mu / eta * dtime * Cu
+            Ci = tm.linalg.det(Ci) ** (-1 / 3) * Ci
+
+            # second Piola-Kirchhoff stress tensor
+            S = mu * tm.special.dev(Cu @ tm.linalg.inv(Ci)) @ tm.linalg.inv(C)
+
+            # first Piola-Kirchhoff stress tensor and state variable
+            return F @ S, tm.special.triu_1d(Ci)
+
+        umat = fem.MaterialAD(
+            viscoelastic, mu=1, eta=1, dtime=1, nstatevars=6
+        )
+
+    See the `documentation of tensortrax <https://github.com/adtzlr/tensortrax>`_
+    for further details.
+
+    """
+
+    def __init__(self, fun, nstatevars=0, parallel=False, **kwargs):
+        if nstatevars > 0:
+            # split the original function into two sub-functions
+            self.fun = tr.take(fun, item=0)
+            self.fun_statevars = tr.take(fun, item=1)
+        else:
+            self.fun = fun
+
+        self.parallel = parallel
+
+        super().__init__(
+            stress=self._stress,
+            elasticity=self._elasticity,
+            nstatevars=nstatevars,
+            **kwargs,
+        )
+
+    def _stress(self, x, **kwargs):
+        F = np.ascontiguousarray(x[0])
+
+        if self.nstatevars > 0:
+            statevars = (x[1],)
+        else:
+            statevars = ()
+
+        dWdF = tr.function(self.fun, wrt=0, ntrax=2, parallel=self.parallel)(
+            F, *statevars, **kwargs
+        )
+        if self.nstatevars > 0:
+            statevars_new = tr.function(
+                self.fun_statevars, wrt=0, ntrax=2, parallel=self.parallel
+            )(F, *statevars, **kwargs)
+        else:
+            statevars_new = None
+        return [dWdF, statevars_new]
+
+    def _elasticity(self, x, **kwargs):
+        F = np.ascontiguousarray(x[0])
+
+        if self.nstatevars > 0:
+            statevars = (x[1],)
+        else:
+            statevars = ()
+
+        d2WdFdF = tr.jacobian(self.fun, wrt=0, ntrax=2, parallel=self.parallel)(
+            F, *statevars, **kwargs
+        )
+        return [d2WdFdF]
```

### Comparing `felupe-7.4.1/src/felupe/constitution/_user_materials_models.py` & `felupe-7.5.0/src/felupe/constitution/_user_materials_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,14 @@
     ζ = ζn
 
     # check yield function and create a mask where plasticity occurs
     mask = (f > 0)[0]
 
     # update stress, tangent and state due to plasticity
     if np.any(mask):
-
         dγ = f / (2 * μ + 2 / 3 * K)
         n = s / norm_s
         εp = εp + dγ * n
         α = α + sqrt(2 / 3) * dγ
 
         # stress
         σ[..., mask] = (σ - 2 * μ * dγ * n)[..., mask]
```

### Comparing `felupe-7.4.1/src/felupe/dof/_boundary.py` & `felupe-7.5.0/src/felupe/dof/_boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
         _fx = fx if callable(fx) else lambda x: np.isclose(x, fx)
         _fy = fy if callable(fy) else lambda y: np.isclose(y, fy)
         _fz = fz if callable(fz) else lambda z: np.isclose(z, fz)
 
         self.fun = [_fx, _fy, _fz][: mesh.dim]
 
         if mask is None:
-
             # apply functions on the points per coordinate
             # fx(x), fy(y), fz(z) and create a mask for each coordinate
             mask = [f(x) for f, x in zip(self.fun, mesh.points.T)]
 
             # select the logical combination function "or" or "and"
             combine = {"or": np.logical_or, "and": np.logical_and}[self.mode]
 
@@ -131,9 +130,8 @@
             # exclude mask from axes which should be skipped
             self.mask[:, np.where(self.skip)[0]] = False
 
         self.dof = dof[self.mask]
         self.points = np.arange(mesh.npoints)[mask]
 
     def update(self, value):
-
         self.value = value
```

### Comparing `felupe-7.4.1/src/felupe/dof/_loadcase.py` & `felupe-7.5.0/src/felupe/dof/_loadcase.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/dof/_tools.py` & `felupe-7.5.0/src/felupe/dof/_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     of the ``field`` based on the keyword ``dof0``."""
 
     # check if a mixed-field is passed
     u = np.concatenate([f.values.ravel() for f in field.fields])
     offsets = np.insert(field.offsets, 0, 0)
 
     for b in bounds.values():
-
         # get offset for field-dof of current boundary
         offset = offsets[[b.field == f for f in field.fields]]
 
         # set prescribed values
         u.ravel()[b.dof + offset] = b.value
 
     if dof0 is None:
```

### Comparing `felupe-7.4.1/src/felupe/element/__init__.py` & `felupe-7.5.0/src/felupe/element/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/element/_base.py` & `felupe-7.5.0/src/felupe/element/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/element/_hexahedron.py` & `felupe-7.5.0/src/felupe/element/_hexahedron.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/element/_lagrange.py` & `felupe-7.5.0/src/felupe/element/_lagrange.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from ._base import Element
 
 
 class ArbitraryOrderLagrange(Element):
     "Lagrange quad/hexahdron finite element of arbitrary order."
 
     def __init__(self, order, dim, interval=(-1, 1)):
-
         self._order = order
         self._nshape = order + 1
         self._npoints = self._nshape**dim
         self._nbasis = self._npoints
         self._interval = interval
 
         super().__init__(shape=(self._npoints, dim))
```

### Comparing `felupe-7.4.1/src/felupe/element/_line.py` & `felupe-7.5.0/src/felupe/element/_line.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/element/_quad.py` & `felupe-7.5.0/src/felupe/element/_quad.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/element/_tetra.py` & `felupe-7.5.0/src/felupe/element/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/element/_triangle.py` & `felupe-7.5.0/src/felupe/element/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/math/__init__.py` & `felupe-7.5.0/src/felupe/math/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/math/_field.py` & `felupe-7.5.0/src/felupe/math/_field.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/math/_math.py` & `felupe-7.5.0/src/felupe/math/_math.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 
 def linsteps(points, num=10, endpoint=True, axis=None, axes=None):
-
     points = np.array(points).ravel()
     start = points[:-1]
     end = points[1:]
     num = np.array([num]).ravel()
 
     if len(num) == 1:
         num = np.tile(num, max(1, len(start)))
@@ -41,15 +40,14 @@
     else:
         steps = np.array([])
 
     if endpoint:
         steps = np.append(steps, points[-1])
 
     if axis is not None:
-
         if axes is None:
             axes = axis + 1
 
         steps_1d = steps
         steps = np.zeros((len(steps_1d), axes))
         steps[:, axis] = steps_1d
```

### Comparing `felupe-7.4.1/src/felupe/math/_spatial.py` & `felupe-7.5.0/src/felupe/math/_spatial.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/math/_tensor.py` & `felupe-7.5.0/src/felupe/math/_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 
     if determinant is None:
         detA = det(A)
     else:
         detA = determinant
 
     if A.shape[0] == 3:
-
         detAinvA[0, 0] = -A[1, 2] * A[2, 1] + A[1, 1] * A[2, 2]
         detAinvA[1, 1] = -A[0, 2] * A[2, 0] + A[0, 0] * A[2, 2]
         detAinvA[2, 2] = -A[0, 1] * A[1, 0] + A[0, 0] * A[1, 1]
 
         detAinvA[0, 1] = A[0, 2] * A[2, 1] - A[0, 1] * A[2, 2]
         detAinvA[0, 2] = -A[0, 2] * A[1, 1] + A[0, 1] * A[1, 2]
         detAinvA[1, 2] = A[0, 2] * A[1, 0] - A[0, 0] * A[1, 2]
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/__init__.py` & `felupe-7.5.0/src/felupe/mechanics/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/mechanics/_curve.py` & `felupe-7.5.0/src/felupe/mechanics/_curve.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,26 +26,24 @@
     def __init__(
         self,
         steps,
         boundary,
         items=None,
         callback=lambda stepnumber, substepnumber, substep: None,
     ):
-
         super().__init__(steps, self._callback)
 
         self.items = items
         self.boundary = boundary
         self.x = []
         self.y = []
         self.res = None
         self._cb = callback
 
     def _callback(self, stepnumber, substepnumber, substep):
-
         if self.items is not None:
             fun = sum([item.results.force for item in self.items])
         else:
             fun = substep.fun
 
         self.x.append(substep.x[0].values[self.boundary.points[0]])
         self.y.append(force(substep.x, fun, self.boundary))
@@ -55,23 +53,24 @@
 
     def plot(
         self,
         x=None,
         y=None,
         xaxis=0,
         yaxis=0,
-        xlabel="x",
-        ylabel="y",
+        xlabel=None,
+        ylabel=None,
         xscale=1,
         yscale=1,
         gradient=False,
+        swapaxes=False,
         fig=None,
         ax=None,
         items=None,
-        **kwargs
+        **kwargs,
     ):
         if self.res is None:
             raise ValueError(
                 "Results are empty. Run `job.evaluate()` and call `job.plot()` again."
             )
 
         import matplotlib.pyplot as plt
@@ -92,12 +91,22 @@
             z = np.gradient(y, x[:, xaxis], edge_order=2, axis=0)
             cuttoff = np.mean(abs(z[:, yaxis])) + 2 * np.std(abs(z[:, yaxis]))
             y[abs(z) > cuttoff] = np.nan
 
         if fig is None or ax is None:
             fig, ax = plt.subplots()
 
+        if swapaxes:
+            x, y = y, x
+            xlabel, ylabel = ylabel, xlabel
+            xaxis, yaxis = yaxis, xaxis
+            xscale, yscale = yscale, xscale
+
         ax.plot(x[:, xaxis] * xscale, y[:, yaxis] * yscale, **kwargs)
-        ax.set_xlabel(xlabel)
-        ax.set_ylabel(ylabel)
+
+        if xlabel is not None:
+            ax.set_xlabel(xlabel)
+
+        if ylabel is not None:
+            ax.set_ylabel(ylabel)
 
         return fig, ax
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_helpers.py` & `felupe-7.5.0/src/felupe/mechanics/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 import numpy as np
 
-from .._assembly import IntegralFormMixed
+from .._assembly import IntegralForm
 from .._field import FieldAxisymmetric
 from ..constitution import AreaChange
 from ..math import det
 
 
 class Assemble:
     "A class with assembly methods of a SolidBody."
@@ -43,39 +43,36 @@
             self.kirchhoff_stress = kirchhoff_stress
 
 
 class Results:
     "A class with intermediate results of a SolidBody."
 
     def __init__(self, stress=False, elasticity=False):
-
         self.force = None
         self._force = None
         self.stiffness = None
         self.kinematics = None
         self.statevars = None
         self._statevars = None
 
         if stress:
             self.stress = None
 
         if elasticity:
             self.elasticity = None
 
     def update_statevars(self):
-
         if self._statevars is not None:
             self.statevars = self._statevars
 
 
 class StateNearlyIncompressible:
     "A State with internal fields for (nearly) incompressible solid bodies."
 
     def __init__(self, field):
-
         self.field = field
         self.dJdF = AreaChange().function
 
         # initial values (on mesh-points) of the displacement field
         self.u = field[0].values
 
         # deformation gradient
@@ -84,15 +81,15 @@
         # cell-values of the internal pressure and volume-ratio fields
         self.p = np.zeros(field.region.mesh.ncells)
         self.J = np.ones(field.region.mesh.ncells)
 
     def h(self, parallel=False):
         "Integrated shape-function gradient w.r.t. the deformed coordinates `x`."
 
-        return IntegralFormMixed(
+        return IntegralForm(
             fun=self.dJdF(self.F), v=self.field, dV=self.field.region.dV
         ).integrate(parallel=parallel)[0]
 
     def v(self):
         "Cell volumes of the deformed configuration."
         dV = self.field.region.dV
         if isinstance(self.field[0], FieldAxisymmetric):
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_job.py` & `felupe-7.5.0/src/felupe/mechanics/_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,32 +140,29 @@
 
         else:  # fake a mesh and a TimeSeriesWriter
             from contextlib import nullcontext
 
             TimeSeriesWriter = nullcontext
 
         with TimeSeriesWriter(filename) as writer:
-
             if filename is not None:
                 writer.write_points_cells(mesh.points, mesh.cells)
 
             if verbose == 1:
                 total = sum([step.nsubsteps for step in self.steps])
                 progress_bar = tqdm(total=total, unit="substep")
 
             for j, step in enumerate(self.steps):
-
                 newton_verbose = False
                 if verbose == 2:
                     print(f"Begin Evaluation of Step {j + 1}.")
                     newton_verbose = True
 
                 substeps = step.generate(verbose=newton_verbose, **kwargs)
                 for i, substep in enumerate(substeps):
-
                     if verbose == 2:
                         _substep = f"Substep {i + 1}/{step.nsubsteps}"
                         _step = f"Step {j + 1}/{self.nsteps}"
 
                         print(f"{_substep} of {_step} successful.")
 
                     self.callback(j, i, substep)
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_multipoint.py` & `felupe-7.5.0/src/felupe/mechanics/_multipoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,14 @@
         indices = np.arange(self.mesh.ndof).reshape(self.mesh.points.shape)
         td = [indices[self.points.reshape(-1, 1), ax].ravel() for ax in self.axes]
         cd = [indices[self.centerpoint, ax].ravel() for ax in self.axes]
 
         L = lil_matrix((self.mesh.ndof, self.mesh.ndof))
 
         for t, c in zip(td, cd):
-
             L[t.reshape(-1, 1), t] = eye(len(t)) * self.multiplier
             L[t.reshape(-1, 1), c] = -self.multiplier
             L[c.reshape(-1, 1), t] = -self.multiplier
             L[c.reshape(-1, 1), c] = eye(len(c)) * self.multiplier * len(self.points)
 
         self.results.stiffness = L.tocsr()
         return self.results.stiffness
@@ -140,15 +139,14 @@
         indices = np.arange(self.mesh.ndof).reshape(self.mesh.points.shape)
         td = [indices[self.points.reshape(-1, 1), ax].ravel() for ax in self.axes]
         cd = [indices[self.centerpoint, ax].ravel() for ax in self.axes]
 
         L = lil_matrix((self.mesh.ndof, self.mesh.ndof))
 
         for t, c, m in zip(td, cd, masks):
-
             L[t[m].reshape(-1, 1), t[m]] = eye(len(t[m])) * self.multiplier
             L[t[m].reshape(-1, 1), c] = -self.multiplier
             L[c.reshape(-1, 1), t[m]] = -self.multiplier
             L[c.reshape(-1, 1), c] = eye(len(c)) * self.multiplier * len(self.points[m])
 
         self.results.stiffness = L.tocsr()
         return self.results.stiffness
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_pointload.py` & `felupe-7.5.0/src/felupe/mechanics/_pointload.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from ._helpers import Assemble, Results
 
 
 class PointLoad:
     "A point load with methods for the assembly of sparse vectors/matrices."
 
     def __init__(self, field, points, values=None, apply_on=0, axisymmetric=False):
-
         self.field = field
         self.points = points
 
         if values is None:
             self.values = 0
         else:
             self.values = values
@@ -38,19 +37,17 @@
         self.apply_on = apply_on
         self.axisymmetric = axisymmetric
 
         self.results = Results()
         self.assemble = Assemble(vector=self._vector, matrix=self._matrix)
 
     def update(self, values):
-
         self.__init__(self.field, self.points, values, self.apply_on, self.axisymmetric)
 
     def _vector(self, field=None, parallel=False):
-
         if field is not None:
             self.field = field
 
         force = [np.zeros_like(f.values) for f in self.field.fields]
         force[self.apply_on][self.points] += self.values
 
         if self.axisymmetric:
@@ -61,15 +58,14 @@
         self.results.force = csr_matrix(
             np.concatenate([f.ravel() for f in force]).reshape(-1, 1)
         )
 
         return -self.results.force
 
     def _matrix(self, field=None, parallel=False):
-
         if field is not None:
             self.field = field
 
         n = np.sum(self.field.fieldsizes)
         self.results.stiffness = csr_matrix(([0], ([0], [0])), shape=(n, n))
 
         return self.results.stiffness
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_solidbody.py` & `felupe-7.5.0/src/felupe/mechanics/_solidbody.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,24 @@
 
 You should have received a copy of the GNU General Public License
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
-from .._assembly import IntegralFormMixed
+from .._assembly import IntegralForm
 from ..constitution import AreaChange
 from ..math import det, dot, transpose
 from ._helpers import Assemble, Evaluate, Results
 
 
 class SolidBody:
     "A SolidBody with methods for the assembly of sparse vectors/matrices."
 
     def __init__(self, umat, field, statevars=None):
-
         self.umat = umat
         self.field = field
 
         self.results = Results(stress=True, elasticity=True)
         self.results.kinematics = self._extract(self.field)
 
         if statevars is not None:
@@ -53,32 +52,30 @@
             hessian=self._hessian,
             cauchy_stress=self._cauchy_stress,
             kirchhoff_stress=self._kirchhoff_stress,
         )
 
         self._area_change = AreaChange()
 
-        self._form = IntegralFormMixed
+        self._form = IntegralForm
 
     def _vector(self, field=None, parallel=False, items=None, args=(), kwargs={}):
-
         if field is not None:
             self.field = field
 
         self.results.stress = self._gradient(field, args=args, kwargs=kwargs)
         self.results.force = self._form(
             fun=self.results.stress[slice(items)],
             v=self.field,
             dV=self.field.region.dV,
         ).assemble(parallel=parallel)
 
         return self.results.force
 
     def _matrix(self, field=None, parallel=False, items=None, args=(), kwargs={}):
-
         if field is not None:
             self.field = field
 
         self.results.elasticity = self._hessian(field, args=args, kwargs=kwargs)
 
         self.results.stiffness = self._form(
             fun=self.results.elasticity[slice(items)],
@@ -86,57 +83,52 @@
             u=self.field,
             dV=self.field.region.dV,
         ).assemble(parallel=parallel)
 
         return self.results.stiffness
 
     def _extract(self, field):
-
         self.field = field
         self.results.kinematics = self.field.extract()
 
         return self.results.kinematics
 
     def _gradient(self, field=None, args=(), kwargs={}):
-
         if field is not None:
             self.field = field
             self.results.kinematics = self._extract(self.field)
 
         gradient = self.umat.gradient(
             [*self.results.kinematics, self.results.statevars], *args, **kwargs
         )
 
         self.results.stress, self.results._statevars = gradient[:-1], gradient[-1]
 
         return self.results.stress
 
     def _hessian(self, field=None, args=(), kwargs={}):
-
         if field is not None:
             self.field = field
             self.results.kinematics = self._extract(self.field)
 
         self.results.elasticity = self.umat.hessian(
             [*self.results.kinematics, self.results.statevars], *args, **kwargs
         )
 
         return self.results.elasticity
 
     def _kirchhoff_stress(self, field=None):
-
         self._gradient(field)
 
         P = self.results.stress[0]
         F = self.results.kinematics[0]
 
         return dot(P, transpose(F))
 
     def _cauchy_stress(self, field=None):
-
         self._gradient(field)
 
         P = self.results.stress[0]
         F = self.results.kinematics[0]
         J = det(F)
 
         return dot(P, transpose(F)) / J
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-7.5.0/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,37 +15,34 @@
 You should have received a copy of the GNU General Public License
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 from scipy.sparse import csr_matrix
 
-from .._assembly import IntegralFormMixed
+from .._assembly import IntegralForm
 from ._helpers import Assemble, Results
 
 
 class SolidBodyGravity:
     "A SolidBody with methods for the assembly of sparse vectors/matrices."
 
     def __init__(self, field, gravity=None, density=1.0):
-
         self.field = field
         self.results = Results(stress=False, elasticity=False)
         self.assemble = Assemble(vector=self._vector, matrix=self._matrix)
-        self._form = IntegralFormMixed
+        self._form = IntegralForm
 
         self.results.gravity = np.array(gravity)
         self.results.density = density
 
     def update(self, gravity):
-
         self.__init__(self.field, gravity, self.results.density)
 
     def _vector(self, field=None, parallel=False):
-
         if field is not None:
             self.field = field
 
         # copy and take only the first (displacement) field of the container
         f = self.field.copy()
         f.fields = f.fields[0:1]
 
@@ -58,15 +55,14 @@
 
         if len(self.field) > 1:
             self.results.force.resize(np.sum(self.field.fieldsizes), 1)
 
         return -self.results.force
 
     def _matrix(self, field=None, parallel=False):
-
         if field is not None:
             self.field = field
 
         n = np.sum(self.field.fieldsizes)
         self.results.stiffness = csr_matrix(([0], ([0], [0])), shape=(n, n))
 
         return self.results.stiffness
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-7.5.0/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 You should have received a copy of the GNU General Public License
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
-from .._assembly import IntegralFormMixed
+from .._assembly import IntegralForm
 from .._field import FieldAxisymmetric
 from ..constitution import AreaChange
 from ..math import ddot, det, dot, dya, transpose
 from ._helpers import Assemble, Evaluate, Results, StateNearlyIncompressible
 
 
 class SolidBodyNearlyIncompressible:
@@ -58,15 +58,15 @@
         """
 
         self.umat = umat
         self.field = field
         self.bulk = bulk
 
         self._area_change = AreaChange()
-        self._form = IntegralFormMixed
+        self._form = IntegralForm
 
         # volume of undeformed configuration
         if isinstance(self.field[0], FieldAxisymmetric):
             R = self.field[0].radius
             dA = self.field.region.dV
             dV = 2 * np.pi * R * dA
         else:
@@ -99,15 +99,14 @@
             gradient=self._gradient,
             hessian=self._hessian,
             cauchy_stress=self._cauchy_stress,
             kirchhoff_stress=self._kirchhoff_stress,
         )
 
     def _vector(self, field=None, parallel=False, items=None, args=(), kwargs={}):
-
         self.results.stress = self._gradient(
             field, parallel=parallel, args=args, kwargs=kwargs
         )
 
         form = self._form(
             fun=self.results.stress,
             v=self.field,
@@ -124,15 +123,14 @@
         ]
 
         self.results.force = form.assemble(values=values)
 
         return self.results.force
 
     def _matrix(self, field=None, parallel=False, items=None, args=(), kwargs={}):
-
         self.results.elasticity = self._hessian(
             field, parallel=parallel, args=args, kwargs=kwargs
         )
 
         form = self._form(
             fun=self.results.elasticity,
             v=self.field,
@@ -145,15 +143,14 @@
         values = [form.integrate(parallel=parallel)[0] + self.bulk / self.V * dya(h, h)]
 
         self.results.stiffness = form.assemble(values=values)
 
         return self.results.stiffness
 
     def _extract(self, field, parallel=False):
-
         u = field[0].values
         u0 = self.results.state.u
         h = self.results.state.h(parallel=parallel)
         v = self.results.state.v()
         J = self.results.state.J
         p = self.results.state.p
 
@@ -170,15 +167,14 @@
         self.results.state.p = p + dp
         self.results.state.J = J + dJ
         self.results.state.u = u
 
         return self.results.kinematics
 
     def _gradient(self, field=None, parallel=False, args=(), kwargs={}):
-
         if field is not None:
             self.results.kinematics = self._extract(field, parallel=parallel)
 
         dJdF = self._area_change.function
         F = self.results.kinematics[0]
         statevars = self.results.statevars
 
@@ -188,15 +184,14 @@
 
         self.results.stress = [gradient[0] + p * dJdF([F])[0]]
         self.results._statevars = gradient[-1]
 
         return self.results.stress
 
     def _hessian(self, field=None, parallel=False, args=(), kwargs={}):
-
         if field is not None:
             self.results.kinematics = self._extract(field, parallel=parallel)
 
         d2JdF2 = self._area_change.gradient
         F = self.results.kinematics[0]
         statevars = self.results.statevars
         p = self.results.state.p
@@ -204,24 +199,22 @@
         self.results.elasticity = [
             self.umat.hessian([F, statevars], *args, **kwargs)[0] + p * d2JdF2([F])[0]
         ]
 
         return self.results.elasticity
 
     def _kirchhoff_stress(self, field=None):
-
         self._gradient(field)
 
         P = self.results.stress[0]
         F = self.results.kinematics[0]
 
         return dot(P, transpose(F))
 
     def _cauchy_stress(self, field=None):
-
         self._gradient(field)
 
         P = self.results.stress[0]
         F = self.results.kinematics[0]
         J = det(F)
 
         return dot(P, transpose(F)) / J
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-7.5.0/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-from .._assembly import IntegralFormMixed
+from .._assembly import IntegralForm
 from ..constitution import AreaChange
 from ._helpers import Assemble, Results
 
 
 class SolidBodyPressure:
     "A hydrostatic pressure boundary on a SolidBody."
 
     def __init__(self, field, pressure=None):
-
         self.field = field
         self._normals = self.field.region.normals
 
         self.results = Results()
         self.results.kinematics = self._extract(self.field)
 
         if pressure is not None:
@@ -37,85 +36,78 @@
         else:
             self.results.pressure = 0
 
         self.assemble = Assemble(vector=self._vector, matrix=self._matrix)
         self._area_change = AreaChange()
 
     def update(self, pressure):
-
         self.__init__(self.field, pressure)
 
     def _extract(self, field):
-
         self.field = field
         self.results.kinematics = self.field.extract()
 
         return self.results.kinematics
 
     def _vector(self, field=None, pressure=None, parallel=False, resize=None):
-
         if field is not None:
-
             self._update(field)
             self.results.kinematics = self._extract(self.field)
 
         fun = self._area_change.function(
             self.results.kinematics,
             self._normals,
             parallel=parallel,
         )
 
         if pressure is not None:
             self.results.pressure = pressure
 
         fun[0] *= self.results.pressure
 
-        self.results.force = IntegralFormMixed(
+        self.results.force = IntegralForm(
             fun=fun, v=self.field, dV=self.field.region.dV, grad_v=[False]
         ).assemble(parallel=parallel)
 
         if resize is not None:
             self.results.force.resize(*resize.shape)
 
         return self.results.force
 
     def _matrix(self, field=None, pressure=None, parallel=False, resize=None):
-
         if field is not None:
-
             self._update(field)
             self.results.kinematics = self._extract(self.field)
 
         fun = self._area_change.gradient(
             self.results.kinematics,
             self._normals,
             parallel=parallel,
         )
 
         if pressure is not None:
             self.results.pressure = pressure
 
         fun[0] *= self.results.pressure
 
-        self.results.stiffness = IntegralFormMixed(
+        self.results.stiffness = IntegralForm(
             fun=fun,
             v=self.field,
             u=self.field,
             dV=self.field.region.dV,
             grad_v=[False],
             grad_u=[True],
         ).assemble(parallel=parallel)
 
         if resize is not None:
             self.results.stiffness.resize(*resize.shape)
 
         return self.results.stiffness
 
     def _update(self, other_field, field=None):
-
         if field is not None:
             self.field = field
 
         self.field[0].values = other_field[0].values
         self.results.kinematics = self._extract(self.field)
 
         return self.field
```

### Comparing `felupe-7.4.1/src/felupe/mechanics/_step.py` & `felupe-7.5.0/src/felupe/mechanics/_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         if "x0" not in kwargs.keys():
             field = self.items[0].field
         else:
             field = kwargs["x0"]
 
         stop = False
         for substep in substeps:
-
             if stop:
                 break
 
             # update items
             for item, value in self.ramp.items():
                 item.update(value[substep])
```

### Comparing `felupe-7.4.1/src/felupe/mesh/__init__.py` & `felupe-7.5.0/src/felupe/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/mesh/_container.py` & `felupe-7.5.0/src/felupe/mesh/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/mesh/_convert.py` & `felupe-7.5.0/src/felupe/mesh/_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,25 +37,23 @@
     ncells = len(cells)
     dim = points.shape[1]
 
     if cell_type not in ["triangle", "tetra", "quad", "hexahedron"]:
         raise NotImplementedError("Cell type not supported for conversion.")
 
     if order == 0:
-
         if calc_points:
             points_new = np.stack([np.mean(points[cell], axis=0) for cell in cells])
         else:
             points_new = np.zeros((ncells, dim), dtype=int)
 
         cells_new = np.arange(ncells).reshape(-1, 1)
         cell_type_new = cell_type
 
     elif order == 2:
-
         points_new, cells_new, cell_type_new = add_midpoints_edges(
             points, cells, cell_type
         )
 
         if calc_midfaces:
             points_new, cells_new, cell_type_new = add_midpoints_faces(
                 points_new, cells_new, cell_type_new
@@ -217,15 +215,14 @@
     if "tetra" in cell_type:
         number_of_vertices = 3
 
     elif "hexahedron" in cell_type:
         number_of_vertices = 8
 
     if cell_type in supported_cell_types:
-
         points_volumes = np.mean(points[cells][:, :number_of_vertices, :], axis=1)
         cells_volumes = np.arange(cells.shape[0]).reshape(-1, 1)
 
     return points_volumes, cells_volumes, cell_type
 
 
 @mesh_or_data
```

### Comparing `felupe-7.4.1/src/felupe/mesh/_discrete_geometry.py` & `felupe-7.5.0/src/felupe/mesh/_discrete_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/mesh/_dual.py` & `felupe-7.5.0/src/felupe/mesh/_dual.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/mesh/_geometry.py` & `felupe-7.5.0/src/felupe/mesh/_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         points, cells, cell_type = cube_hexa(a, b, n)
 
         super().__init__(points, cells, cell_type)
 
 
 class Grid(Mesh):
     def __init__(self, *xi, indexing="ij", **kwargs):
-
         shape = np.array([len(x) for x in xi])
         n = shape if len(shape) > 1 else shape[0]
 
         M = [None, line_line, rectangle_quad, cube_hexa][len(xi)]
         points, cells, cell_type = M(n=n)
 
         super().__init__(points, cells, cell_type)
```

### Comparing `felupe-7.4.1/src/felupe/mesh/_helpers.py` & `felupe-7.5.0/src/felupe/mesh/_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,24 +22,21 @@
 def mesh_or_data(meshfun):
     """If a ``DiscreteGeometry`` is passed to a mesh function, extract ``points`` and
     ``cells`` arrays along with the ``cell_type`` and return a ``DiscreteGeometry``
     as a result."""
 
     @wraps(meshfun)
     def mesh_or_points_cells_type(*args, **kwargs):
-
         # init mesh flag
         is_mesh = False
 
         # check if unnamed args are passed
         if len(args) > 0:
-
             # meshfun(DiscreteGeometry)
             if hasattr(args[0], "__mesh__"):
-
                 # set mesh flag
                 is_mesh = True
 
                 # get points, cells and cell_type
                 points = args[0].points
                 cells = args[0].cells
                 cell_type = args[0].cell_type
@@ -47,15 +44,14 @@
                 # get mesh class
                 Mesh = args[0].__mesh__
 
                 # remove Mesh from args
                 args = args[1:]
 
         if not is_mesh:
-
             # meshfun(points:ndarray, cells:ndarray, cell_type:str)
             if "points" in kwargs.keys():
                 # get points, cells and cell_type from keyword arguments
                 points = kwargs.pop("points")
                 cells = kwargs.pop("cells")
                 cell_type = kwargs.pop("cell_type")
```

### Comparing `felupe-7.4.1/src/felupe/mesh/_line_rectangle_cube.py` & `felupe-7.5.0/src/felupe/mesh/_line_rectangle_cube.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/mesh/_mesh.py` & `felupe-7.5.0/src/felupe/mesh/_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/mesh/_read.py` & `felupe-7.5.0/src/felupe/mesh/_read.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/mesh/_tools.py` & `felupe-7.5.0/src/felupe/mesh/_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,14 @@
     ----------
     [1] Dompierre, J., Labbé, P., Vallet, M. G., & Camarero, R. (1999).
     How to Subdivide Pyramids, Prisms, and Hexahedra into Tetrahedra.
     IMR, 99, 195.
     """
 
     if cell_type == "quad":
-
         # triangles out of a quad
         i = [0, 3]
         j = [1, 1]
         k = [3, 2]
 
         cells_new = np.dstack(
             (
@@ -457,15 +456,14 @@
                 cells[:, k],
             )
         )
 
         cell_type_new = "triangle"
 
     elif cell_type == "hexahedron":
-
         # tets out of a hex
         # mode ... no. of diagional through hex-point 6.
         if mode == 0:
             i = [0, 0, 0, 0, 2]
             j = [1, 2, 2, 5, 7]
             k = [2, 7, 3, 7, 5]
             m = [5, 5, 7, 4, 6]
@@ -552,12 +550,11 @@
     # check symmetry
     if top == centerpoint[axis] or bottom == centerpoint[axis]:
         half_height = top - bottom
     else:
         half_height = (top - bottom) / 2
 
     for i, coord in enumerate(runout_along[axis][: dim - 1]):
-
         factor = (abs(points_new[mask, axis]) / half_height) ** exponent
         points_new[mask, coord] *= 1 + factor * values[i]
 
     return points_new + centerpoint, cells, cell_type
```

### Comparing `felupe-7.4.1/src/felupe/quadrature/_base.py` & `felupe-7.5.0/src/felupe/quadrature/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/quadrature/_gausslegendre.py` & `felupe-7.5.0/src/felupe/quadrature/_gausslegendre.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/quadrature/_tetra.py` & `felupe-7.5.0/src/felupe/quadrature/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/quadrature/_triangle.py` & `felupe-7.5.0/src/felupe/quadrature/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/region/__init__.py` & `felupe-7.5.0/src/felupe/region/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/region/_boundary.py` & `felupe-7.5.0/src/felupe/region/_boundary.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,51 +281,50 @@
     mesh : Mesh
         A mesh with points and cells.
     element : Finite element
         The finite element formulation to be applied on the cells.
     quadrature: Quadrature scheme
         An element-compatible numeric integration scheme with points and weights.
     h : ndarray
-        Element shape function array ``h_ap`` of shape function ``a`` evaluated at
-        quadrature point ``p``.
+        Element shape function array ``h_aq`` of shape function ``a`` evaluated at
+        quadrature point ``q``.
     dhdr : ndarray
-        Partial derivative of element shape function array ``dhdr_aJp`` with shape
+        Partial derivative of element shape function array ``dhdr_aJq`` with shape
         function ``a`` w.r.t. natural element coordinate ``J`` evaluated at quadrature
-        point ``p`` for every cell ``c`` (geometric gradient or **Jacobian**
+        point ``q`` for every cell ``c`` (geometric gradient or **Jacobian**
         transformation between ``X`` and ``r``).
     dXdr : ndarray
-        Geometric gradient ``dXdr_IJpc`` as partial derivative of undeformed coordinate
+        Geometric gradient ``dXdr_IJqc`` as partial derivative of undeformed coordinate
         ``I`` w.r.t. natural element coordinate ``J`` evaluated at quadrature point
-        ``p`` for every cell ``c`` (geometric gradient or **Jacobian** transformation
+        ``q`` for every cell ``c`` (geometric gradient or **Jacobian** transformation
         between ``X`` and ``r``).
     drdX : ndarray
         Inverse of dXdr.
     dA : ndarray
         Numeric *Differential area vectors*.
     normals : ndarray
         Area unit normal vectors.
     dV : ndarray
         Numeric *Differential volume element* as norm of *Differential area vectors*.
     dhdX : ndarray
-        Partial derivative of element shape functions ``dhdX_aJpc`` of shape function
-        ``a`` w.r.t. undeformed coordinate ``J`` evaluated at quadrature point ``p`` for
+        Partial derivative of element shape functions ``dhdX_aJqc`` of shape function
+        ``a`` w.r.t. undeformed coordinate ``J`` evaluated at quadrature point ``q`` for
         every cell ``c``.
     """
 
     def __init__(
         self,
         mesh,
         element,
         quadrature,
         grad=True,
         only_surface=True,
         mask=None,
         ensure_3d=False,
     ):
-
         self.only_surface = only_surface
         self.mask = mask
         self.ensure_3d = ensure_3d
 
         if mesh.cell_type == "quad":
             cells, cells_faces = boundary_cells_quad(mesh)
         elif mesh.cell_type == "quad8":
@@ -385,15 +384,14 @@
         "Initialize (norm of) face normals of cells."
 
         if (
             self.mesh.cell_type == "quad"
             or self.mesh.cell_type == "quad8"
             or self.mesh.cell_type == "quad9"
         ):
-
             dA_1 = self.dXdr[:, 0][::-1]
             dA_1[0] = -dA_1[0]
 
         elif (
             self.mesh.cell_type == "hexahedron"
             or self.mesh.cell_type == "hexahedron20"
             or self.mesh.cell_type == "hexahedron27"
@@ -403,15 +401,14 @@
         dA = -dA_1 * self.quadrature.weights.reshape(-1, 1)
 
         # norm and unit normal vector
         dV = np.linalg.norm(dA, axis=0)
         normals = dA / dV
 
         if self.ensure_3d:
-
             if dA.shape[0] == 2:
                 dA = np.pad(dA, ((0, 1), (0, 0), (0, 0)))
                 normals = np.pad(normals, ((0, 1), (0, 0), (0, 0)))
 
         return dA, dV, normals
 
     def mesh_faces(self):
```

### Comparing `felupe-7.4.1/src/felupe/region/_region.py` & `felupe-7.5.0/src/felupe/region/_region.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,61 +56,59 @@
     mesh : Mesh
         A mesh with points and cells.
     element : Finite element
         The finite element formulation to be applied on the cells.
     quadrature: Quadrature scheme
         An element-compatible numeric integration scheme with points and weights.
     h : ndarray
-        Element shape function array ``h_ap`` of shape function ``a`` evaluated at
-        quadrature point ``p``.
+        Element shape function array ``h_aq`` of shape function ``a`` evaluated at
+        quadrature point ``q``.
     dhdr : ndarray
-        Partial derivative of element shape function array ``dhdr_aJp`` with shape
+        Partial derivative of element shape function array ``dhdr_aJq`` with shape
         function ``a`` w.r.t. natural element coordinate ``J`` evaluated at quadrature
-        point ``p`` for every cell ``c`` (geometric gradient or **Jacobian**
+        point ``q`` for every cell ``c`` (geometric gradient or **Jacobian**
         transformation between ``X`` and ``r``).
     dXdr : ndarray
-        Geometric gradient ``dXdr_IJpc`` as partial derivative of undeformed coordinate
+        Geometric gradient ``dXdr_IJqc`` as partial derivative of undeformed coordinate
         ``I`` w.r.t. natural element coordinate ``J`` evaluated at quadrature point
-        ``p`` for every cell ``c`` (geometric gradient or **Jacobian** transformation
+        ``q`` for every cell ``c`` (geometric gradient or **Jacobian** transformation
         between ``X`` and ``r``).
     drdX : ndarray
         Inverse of dXdr.
     dV : ndarray
         Numeric *Differential volume element* as product of determinant of geometric
-        gradient  ``dV_pc = det(dXdr)_pc w_p`` and quadrature weight ``w_p``, evaluated
-        at quadrature point ``p`` for every cell ``c``.
+        gradient  ``dV_qc = det(dXdr)_qc w_q`` and quadrature weight ``w_q``, evaluated
+        at quadrature point ``q`` for every cell ``c``.
     dhdX : ndarray
-        Partial derivative of element shape functions ``dhdX_aJpc`` of shape function
-        ``a`` w.r.t. undeformed coordinate ``J`` evaluated at quadrature point ``p`` for
+        Partial derivative of element shape functions ``dhdX_aJqc`` of shape function
+        ``a`` w.r.t. undeformed coordinate ``J`` evaluated at quadrature point ``q`` for
         every cell ``c``.
     """
 
     def __init__(self, mesh, element, quadrature, grad=True):
-
         self.mesh = mesh
         self.element = element
         self.quadrature = quadrature
 
         # element shape function
         self.element.h = np.array(
-            [self.element.function(p) for p in self.quadrature.points]
+            [self.element.function(q) for q in self.quadrature.points]
         ).T
         self.h = np.tile(np.expand_dims(self.element.h, -1), self.mesh.ncells)
 
         # partial derivative of element shape function
         self.element.dhdr = np.array(
-            [self.element.gradient(p) for p in self.quadrature.points]
+            [self.element.gradient(q) for q in self.quadrature.points]
         ).transpose(1, 2, 0)
         self.dhdr = np.tile(np.expand_dims(self.element.dhdr, -1), self.mesh.ncells)
 
         if grad:
-
             # geometric gradient
             self.dXdr = np.einsum(
-                "caI,aJpc->IJpc", self.mesh.points[self.mesh.cells], self.dhdr
+                "caI,aJqc->IJqc", self.mesh.points[self.mesh.cells], self.dhdr
             )
 
             # inverse of dXdr
             self.drdX = inv(self.dXdr)
 
             # numeric **differential volume element**
             self.dV = det(self.dXdr) * self.quadrature.weights.reshape(-1, 1)
@@ -125,15 +123,15 @@
                         "and re-create the region.",
                     ]
                 )
                 warnings.warn(message_negative_volumes)
 
             # Partial derivative of element shape function
             # w.r.t. undeformed coordinates
-            self.dhdX = np.einsum("aIpc,IJpc->aJpc", self.dhdr, self.drdX)
+            self.dhdX = np.einsum("aIqc,IJqc->aJqc", self.dhdr, self.drdX)
 
     def __repr__(self):
         header = "<felupe Region object>"
         element = f"  Element formulation: {type(self.element).__name__}"
         quadrature = f"  Quadrature rule: {type(self.quadrature).__name__}"
         grad = f"  Gradient evaluated: {hasattr(self, 'dV')}"
```

### Comparing `felupe-7.4.1/src/felupe/region/_templates.py` & `felupe-7.5.0/src/felupe/region/_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,50 +46,46 @@
 
     def __init__(
         self,
         mesh,
         quadrature=GaussLegendre(order=1, dim=2),
         grad=False,
     ):
-
         element = ConstantQuad()
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuad(Region):
     "A region with a quad element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=1, dim=2), grad=True):
-
         element = Quad()
 
         if len(mesh.cells.T) > 4:
             mesh = Mesh(mesh.points, mesh.cells[:, :4], "quad")
 
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuadraticQuad(Region):
     "A region with a (serendipity) quadratic quad element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=2, dim=2), grad=True):
-
         element = QuadraticQuad()
 
         if len(mesh.cells.T) > 8:
             mesh = Mesh(mesh.points, mesh.cells[:, :8], "quad8")
 
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionBiQuadraticQuad(Region):
     "A region with a bi-quadratic (lagrange) quad element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=2, dim=2), grad=True):
-
         element = BiQuadraticQuad()
 
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuadBoundary(RegionBoundary):
     "A region with a quad element."
@@ -99,15 +95,14 @@
         mesh,
         quadrature=GaussLegendreBoundary(order=1, dim=2),
         grad=True,
         only_surface=True,
         mask=None,
         ensure_3d=False,
     ):
-
         element = Quad()
 
         super().__init__(
             mesh,
             element,
             quadrature,
             grad=grad,
@@ -125,15 +120,14 @@
         mesh,
         quadrature=GaussLegendreBoundary(order=2, dim=2),
         grad=True,
         only_surface=True,
         mask=None,
         ensure_3d=False,
     ):
-
         element = QuadraticQuad()
 
         super().__init__(
             mesh,
             element,
             quadrature,
             grad=grad,
@@ -151,15 +145,14 @@
         mesh,
         quadrature=GaussLegendreBoundary(order=2, dim=2),
         grad=True,
         only_surface=True,
         mask=None,
         ensure_3d=False,
     ):
-
         element = BiQuadraticQuad()
 
         super().__init__(
             mesh,
             element,
             quadrature,
             grad=grad,
@@ -174,24 +167,22 @@
 
     def __init__(
         self,
         mesh,
         quadrature=GaussLegendre(order=1, dim=3),
         grad=False,
     ):
-
         element = ConstantHexahedron()
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionHexahedron(Region):
     "A region with a hexahedron element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=1, dim=3), grad=True):
-
         element = Hexahedron()
 
         if len(mesh.cells.T) > 8:
             mesh = Mesh(mesh.points, mesh.cells[:, :8], "hexahedron")
 
         super().__init__(mesh, element, quadrature, grad=grad)
 
@@ -203,26 +194,24 @@
         self,
         mesh,
         quadrature=GaussLegendreBoundary(order=1, dim=3),
         grad=True,
         only_surface=True,
         mask=None,
     ):
-
         element = Hexahedron()
         super().__init__(
             mesh, element, quadrature, grad=grad, only_surface=only_surface, mask=mask
         )
 
 
 class RegionQuadraticHexahedron(Region):
     "A region with a (serendipity) quadratic hexahedron element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=2, dim=3), grad=True):
-
         element = QuadraticHexahedron()
 
         if len(mesh.cells.T) > 20:
             mesh = Mesh(mesh.points, mesh.cells[:, :20], "hexahedron20")
 
         super().__init__(mesh, element, quadrature, grad=grad)
 
@@ -234,26 +223,24 @@
         self,
         mesh,
         quadrature=GaussLegendreBoundary(order=2, dim=3),
         grad=True,
         only_surface=True,
         mask=None,
     ):
-
         element = QuadraticHexahedron()
         super().__init__(
             mesh, element, quadrature, grad=grad, only_surface=only_surface, mask=mask
         )
 
 
 class RegionTriQuadraticHexahedron(Region):
     "A region with a tri-quadratic (lagrange) hexahedron element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=2, dim=3), grad=True):
-
         element = TriQuadraticHexahedron()
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionTriQuadraticHexahedronBoundary(RegionBoundary):
     "A boundary region with a tri-quadratic (lagrange) hexahedron element."
 
@@ -261,92 +248,84 @@
         self,
         mesh,
         quadrature=GaussLegendreBoundary(order=2, dim=3),
         grad=True,
         only_surface=True,
         mask=None,
     ):
-
         element = TriQuadraticHexahedron()
         super().__init__(
             mesh, element, quadrature, grad=grad, only_surface=only_surface, mask=mask
         )
 
 
 class RegionLagrange(Region):
     "A region with an arbitrary order lagrange element."
 
     def __init__(self, mesh, order, dim, quadrature=None, grad=True):
-
         if quadrature is None:
             quadrature = GaussLegendre(order=order, dim=dim, permute=False)
 
         element = ArbitraryOrderLagrange(order, dim)
         self.order = order
 
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionTriangle(Region):
     "A region with a triangle element."
 
     def __init__(self, mesh, quadrature=TriangleQuadrature(order=1), grad=True):
-
         element = Triangle()
 
         if len(mesh.cells.T) > 3:
             m = Mesh(mesh.points, mesh.cells[:, :3], "triangle")
         else:
             m = mesh
 
         super().__init__(m, element, quadrature, grad=grad)
 
 
 class RegionTetra(Region):
     "A region with a tetra element."
 
     def __init__(self, mesh, quadrature=TetraQuadrature(order=1), grad=True):
-
         element = Tetra()
 
         if len(mesh.cells.T) > 4:
             m = Mesh(mesh.points, mesh.cells[:, :4], "tetra")
         else:
             m = mesh
 
         super().__init__(m, element, quadrature, grad=grad)
 
 
 class RegionTriangleMINI(Region):
     "A region with a triangle-MINI element."
 
     def __init__(self, mesh, quadrature=TriangleQuadrature(order=2), grad=True):
-
         element = TriangleMINI()
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionTetraMINI(Region):
     "A region with a tetra-MINI element."
 
     def __init__(self, mesh, quadrature=TetraQuadrature(order=2), grad=True):
-
         element = TetraMINI()
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuadraticTriangle(Region):
     "A region with a quadratic triangle element."
 
     def __init__(self, mesh, quadrature=TriangleQuadrature(order=2), grad=True):
-
         element = QuadraticTriangle()
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuadraticTetra(Region):
     "A region with a quadratic tetra element."
 
     def __init__(self, mesh, quadrature=TetraQuadrature(order=2), grad=True):
-
         element = QuadraticTetra()
         super().__init__(mesh, element, quadrature, grad=grad)
```

### Comparing `felupe-7.4.1/src/felupe/solve/_solve.py` & `felupe-7.5.0/src/felupe/solve/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/tools/_misc.py` & `felupe-7.5.0/src/felupe/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/tools/_newton.py` & `felupe-7.5.0/src/felupe/tools/_newton.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from time import perf_counter
 
 import numpy as np
 from scipy.sparse import csr_matrix
 from scipy.sparse.linalg import spsolve
 
 from .. import solve as fesolve
-from .._assembly import IntegralFormMixed
+from .._assembly import IntegralForm
 from ..math import norm
 
 
 class Result:
     def __init__(self, x, fun=None, jac=None, success=None, iterations=None):
         "Result class."
         self.x = x
@@ -89,30 +89,30 @@
     return matrix
 
 
 def fun(x, umat, parallel=False, grad=True, add_identity=True, sym=False):
     "Force residuals from assembly of equilibrium (weak form)."
 
     return (
-        IntegralFormMixed(
+        IntegralForm(
             fun=umat.gradient(x.extract(grad=grad, add_identity=add_identity, sym=sym))[
                 :-1
             ],
             v=x,
             dV=x.region.dV,
         )
         .assemble(parallel=parallel)
         .toarray()[:, 0]
     )
 
 
 def jac(x, umat, parallel=False, grad=True, add_identity=True, sym=False):
     "Tangent stiffness matrix from assembly of linearized equilibrium."
 
-    return IntegralFormMixed(
+    return IntegralForm(
         fun=umat.hessian(x.extract(grad=grad, add_identity=add_identity, sym=sym)),
         v=x,
         dV=x.region.dV,
         u=x,
     ).assemble(parallel=parallel)
```

### Comparing `felupe-7.4.1/src/felupe/tools/_plot.py` & `felupe-7.5.0/src/felupe/tools/_plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 You should have received a copy of the GNU General Public License
 along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
+from ..math import eigvalsh, tovoigt
 from ..mechanics._job import (
     deformation_gradient,
     displacement,
     log_strain,
     log_strain_principal,
 )
 
@@ -108,20 +109,24 @@
         if plotter is None:
             plotter = pv.Plotter(off_screen=off_screen)
 
         if scalar_bar_args is None:
             scalar_bar_args = {}
 
         if name is not None:
+            if component is not None:
+                if name in self.mesh.point_data.keys():
+                    data = self.mesh.point_data[name]
+                else:
+                    data = self.mesh.cell_data[name]
 
-            if label is None:
-                data_label = name
+        if name is not None and label is None:
+            data_label = name
 
             if component is not None:
-
                 if name in self.mesh.point_data.keys():
                     data = self.mesh.point_data[name]
                 else:
                     data = self.mesh.cell_data[name]
 
                 dim = 1
 
@@ -142,15 +147,15 @@
                         "YZ",
                         "ZX",
                         "ZY",
                         "ZZ",
                     ],
                 }
 
-                if "Principal Values of " in name:
+                if "Principal Values of " in data_label:
                     component_labels_dict[2] = [
                         "(Max. Principal)",
                         "(Min. Principal)",
                     ]
                     component_labels_dict[3] = [
                         "(Max. Principal)",
                         "(Int. Principal)",
@@ -169,40 +174,38 @@
 
             label = f"{data_label} {component_label}"
 
         if show_undeformed:
             show_edges_undeformed = False
             opacity_undeformed = 0.2
 
-            if name is None:
-                show_edges_undeformed = show_edges
-                opacity_undeformed = None
-
             plotter.add_mesh(
                 self.mesh, show_edges=show_edges_undeformed, opacity=opacity_undeformed
             )
 
-        if name is not None:
-            plotter.add_mesh(
-                mesh=self.mesh.warp_by_vector("Displacement", factor=factor),
-                scalars=name,
-                component=component,
-                show_edges=show_edges,
-                cmap=cmap,
-                scalar_bar_args={
-                    "title": label,
-                    "interactive": True,
-                    "vertical": scalar_bar_vertical,
-                    **scalar_bar_args,
-                },
-                **kwargs,
-            )
+        mesh = self.mesh
+        if "Displacement" in self.mesh.point_data.keys():
+            mesh = mesh.warp_by_vector("Displacement", factor=factor)
+
+        plotter.add_mesh(
+            mesh=mesh,
+            scalars=name,
+            component=component,
+            show_edges=show_edges,
+            cmap=cmap,
+            scalar_bar_args={
+                "title": label,
+                "interactive": True,
+                "vertical": scalar_bar_vertical,
+                **scalar_bar_args,
+            },
+            **kwargs,
+        )
 
         if view == "default":
-
             if np.allclose(self.mesh.points[:, 2], 0):
                 view = "xy"
 
             else:
                 view = None
                 plotter.camera.elevation = -15
                 plotter.camera.azimuth = -100
@@ -261,33 +264,37 @@
     def set_active_time_value(self, time):
         "Set new active time value and re-read the mesh."
 
         self.mesh = self._read(time)
 
 
 class ViewMesh(Scene):
-    """Provide Visualization methods for :class:`felupe.Mesh`.
+    """Provide Visualization methods for :class:`felupe.Mesh` with optional given
+    dicts of point- and cell-data items.
 
     Parameters
     ----------
     mesh : felupe.Mesh
         The mesh object.
+    point_data : dict or None, optional
+        Additional point-data dict (default is None).
+    cell_data : dict or None, optional
+        Additional cell-data dict (default is None).
     cell_type : pyvista.CellType or None, optional
         Cell-type of PyVista (default is None).
 
     Attributes
     ----------
     mesh : pyvista.UnstructuredGrid
         A generalized Dataset with the mesh as well as point- and cell-data. This is
         not an instance of :class:`felupe.Mesh`.
 
     """
 
-    def __init__(self, mesh, cell_type=None):
-
+    def __init__(self, mesh, point_data=None, cell_data=None, cell_type=None):
         import pyvista as pv
 
         points = np.pad(mesh.points, ((0, 0), (0, 3 - mesh.points.shape[1])))
         cells = np.pad(
             mesh.cells, ((0, 0), (1, 0)), constant_values=mesh.cells.shape[1]
         )
 
@@ -307,18 +314,38 @@
             }
             cell_type = meshio_to_pyvista_cell_types[mesh.cell_type]
 
         cell_types = cell_type * np.ones(mesh.ncells, dtype=int)
 
         self.mesh = pv.UnstructuredGrid(cells, cell_types, points)
 
+        if point_data is None:
+            point_data = {}
+
+        if cell_data is None:
+            cell_data = {}
+
+        for label, data in point_data.items():
+            self.mesh.point_data[label] = data
+
+        for label, data in cell_data.items():
+            self.mesh.cell_data[label] = data
+
+        self.mesh.set_active_scalars(None)
+        self.mesh.set_active_vectors(None)
+        self.mesh.set_active_tensors(None)
+
 
 class ViewField(ViewMesh):
     """Provide Visualization methods for :class:`felupe.Field`. The warped (deformed)
-    mesh is created from the values of the first field (displacements).
+    mesh is created from the values of the first field (displacements). By default,
+    the "Deformation Gradient" tensor, the "Logarithmic Strain" tensor and the
+    "Principal Values of Logarithmic Strain" are evaluated as field-related items of the
+    cell-data dict. Optional items of given point- and cell-data overwrite these default
+    field-related cell-data items.
 
     Parameters
     ----------
     field : felupe.FieldContainer
         The field-container.
     point_data : dict or None, optional
         Additional point-data dict (default is None).
@@ -332,38 +359,93 @@
     mesh : pyvista.UnstructuredGrid
         A generalized Dataset with the mesh as well as point- and cell-data. This is
         not an instance of :class:`felupe.Mesh`.
 
     """
 
     def __init__(self, field, point_data=None, cell_data=None, cell_type=None):
+        point_data_from_field = {"Displacement": displacement(field)}
+        cell_data_from_field = {
+            "Deformation Gradient": deformation_gradient(field)[0],
+            "Logarithmic Strain": log_strain(field)[0],
+            "Principal Values of Logarithmic Strain": log_strain_principal(field)[0],
+        }
 
-        super().__init__(mesh=field.region.mesh, cell_type=cell_type)
+        if point_data is None:
+            point_data = {}
 
-        point_data_from_field = {}
-        cell_data_from_field = {}
+        if cell_data is None:
+            cell_data = {}
 
-        point_data_from_field["Displacement"] = displacement(field)
-        cell_data_from_field["Deformation Gradient"] = deformation_gradient(field)[0]
-        cell_data_from_field["Logarithmic Strain"] = log_strain(field)[0]
-        cell_data_from_field[
-            "Principal Values of Logarithmic Strain"
-        ] = log_strain_principal(field)[0]
+        super().__init__(
+            mesh=field.region.mesh,
+            point_data={**point_data_from_field, **point_data},
+            cell_data={**cell_data_from_field, **cell_data},
+            cell_type=cell_type,
+        )
 
-        if point_data is None:
-            point_data = {}
 
+class ViewSolid(ViewField):
+    """Provide Visualization methods for :class:`felupe.Field` and `felupe.SolidBody`.
+    The warped (deformed) mesh is created from the values of the first field
+    (displacements). By default, the "Deformation Gradient" tensor, the
+    "Logarithmic Strain" tensor and the "Principal Values of Logarithmic Strain" are
+    evaluated as field-related items of the cell-data dict. Optional items of given
+    point- and cell-data overwrite these default field-related cell-data items.
+
+    Parameters
+    ----------
+    field : felupe.FieldContainer
+        The field-container.
+    solid : felupe.SolidBody or felupe.SolidBodyIncompressible or None, optional
+        A solid body to evaluate the (Cauchy) stress (default is None).
+    stress_type : str, optional
+        The type of stress, either "Cauchy" or "Kirchhoff, which is exported (default is
+        "Cauchy").
+    point_data : dict or None, optional
+        Additional point-data dict (default is None).
+    cell_data : dict or None, optional
+        Additional cell-data dict (default is None).
+    cell_type : pyvista.CellType or None, optional
+        Cell-type of PyVista (default is None).
+
+    Attributes
+    ----------
+    mesh : pyvista.UnstructuredGrid
+        A generalized Dataset with the mesh as well as point- and cell-data. This is
+        not an instance of :class:`felupe.Mesh`.
+
+    """
+
+    def __init__(
+        self,
+        field,
+        solid=None,
+        stress_type="Cauchy",
+        point_data=None,
+        cell_data=None,
+        cell_type=None,
+    ):
         if cell_data is None:
             cell_data = {}
 
-        pdata = {**point_data_from_field, **point_data}
-        cdata = {**cell_data_from_field, **cell_data}
+        cell_data_from_solid = {}
 
-        for label, data in pdata.items():
-            self.mesh.point_data[label] = data
+        if solid is not None:
+            stress_from_field = {
+                "cauchy": solid.evaluate.cauchy_stress,
+                "kirchhoff": solid.evaluate.kirchhoff_stress,
+            }
+            stress = stress_from_field[stress_type.lower()](field)
+            stress_label = f"{stress_type.title()} Stress"
 
-        for label, data in cdata.items():
-            self.mesh.cell_data[label] = data
+            cell_data_from_solid[stress_label] = tovoigt(stress.mean(-2)).T
+            cell_data_from_solid[f"Principal Values of {stress_label}"] = (
+                eigvalsh(stress).mean(-2)[::-1].T
+            )
 
-        self.mesh.set_active_scalars(None)
-        self.mesh.set_active_vectors(None)
-        self.mesh.set_active_tensors(None)
+        super().__init__(
+            field=field,
+            point_data=point_data,
+            cell_data={**cell_data_from_solid, **cell_data},
+            cell_type=cell_type,
+        )
```

### Comparing `felupe-7.4.1/src/felupe/tools/_post.py` & `felupe-7.5.0/src/felupe/tools/_post.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe/tools/_project.py` & `felupe-7.5.0/src/felupe/tools/_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from scipy.sparse import csr_matrix as sparsematrix
 
 from .._field import Field
 from ..region import Region
 
 
 def topoints(values, region, sym=True, mode="tensor"):
-
     rows = region.mesh.cells.T.ravel()
     cols = np.zeros_like(rows)
 
     if mode == "tensor":
         dim = values.shape[0]
         if sym:
             if dim == 3:
@@ -82,15 +81,14 @@
 
     # transpose values
     idx = np.arange(len(values.shape))
     idx[: len(dim)] = idx[: len(dim)][::-1]
     values = values.transpose(idx)
 
     if mean:
-
         # evaluate how often the values must be repeated to match the number
         # of element-points
         reps = np.ones(len(values.shape), dtype=int)
         reps[-2] = len(region.element.points)
 
         # np.average(keepdims=True) requires numpy >= 1.23.0
         values = np.average(values, axis=-2, weights=weights)
@@ -119,33 +117,30 @@
         r = Region(m, region.element, region.quadrature.inv(), grad=False)
 
     # field for values on disconnected mesh; project values to mesh-points
     f = Field(r, dim=size, values=u)
     v = f.interpolate()
 
     if mean:
-
         # due to the usage of the original quadrature scheme the averaging must be
         # applied again
         # np.average(keepdims=True) requires numpy >= 1.23.0
         v = np.average(v, axis=-2, weights=weights).reshape(size, 1, -1)
 
         # broadcast averaged values to match the number of element-points
         shape = np.array([*v.shape[:-2], len(region.element.points), v.shape[-1]])
         v = np.broadcast_to(v, shape=shape)
 
     if average:
-
         # create dummy field for values on original mesh
         # (used for calculation of sparse-matrix indices)
         g = Field(region, dim=size)
 
         # average values
         w = sparsematrix(
             (v.T.ravel(), g.indices.ai), shape=(size * region.mesh.npoints, 1)
         ).toarray().reshape(-1, size) / region.mesh.cells_per_point.reshape(-1, 1)
 
     else:
-
         w = v.T.reshape(-1, size)
 
     return w
```

### Comparing `felupe-7.4.1/src/felupe/tools/_save.py` & `felupe-7.5.0/src/felupe/tools/_save.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     r=None,
     gradient=None,
     converged=True,
     filename="result.vtk",
     cell_data=None,
     point_data=None,
 ):
-
     u = fields.fields[0]
     mesh = region.mesh
 
     offsets = fields.offsets
 
     if point_data is None:
         point_data = {}
```

### Comparing `felupe-7.4.1/src/felupe/tools/_solve.py` & `felupe-7.5.0/src/felupe/tools/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/src/felupe.egg-info/PKG-INFO` & `felupe-7.5.0/src/felupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.4.1
+Version: 7.5.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -791,19 +791,20 @@
 
 # Documentation
 The documentation is located [here](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 # Extension Packages
 The capabilities of FElupe may be enhanced with extension packages created by the community.
 
-| **Package** |                     **Description**                     |                **Link**               |
-|:-----------:|:-------------------------------------------------------:|:-------------------------------------:|
-|  tensortrax |     Math on (Hyper-Dual) Tensors with Trailing Axes     |  https://github.com/adtzlr/tensortrax |
-|    matADi   | Material Definition with Automatic Differentiation (AD) |    https://github.com/adtzlr/matadi   |
-|    FEplot   |             A visualization tool for FElupe             | https://github.com/ZAARAOUI999/feplot |
+|                    **Package**                          |                     **Description**                     |
+|:-------------------------------------------------------:|:-------------------------------------------------------:|
+|  [hyperelastic](https://github.com/adtzlr/hyperelastic) |     Constitutive hyperelastic material formulations     |
+|    [matadi](https://github.com/adtzlr/matadi)           | Material Definition with Automatic Differentiation (AD) |
+|  [tensortrax](https://github.com/adtzlr/tensortrax)     |     Math on (Hyper-Dual) Tensors with Trailing Axes     |
+|    [feplot](https://github.com/ZAARAOUI999/feplot)      |             A visualization tool for FElupe             |
 
 # Changelog
 All notable changes to this project will be documented in [this file](CHANGELOG.md). The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 # License
 FElupe - finite element analysis (C) 2023 Andreas Dutzler, Graz (Austria).
```

### Comparing `felupe-7.4.1/src/felupe.egg-info/SOURCES.txt` & `felupe-7.5.0/src/felupe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 src/felupe.egg-info/PKG-INFO
 src/felupe.egg-info/SOURCES.txt
 src/felupe.egg-info/dependency_links.txt
 src/felupe.egg-info/requires.txt
 src/felupe.egg-info/top_level.txt
 src/felupe/_assembly/__init__.py
 src/felupe/_assembly/_axi.py
-src/felupe/_assembly/_base.py
 src/felupe/_assembly/_form.py
-src/felupe/_assembly/_mixed.py
+src/felupe/_assembly/_integral.py
+src/felupe/_assembly/_weak.py
 src/felupe/_basis/__init__.py
 src/felupe/_basis/_basis.py
 src/felupe/_field/__init__.py
 src/felupe/_field/_axi.py
 src/felupe/_field/_base.py
 src/felupe/_field/_container.py
 src/felupe/_field/_fields.py
```

### Comparing `felupe-7.4.1/tests/test_basis.py` & `felupe-7.5.0/tests/test_basis.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,33 +28,29 @@
 import numpy as np
 import pytest
 
 import felupe as fe
 
 
 def pre(dim):
-
     m = fe.Cube(n=3)
     r = fe.RegionHexahedron(m)
     u = fe.FieldContainer([fe.Field(r, dim=dim)])
     return r, u
 
 
 def pre_constant(dim):
-
     m = fe.Cube(n=3)
     r = fe.RegionConstantHexahedron(m)
     u = fe.FieldContainer([fe.Field(r, dim=dim)])
     return r, u
 
 
 def test_basis():
-
     for parallel in [False, True]:
-
         r, u = pre(dim=3)
         b = fe.Basis(u, parallel=parallel)
 
         assert b[0].grad is not None
 
         r, u = pre(dim=1)
         b = fe.Basis(u, parallel=parallel)
```

### Comparing `felupe-7.4.1/tests/test_bilinearform.py` & `felupe-7.5.0/tests/test_bilinearform.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,27 +64,25 @@
 
 
 def a_pp(q, r, F, p):
     return dot(p, q) * dot(r, p)
 
 
 def pre(dim):
-
     mesh = fe.Cube(n=3)
     region = fe.RegionHexahedron(mesh)
     region0 = fe.RegionConstantHexahedron(mesh.dual(points_per_cell=1))
     u = fe.Field(region, dim=3)
     p = fe.Field(region0)
     up = fe.FieldContainer([u, p])
 
     return up
 
 
 def test_form_decorator():
-
     field = pre(dim=3)
     F, p = field.extract()
     b = fe.Basis(field)
 
     @fe.Form(v=field, u=field, grad_v=(True, False), grad_u=(True, False))
     def a():
         return (a_uu, a_up, a_pp)
```

### Comparing `felupe-7.4.1/tests/test_composite.py` & `felupe-7.5.0/tests/test_composite.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import numpy as np
 
 import felupe as fe
 
 
 def test_composite():
-
     n = 5
     mesh = fe.Cube(n=n)
     region = fe.RegionHexahedron(mesh)
 
     points = np.arange(mesh.npoints)[
         np.logical_or.reduce(
             (
@@ -66,15 +65,14 @@
 
     res = fe.newtonrhapson(field, items=[rubber, reinforced], **loadcase)
 
     fe.save(region, res.x)
 
 
 def test_composite_planestrain():
-
     n = 5
     mesh = fe.Rectangle(n=n)
     region = fe.RegionQuad(mesh)
 
     points = np.arange(mesh.npoints)[
         np.logical_or.reduce(
             (
```

### Comparing `felupe-7.4.1/tests/test_constitution.py` & `felupe-7.5.0/tests/test_constitution.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,25 @@
 """
 import numpy as np
 import pytest
 
 import felupe as fe
 
 
-def pre(sym, add_identity):
+def pre(sym, add_identity, add_random=False):
     m = fe.mesh.Cube()
     e = fe.element.Hexahedron()
     q = fe.quadrature.GaussLegendre(1, 3)
     r = fe.Region(m, e, q)
     u = fe.Field(r, dim=3)
+
+    if add_random:
+        np.random.seed(55601)
+        u.values += np.random.rand(*u.values.shape) / 20
+
     v = fe.FieldContainer([u])
     return r, v.extract(grad=True, sym=sym, add_identity=add_identity)
 
 
 def pre_mixed(sym, add_identity):
     m = fe.mesh.Cube()
     e = fe.element.Hexahedron()
@@ -52,15 +57,14 @@
     return r, w.extract(grad=True, sym=sym, add_identity=add_identity), m
 
 
 def test_nh():
     r, F = pre(sym=False, add_identity=True)
 
     for parallel in [False, True]:
-
         nh = fe.constitution.NeoHooke(mu=1.0, bulk=2.0, parallel=parallel)
 
         W = nh.function(F)
         P = nh.gradient(F)[:-1]
         A = nh.hessian(F)
 
         Wx = nh.energy(F)
@@ -105,15 +109,14 @@
     check_dsde = []
 
     for Material in [
         (fe.constitution.LinearElastic, {}),
         (fe.constitution.LinearElasticTensorNotation, dict(parallel=False)),
         (fe.constitution.LinearElasticTensorNotation, dict(parallel=True)),
     ]:
-
         LinearElastic, kwargs = Material
 
         le = LinearElastic(E=1.0, nu=0.3, **kwargs)
 
         stress = le.gradient(F)[:-1]
         dsde = le.hessian(F)
         dsde2 = le.hessian(shape=F[0].shape[-2:])
@@ -206,15 +209,14 @@
 
 def test_kinematics():
     r, F = pre(sym=False, add_identity=True)
 
     N = F[0][:, 0]
 
     for parallel in [False, True]:
-
         lc = fe.constitution.LineChange(parallel=parallel)
         ac = fe.constitution.AreaChange(parallel=parallel)
         vc = fe.constitution.VolumeChange(parallel=parallel)
 
         xf = lc.function(F)
         xg = lc.gradient(F)
         xg = lc.gradient(F, parallel=parallel)
@@ -278,15 +280,15 @@
 
         # user code for fourth-order elasticity tensor
         d = identity(F)
         dsde = 2 * mu * cdya(d, d) + lmbda * dya(d, d)
 
         return [dsde]
 
-    linear_elastic = fe.UserMaterial(stress, elasticity, mu=1, lmbda=2)
+    linear_elastic = fe.Material(stress, elasticity, mu=1, lmbda=2)
 
     s, statevars_new = linear_elastic.gradient([F, None])
     dsde = linear_elastic.hessian([F, None])
 
 
 def test_umat_hyperelastic():
     r, x = pre(sym=False, add_identity=True)
@@ -314,23 +316,51 @@
             {"Gc": 0.1867, "Ge": 0.2169, "beta": 0.2, "delta": 0.09693},
         ),
         (
             fe.constitution.van_der_waals,
             {"mu": 1.0, "beta": 0.1, "a": 0.5, "limit": 5.0},
         ),
     ]:
-
-        umat = fe.UserMaterialHyperelastic(model, **kwargs)
+        umat = fe.Hyperelastic(model, **kwargs)
 
         s, statevars_new = umat.gradient([F, None])
         dsde = umat.hessian([F, None])
 
 
+def test_umat_hyperelastic2():
+    r, x = pre(sym=False, add_identity=True, add_random=True)
+    F = x[0]
+
+    import tensortrax.math as tm
+
+    def neo_hooke(F, mu=1):
+        "First Piola-Kirchhoff stress of the Neo-Hookean material formulation."
+
+        C = tm.dot(tm.transpose(F), F)
+        Cu = tm.linalg.det(C) ** (-1 / 3) * C
+
+        return mu * F @ tm.special.dev(Cu) @ tm.linalg.inv(C)
+
+    kwargs = {"mu": 1}
+    umat = fe.MaterialAD(neo_hooke, **kwargs)
+
+    s, statevars_new = umat.gradient([F, None])
+    dsde = umat.hessian([F, None])
+
+    umat = fe.Hyperelastic(fe.constitution.neo_hooke, **kwargs)
+
+    s2, statevars_new = umat.gradient([F, None])
+    dsde2 = umat.hessian([F, None])
+
+    assert np.allclose(s, s2)
+    assert np.allclose(dsde, dsde2)
+
+
 def test_umat_viscoelastic():
-    r, x = pre(sym=False, add_identity=True)
+    r, x = pre(sym=False, add_identity=True, add_random=True)
     F = x[0]
 
     import tensortrax.math as tm
 
     def viscoelastic(C, Cin, mu, eta, dtime):
         "Finite strain viscoelastic material formulation."
         Ci = (
@@ -339,69 +369,102 @@
         )
         Ci = tm.linalg.det(Ci) ** (-1 / 3) * Ci
         I1 = tm.linalg.det(C) ** (-1 / 3) * tm.trace(C @ tm.linalg.inv(Ci))
 
         return mu / 2 * (I1 - 3), tm.special.triu_1d(Ci)
 
     kwargs = {"mu": 1, "eta": 1, "dtime": 1}
-    umat = fe.UserMaterialHyperelastic(viscoelastic, nstatevars=6, **kwargs)
+    umat = fe.Hyperelastic(viscoelastic, nstatevars=6, **kwargs)
 
     statevars = np.zeros((6, *F.shape[-2:]))
     s, statevars_new = umat.gradient([F, statevars])
     dsde = umat.hessian([F, statevars])
 
-    umat = fe.UserMaterialHyperelastic(
+    umat = fe.Hyperelastic(
         fe.constitution.finite_strain_viscoelastic, nstatevars=6, **kwargs
     )
 
     s2, statevars_new = umat.gradient([F, statevars])
     dsde2 = umat.hessian([F, statevars])
 
     assert np.allclose(s, s2)
     assert np.allclose(dsde, dsde2)
 
 
-def test_umat_strain():
+def test_umat_viscoelastic2():
+    r, x = pre(sym=False, add_identity=True)
+    F = x[0]
+
+    import tensortrax.math as tm
 
+    def viscoelastic(F, Cin, mu, eta, dtime):
+        "Finite strain viscoelastic material formulation."
+        C = tm.dot(tm.transpose(F), F)
+        Cu = tm.linalg.det(C) ** (-1 / 3) * C
+        Ci = (
+            tm.special.from_triu_1d(Cin, like=C)
+            + mu / eta * dtime * tm.linalg.det(C) ** (-1 / 3) * C
+        )
+        Ci = tm.linalg.det(Ci) ** (-1 / 3) * Ci
+        S = mu * tm.special.dev(Cu @ tm.linalg.inv(Ci)) @ tm.linalg.inv(C)
+        return F @ S, tm.special.triu_1d(Ci)
+
+    kwargs = {"mu": 1, "eta": 1, "dtime": 1}
+    umat = fe.MaterialAD(viscoelastic, nstatevars=6, **kwargs)
+
+    statevars = np.zeros((6, *F.shape[-2:]))
+    s, statevars_new = umat.gradient([F, statevars])
+    dsde = umat.hessian([F, statevars])
+
+    umat = fe.Hyperelastic(
+        fe.constitution.finite_strain_viscoelastic, nstatevars=6, **kwargs
+    )
+
+    s2, statevars_new = umat.gradient([F, statevars])
+    dsde2 = umat.hessian([F, statevars])
+
+    assert np.allclose(s, s2)
+    assert np.allclose(dsde, dsde2)
+
+
+def test_umat_strain():
     r, x = pre(sym=False, add_identity=True)
     F = x[0]
     statevars = np.zeros((18, *F.shape[-2:]))
 
-    umat = fe.UserMaterialStrain(
+    umat = fe.MaterialStrain(
         material=fe.constitution.linear_elastic,
         λ=1,
         μ=1,
     )
 
     s, statevars_new = umat.gradient([F, statevars])
     dsde = umat.hessian([F, statevars])
 
 
 def test_umat_strain_plasticity():
-
     r, x = pre(sym=False, add_identity=True)
     F = x[0]
 
     statevars = np.ones((28, *F.shape[-2:]))
 
-    umat = fe.UserMaterialStrain(
+    umat = fe.MaterialStrain(
         material=fe.constitution.linear_elastic_plastic_isotropic_hardening,
         λ=1,
         μ=1,
         σy=0,
         K=0.1,
         statevars=(1, (3, 3)),
     )
 
     s, statevars_new = umat.gradient([F, statevars])
     dsde = umat.hessian([F, statevars])
 
 
 def test_elpliso():
-
     r, x = pre(sym=False, add_identity=True)
     F = x[0]
     statevars = np.zeros((28, *F.shape[-2:]))
 
     umat = fe.LinearElasticPlasticIsotropicHardening(E=3, nu=0.3, sy=1, K=0.1)
 
     s, statevars_new = umat.gradient([F, statevars])
@@ -412,11 +475,13 @@
     test_nh()
     test_linear()
     test_linear_planestress()
     test_linear_planestrain()
     test_kinematics()
     test_umat()
     test_umat_hyperelastic()
+    test_umat_hyperelastic2()
     test_umat_viscoelastic()
+    test_umat_viscoelastic2()
     test_umat_strain()
     test_umat_strain_plasticity()
     test_elpliso()
```

### Comparing `felupe-7.4.1/tests/test_dof.py` & `felupe-7.5.0/tests/test_dof.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,30 +59,28 @@
     r = fe.Region(m, e, q)
     u = fe.Field(r, dim=3)
     v = fe.FieldContainer([u])
     return v
 
 
 def test_boundary():
-
     u = pre3d()
     bounds = {"boundary-label": fe.Boundary(u[0])}
 
     v = fe.dof.apply(u, bounds, dof0=None)
     assert np.allclose(u[0].values.ravel(), v)
 
     mask = np.ones(u.region.mesh.npoints, dtype=bool)
     bounds = {"boundary-label": fe.Boundary(u[0], mask=mask)}
 
     v = fe.dof.apply(u, bounds, dof0=None)
     assert np.allclose(u[0].values.ravel(), v)
 
 
 def test_loadcase():
-
     ux = fe.dof.uniaxial(pre1d())
     assert len(ux) == 2
 
     for u in [pre2d(), pre3d()]:
         v = fe.FieldContainer([u[0], deepcopy(u[0])])
 
         ux = fe.dof.uniaxial(u, right=1.0, move=0.2, clamped=False, sym=True)
```

### Comparing `felupe-7.4.1/tests/test_element.py` & `felupe-7.5.0/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/tests/test_field.py` & `felupe-7.5.0/tests/test_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,42 +28,39 @@
 import numpy as np
 import pytest
 
 import felupe as fe
 
 
 def pre(values=0):
-
     m = fe.Cube(n=3)
     e = fe.Hexahedron()
     q = fe.GaussLegendre(1, 3)
     r = fe.Region(m, e, q)
     u = fe.Field(r, dim=3, values=values)
     v = fe.FieldContainer([u])
 
     return r, v
 
 
 def pre_axi():
-
     m = fe.Rectangle(n=3)
     e = fe.Quad()
     q = fe.GaussLegendre(1, 2)
     r = fe.Region(m, e, q)
 
     u = fe.FieldAxisymmetric(r)
     v = fe.FieldContainer([u])
 
     print(m), print(r), print(v)
 
     return r, v
 
 
 def pre_mixed():
-
     m = fe.Cube(n=3)
     e = fe.Hexahedron()
     q = fe.GaussLegendre(1, 3)
     r = fe.Region(m, e, q)
 
     u = fe.Field(r, dim=3)
     p = fe.Field(r)
@@ -80,15 +77,14 @@
 
     fe.Field(r, dim=9, values=np.eye(3))
 
     return r, f, u, p, J
 
 
 def pre_axi_mixed():
-
     m = fe.Rectangle(n=3)
     e = fe.Quad()
     q = fe.GaussLegendre(1, 2)
     r = fe.Region(m, e, q)
 
     u = fe.FieldAxisymmetric(r, dim=2)
     p = fe.Field(r)
@@ -99,28 +95,26 @@
     u.values[0] = np.ones(2)
     assert np.all(f.values()[0][0] == 1)
 
     return r, f, u, p, J
 
 
 def test_axi():
-
     r, u = pre_axi()
     u += u.values()
 
     r, f, u, p, J = pre_axi_mixed()
 
     u.extract()
     u.extract(grad=False)
     u.extract(grad=True, sym=True)
     u.extract(grad=True, add_identity=False)
 
 
 def test_mixed_lagrange():
-
     order = 4
 
     m = fe.Cube(n=order + 1)
     md = fe.Cube(n=order)
 
     m.update(np.arange(m.npoints).reshape(1, -1), cell_type="VTK_LAGRANGE_HEXAHEDRON")
     md.update(np.arange(md.npoints).reshape(1, -1), cell_type="VTK_LAGRANGE_HEXAHEDRON")
@@ -128,24 +122,22 @@
     r = fe.RegionLagrange(m, order=order, dim=3)
     g = fe.FieldsMixed(r, mesh=md)
 
     assert len(g.fields) == 3
 
 
 def test_3d():
-
     r, u = pre()
     u += u.values()
 
     with pytest.raises(ValueError):
         r, u = pre(values=np.ones(2))
 
 
 def test_3d_mixed():
-
     r, f, u, p, J = pre_mixed()
 
     f.extract()
     f.extract(grad=False)
     f.extract(grad=(False,))
     f.extract(grad=True, sym=True)
     f.extract(grad=True, add_identity=False)
```

### Comparing `felupe-7.4.1/tests/test_form.py` & `felupe-7.5.0/tests/test_form.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import numpy as np
 import pytest
 
 import felupe as fe
 
 
 def pre():
-
     m = fe.Cube(n=3)
     r = fe.RegionHexahedron(m)
 
     u = fe.Field(r, dim=3)
     p = fe.Field(r)
 
     v = fe.FieldContainer([u])
@@ -48,15 +47,14 @@
     P = W.gradient(F)[:-1]
     A = W.hessian(F)
 
     return r, v, q, P, A
 
 
 def pre_broadcast():
-
     m = fe.Cube(n=3)
     e = fe.Hexahedron()
     q = fe.GaussLegendre(1, 3)
     r = fe.Region(m, e, q)
 
     u = fe.Field(r, dim=3)
     p = fe.Field(r)
@@ -72,15 +70,14 @@
 
     P = [P[0][:, :, 0, 0].reshape(3, 3, 1, 1)]
 
     return r, v, q, P, A
 
 
 def pre_axi():
-
     m = fe.Rectangle(n=3)
     r = fe.RegionQuad(m)
 
     u = fe.FieldAxisymmetric(r)
     v = fe.FieldContainer([u])
 
     W = fe.constitution.NeoHooke(1, 3)
@@ -89,15 +86,14 @@
     P = W.gradient(F)[:-1]
     A = W.hessian(F)
 
     return r, v, P, A
 
 
 def pre_mixed():
-
     m = fe.mesh.Cube(n=3)
     e = fe.element.Hexahedron()
     q = fe.quadrature.GaussLegendre(1, 3)
     r = fe.Region(m, e, q)
 
     u = fe.Field(r, dim=3)
     p = fe.Field(r)
@@ -108,15 +104,14 @@
     nh = fe.NeoHooke(1, 3)
     W = fe.ThreeFieldVariation(nh)
 
     return r, f, W.gradient(f.extract())[:-1], W.hessian(f.extract())
 
 
 def pre_axi_mixed():
-
     m = fe.mesh.Rectangle(n=3)
     e = fe.element.Quad()
     q = fe.quadrature.GaussLegendre(1, 2)
     r = fe.Region(m, e, q)
 
     u = fe.FieldAxisymmetric(r, dim=2)
     p = fe.Field(r)
@@ -127,19 +122,17 @@
     nh = fe.NeoHooke(1, 3)
     W = fe.ThreeFieldVariation(nh)
 
     return r, f, W.gradient(f.extract())[:-1], W.hessian(f.extract())
 
 
 def test_axi():
-
     r, u, P, A = pre_axi()
 
     for parallel in [False, True]:
-
         L = fe.IntegralForm(P, u, r.dV)
         x = L.integrate(parallel=parallel)
 
         b = L.assemble(x, parallel=parallel).toarray()
         assert b.shape == (r.mesh.ndof, 1)
 
         b = L.assemble(parallel=parallel).toarray()
@@ -152,19 +145,17 @@
         assert K.shape == (r.mesh.ndof, r.mesh.ndof)
 
         K = a.assemble(parallel=parallel).toarray()
         assert K.shape == (r.mesh.ndof, r.mesh.ndof)
 
 
 def test_linearform():
-
     r, u, p, P, A = pre()
 
     for parallel in [False, True]:
-
         L = fe.IntegralForm(P, u, r.dV, grad_v=[True])
         x = L.integrate(parallel=parallel)
         b = L.assemble(x, parallel=parallel).toarray()
         assert b.shape == (r.mesh.ndof, 1)
         b = L.assemble(parallel=parallel).toarray()
         assert b.shape == (r.mesh.ndof, 1)
 
@@ -173,19 +164,17 @@
         b = L.assemble(x, parallel=parallel).toarray()
         assert b.shape == (r.mesh.npoints, 1)
         b = L.assemble(parallel=parallel).toarray()
         assert b.shape == (r.mesh.npoints, 1)
 
 
 def test_linearform_broadcast():
-
     r, u, p, P, A = pre_broadcast()
 
     for parallel in [False, True]:
-
         L = fe.IntegralForm(P, u, r.dV, grad_v=[True])
         x = L.integrate(parallel=parallel)
         b = L.assemble(x, parallel=parallel).toarray()
         assert b.shape == (r.mesh.ndof, 1)
         b = L.assemble(parallel=parallel).toarray()
         assert b.shape == (r.mesh.ndof, 1)
 
@@ -194,19 +183,17 @@
         b = L.assemble(x, parallel=parallel).toarray()
         assert b.shape == (r.mesh.npoints, 1)
         b = L.assemble(parallel=parallel).toarray()
         assert b.shape == (r.mesh.npoints, 1)
 
 
 def test_bilinearform():
-
     r, u, p, P, A = pre()
 
     for parallel in [False, True]:
-
         a = fe.IntegralForm(A, u, r.dV, u)
         y = a.integrate(parallel=parallel)
         K = a.assemble(y, parallel=parallel).toarray()
         assert K.shape == (r.mesh.ndof, r.mesh.ndof)
         K = a.assemble(parallel=parallel).toarray()
         assert K.shape == (r.mesh.ndof, r.mesh.ndof)
 
@@ -215,19 +202,17 @@
         K = a.assemble(y, parallel=parallel).toarray()
         assert K.shape == (r.mesh.ndof, r.mesh.npoints)
         K = a.assemble(parallel=parallel).toarray()
         assert K.shape == (r.mesh.ndof, r.mesh.npoints)
 
 
 def test_bilinearform_broadcast():
-
     r, u, p, P, A = pre_broadcast()
 
     for parallel in [False, True]:
-
         a = fe.IntegralForm(A, u, r.dV, u, [True], [True])
         y = a.integrate(parallel=parallel)
         K = a.assemble(y, parallel=parallel).toarray()
         assert K.shape == (r.mesh.ndof, r.mesh.ndof)
         K = a.assemble(parallel=parallel).toarray()
         assert K.shape == (r.mesh.ndof, r.mesh.ndof)
 
@@ -245,19 +230,17 @@
         K = a.assemble(y, parallel=parallel).toarray()
         assert K.shape == (r.mesh.npoints, r.mesh.npoints)
         K = a.assemble(parallel=parallel).toarray()
         assert K.shape == (r.mesh.npoints, r.mesh.npoints)
 
 
 def test_mixed():
-
     r, v, f, A = pre_mixed()
 
     for parallel in [False, True]:
-
         a = fe.IntegralForm(A, v, r.dV, v)
         y = a.integrate(parallel=parallel)
         K = a.assemble(y, parallel=parallel).toarray()
         K = a.assemble(parallel=parallel).toarray()
 
         z = r.mesh.ndof + 2 * r.mesh.npoints
         assert K.shape == (z, z)
@@ -268,15 +251,14 @@
         b = L.assemble(parallel=parallel).toarray()
 
         assert b.shape == (z, 1)
 
     r, v, f, A = pre_axi_mixed()
 
     for parallel in [False, True]:
-
         a = fe.IntegralForm(A, v, r.dV, v)
         y = a.integrate(parallel=parallel)
         K = a.assemble(y, parallel=parallel).toarray()
         K = a.assemble(parallel=parallel).toarray()
 
         z = r.mesh.ndof + 2 * r.mesh.npoints
         assert K.shape == (z, z)
```

### Comparing `felupe-7.4.1/tests/test_job.py` & `felupe-7.5.0/tests/test_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import numpy as np
 import pytest
 
 import felupe as fem
 
 
 def pre():
-
     mesh = fem.Rectangle(n=2)
     region = fem.RegionQuad(mesh)
     field = fem.FieldsMixed(region, n=3, axisymmetric=True)
 
     umat = fem.ThreeFieldVariation(fem.NeoHooke(1, 5000))
     body = fem.SolidBody(umat, field)
     bounds, loadcase = fem.dof.uniaxial(field)
@@ -40,48 +39,44 @@
         boundaries=bounds,
     )
 
     return field, step
 
 
 def test_job():
-
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate()
 
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate(parallel=True, kwargs={"parallel": False}, verbose=0)
 
 
 def test_job_xdmf():
-
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate()
 
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate(filename="result.xdmf", parallel=True, verbose=2)
 
 
 def test_job_xdmf_global_field():
-
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate()
 
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate(filename="result.xdmf", x0=field)
 
 
 def test_curve():
-
     field, step = pre()
 
     curve = fem.CharacteristicCurve(steps=[step], boundary=step.boundaries["move"])
 
     with pytest.raises(ValueError):
         curve.plot()
 
@@ -93,62 +88,58 @@
     area = 1**2 * np.pi
     force = (stretch - 1 / stretch**2) * area
 
     assert np.allclose(np.array(curve.y)[:, 0], force, rtol=0.01)
 
 
 def test_curve2():
-
     field, step = pre()
 
     curve = fem.CharacteristicCurve(steps=[step], boundary=step.boundaries["move"])
     curve.evaluate()
     curve.plot(xaxis=0, yaxis=0)
 
     stretch = 1 + np.array(curve.x)[:, 0]
     area = 1**2 * np.pi
     force = (stretch - 1 / stretch**2) * area
 
     assert np.allclose(np.array(curve.y)[:, 0], force, rtol=0.01)
 
 
 def test_curve_custom_items():
-
     field, step = pre()
 
     curve = fem.CharacteristicCurve(
         steps=[step], items=step.items, boundary=step.boundaries["move"]
     )
     curve.evaluate()
-    curve.plot(xaxis=0, yaxis=0, gradient=True)
+    curve.plot(xaxis=0, yaxis=0, gradient=True, swapaxes=True, xlabel="x", ylabel="y")
     curve.plot(x=np.zeros((10, 2)), y=np.ones((10, 2)), xaxis=0, yaxis=0)
 
     stretch = 1 + np.array(curve.x)[:, 0]
     area = 1**2 * np.pi
     force = (stretch - 1 / stretch**2) * area
 
     assert np.allclose(np.array(curve.y)[:, 0], force, rtol=0.01)
 
 
 def test_empty():
-
     mesh = fem.Cube(n=2)
     region = fem.RegionHexahedron(mesh)
     field = fem.FieldsMixed(region, n=1)
 
     umat = fem.NeoHooke(mu=1, bulk=5000)
     solid = fem.SolidBody(umat, field)
 
     step = fem.Step(items=[solid], ramp=None, boundaries=None)
     job = fem.Job(steps=[step])
     job.evaluate()
 
 
 def test_noramp():
-
     mesh = fem.Cube(n=2)
     region = fem.RegionHexahedron(mesh)
     field = fem.FieldsMixed(region, n=1)
 
     umat = fem.LinearElastic(E=1, nu=0.3)
     solid = fem.SolidBody(umat, field)
     bounds = fem.dof.uniaxial(field)[0]
```

### Comparing `felupe-7.4.1/tests/test_math.py` & `felupe-7.5.0/tests/test_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,14 @@
     fe.math.eig(C)
 
     fe.math.majortranspose(A)
     fe.math.trace(C)
 
 
 def test_math_linsteps():
-
     steps = fe.math.linsteps([0, 1], num=10)
     assert len(steps) == 11
 
     steps = fe.math.linsteps([0, 1, 0], num=(10, 100))
     assert len(steps) == 111
 
     steps = fe.math.linsteps([1], num=0)
```

### Comparing `felupe-7.4.1/tests/test_mechanics.py` & `felupe-7.5.0/tests/test_mechanics.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import numpy as np
 import pytest
 
 import felupe as fe
 
 
 def test_simple():
-
     umat = fe.LinearElastic(E=1, nu=0.3)
 
     m = fe.Cube(n=3)
     r = fe.RegionHexahedron(m)
     u = fe.FieldContainer([fe.Field(r, dim=3)])
 
     b = fe.SolidBody(umat, u)
@@ -56,15 +55,14 @@
     assert P[0].shape == (3, 3, 8, 8)
     assert s.shape == (3, 3, 8, 8)
     assert t.shape == (3, 3, 8, 8)
     assert C[0].shape == (3, 3, 3, 3, 1, 1)
 
 
 def test_pressure():
-
     umat = fe.LinearElastic(E=1, nu=0.3)
 
     m = fe.Cube(n=3)
     h = fe.RegionHexahedron(m)
     u = fe.Field(h, dim=3)
 
     np.random.seed(156)
@@ -114,43 +112,40 @@
     w[0].values = np.random.rand(*w[0].values.shape) / 10
 
     c._update(w, v)
     assert np.allclose(w[0].values, v[0].values)
 
 
 def pre(dim, bulk=2):
-
     umat = fe.NeoHooke(mu=1, bulk=bulk)
 
     m = fe.Cube(n=3)
     r = fe.RegionHexahedron(m)
     u = fe.Field(r, dim=dim)
 
     np.random.seed(156)
     u.values = np.random.rand(*u.values.shape) / 10
 
     return umat, fe.FieldContainer([u])
 
 
 def pre_axi(bulk=2):
-
     umat = fe.NeoHooke(mu=1, bulk=bulk)
 
     m = fe.Rectangle(n=3)
     r = fe.RegionQuad(m)
     u = fe.FieldAxisymmetric(r)
 
     np.random.seed(156)
     u.values = np.random.rand(*u.values.shape) / 10
 
     return umat, fe.FieldContainer([u])
 
 
 def pre_mixed(dim):
-
     umat = fe.ThreeFieldVariation(fe.NeoHooke(mu=1, bulk=2))
 
     m = fe.Cube(n=3)
     r = fe.RegionHexahedron(m)
     u = fe.FieldsMixed(r, n=3)
 
     np.random.seed(156)
@@ -158,20 +153,18 @@
     u[1].values = np.random.rand(*u[1].values.shape) / 10
     u[2].values = np.random.rand(*u[2].values.shape) / 10
 
     return umat, u
 
 
 def test_solidbody():
-
     umat, u = pre(dim=3)
     b = fe.SolidBody(umat=umat, field=u, statevars=np.ones(5))
 
     for parallel in [False, True]:
-
         kwargs = {"parallel": parallel}
 
         r1 = b.assemble.vector(u, **kwargs)
         assert r1.shape == (81, 1)
 
         r1b = b.results.force
         assert np.allclose(r1.toarray(), r1b.toarray())
@@ -208,27 +201,25 @@
 
         t1 = b.evaluate.kirchhoff_stress()
         t2 = b.evaluate.kirchhoff_stress(u)
         assert np.allclose(t1, t2)
 
 
 def test_solidbody_incompressible():
-
     umat, u = pre(dim=3, bulk=None)
     b = fe.SolidBodyNearlyIncompressible(
         umat=umat, field=u, bulk=5000, statevars=np.ones(5)
     )
 
     umat = fe.OgdenRoxburgh(fe.NeoHooke(mu=1), r=3, m=1, beta=0)
     b = fe.SolidBodyNearlyIncompressible(
         umat=umat, field=u, bulk=5000, state=fe.StateNearlyIncompressible(u)
     )
 
     for parallel in [False, True]:
-
         kwargs = {"parallel": parallel}
 
         r1 = b.assemble.vector(u, **kwargs)
         assert r1.shape == (81, 1)
 
         r1b = b.results.force
         assert np.allclose(r1.toarray(), r1b.toarray())
@@ -265,23 +256,21 @@
 
         t1 = b.evaluate.kirchhoff_stress()
         t2 = b.evaluate.kirchhoff_stress(u)
         assert np.allclose(t1, t2)
 
 
 def test_solidbody_axi():
-
     umat, u = pre_axi(bulk=None)
     b = fe.SolidBodyNearlyIncompressible(umat=umat, field=u, bulk=5000)
     b = fe.SolidBodyNearlyIncompressible(
         umat=umat, field=u, bulk=5000, state=fe.StateNearlyIncompressible(u)
     )
 
     for parallel in [False, True]:
-
         kwargs = {"parallel": parallel}
 
         r1 = b.assemble.vector(u, **kwargs)
         assert r1.shape == (18, 1)
 
         r2 = b.assemble.vector(**kwargs)
         assert np.allclose(r1.toarray(), r2.toarray())
@@ -312,20 +301,18 @@
 
         t1 = b.evaluate.kirchhoff_stress()
         t2 = b.evaluate.kirchhoff_stress(u)
         assert np.allclose(t1, t2)
 
 
 def test_solidbody_axi_incompressible():
-
     umat, u = pre_axi()
     b = fe.SolidBody(umat=umat, field=u)
 
     for parallel in [False, True]:
-
         kwargs = {"parallel": parallel}
 
         r1 = b.assemble.vector(u, **kwargs)
         assert r1.shape == (18, 1)
 
         r2 = b.assemble.vector(**kwargs)
         assert np.allclose(r1.toarray(), r2.toarray())
@@ -356,23 +343,21 @@
 
         t1 = b.evaluate.kirchhoff_stress()
         t2 = b.evaluate.kirchhoff_stress(u)
         assert np.allclose(t1, t2)
 
 
 def test_solidbody_mixed():
-
     umat, u = pre_mixed(dim=3)
     b = fe.SolidBody(umat=umat, field=u)
     g = fe.SolidBodyGravity(field=u, gravity=[9810, 0, 0], density=7.85e-9)
 
     g.assemble.vector()
 
     for parallel in [False, True]:
-
         kwargs = {"parallel": parallel}
 
         r1 = b.assemble.vector(u, **kwargs)
         r1 = b.assemble.vector(u, items=3, **kwargs)
         assert r1.shape == (97, 1)
 
         r2 = b.assemble.vector(**kwargs)
@@ -422,17 +407,15 @@
 
         Kg2 = g.assemble.matrix(**kwargs)
         assert Kg1.shape == (97, 97)
         assert np.allclose(Kg1.toarray(), Kg2.toarray())
 
 
 def test_load():
-
     for axi in [False, True]:
-
         if axi:
             umat, field = pre(dim=3)
         else:
             umat, field = pre_axi()
 
         mask = field.region.mesh.points[:, 0] == 1
         values = 0.1
```

### Comparing `felupe-7.4.1/tests/test_mesh.py` & `felupe-7.5.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-7.4.1/tests/test_mpc.py` & `felupe-7.5.0/tests/test_mpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import numpy as np
 import pytest
 
 import felupe as fe
 
 
 def test_mpc():
-
     mesh = fe.Cube(n=3)
     mesh.points = np.vstack((mesh.points, [2, 0, 0]))
     mesh.update(mesh.cells)
 
     region = fe.RegionHexahedron(mesh)
 
     u = fe.FieldContainer([fe.Field(region, dim=3)])
@@ -68,15 +67,14 @@
         K = bilinearform.assemble() + K_RBE2
 
         assert r.shape == (84, 1)
         assert K.shape == (84, 84)
 
 
 def pre_mpc_mixed(point, values):
-
     mesh = fe.mesh.Cube(n=3)
     mesh.points = np.vstack((mesh.points, point))
     mesh.update(mesh.cells)
 
     region = fe.RegionHexahedron(mesh)
     dV = region.dV
 
@@ -127,15 +125,14 @@
 
 def test_mpc_mixed():
     pre_mpc_mixed(point=[2, 0, 0], values=[0, 0, 0])
     pre_mpc_mixed(point=[2, 0, 0], values=[-5, 0, 0])
 
 
 def test_mpc_isolated():
-
     mesh = fe.mesh.Line(n=3)
     mesh.update(mesh.cells[:1])
     mesh.points = np.pad(mesh.points, ((0, 0), (0, 2)))
     mesh.points[-1] = np.array([1, 0.5, 0.5])
     mesh.dim = 3
     mesh.ndof = 9
```

### Comparing `felupe-7.4.1/tests/test_planestrain.py` & `felupe-7.5.0/tests/test_planestrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import numpy as np
 import pytest
 
 import felupe as fem
 
 
 def test_axi():
-
     m = fem.Rectangle(n=11)
     r = fem.RegionQuad(m)
     f = fem.FieldsMixed(r, n=1, axisymmetric=True)
     u = fem.NeoHooke(mu=1, bulk=1)
     b = fem.SolidBody(u, f)
     loadcase = fem.dof.uniaxial(f, clamped=True)[-1]
     res = fem.newtonrhapson(items=[b], **loadcase)
@@ -47,15 +46,14 @@
     assert len(u) == 3
     assert strain.shape[:-2] == (3, 3)
 
     assert res.success
 
 
 def test_axi_mixed():
-
     m = fem.Rectangle(n=6)
     r = fem.RegionQuad(m)
     f = fem.FieldsMixed(r, n=3, axisymmetric=True)
     u = fem.ThreeFieldVariation(fem.NeoHooke(mu=1, bulk=5000))
     b = fem.SolidBody(u, f)
     loadcase = fem.dof.uniaxial(f, clamped=True)[-1]
     res = fem.newtonrhapson(items=[b], **loadcase)
@@ -66,15 +64,14 @@
     assert len(u) == 3
     assert strain.shape[:-2] == (3, 3)
 
     assert res.success
 
 
 def test_planestrain():
-
     m = fem.Rectangle(n=6)
     r = fem.RegionQuad(m)
 
     f = fem.FieldsMixed(r, n=1, planestrain=True)
     g = fem.FieldsMixed(r, n=1, planestrain=False)
 
     u = fem.LinearElastic(E=1, nu=0.3)
@@ -87,15 +84,14 @@
     s = fem.newtonrhapson(items=[c], **fem.dof.uniaxial(f, clamped=True)[-1])
 
     assert np.allclose(r.x.values(), s.x.values())
     assert np.allclose(r.fun, s.fun)
 
 
 def test_planestrain_nh():
-
     m = fem.Rectangle(n=6)
     r = fem.RegionQuad(m)
     f = fem.FieldsMixed(r, n=1, planestrain=True)
     u = fem.NeoHooke(mu=1, bulk=2)
     b = fem.SolidBody(u, f)
     loadcase = fem.dof.uniaxial(f, clamped=True)[-1]
     res = fem.newtonrhapson(items=[b], **loadcase)
@@ -106,15 +102,14 @@
     assert len(u) == 3
     assert strain.shape[:-2] == (3, 3)
 
     assert res.success
 
 
 def test_planestrain_nh_mixed():
-
     m = fem.Rectangle(n=6)
     r = fem.RegionQuad(m)
     f = fem.FieldsMixed(r, n=3, planestrain=True)
     u = fem.ThreeFieldVariation(fem.NeoHooke(mu=1, bulk=5000))
     b = fem.SolidBody(u, f)
     loadcase = fem.dof.uniaxial(f, clamped=True)[-1]
     res = fem.newtonrhapson(items=[b], **loadcase)
```

### Comparing `felupe-7.4.1/tests/test_plot.py` & `felupe-7.5.0/tests/test_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000)
     move = fem.math.linsteps([0, 1], num=3)
     step = fem.Step(
         items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries
     )
     fem.Job(steps=[step]).evaluate(filename="result.xdmf", verbose=False)
 
-    return mesh, field
+    return mesh, field, solid
 
 
 def pre_2d(n=3):
     mesh = fem.Rectangle(n=n)
     region = fem.RegionQuad(mesh)
     field = fem.FieldContainer([fem.FieldPlaneStrain(region, dim=2)])
     boundaries = fem.dof.uniaxial(field, clamped=True)[0]
@@ -53,19 +53,18 @@
     solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000)
     move = fem.math.linsteps([0, 1], num=3)
     step = fem.Step(
         items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries
     )
     fem.Job(steps=[step]).evaluate(filename="result.xdmf", verbose=False)
 
-    return mesh, field
+    return mesh, field, solid
 
 
 def test_xdmf_cell_data():
-
     try:
         import pyvista
 
         pre(n=3)
 
         # TODO: Remove if pyvista has a release with ``XdmfReader`` included.
         major, minor = pyvista.__version__.split(".")[:2]
@@ -80,15 +79,14 @@
             # plotter.show(screenshot="cube-xdmf.png")
 
     except ModuleNotFoundError:
         pass
 
 
 def test_xdmf_point_data():
-
     try:
         import pyvista
 
         pre_2d(n=3)
 
         # TODO: Remove if pyvista has a release with ``XdmfReader`` included.
         major, minor = pyvista.__version__.split(".")[:2]
@@ -104,19 +102,18 @@
             # plotter.show(screenshot="rectangle-xdmf.png")
 
     except ModuleNotFoundError:
         pass
 
 
 def test_cell_data():
-
     try:
         import pyvista
 
-        mesh, field = pre(n=3)
+        mesh, field, solid = pre(n=3)
         view = fem.View(
             field,
             point_data={"My Displacements": field[0].values},
             cell_data={"Cell Volume": field.region.dV.sum(0).ravel()},
             cell_type=pyvista.CellType.HEXAHEDRON,
         )
         plotter = view.plot(
@@ -131,48 +128,45 @@
         # plotter.show(screenshot="cube.png")
 
     except ModuleNotFoundError:
         pass
 
 
 def test_point_data():
-
     try:
-        mesh, field = pre_2d(n=3)
+        mesh, field, solid = pre_2d(n=3)
         view = fem.View(field)
         plotter = view.plot(
             "Displacement",
             off_screen=True,
             scalar_bar_vertical=False,
         )
         # plotter.show(screenshot="rectangle.png")
 
     except ModuleNotFoundError:
         pass
 
 
 def test_mesh():
-
     try:
-        mesh, field = pre(n=3)
+        mesh, field, solid = pre(n=3)
         view = fem.ViewMesh(mesh)
         plotter = view.plot(
             off_screen=True,
         )
         # plotter.show(screenshot="cube.png")
 
     except ModuleNotFoundError:
         pass
 
 
 def test_model():
-
     try:
-        mesh, field = pre(n=3)
-        view = fem.View(field)
+        mesh, field, solid = pre(n=3)
+        view = fem.View(field, solid=solid)
         plotter = view.plot(
             off_screen=True,
         )
         # plotter.show(screenshot="undeformed.png")
 
     except ModuleNotFoundError:
         pass
```

### Comparing `felupe-7.4.1/tests/test_quadrature.py` & `felupe-7.5.0/tests/test_quadrature.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     assert np.allclose(q23.weights, q23.inv().weights)
 
     with pytest.raises(ValueError):
         fe.GaussLegendre(order=1, dim=4)
 
 
 def test_gausslegendre_boundary():
-
     with pytest.raises(ValueError):
         q11 = fe.GaussLegendreBoundary(order=1, dim=1)
         assert q11.points.shape == (2, 1)
         assert q11.weights.sum() == 2
 
     for permute in [False, True]:
         q12 = fe.GaussLegendreBoundary(order=1, dim=2, permute=permute)
```

### Comparing `felupe-7.4.1/tests/test_readme.py` & `felupe-7.5.0/tests/test_readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 @author: adutz
 """
 
 import numpy as np
 
 
 def test_readme():
-
     import felupe
 
     mesh = felupe.Cube(n=9)
     element = felupe.Hexahedron()
     quadrature = felupe.GaussLegendre(order=1, dim=3)
 
     region = felupe.Region(mesh, element, quadrature)
```

### Comparing `felupe-7.4.1/tests/test_region.py` & `felupe-7.5.0/tests/test_region.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import numpy as np
 import pytest
 
 import felupe as fe
 
 
 def test_region():
-
     mesh = fe.Rectangle()
     r = fe.RegionQuad(mesh)
     r = fe.RegionQuadBoundary(mesh)
     r = fe.RegionQuadBoundary(mesh, ensure_3d=True)
     r = fe.RegionConstantQuad(mesh)
 
     mesh2 = fe.mesh.convert(mesh, 2, True, False, False)
```

### Comparing `felupe-7.4.1/tests/test_solve.py` & `felupe-7.5.0/tests/test_solve.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 import numpy as np
 
 import felupe as fe
 
 
 def test_solve():
-
     m = fe.Cube(n=3)
     e = fe.Hexahedron()
     q = fe.GaussLegendre(1, 3)
     r = fe.Region(m, e, q)
     u = fe.Field(r, dim=3)
     v = fe.FieldContainer([u])
```

### Comparing `felupe-7.4.1/tests/test_tools.py` & `felupe-7.5.0/tests/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,26 @@
 import numpy as np
 import pytest
 
 import felupe as fe
 
 
 def pre():
-
     r = fe.RegionHexahedron(fe.Cube(n=3))
 
     u = fe.Field(r, dim=3)
     p = fe.Field(r)
     J = fe.Field(r, values=1)
 
     f = fe.FieldContainer((u, p, J))
 
     return r, f, (u, p, J)
 
 
 def test_solve():
-
     r, _, (u, p, J) = pre()
     f = fe.FieldContainer([u])
 
     W = fe.constitution.NeoHooke(1, 3)
 
     F = f.extract()
 
@@ -92,15 +90,14 @@
     assert cauchy.shape == (r.mesh.cells.size, 6)
 
     cauchy = fe.tools.project(fe.math.tovoigt(s), region=r, mean=True)
     assert cauchy.shape == (r.mesh.npoints, 6)
 
 
 def test_solve_mixed():
-
     r, f, fields = pre()
     u = fields[0]
 
     f = fe.FieldContainer(fields)
 
     F, p, J = f.extract()
 
@@ -165,39 +162,36 @@
 
     with pytest.raises(ValueError):
         x0 = np.array([np.nan])
         res = fe.tools.newtonrhapson(x0, fun, jac, solve=np.linalg.solve)
 
 
 def test_newton():
-
     # create a hexahedron-region on a cube
     region = fe.RegionHexahedron(fe.Cube(n=6))
 
     # add a displacement field and apply a uniaxial elongation on the cube
     displacement = fe.Field(region, dim=3)
     field = fe.FieldContainer([displacement])
     boundaries, loadcase = fe.dof.uniaxial(field, move=0.2, clamped=True)
 
     # define the constitutive material behavior
     umat = fe.NeoHooke(mu=1.0, bulk=2.0)
 
     for kwargs in [{"parallel": True, "umat": umat}]:
-
         # newton-rhapson procedure
         res = fe.newtonrhapson(
             field,
             verbose=True,
             kwargs=kwargs,
             **loadcase,
         )
 
 
 def test_newton_plane():
-
     # create a quad-region on a rectangle
     region = fe.RegionQuad(fe.Rectangle(n=6))
 
     # add a displacement field and apply a uniaxial elongation on the rectangle
     displacement = fe.Field(region, dim=2)
     field = fe.FieldContainer([displacement])
     boundaries, loadcase = fe.dof.uniaxial(field, move=0.2, clamped=True)
@@ -222,15 +216,14 @@
         verbose=True,
         kwargs=dict(umat=umat),
         **loadcase,
     )
 
 
 def test_newton_linearelastic():
-
     # create a hexahedron-region on a cube
     region = fe.RegionHexahedron(fe.Cube(n=6))
 
     # add a displacement field and apply a uniaxial elongation on the cube
     displacement = fe.Field(region, dim=3)
     field = fe.FieldContainer([displacement])
     boundaries, loadcase = fe.dof.uniaxial(field, move=0.2, clamped=True)
@@ -244,15 +237,14 @@
         verbose=True,
         kwargs={"umat": umat, "grad": True, "sym": True, "add_identity": False},
         **loadcase,
     )
 
 
 def test_newton_mixed():
-
     # create a hexahedron-region on a cube
     mesh = fe.Cube(n=6)
     region = fe.RegionHexahedron(mesh)
     region0 = fe.RegionConstantHexahedron(fe.mesh.convert(mesh, 0))
 
     # add a displacement field and apply a uniaxial elongation on the cube
     u = fe.Field(region, dim=3)
@@ -272,15 +264,14 @@
     umat = fe.ThreeFieldVariation(nh)
 
     # newton-rhapson procedure
     res = fe.newtonrhapson(x0=field, kwargs=dict(umat=umat), **loadcase)
 
 
 def test_newton_body():
-
     # create a hexahedron-region on a cube
     mesh = fe.Cube(n=6)
     region = fe.RegionHexahedron(mesh)
     region0 = fe.RegionConstantHexahedron(fe.mesh.convert(mesh, 0))
 
     # add a displacement field and apply a uniaxial elongation on the cube
     u = fe.Field(region, dim=3)
```

