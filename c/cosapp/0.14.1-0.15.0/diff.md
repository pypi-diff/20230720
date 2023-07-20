# Comparing `tmp/cosapp-0.14.1.tar.gz` & `tmp/cosapp-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosapp-0.14.1.tar", last modified: Thu Jun  8 20:17:01 2023, max compression
+gzip compressed data, was "cosapp-0.15.0.tar", last modified: Thu Jul 20 16:29:43 2023, max compression
```

## Comparing `cosapp-0.14.1.tar` & `cosapp-0.15.0.tar`

### file list

```diff
@@ -1,494 +1,497 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.583432 cosapp-0.14.1/
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-06-08 20:16:27.000000 cosapp-0.14.1/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)     3488 2023-06-08 20:16:27.000000 cosapp-0.14.1/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    41166 2023-06-08 20:16:27.000000 cosapp-0.14.1/HISTORY.md
--rw-rw-rw-   0 root         (0) root         (0)     6572 2023-06-08 20:16:27.000000 cosapp-0.14.1/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      754 2023-06-08 20:16:27.000000 cosapp-0.14.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    43628 2023-06-08 20:17:01.583432 cosapp-0.14.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-06-08 20:16:27.000000 cosapp-0.14.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.492431 cosapp-0.14.1/cosapp/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.493431 cosapp-0.14.1/cosapp/base/
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.495431 cosapp-0.14.1/cosapp/core/
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4354 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/configuration_schema.json
--rw-rw-rw-   0 root         (0) root         (0)    18754 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/eval_str.py
--rw-rw-rw-   0 root         (0) root         (0)    15819 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.497431 cosapp-0.14.1/cosapp/core/numerics/
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/numerics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27541 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/numerics/basics.py
--rw-rw-rw-   0 root         (0) root         (0)    28053 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/numerics/boundary.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/numerics/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2948 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/numerics/mathematicalproblem.schema.json
--rw-rw-rw-   0 root         (0) root         (0)    13455 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/numerics/residues.py
--rw-rw-rw-   0 root         (0) root         (0)    19400 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/numerics/root.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/numerics/sobol_seq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.497431 cosapp-0.14.1/cosapp/core/signal/
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/signal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4972 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/signal/signal.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/signal/slot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.499431 cosapp-0.14.1/cosapp/core/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8079 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15027 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/tests/test_AssignString.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/tests/test_ContextLocals.py
--rw-rw-rw-   0 root         (0) root         (0)    12340 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/tests/test_EvalString.py
--rw-rw-rw-   0 root         (0) root         (0)    13397 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/tests/test_Module.py
--rw-rw-rw-   0 root         (0) root         (0)     6502 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/tests/test_coSAppConfiguration.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/tests/test_time.py
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/core/variableref.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.502431 cosapp-0.14.1/cosapp/drivers/
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/abstractsetofcases.py
--rw-rw-rw-   0 root         (0) root         (0)    12109 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/abstractsolver.py
--rw-rw-rw-   0 root         (0) root         (0)     8692 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/driver.py
--rw-rw-rw-   0 root         (0) root         (0)     9484 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/influence.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/iterativecase.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/lineardoe.py
--rw-rw-rw-   0 root         (0) root         (0)     3131 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/metasystembuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    10683 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/montecarlo.py
--rw-rw-rw-   0 root         (0) root         (0)    26684 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/nonlinearsolver.py
--rw-rw-rw-   0 root         (0) root         (0)    22339 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/optimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/optionaldriver.py
--rw-rw-rw-   0 root         (0) root         (0)     6655 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/runonce.py
--rw-rw-rw-   0 root         (0) root         (0)    11432 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/runsinglecase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.503431 cosapp-0.14.1/cosapp/drivers/time/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/euler.py
--rw-rw-rw-   0 root         (0) root         (0)    19963 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3457 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/runge_kutta.py
--rw-rw-rw-   0 root         (0) root         (0)    13729 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.508431 cosapp-0.14.1/cosapp/drivers/time/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15016 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6501 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_BouncingBall.py
--rw-rw-rw-   0 root         (0) root         (0)     2599 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_DiscreteStepper.py
--rw-rw-rw-   0 root         (0) root         (0)     4202 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_EulerExplicit.py
--rw-rw-rw-   0 root         (0) root         (0)    18994 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py
--rw-rw-rw-   0 root         (0) root         (0)     1501 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_InterpolAssignString.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_Interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_NewtonPendulum.py
--rw-rw-rw-   0 root         (0) root         (0)    25908 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_RungeKutta.py
--rw-rw-rw-   0 root         (0) root         (0)    22334 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_Scenario.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_SystemInterpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeAssignString.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeStepManager.py
--rw-rw-rw-   0 root         (0) root         (0)     8108 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeUnknownDict.py
--rw-rw-rw-   0 root         (0) root         (0)     4478 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeUnknownStack.py
--rw-rw-rw-   0 root         (0) root         (0)     2914 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeVarManager.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py
--rw-rw-rw-   0 root         (0) root         (0)     9926 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_event_cascades.py
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/tests/test_modevar_init.py
--rw-rw-rw-   0 root         (0) root         (0)    21544 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/time/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    15033 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/drivers/validitycheck.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.508431 cosapp-0.14.1/cosapp/multimode/
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/multimode/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5937 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/multimode/discreteStepper.py
--rw-rw-rw-   0 root         (0) root         (0)    11879 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/multimode/event.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/multimode/zeroCrossing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.509431 cosapp-0.14.1/cosapp/patterns/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/patterns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3411 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/patterns/observer.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/patterns/singleton.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/patterns/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.511431 cosapp-0.14.1/cosapp/ports/
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16224 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4019 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/mode_variable.py
--rw-rw-rw-   0 root         (0) root         (0)    34280 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/port.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/unit_library.ini
--rw-rw-rw-   0 root         (0) root         (0)    33349 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/units.py
--rw-rw-rw-   0 root         (0) root         (0)    31417 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/ports/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.512431 cosapp-0.14.1/cosapp/recorders/
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/recorders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4628 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/recorders/dataframe_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)     7847 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/recorders/dsv_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)    13366 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/recorders/recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.514431 cosapp-0.14.1/cosapp/systems/
--rw-rw-rw-   0 root         (0) root         (0)      741 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6623 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/externalsystem.py
--rw-rw-rw-   0 root         (0) root         (0)    13327 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/metamodels.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/processsystem.py
--rw-rw-rw-   0 root         (0) root         (0)     5246 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/structure.schema.json
--rw-rw-rw-   0 root         (0) root         (0)   132189 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/system.py
--rw-rw-rw-   0 root         (0) root         (0)     3095 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/system.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/systemConnector.py
--rw-rw-rw-   0 root         (0) root         (0)    15645 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/systemSurrogate.py
--rw-rw-rw-   0 root         (0) root         (0)     5515 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/systems/systemfamily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.517431 cosapp-0.14.1/cosapp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/all_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.520431 cosapp-0.14.1/cosapp/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      356 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/default_dataframe.json
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/export_doe.cs
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/export_doe.csv
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/export_doe.json
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/export_doe.txt
--rw-rw-rw-   0 root         (0) root         (0)     1701 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config.json
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_ducts.json
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss.json
--rw-rw-rw-   0 root         (0) root         (0)      312 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss1.json
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss11.json
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss11bis.json
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss12.json
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss121.json
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss131.json
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss2.json
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss22.json
--rw-rw-rw-   0 root         (0) root         (0)     2537 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss222.json
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss2tank.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.521431 cosapp-0.14.1/cosapp/tests/library/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/ports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.522431 cosapp-0.14.1/cosapp/tests/library/systems/
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/systems/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/systems/basicalgebra.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/systems/dynamics.py
--rw-rw-rw-   0 root         (0) root         (0)     3257 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/systems/elec.py
--rw-rw-rw-   0 root         (0) root         (0)     8536 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/systems/multiply.py
--rw-rw-rw-   0 root         (0) root         (0)    11780 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/systems/others.py
--rw-rw-rw-   0 root         (0) root         (0)     4826 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/systems/pressurelossvarious.py
--rw-rw-rw-   0 root         (0) root         (0)     1986 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/library/systems/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_ComplexDuct.py
--rw-rw-rw-   0 root         (0) root         (0)    10101 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_MathematicalProblem_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    10653 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_Turbofan.py
--rw-rw-rw-   0 root         (0) root         (0)     3960 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_dynamics.py
--rw-rw-rw-   0 root         (0) root         (0)     6650 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_electric_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_multimode.py
--rw-rw-rw-   0 root         (0) root         (0)     8095 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_system_pressureloss.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    11887 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_unknown_aliasing.py
--rw-rw-rw-   0 root         (0) root         (0)     5568 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tests/test_visitor_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.523431 cosapp-0.14.1/cosapp/tools/
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.523431 cosapp-0.14.1/cosapp/tools/fmu/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/fmu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22009 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/fmu/exporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3204 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/fmu/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.524431 cosapp-0.14.1/cosapp/tools/fmu/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/fmu/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2606 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/fmu/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    13896 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/fmu/tests/test_exporter.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/fmu/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     4117 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/help.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.525431 cosapp-0.14.1/cosapp/tools/module_parser/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/module_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4279 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/module_parser/package_metadata.schema.json
--rw-rw-rw-   0 root         (0) root         (0)    14905 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/module_parser/parseModule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.525431 cosapp-0.14.1/cosapp/tools/problem_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7945 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/problem_viewer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.526431 cosapp-0.14.1/cosapp/tools/problem_viewer/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   250263 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.526431 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/
--rw-rw-rw-   0 root         (0) root         (0)     9254 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.528431 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/
--rw-rw-rw-   0 root         (0) root         (0)     9483 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js
--rw-rw-rw-   0 root         (0) root         (0)   211120 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/http.js
--rw-rw-rw-   0 root         (0) root         (0)    86659 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js
--rw-rw-rw-   0 root         (0) root         (0)     4679 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.529431 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/constants.js
--rw-rw-rw-   0 root         (0) root         (0)    16285 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/draw.js
--rw-rw-rw-   0 root         (0) root         (0)     5771 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/legend.js
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/modal.js
--rw-rw-rw-   0 root         (0) root         (0)    70307 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/ptN2.js
--rw-rw-rw-   0 root         (0) root         (0)     9486 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/search.js
--rw-rw-rw-   0 root         (0) root         (0)     4155 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/svg.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.530431 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/style/
--rw-rw-rw-   0 root         (0) root         (0)     1815 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/style/awesomplete.css
--rw-rw-rw-   0 root         (0) root         (0)     5612 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/style/fontello.woff
--rw-rw-rw-   0 root         (0) root         (0)     5815 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/style/partition_tree.css
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/problem_viewer/webview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.531431 cosapp-0.14.1/cosapp/tools/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.532431 cosapp-0.14.1/cosapp/tools/templates/lib/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/lib/Readme.txt
--rw-rw-rw-   0 root         (0) root         (0)   236746 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/lib/d3.min.js
--rw-rw-rw-   0 root         (0) root         (0)    23777 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/lib/vis.min.css
--rw-rw-rw-   0 root         (0) root         (0)   663624 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/lib/vis.min.js
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/pythonfmu.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.533431 cosapp-0.14.1/cosapp/tools/templates/src/
--rw-rw-rw-   0 root         (0) root         (0)     4751 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/src/d3_draw.js
--rw-rw-rw-   0 root         (0) root         (0)      451 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/src/d3_styles.css
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/system_d3.html
--rw-rw-rw-   0 root         (0) root         (0)     8155 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/templates/system_repr.html
--rw-rw-rw-   0 root         (0) root         (0)     6675 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.534431 cosapp-0.14.1/cosapp/tools/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/baseRenderer.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/d3js.py
--rw-rw-rw-   0 root         (0) root         (0)     4753 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/markdown.py
--rw-rw-rw-   0 root         (0) root         (0)    20440 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/prettyprint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.535431 cosapp-0.14.1/cosapp/tools/views/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2105 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/tests/test_VisJsRenderer.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/tests/test_d3.py
--rw-rw-rw-   0 root         (0) root         (0)     7927 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/tests/test_markdown.py
--rw-rw-rw-   0 root         (0) root         (0)     5912 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/tests/test_prettyprint.py
--rw-rw-rw-   0 root         (0) root         (0)    16980 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tools/views/visjs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.541431 cosapp-0.14.1/cosapp/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)     3222 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/00-Introduction.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    20810 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/01-Systems.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    15181 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/02-Ports.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18911 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/03-Drivers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2711 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/04-Triggers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18216 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/05-Validation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10391 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/06-Visibility.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8547 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/07-Metamodels.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19784 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/08-Multipoints-Design.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14617 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/09-MonteCarlo.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5749 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/10-Recorders.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10084 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/11-DesignMethods.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/CustomConnectors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3536 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/FMI.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    28157 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/Guidelines.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14967 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/HybridSimulations.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    13505 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/Logging.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4336 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/Optimization.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17402 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/SystemSurrogates.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    21247 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17257 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/Targets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19106 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/TimeDriver.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    16763 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/TimeDriverAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19901 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/TipsAndTricks.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10059 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/Visitors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10314 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/aa-SimpleCircuit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/exprampode_fmu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.546431 cosapp-0.14.1/cosapp/tutorials/images/
--rw-rw-rw-   0 root         (0) root         (0)     3204 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/cosapp.svg
--rw-rw-rw-   0 root         (0) root         (0)    17745 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/design_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)    23419 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/drivers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6953 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/drivers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     7366 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/drivers_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    40831 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/drivers_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     8450 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/drivers_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     4537 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/drivers_nonlinear.svg
--rw-rw-rw-   0 root         (0) root         (0)     2309 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/experimental.svg
--rw-rw-rw-   0 root         (0) root         (0)    10190 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/in_progress.svg
--rw-rw-rw-   0 root         (0) root         (0)    26687 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/ports_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    19983 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/ports_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    30601 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/ports_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    16538 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/simple_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)     9156 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/systems_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    18904 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/systems_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    18945 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/systems_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    24136 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/systems_4.svg
--rw-rw-rw-   0 root         (0) root         (0)    28090 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/systems_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     5070 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/tanks.svg
--rw-rw-rw-   0 root         (0) root         (0)    27536 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/triggers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    24504 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/triggers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6961 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/validity.svg
--rw-rw-rw-   0 root         (0) root         (0)    85431 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/images/visibility.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.547431 cosapp-0.14.1/cosapp/tutorials/multimode/
--rw-rw-rw-   0 root         (0) root         (0)     7019 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/multimode/BouncingBall.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/multimode/MultimodeOde.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5205 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/multimode/NewtonPendulum.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.547431 cosapp-0.14.1/cosapp/tutorials/optimization/
--rw-rw-rw-   0 root         (0) root         (0)     7559 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/optimization/BetzLimit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8420 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/optimization/Sellar.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4400 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/quickstart.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/tutorials/time_solutions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.550431 cosapp-0.14.1/cosapp/utils/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.551431 cosapp-0.14.1/cosapp/utils/distributions/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     2693 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/normal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.552431 cosapp-0.14.1/cosapp/utils/distributions/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/tests/test_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/tests/test_normal.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/tests/test_triangular.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/tests/test_uniform.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/triangular.py
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/distributions/uniform.py
--rw-rw-rw-   0 root         (0) root         (0)     6715 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/find_variables.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/graph_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4604 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/json.py
--rw-rw-rw-   0 root         (0) root         (0)    16769 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3694 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/naming.py
--rw-rw-rw-   0 root         (0) root         (0)    14038 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/options_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)     5169 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     3856 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/pull_variables.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/state_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.554431 cosapp-0.14.1/cosapp/utils/surrogate_models/
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9528 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/kriging.py
--rw-rw-rw-   0 root         (0) root         (0)    39321 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/multifi_cokriging.py
--rw-rw-rw-   0 root         (0) root         (0)     5292 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/nearest_neighbor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.555431 cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5286 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     3158 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py
--rw-rw-rw-   0 root         (0) root         (0)    18553 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     5287 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/response_surface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.556431 cosapp-0.14.1/cosapp/utils/surrogate_models/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/tests/test_kriging.py
--rw-rw-rw-   0 root         (0) root         (0)     6925 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py
--rw-rw-rw-   0 root         (0) root         (0)    16170 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py
--rw-rw-rw-   0 root         (0) root         (0)     3709 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/surrogate_models/tests/test_response_surface.py
--rw-rw-rw-   0 root         (0) root         (0)     8056 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/testing.py
--rw-rw-rw-   0 root         (0) root         (0)     1334 2023-06-08 20:16:27.000000 cosapp-0.14.1/cosapp/utils/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.493431 cosapp-0.14.1/cosapp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43628 2023-06-08 20:17:01.000000 cosapp-0.14.1/cosapp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15997 2023-06-08 20:17:01.000000 cosapp-0.14.1/cosapp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 20:17:01.000000 cosapp-0.14.1/cosapp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 20:17:01.000000 cosapp-0.14.1/cosapp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-08 20:17:01.000000 cosapp-0.14.1/cosapp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 20:17:01.000000 cosapp-0.14.1/cosapp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.558431 cosapp-0.14.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)    11509 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.558431 cosapp-0.14.1/docs/cosapp_theme/
--rw-rw-rw-   0 root         (0) root         (0)     2422 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/layout.html
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.559431 cosapp-0.14.1/docs/cosapp_theme/static/
--rw-rw-rw-   0 root         (0) root         (0)     8997 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/cosapp.css_t
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.561432 cosapp-0.14.1/docs/cosapp_theme/static/css/
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/custom.css
--rw-rw-rw-   0 root         (0) root         (0)    31000 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/font.css
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/highlight.css
--rw-rw-rw-   0 root         (0) root         (0)    40062 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/kube.css
--rw-rw-rw-   0 root         (0) root         (0)     8764 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/kube.demo.css
--rw-rw-rw-   0 root         (0) root         (0)     9250 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/kube.legenda.css
--rw-rw-rw-   0 root         (0) root         (0)    30268 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/kube.min.css
--rw-rw-rw-   0 root         (0) root         (0)    26211 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/master.css
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/css/mermaid.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.563431 cosapp-0.14.1/docs/cosapp_theme/static/font/
--rw-rw-rw-   0 root         (0) root         (0)   297272 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Black.woff
--rw-rw-rw-   0 root         (0) root         (0)   328952 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Bold.woff
--rw-rw-rw-   0 root         (0) root         (0)   347092 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-BoldItalic.woff
--rw-rw-rw-   0 root         (0) root         (0)   343528 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Italic.woff
--rw-rw-rw-   0 root         (0) root         (0)   323172 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Regular.woff
--rw-rw-rw-   0 root         (0) root         (0)   326132 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Semibold.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.564432 cosapp-0.14.1/docs/cosapp_theme/static/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    98024 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.564432 cosapp-0.14.1/docs/cosapp_theme/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     5930 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/img/cosapp.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.565431 cosapp-0.14.1/docs/cosapp_theme/static/js/
--rw-rw-rw-   0 root         (0) root         (0)    84380 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/js/jquery-2.1.4.min.js
--rw-rw-rw-   0 root         (0) root         (0)    56646 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/js/kube.js
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/js/kube.legenda.js
--rw-rw-rw-   0 root         (0) root         (0)    31683 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/js/kube.min.js
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/js/master.js
--rw-rw-rw-   0 root         (0) root         (0)    12047 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/js/tocbot.min.js
--rw-rw-rw-   0 root         (0) root         (0)     5219 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/static/sidebar.js_t
--rw-rw-rw-   0 root         (0) root         (0)      736 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/cosapp_theme/theme.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.566431 cosapp-0.14.1/docs/developer/
--rw-rw-rw-   0 root         (0) root         (0)     2923 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/developer/installation_cases.rst
--rw-rw-rw-   0 root         (0) root         (0)     8633 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/developer/logger.rst
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/developer/project_structure.rst
--rw-rw-rw-   0 root         (0) root         (0)    12553 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/developer/scenarii.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.567432 cosapp-0.14.1/docs/img/
--rw-rw-rw-   0 root         (0) root         (0)     2475 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/img/gitlab-cosapp-f4950f.svg
--rw-rw-rw-   0 root         (0) root         (0)     4393 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/img/website-docs-blue.svg
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/license.rst
--rw-rw-rw-   0 root         (0) root         (0)     6499 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.489431 cosapp-0.14.1/docs/nb_thumbnails/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.569431 cosapp-0.14.1/docs/nb_thumbnails/_images/
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/desktop-download.svg
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/eye.svg
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/file-code.svg
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/file-text.svg
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/fold.svg
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/package.svg
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/pencil.svg
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/play.svg
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/plug.svg
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/pulse.svg
--rw-rw-rw-   0 root         (0) root         (0)      729 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/verified.svg
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/nb_thumbnails/_images/zap.svg
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.569431 cosapp-0.14.1/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)     3731 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/source/modules.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.570432 cosapp-0.14.1/docs/tools/
--rw-rw-rw-   0 root         (0) root         (0)    13384 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tools/mermaid.py
--rw-rw-rw-   0 root         (0) root         (0)    10131 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tools/mermaid_inheritance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.576432 cosapp-0.14.1/docs/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)     3222 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/00-Introduction.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    20810 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/01-Systems.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    15181 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/02-Ports.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18911 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/03-Drivers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2711 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/04-Triggers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18216 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/05-Validation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10391 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/06-Visibility.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8547 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/07-Metamodels.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19784 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/08-Multipoints-Design.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14617 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/09-MonteCarlo.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5749 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/10-Recorders.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10084 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/11-DesignMethods.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/CustomConnectors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3536 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/FMI.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    28157 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/Guidelines.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14967 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/HybridSimulations.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    13505 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/Logging.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4336 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/Optimization.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17402 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/SystemSurrogates.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    21247 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/SystemSurrogatesAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17257 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/Targets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19106 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/TimeDriver.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    16763 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/TimeDriverAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19901 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/TipsAndTricks.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10059 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/Visitors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10314 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/aa-SimpleCircuit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/exprampode_fmu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.581431 cosapp-0.14.1/docs/tutorials/images/
--rw-rw-rw-   0 root         (0) root         (0)    84424 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/Moise_tables_loi.jpg
--rw-rw-rw-   0 root         (0) root         (0)     3204 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/cosapp.svg
--rw-rw-rw-   0 root         (0) root         (0)    17745 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/design_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)    23419 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/drivers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6953 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/drivers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     7366 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/drivers_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    40831 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/drivers_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     8450 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/drivers_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     4537 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/drivers_nonlinear.svg
--rw-rw-rw-   0 root         (0) root         (0)     2309 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/experimental.svg
--rw-rw-rw-   0 root         (0) root         (0)    10190 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/in_progress.svg
--rw-rw-rw-   0 root         (0) root         (0)    26687 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/ports_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    19983 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/ports_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    30601 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/ports_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    16538 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/simple_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)     9156 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/systems_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    18904 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/systems_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    18945 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/systems_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    24136 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/systems_4.svg
--rw-rw-rw-   0 root         (0) root         (0)    28090 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/systems_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     5070 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/tanks.svg
--rw-rw-rw-   0 root         (0) root         (0)    27536 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/triggers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    24504 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/triggers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6961 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/validity.svg
--rw-rw-rw-   0 root         (0) root         (0)    85431 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/images/visibility.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.582432 cosapp-0.14.1/docs/tutorials/multimode/
--rw-rw-rw-   0 root         (0) root         (0)     7019 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/multimode/BouncingBall.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4001 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/multimode/MultimodeOde.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5205 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/multimode/NewtonPendulum.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 20:17:01.583432 cosapp-0.14.1/docs/tutorials/optimization/
--rw-rw-rw-   0 root         (0) root         (0)     7559 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/optimization/BetzLimit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8420 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/optimization/Sellar.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4400 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/quickstart.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3233 2023-06-08 20:16:27.000000 cosapp-0.14.1/docs/tutorials/time_solutions.py
--rw-rw-rw-   0 root         (0) root         (0)     2035 2023-06-08 20:17:01.584432 cosapp-0.14.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-08 20:16:27.000000 cosapp-0.14.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.606434 cosapp-0.15.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-07-20 16:29:08.000000 cosapp-0.15.0/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)     3488 2023-07-20 16:29:08.000000 cosapp-0.15.0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    42310 2023-07-20 16:29:08.000000 cosapp-0.15.0/HISTORY.md
+-rw-rw-rw-   0 root         (0) root         (0)     6572 2023-07-20 16:29:08.000000 cosapp-0.15.0/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      754 2023-07-20 16:29:08.000000 cosapp-0.15.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    44772 2023-07-20 16:29:43.606434 cosapp-0.15.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-20 16:29:08.000000 cosapp-0.15.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.518435 cosapp-0.15.0/cosapp/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.520269 cosapp-0.15.0/cosapp/base/
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.521185 cosapp-0.15.0/cosapp/core/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5176 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/configuration_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    18754 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/eval_str.py
+-rw-rw-rw-   0 root         (0) root         (0)    15819 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.523935 cosapp-0.15.0/cosapp/core/numerics/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/numerics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27753 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/numerics/basics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28415 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/numerics/boundary.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/numerics/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2948 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/numerics/mathematicalproblem.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    13455 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/numerics/residues.py
+-rw-rw-rw-   0 root         (0) root         (0)    19400 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/numerics/root.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/numerics/sobol_seq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.523935 cosapp-0.15.0/cosapp/core/signal/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/signal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4972 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/signal/signal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/signal/slot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.525769 cosapp-0.15.0/cosapp/core/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8079 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15027 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/tests/test_AssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)    12270 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/tests/test_CoSAppConfiguration.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/tests/test_ContextLocals.py
+-rw-rw-rw-   0 root         (0) root         (0)    12340 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/tests/test_EvalString.py
+-rw-rw-rw-   0 root         (0) root         (0)    13397 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/tests/test_Module.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/tests/test_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/core/variableref.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.528519 cosapp-0.15.0/cosapp/drivers/
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/abstractsetofcases.py
+-rw-rw-rw-   0 root         (0) root         (0)    11978 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/abstractsolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     8692 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     9499 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/influence.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/iterativecase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/lineardoe.py
+-rw-rw-rw-   0 root         (0) root         (0)     3131 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/metasystembuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10683 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/montecarlo.py
+-rw-rw-rw-   0 root         (0) root         (0)    29258 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/nonlinearsolver.py
+-rw-rw-rw-   0 root         (0) root         (0)    21794 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/optimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/optionaldriver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6674 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/runonce.py
+-rw-rw-rw-   0 root         (0) root         (0)    12603 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/runsinglecase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.529435 cosapp-0.15.0/cosapp/drivers/time/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/euler.py
+-rw-rw-rw-   0 root         (0) root         (0)    19963 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/runge_kutta.py
+-rw-rw-rw-   0 root         (0) root         (0)    14133 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.533102 cosapp-0.15.0/cosapp/drivers/time/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15016 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6501 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_BouncingBall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_DiscreteStepper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_EulerExplicit.py
+-rw-rw-rw-   0 root         (0) root         (0)    18994 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_InterpolAssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_Interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5336 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_NewtonPendulum.py
+-rw-rw-rw-   0 root         (0) root         (0)    25908 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_RungeKutta.py
+-rw-rw-rw-   0 root         (0) root         (0)    22357 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_Scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_SystemInterpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeAssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeStepManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     8108 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeUnknownDict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4478 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeUnknownStack.py
+-rw-rw-rw-   0 root         (0) root         (0)     2914 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeVarManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py
+-rw-rw-rw-   0 root         (0) root         (0)     9926 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_event_cascades.py
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/tests/test_modevar_init.py
+-rw-rw-rw-   0 root         (0) root         (0)    21544 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/time/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15033 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/drivers/validitycheck.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.534019 cosapp-0.15.0/cosapp/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/multimode/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5937 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/multimode/discreteStepper.py
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/multimode/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/multimode/zeroCrossing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.535852 cosapp-0.15.0/cosapp/patterns/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/patterns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3411 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/patterns/observer.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/patterns/singleton.py
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/patterns/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.536769 cosapp-0.15.0/cosapp/ports/
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16224 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4022 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/mode_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)    34280 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/port.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/unit_library.ini
+-rw-rw-rw-   0 root         (0) root         (0)    33349 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/units.py
+-rw-rw-rw-   0 root         (0) root         (0)    31417 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/ports/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.537685 cosapp-0.15.0/cosapp/recorders/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/recorders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/recorders/dataframe_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)     7847 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/recorders/dsv_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)    14338 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/recorders/recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.539518 cosapp-0.15.0/cosapp/systems/
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6623 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/externalsystem.py
+-rw-rw-rw-   0 root         (0) root         (0)    13327 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/metamodels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/processsystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     5246 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/structure.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)   132243 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/system.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/system.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/systemConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)    15658 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/systemSurrogate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5515 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/systems/systemfamily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.542268 cosapp-0.15.0/cosapp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/all_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.545018 cosapp-0.15.0/cosapp/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)      356 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/default_dataframe.json
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/export_doe.cs
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/export_doe.csv
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/export_doe.json
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/export_doe.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_ducts.json
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss.json
+-rw-rw-rw-   0 root         (0) root         (0)      312 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss1.json
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss11.json
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss11bis.json
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss12.json
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss121.json
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss131.json
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss2.json
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss22.json
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss222.json
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss2tank.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.546852 cosapp-0.15.0/cosapp/tests/library/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/ports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.547768 cosapp-0.15.0/cosapp/tests/library/systems/
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/systems/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7259 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/systems/basicalgebra.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/systems/dynamics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/systems/elec.py
+-rw-rw-rw-   0 root         (0) root         (0)     8536 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/systems/multiply.py
+-rw-rw-rw-   0 root         (0) root         (0)    11780 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/systems/others.py
+-rw-rw-rw-   0 root         (0) root         (0)     4826 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/systems/pressurelossvarious.py
+-rw-rw-rw-   0 root         (0) root         (0)     1986 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/library/systems/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_ComplexDuct.py
+-rw-rw-rw-   0 root         (0) root         (0)    10101 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_MathematicalProblem_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)    10653 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_Turbofan.py
+-rw-rw-rw-   0 root         (0) root         (0)     3960 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_dynamics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6650 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_electric_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_multimode.py
+-rw-rw-rw-   0 root         (0) root         (0)     8225 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_system_pressureloss.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_tutorials.py
+-rw-rw-rw-   0 root         (0) root         (0)    11905 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_unknown_aliasing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5540 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tests/test_visitor_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.548685 cosapp-0.15.0/cosapp/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.548685 cosapp-0.15.0/cosapp/tools/fmu/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/fmu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22336 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/fmu/exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/fmu/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.549602 cosapp-0.15.0/cosapp/tools/fmu/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/fmu/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/fmu/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    13858 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/fmu/tests/test_exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/fmu/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     4117 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/help.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.550518 cosapp-0.15.0/cosapp/tools/module_parser/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/module_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4279 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/module_parser/package_metadata.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    14905 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/module_parser/parseModule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.550518 cosapp-0.15.0/cosapp/tools/problem_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7945 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/problem_viewer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.551435 cosapp-0.15.0/cosapp/tools/problem_viewer/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   250263 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.551435 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)     9254 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.553268 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     9483 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js
+-rw-rw-rw-   0 root         (0) root         (0)   211120 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/http.js
+-rw-rw-rw-   0 root         (0) root         (0)    86659 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.554185 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/constants.js
+-rw-rw-rw-   0 root         (0) root         (0)    16285 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/draw.js
+-rw-rw-rw-   0 root         (0) root         (0)     5771 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/legend.js
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/modal.js
+-rw-rw-rw-   0 root         (0) root         (0)    70307 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/ptN2.js
+-rw-rw-rw-   0 root         (0) root         (0)     9486 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/search.js
+-rw-rw-rw-   0 root         (0) root         (0)     4155 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/svg.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.555102 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/style/
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/style/awesomplete.css
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/style/fontello.woff
+-rw-rw-rw-   0 root         (0) root         (0)     5815 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/style/partition_tree.css
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/problem_viewer/webview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.555102 cosapp-0.15.0/cosapp/tools/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.556018 cosapp-0.15.0/cosapp/tools/templates/lib/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/lib/Readme.txt
+-rw-rw-rw-   0 root         (0) root         (0)   236746 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/lib/d3.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    23777 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/lib/vis.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   663624 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/lib/vis.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     3800 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/pythonfmu.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.557852 cosapp-0.15.0/cosapp/tools/templates/src/
+-rw-rw-rw-   0 root         (0) root         (0)     4751 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/src/d3_draw.js
+-rw-rw-rw-   0 root         (0) root         (0)      451 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/src/d3_styles.css
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/system_d3.html
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/templates/system_repr.html
+-rw-rw-rw-   0 root         (0) root         (0)     6675 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.559685 cosapp-0.15.0/cosapp/tools/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/baseRenderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/d3js.py
+-rw-rw-rw-   0 root         (0) root         (0)     4753 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/markdown.py
+-rw-rw-rw-   0 root         (0) root         (0)    20440 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/prettyprint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.560602 cosapp-0.15.0/cosapp/tools/views/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/tests/test_VisJsRenderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/tests/test_d3.py
+-rw-rw-rw-   0 root         (0) root         (0)     7927 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/tests/test_markdown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5912 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/tests/test_prettyprint.py
+-rw-rw-rw-   0 root         (0) root         (0)    16980 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tools/views/visjs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.566101 cosapp-0.15.0/cosapp/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)     3288 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/00-Introduction.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    20810 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/01-Systems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15181 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/02-Ports.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18919 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/03-Drivers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/04-Triggers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18216 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/05-Validation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10391 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/06-Visibility.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8547 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/07-Metamodels.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    23655 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/08-Multipoints-Design.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14617 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/09-MonteCarlo.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/10-Recorders.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10256 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/11-DesignMethods.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/CustomConnectors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/FMI.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    28157 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/Guidelines.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15090 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/HybridSimulations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    13505 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/Logging.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4336 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/Optimization.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7358 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/SwapSystems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17402 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/SystemSurrogates.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    21247 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19955 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/Targets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19043 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/TimeDriver.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    16726 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/TimeDriverAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    20413 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/TipsAndTricks.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10059 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/Visitors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10359 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/aa-SimpleCircuit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/exprampode_fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.571601 cosapp-0.15.0/cosapp/tutorials/images/
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/cosapp.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17745 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/design_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23419 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/drivers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/drivers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/drivers_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    40831 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/drivers_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8450 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/drivers_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4537 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/drivers_nonlinear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/experimental.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10190 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/in_progress.svg
+-rw-rw-rw-   0 root         (0) root         (0)    26687 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/ports_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19983 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/ports_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30601 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/ports_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16538 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/simple_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/systems_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18904 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/systems_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18945 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/systems_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24136 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/systems_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)    28090 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/systems_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/tanks.svg
+-rw-rw-rw-   0 root         (0) root         (0)    27536 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/triggers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24504 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/triggers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6961 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/validity.svg
+-rw-rw-rw-   0 root         (0) root         (0)    85431 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/images/visibility.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.571601 cosapp-0.15.0/cosapp/tutorials/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)     7025 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/multimode/BouncingBall.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/multimode/MultimodeOde.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/multimode/NewtonPendulum.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.572518 cosapp-0.15.0/cosapp/tutorials/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)     7559 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/optimization/BetzLimit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8420 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/optimization/Sellar.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/quickstart.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/tutorials/time_solutions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.575268 cosapp-0.15.0/cosapp/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.575268 cosapp-0.15.0/cosapp/utils/distributions/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2693 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/normal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.576185 cosapp-0.15.0/cosapp/utils/distributions/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/tests/test_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/tests/test_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2912 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/tests/test_triangular.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/tests/test_uniform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/triangular.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/distributions/uniform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8441 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/find_variables.py
+-rw-rw-rw-   0 root         (0) root         (0)     3677 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/graph_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4604 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    16769 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/naming.py
+-rw-rw-rw-   0 root         (0) root         (0)    14038 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/options_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5169 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3856 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/pull_variables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/state_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.578018 cosapp-0.15.0/cosapp/utils/surrogate_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9528 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/kriging.py
+-rw-rw-rw-   0 root         (0) root         (0)    39321 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/multifi_cokriging.py
+-rw-rw-rw-   0 root         (0) root         (0)     5292 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/nearest_neighbor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.578018 cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5286 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    18553 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5287 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/response_surface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.579851 cosapp-0.15.0/cosapp/utils/surrogate_models/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/tests/test_kriging.py
+-rw-rw-rw-   0 root         (0) root         (0)     6925 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py
+-rw-rw-rw-   0 root         (0) root         (0)    16170 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/surrogate_models/tests/test_response_surface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/swap_system.py
+-rw-rw-rw-   0 root         (0) root         (0)     8056 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/testing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2023-07-20 16:29:08.000000 cosapp-0.15.0/cosapp/utils/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.519352 cosapp-0.15.0/cosapp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    44772 2023-07-20 16:29:43.000000 cosapp-0.15.0/cosapp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16093 2023-07-20 16:29:43.000000 cosapp-0.15.0/cosapp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:29:43.000000 cosapp-0.15.0/cosapp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:29:43.000000 cosapp-0.15.0/cosapp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      254 2023-07-20 16:29:43.000000 cosapp-0.15.0/cosapp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-20 16:29:43.000000 cosapp-0.15.0/cosapp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.581685 cosapp-0.15.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11509 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.582601 cosapp-0.15.0/docs/cosapp_theme/
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/layout.html
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.582601 cosapp-0.15.0/docs/cosapp_theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)     8997 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/cosapp.css_t
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.584435 cosapp-0.15.0/docs/cosapp_theme/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)    31000 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/font.css
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/highlight.css
+-rw-rw-rw-   0 root         (0) root         (0)    40062 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/kube.css
+-rw-rw-rw-   0 root         (0) root         (0)     8764 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/kube.demo.css
+-rw-rw-rw-   0 root         (0) root         (0)     9250 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/kube.legenda.css
+-rw-rw-rw-   0 root         (0) root         (0)    30268 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/kube.min.css
+-rw-rw-rw-   0 root         (0) root         (0)    26211 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/master.css
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/css/mermaid.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.587185 cosapp-0.15.0/docs/cosapp_theme/static/font/
+-rw-rw-rw-   0 root         (0) root         (0)   297272 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Black.woff
+-rw-rw-rw-   0 root         (0) root         (0)   328952 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Bold.woff
+-rw-rw-rw-   0 root         (0) root         (0)   347092 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-BoldItalic.woff
+-rw-rw-rw-   0 root         (0) root         (0)   343528 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Italic.woff
+-rw-rw-rw-   0 root         (0) root         (0)   323172 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)   326132 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Semibold.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.587185 cosapp-0.15.0/docs/cosapp_theme/static/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    98024 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.588101 cosapp-0.15.0/docs/cosapp_theme/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/img/cosapp.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.589018 cosapp-0.15.0/docs/cosapp_theme/static/js/
+-rw-rw-rw-   0 root         (0) root         (0)    84380 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/js/jquery-2.1.4.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    56646 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/js/kube.js
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/js/kube.legenda.js
+-rw-rw-rw-   0 root         (0) root         (0)    31683 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/js/kube.min.js
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/js/master.js
+-rw-rw-rw-   0 root         (0) root         (0)    12047 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/js/tocbot.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     5219 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/static/sidebar.js_t
+-rw-rw-rw-   0 root         (0) root         (0)      736 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/cosapp_theme/theme.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.590851 cosapp-0.15.0/docs/developer/
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/developer/installation_cases.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8633 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/developer/logger.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/developer/project_structure.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12553 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/developer/scenarii.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.590851 cosapp-0.15.0/docs/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/img/gitlab-cosapp-f4950f.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4393 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/img/website-docs-blue.svg
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/license.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6499 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.515685 cosapp-0.15.0/docs/nb_thumbnails/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.592685 cosapp-0.15.0/docs/nb_thumbnails/_images/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/desktop-download.svg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/eye.svg
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/file-code.svg
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/file-text.svg
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/fold.svg
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/package.svg
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/pencil.svg
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/play.svg
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/plug.svg
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/pulse.svg
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/verified.svg
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/nb_thumbnails/_images/zap.svg
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.593601 cosapp-0.15.0/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)     3759 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/source/modules.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.593601 cosapp-0.15.0/docs/tools/
+-rw-rw-rw-   0 root         (0) root         (0)    13384 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tools/mermaid.py
+-rw-rw-rw-   0 root         (0) root         (0)    10131 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tools/mermaid_inheritance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.599101 cosapp-0.15.0/docs/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)     3288 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/00-Introduction.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    20810 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/01-Systems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15181 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/02-Ports.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18919 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/03-Drivers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/04-Triggers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18216 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/05-Validation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10391 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/06-Visibility.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8547 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/07-Metamodels.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    23655 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/08-Multipoints-Design.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14617 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/09-MonteCarlo.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/10-Recorders.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10256 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/11-DesignMethods.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/CustomConnectors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/FMI.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    28157 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/Guidelines.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15090 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/HybridSimulations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    13505 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/Logging.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4336 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/Optimization.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7358 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/SwapSystems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17402 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/SystemSurrogates.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    21247 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/SystemSurrogatesAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19955 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/Targets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19043 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/TimeDriver.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    16726 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/TimeDriverAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    20413 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/TipsAndTricks.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10059 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/Visitors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10359 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/aa-SimpleCircuit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/exprampode_fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.605518 cosapp-0.15.0/docs/tutorials/images/
+-rw-rw-rw-   0 root         (0) root         (0)    84424 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/Moise_tables_loi.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/cosapp.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17745 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/design_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23419 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/drivers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/drivers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/drivers_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    40831 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/drivers_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8450 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/drivers_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4537 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/drivers_nonlinear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/experimental.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10190 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/in_progress.svg
+-rw-rw-rw-   0 root         (0) root         (0)    26687 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/ports_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19983 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/ports_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30601 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/ports_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16538 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/simple_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/systems_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18904 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/systems_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18945 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/systems_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24136 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/systems_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)    28090 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/systems_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/tanks.svg
+-rw-rw-rw-   0 root         (0) root         (0)    27536 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/triggers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24504 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/triggers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6961 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/validity.svg
+-rw-rw-rw-   0 root         (0) root         (0)    85431 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/images/visibility.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.605518 cosapp-0.15.0/docs/tutorials/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)     7025 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/multimode/BouncingBall.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/multimode/MultimodeOde.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/multimode/NewtonPendulum.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:29:43.606434 cosapp-0.15.0/docs/tutorials/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)     7559 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/optimization/BetzLimit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8420 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/optimization/Sellar.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/quickstart.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-07-20 16:29:08.000000 cosapp-0.15.0/docs/tutorials/time_solutions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2023-07-20 16:29:43.607351 cosapp-0.15.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-20 16:29:08.000000 cosapp-0.15.0/setup.py
```

### Comparing `cosapp-0.14.1/AUTHORS.md` & `cosapp-0.15.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/CONTRIBUTING.md` & `cosapp-0.15.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/HISTORY.md` & `cosapp-0.15.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # History
 
+## 0.15.0 (2023-07-20)
+
+### New features & API changes
+
+- Suppression of default `RunSingleCase` subdriver `runner` in `NonLinearSolver` drivers (MR [#239](https://gitlab.com/cosapp/cosapp/-/merge_requests/239)).
+- Enable target initialization in multi-point design problems (MR [#233](https://gitlab.com/cosapp/cosapp/-/merge_requests/233)).
+- New utility function `swap_system` to replace on the fly a subsystem by another `System` instance (MR [#238](https://gitlab.com/cosapp/cosapp/-/merge_requests/238)).
+
+### Bug fixes and code quality
+
+- Refactor driver `Optimizer` (MR [#240](https://gitlab.com/cosapp/cosapp/-/merge_requests/240)).
+- Various bug fixes (MRs [#234](https://gitlab.com/cosapp/cosapp/-/merge_requests/234), [#235](https://gitlab.com/cosapp/cosapp/-/merge_requests/235), [#241](https://gitlab.com/cosapp/cosapp/-/merge_requests/241)).
+
+### Documentation
+
+- New tutorial on `swap_system` (MR [#243](https://gitlab.com/cosapp/cosapp/-/merge_requests/243)).
+- General update of tutorials (MRs [#232](https://gitlab.com/cosapp/cosapp/-/merge_requests/232) and [#242](https://gitlab.com/cosapp/cosapp/-/merge_requests/242)).
+
+
 ## 0.14.1 (2023-06-08)
 
 ### Bug fixes and code quality
 
 - Fix incorrect output file name in `cosapp.tools.parse_module` (MR [#229](https://gitlab.com/cosapp/cosapp/-/merge_requests/229)).
 - Refactoring pass (MR [#230](https://gitlab.com/cosapp/cosapp/-/merge_requests/230)).
```

### Comparing `cosapp-0.14.1/LICENSE.rst` & `cosapp-0.15.0/LICENSE.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2017-2020 Safran SA - All Rights Reserved
+Copyright (C) 2017-2023 Safran SA - All Rights Reserved
 
 CoSApp Open Source License:
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this software except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `cosapp-0.14.1/MANIFEST.in` & `cosapp-0.15.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/PKG-INFO` & `cosapp-0.15.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosapp
-Version: 0.14.1
+Version: 0.15.0
 Summary: CoSApp, the Collaborative System Approach.
 Home-page: https://cosapp.readthedocs.io
 Author: CoSApp Development Team
 License: Apache-2.0
 Keywords: cosapp,system simulation,system design
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -55,14 +55,33 @@
 # Try it now!
 Run a Jupyter Lab instance with binder to try out CoSApp features through examples.
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cosapp%2Fcosapp/master?urlpath=lab/tree/docs/tutorials)
 
 # History
 
+## 0.15.0 (2023-07-20)
+
+### New features & API changes
+
+- Suppression of default `RunSingleCase` subdriver `runner` in `NonLinearSolver` drivers (MR [#239](https://gitlab.com/cosapp/cosapp/-/merge_requests/239)).
+- Enable target initialization in multi-point design problems (MR [#233](https://gitlab.com/cosapp/cosapp/-/merge_requests/233)).
+- New utility function `swap_system` to replace on the fly a subsystem by another `System` instance (MR [#238](https://gitlab.com/cosapp/cosapp/-/merge_requests/238)).
+
+### Bug fixes and code quality
+
+- Refactor driver `Optimizer` (MR [#240](https://gitlab.com/cosapp/cosapp/-/merge_requests/240)).
+- Various bug fixes (MRs [#234](https://gitlab.com/cosapp/cosapp/-/merge_requests/234), [#235](https://gitlab.com/cosapp/cosapp/-/merge_requests/235), [#241](https://gitlab.com/cosapp/cosapp/-/merge_requests/241)).
+
+### Documentation
+
+- New tutorial on `swap_system` (MR [#243](https://gitlab.com/cosapp/cosapp/-/merge_requests/243)).
+- General update of tutorials (MRs [#232](https://gitlab.com/cosapp/cosapp/-/merge_requests/232) and [#242](https://gitlab.com/cosapp/cosapp/-/merge_requests/242)).
+
+
 ## 0.14.1 (2023-06-08)
 
 ### Bug fixes and code quality
 
 - Fix incorrect output file name in `cosapp.tools.parse_module` (MR [#229](https://gitlab.com/cosapp/cosapp/-/merge_requests/229)).
 - Refactoring pass (MR [#230](https://gitlab.com/cosapp/cosapp/-/merge_requests/230)).
```

### Comparing `cosapp-0.14.1/README.md` & `cosapp-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/config.py` & `cosapp-0.15.0/cosapp/core/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,147 +1,171 @@
 """
 Configuration of CoSApp.
 """
 import os
-import sys
 import json
 
 try:
     from json import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
 import logging
 from pathlib import Path
-from typing import FrozenSet
+from typing import FrozenSet, Union
 
 import jsonschema
 
 logger = logging.getLogger(__name__)
 
 
 class CoSAppConfiguration:
     r"""Encapsulate CoSApp configuration parameters and its handlers.
     
-    CoSApp configuration folder are by default store in 
-    On Linux::
-
-       $HOME/.cosapp.d
-
-    On Windows::
-
-       %USERPROFILE%\.cosapp.d
+    By default, CoSApp configuration folder is stored in 
+    - `$HOME/.cosapp.d` (Linux)
+    - `%USERPROFILE%\.cosapp.d` (MS Windows)
 
     This default configuration folder is overwritten by the environment
     variable ``COSAPP_CONFIG_DIR``.
     """
 
     COSAPP_CONFIG_DIR = ".cosapp.d"
-    CONFIG_FILE = "cosapp_config.json"  # type: str
+    CONFIG_FILE = "cosapp_config.json"
 
     def __init__(self) -> None:
         """Constructor"""
-        self._userid = ""  # type: str
-        self._roles = frozenset()  # type: FrozenSet[FrozenSet[str]]
+        self._userid = ""
+        self._roles: FrozenSet[FrozenSet[str]] = frozenset()
 
         self.__load_configuration()
 
-    def __get_config_path(self) -> str:
-        folder = Path(
-            os.environ.get("COSAPP_CONFIG_DIR", None) or 
-            Path.home().joinpath(CoSAppConfiguration.COSAPP_CONFIG_DIR)
-        )
-        return folder.joinpath(CoSAppConfiguration.CONFIG_FILE)
-
     def __load_configuration(self) -> None:
         """Read configuration from file or generate the default.
 
         Raises
         ------
         OSError
             If the current platform is not recognized
         """
-        fullpath = self.__get_config_path()
-        warning_msg = "The configuration file cannot be opened, fall back to default."
+        fullpath = self.get_config_filename()
+        ok = False
+
         if os.path.isfile(fullpath):  # Load local parameters - offline connection
             try:
                 parameters = self.validate_file(fullpath)
+            except (OSError, JSONDecodeError):
+                ok = False
+            else:
+                ok = True
                 self._userid = parameters["userid"]
-                self._roles = frozenset(
-                    [frozenset(role) for role in parameters["roles"]]
+                self._roles = frozenset(map(frozenset, parameters["roles"]))
+
+        if not ok:
+            logger.warn(
+                f"Configuration file `{fullpath!s}` cannot be opened; fall back to default."
+            )
+            try:
+                self.update_userid()
+            except OSError:
+                self._userid = unknwon_id = "UNKNOWN"
+                self._roles = frozenset()
+                logger.warn(
+                    f"Unable to determine user ID; fall back to {unknwon_id!r}."
                 )
-            except (OSError, JSONDecodeError):
-                logger.warning(warning_msg)
-        else:
-            logger.warning(warning_msg)
-        self.update_configuration()  # Try to update user permission from official root
+            # Try to update user permission from official root
+            self.update_configuration()
+
+    @staticmethod
+    def get_config_dir() -> Path:
+        try:
+            return Path(os.environ["COSAPP_CONFIG_DIR"])
+        except KeyError:
+            return Path.home().joinpath(CoSAppConfiguration.COSAPP_CONFIG_DIR)
+
+    @classmethod
+    def get_config_filename(cls) -> Path:
+        config_dir = cls.get_config_dir()
+        return config_dir.joinpath(cls.CONFIG_FILE)
 
     @property
     def userid(self) -> str:
         """str : User ID"""
         return self._userid
 
     @property
     def roles(self) -> FrozenSet[FrozenSet[str]]:
-        """FrozenSet[FrozenSet[str]] : Roles that the user can impersonate."""
+        """FrozenSet[FrozenSet[str]] : Roles assigned to user."""
         return self._roles
 
     @staticmethod
-    def validate_file(path: str) -> dict:
+    def config_schema() -> dict:
+        """Static method returning the JSON validation schema of the class."""
+        path = os.path.dirname(os.path.abspath(__file__))
+        with open(os.path.join(path , "configuration_schema.json"), "r") as fp:
+            config_schema = json.load(fp)
+        return config_schema
+
+    @classmethod
+    def validate_file(cls, filename: Union[str, Path]) -> dict:
         """Validate the provided file against JSON schema for configuration file.
 
         Parameters
         ----------
-        path : str
+        filename : str or Path
             Absolute path to the file to be tested.
 
         Returns
         -------
         dict
             The dictionary read in the validated file
 
         Raises
         ------
-        jsonschema.exceptions.ValidationError
+        `OSError` (and derived exceptions)
+            If a problem occurs while opening the file.
+        `jsonschema.exceptions.ValidationError`
             If the provided file does not conform to the JSON schema.
         """
-        with open(
-            os.path.join(
-                os.path.dirname(os.path.abspath(__file__)), "configuration_schema.json"
-            )
-        ) as fp:
-            config_schema = json.load(fp)
-        with open(path) as untested_file:
-            params = json.load(untested_file)
+        with open(filename, "r") as fp:
+            params = json.load(fp)
 
-        jsonschema.validate(params, config_schema)
+        jsonschema.validate(params, cls.config_schema())
 
         return params
 
-    def update_configuration(self) -> None:
-        """Update the configuration file for the current user.
-
-        The update process ask the server about updated role.
+    def update_userid(self) -> None:
+        """Update current user id.
         """
-        if len(self._userid) == 0:
-            self._userid = os.environ.get("USERNAME", "") or os.environ.get("USER", "")
+        candidates = iter(["USERNAME", "USER"])
+        old_id = self._userid
 
-            if not self._userid:
-                raise OSError("Unable to find the user id.")
+        while not self._userid:
+            try:
+                self._userid = os.environ.get(next(candidates), "")
+            except StopIteration:
+                raise OSError("Unable to determine user ID.")
+        
+        if self._userid != old_id:
+            logger.info(f"User ID changed from {old_id!r} to {self._userid!r}.")
 
+    def update_configuration(self) -> None:
+        """Update current user configuration file.
+        """
         # TODO - request reference roles source here
 
-        # Save back the changes following the update
-        parameters = {"userid": self.userid, "roles": list()}
-
-        for role in self.roles:
-            parameters["roles"].append(list(role))
+        # Save back changes following the update
+        parameters = {
+            "userid": self.userid,
+            "roles": list(map(list, self.roles)),
+        }
 
         try:
-            config_file = self.__get_config_path()
+            config_file = self.get_config_filename()
             config_dir = os.path.dirname(config_file)
             if not os.path.isdir(config_dir):
                 os.makedirs(config_dir)
 
             with open(config_file, "w") as file:
                 json.dump(parameters, file, sort_keys=True)
+
         except OSError:
-            logger.warning("Fail to save configuration locally.")
+            logger.warning("Failed to save configuration locally.")
```

### Comparing `cosapp-0.14.1/cosapp/core/configuration_schema.json` & `cosapp-0.15.0/cosapp/core/configuration_schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/eval_str.py` & `cosapp-0.15.0/cosapp/core/eval_str.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/module.py` & `cosapp-0.15.0/cosapp/core/module.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/numerics/basics.py` & `cosapp-0.15.0/cosapp/core/numerics/basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,36 +165,60 @@
         if self._context is None:
             self._context = context
         elif context is not self._context:
             raise ValueError(f"Context is already set to {self._context.name!r}.")
 
     @property
     def residues(self) -> Dict[str, Residue]:
-        """Dict[str, Residue] : Residue equations."""
+        """Dict[str, Residue]: Residue dictionary defined in problem."""
         return self._residues
 
     @property
-    def residues_names(self) -> Tuple[str]:
-        """Tuple[str] : Names of residues, flattened to have the same size as `residues_vector`."""
+    def unknowns(self) -> Dict[str, Unknown]:
+        """Dict[str, Unknown]: Unknown dictionary defined in problem."""
+        return self._unknowns
+
+    def residue_vector(self) -> numpy.ndarray:
+        """numpy.ndarray: Residue values stacked into a vector."""
+        return self.__as_vector(self.residues)
+
+    def unknown_vector(self):
+        """numpy.ndarray: Unknown values stacked into a vector."""
+        return self.__as_vector(self.unknowns)
+
+    def __as_vector(self, collection: dict):
+        values = tuple(
+            element.value for element in collection.values()
+        )
+        return numpy.hstack(values) if values else numpy.empty(0)
+
+    def residue_names(self) -> Tuple[str]:
+        """Tuple[str]: Names of residues, flattened to have the same size as `residue_vector()`."""
         names = []
         for name, residue in self.residues.items():
             n_values = numpy.size(residue.value)
             if n_values > 1:
                 names.extend(f"{name}[{i}]" for i in range(n_values))
             else:
                 names.append(name)
         return tuple(names)
 
-    @property
-    def residues_vector(self) -> numpy.ndarray:
-        """numpy.ndarray : Vector of residues."""
-        values = tuple(
-            residue.value for residue in self.residues.values()
-        )
-        return numpy.hstack(values) if values else numpy.empty(0)
+    def unknown_names(self) -> Tuple[str]:
+        """Tuple[str]: Names of unknowns flatten to have the same size as `unknown_vector()`."""
+        names = []
+        for unknown in self.unknowns.values():
+            if unknown.mask is None:
+                names.append(unknown.name)
+            else:
+                basename = unknown.basename
+                ref_size = numpy.size(unknown.ref.value)
+                names.extend(
+                    f"{basename}[{i}]" for i in numpy.arange(ref_size)[unknown.mask.flatten()]
+                )
+        return tuple(names)
 
     @property
     def n_unknowns(self) -> int:
         """int: Number of unknowns."""
         return sum(
             numpy.size(unknown.value) 
             for unknown in self.unknowns.values()
@@ -217,34 +241,14 @@
     def shape(self) -> Tuple[int, int]:
         """(int, int) : Number of unknowns and equations."""
         return (self.n_unknowns, self.n_equations)
 
     def is_empty(self) -> bool:
         return self.shape == (0, 0)
 
-    @property
-    def unknowns(self) -> Dict[str, Unknown]:
-        """Dict[str, Unknown] : Unknown numerical features defined for this system."""
-        return self._unknowns
-
-    @property
-    def unknowns_names(self) -> Tuple[str]:
-        """Tuple[str] : Names of unknowns flatten to have the same size as `residues_vector`."""
-        names = []
-        for unknown in self.unknowns.values():
-            if unknown.mask is None:
-                names.append(unknown.name)
-            else:
-                basename = unknown.basename
-                ref_size = numpy.size(unknown.ref.value)
-                names.extend(
-                    f"{basename}[{i}]" for i in numpy.arange(ref_size)[unknown.mask.flatten()]
-                )
-        return tuple(names)
-
     def add_unknown(self,
         name: Union[str, Iterable[Union[dict, str, Unknown]]],
         max_abs_step: Number = numpy.inf,
         max_rel_step: Number = numpy.inf,
         lower_bound: Number = -numpy.inf,
         upper_bound: Number = numpy.inf,
         mask: Optional[numpy.ndarray] = None,
```

### Comparing `cosapp-0.14.1/cosapp/core/numerics/boundary.py` & `cosapp-0.15.0/cosapp/core/numerics/boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,57 +15,63 @@
 
 
 class Boundary:
     """Numerical solver boundary.
 
     Parameters
     ----------
-    context : cosapp.systems.System
+    context: cosapp.systems.System
         System in which the boundary is defined.
-    name : str
+    name: str
         Name of the boundary
-    mask : numpy.ndarray or None
+    mask: numpy.ndarray or None
         Mask of the values in the vector boundary.
-    default : Number, numpy.ndarray or None
+    default: Number, numpy.ndarray or None
         Default value to set the boundary with.
+    inputs_only: bool, optional
+        If `True` (default), output variables are regarded as invalid.
     """
     def __init__(self,
         context: "cosapp.systems.System",
         name: str,
         mask: Optional[numpy.ndarray] = None,
         default: Union[Number, numpy.ndarray, None] = None,
-        **kwargs
+        inputs_only: bool = True,
+        **kwargs,
     ):
         super().__init__(**kwargs)  # for collaborative inheritance
-        self.__info = info = Boundary.parse(context, name, mask)
+        self.__info = info = Boundary.parse(context, name, mask, inputs_only)
 
         self._context = context  # type: cosapp.systems.System
         self._default_value = None  # type: Union[Number, numpy.ndarray, None]
 
         self.mask = info.mask
         self.set_default_value(default, self.mask)
 
     @staticmethod
     def parse(
         context: "cosapp.systems.System",
         name: str,
-        mask: Optional[numpy.ndarray] = None
+        mask: Optional[numpy.ndarray] = None,
+        inputs_only: bool = False,
     ) -> SimpleNamespace:
         """
         Parse port and variable name from a name and its evaluation context.
         Also checks that the variable belongs to an input port.
 
         Parameters
         ----------
-        - context : cosapp.systems.System
+        - context [cosapp.systems.System]:
             System in which the boundary is defined.
-        - name : str
+        - name [str]:
             Name of the boundary
-        - mask : numpy.ndarray[bool] or None, optional
+        - mask [numpy.ndarray[bool] or None, optional]:
             Mask to apply on the variable; default is None (i.e. no mask)
+        - inputs_only [bool, optional]:
+            If `True`, output variables are regarded as invalid. Default is `False`.
 
         Returns
         -------
         info: SimpleNameSpace
             Structure containing fields `varname`, `fullname`, `port` and `mask`.
         """
         from cosapp.ports.port import BasePort
@@ -76,15 +82,15 @@
         ref = context.name2variable[info.basename]
         container = ref.mapping
 
         if not isinstance(container, BasePort):
             raise TypeError(
                 f"Only variables can be used in mathematical algorithms; got {info.basename!r} in {context.name!r}"
             )
-        if not container.is_input:
+        if inputs_only and not container.is_input:
             raise ValueError(
                 f"Only variables in input ports can be used as boundaries; got {info.basename!r} in {container.contextual_name!r}."
             )
         # Test if type and scope are compatible with boundary status
         try:
             container.validate(ref.key, ref.value)
         except ScopeError:  # Type error should still be raised
@@ -381,15 +387,15 @@
         max_abs_step: Number = numpy.inf,
         max_rel_step: Number = numpy.inf,
         lower_bound: Number = -numpy.inf,
         upper_bound: Number = numpy.inf,
         # reference: Union[Number, numpy.ndarray] = 1.,  # TODO normalize unknown
         mask: Optional[numpy.ndarray] = None,
     ):
-        super().__init__(context, name, mask)
+        super().__init__(context, name, mask, inputs_only=True)
 
         check_arg(max_abs_step, 'max_abs_step', Number, lambda x: x > 0)
         check_arg(max_rel_step, 'max_rel_step', Number, lambda x: x > 0)
         check_arg(lower_bound, 'lower_bound', Number)
         check_arg(upper_bound, 'upper_bound', Number)
 
         # TODO take into account the variable dimension in the constructor ?
@@ -679,22 +685,21 @@
     name : str
         Name of the variable
     source : str
         Variable such that name = d(source)/dt
     initial_value : Any
         Time derivative initial value
     """
-
     def __init__(self,
         context: "cosapp.systems.System",
         name: str,
         source: Any,
         initial_value: Any = None,
     ):
-        super().__init__(context, name)
+        super().__init__(context, name, inputs_only=True)
         self.__shape = None
         self.__previous = None
         eval_string, value, self.__type = self.source_type(source, self.context)
         if self.__type is numpy.ndarray:
             self.__shape = value.shape
         # Set source & initial value
         self.source = source
```

### Comparing `cosapp-0.14.1/cosapp/core/numerics/enum.py` & `cosapp-0.15.0/cosapp/core/numerics/enum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/numerics/mathematicalproblem.schema.json` & `cosapp-0.15.0/cosapp/core/numerics/mathematicalproblem.schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/numerics/residues.py` & `cosapp-0.15.0/cosapp/core/numerics/residues.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/numerics/root.py` & `cosapp-0.15.0/cosapp/core/numerics/root.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/numerics/sobol_seq.py` & `cosapp-0.15.0/cosapp/core/numerics/sobol_seq.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/signal/signal.py` & `cosapp-0.15.0/cosapp/core/signal/signal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/signal/slot.py` & `cosapp-0.15.0/cosapp/core/signal/slot.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/tests/conftest.py` & `cosapp-0.15.0/cosapp/core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/tests/test_AssignString.py` & `cosapp-0.15.0/cosapp/core/tests/test_AssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/tests/test_ContextLocals.py` & `cosapp-0.15.0/cosapp/core/tests/test_ContextLocals.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/tests/test_EvalString.py` & `cosapp-0.15.0/cosapp/core/tests/test_EvalString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/tests/test_Module.py` & `cosapp-0.15.0/cosapp/core/tests/test_Module.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/tests/test_time.py` & `cosapp-0.15.0/cosapp/core/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/time.py` & `cosapp-0.15.0/cosapp/core/time.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/core/variableref.py` & `cosapp-0.15.0/cosapp/core/variableref.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/__init__.py` & `cosapp-0.15.0/cosapp/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/abstractsetofcases.py` & `cosapp-0.15.0/cosapp/drivers/abstractsetofcases.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/abstractsolver.py` & `cosapp-0.15.0/cosapp/drivers/abstractsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,19 +99,14 @@
             except KeyError:
                 pass
             if key in self.options:
                 self.options[key] = value
             else:
                 raise KeyError(f"Unknown solver option {key!r}")
 
-    @property
-    def _default_driver_name(self) -> str:
-        """str : Name for the default driver."""
-        return "runner"
-
     def _get_solver_limits(self) -> Dict[str, numpy.ndarray]:
         """Returns the step limitations for all iteratives.
 
         There are 4 types of limits defined:
         - lower_bound: lower bound of the iteratives
         - upper_bound: upper bound of the iteratives
         - abs_step: maximal absolute step of the iteratives
```

### Comparing `cosapp-0.14.1/cosapp/drivers/driver.py` & `cosapp-0.15.0/cosapp/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/influence.py` & `cosapp-0.15.0/cosapp/drivers/influence.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas
 from typing import List, Set, Union, Optional
 
 from cosapp.drivers.abstractsetofcases import AbstractSetOfCases
 from cosapp.drivers.optionaldriver import OptionalDriver
 from cosapp.recorders.dataframe_recorder import DataFrameRecorder
 from cosapp.utils.helpers import check_arg, is_number
-from cosapp.utils.find_variables import find_variables
+from cosapp.utils.find_variables import find_variable_names
 
 
 # TODO This does not support multipoints cases
 class Influence(AbstractSetOfCases):
     """
     This driver evaluate the influence between inputs and outputs (floats only)
     In input :
@@ -141,22 +141,22 @@
             DataFrameRecorder(
                 includes=self.input_vars + self.response_vars,
                 raw_output=True,
                 numerical_only=True,
             )
         )
 
-        self.found_input_vars = find_variables(
+        self.found_input_vars = find_variable_names(
             self.owner,
             includes=self.input_vars,
             excludes=[],
             advanced_filter=lambda x: is_number(x),
             outputs=False,
         )
-        self.found_response_vars = find_variables(
+        self.found_response_vars = find_variable_names(
             self.owner,
             includes=self.response_vars,
             excludes=[],
             advanced_filter=lambda x: is_number(x),
             inputs=False,
         )
```

### Comparing `cosapp-0.14.1/cosapp/drivers/iterativecase.py` & `cosapp-0.15.0/cosapp/drivers/iterativecase.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/lineardoe.py` & `cosapp-0.15.0/cosapp/drivers/lineardoe.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/metasystembuilder.py` & `cosapp-0.15.0/cosapp/drivers/metasystembuilder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/montecarlo.py` & `cosapp-0.15.0/cosapp/drivers/montecarlo.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/nonlinearsolver.py` & `cosapp-0.15.0/cosapp/drivers/nonlinearsolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,68 @@
 import copy
 import numpy
+import abc
 import csv
 from io import StringIO
 from numbers import Number
 from typing import (
     Any, Callable, Dict, List, Optional,
     Sequence, Tuple, Union, Iterable,
     TypeVar,
 )
 
 from cosapp.core.numerics.basics import MathematicalProblem, SolverResults
 from cosapp.core.numerics.enum import NonLinearMethods
 from cosapp.core.numerics.root import root
 from cosapp.drivers.driver import Driver
 from cosapp.drivers.abstractsolver import AbstractSolver
-from cosapp.drivers.driver import Driver
 from cosapp.drivers.runsinglecase import RunSingleCase
 from cosapp.drivers.utils import DesignProblemHandler
 from cosapp.utils.helpers import check_arg
 from cosapp.utils.logging import LogFormat, LogLevel
 
 import logging
 logger = logging.getLogger(__name__)
 
 AnyDriver = TypeVar("AnyDriver", bound=Driver)
 
 
+class BaseSolverBuilder(abc.ABC):
+    """Base interface for numerical system building strategy used by `NonLinearSolver`.
+    Implementations will differ for single- or multi-point design.
+    """
+    def __init__(self, solver: AbstractSolver):
+        self.solver = solver
+        self.problem = MathematicalProblem(solver.name, solver.owner)
+        self.initial_values = numpy.empty(0)
+        self.is_design_unknown: Dict[str, bool] = dict()
+
+    @abc.abstractmethod
+    def build_system(self) -> None:
+        pass
+
+    @abc.abstractmethod
+    def update_residues(self) -> None:
+        pass
+
+    def update_unknowns(self, x: numpy.ndarray) -> None:
+        counter = 0
+        for name, unknown in self.problem.unknowns.items():
+            if unknown.mask is None:
+                unknown.set_default_value(x[counter])
+                counter += 1
+            else:
+                n = numpy.count_nonzero(unknown.mask)
+                unknown.set_default_value(x[counter : counter + n])
+                counter += n
+            # Update design unknowns
+            if self.is_design_unknown[name]:
+                unknown.set_to_default()
+
+
 class NonLinearSolver(AbstractSolver):
     """Solve mathematical problem with algebraic variables.
 
     Attributes
     ----------
     compute_jacobian : bool
         Should the Jacobian matrix be computed? ; default True
@@ -38,14 +71,15 @@
     jac : ndarray, optional
         Latest Jacobian matrix computed (if available, None otherwise)
     """
 
     __slots__ = (
         '__method', '__option_aliases', '__trace', '__results',
         '__design_unknowns', 'compute_jacobian', 'jac_lup', 'jac',
+        '__builder',
     )
 
     def __init__(self, 
         name: str, 
         owner: Optional["cosapp.systems.System"] = None, 
         method: Union[NonLinearMethods, str] = NonLinearMethods.NR, 
         **kwargs
@@ -70,25 +104,24 @@
         else:
             check_arg(method, 'method', NonLinearMethods)
         self.__method = method
         self.__option_aliases = dict()
         self.__set_method(method, **kwargs)
         self.__trace: List[Dict[str, Any]] = list()
         self.__results: SolverResults = None
+        self.__builder: BaseSolverBuilder = None
 
         self.compute_jacobian = True  # type: bool
             # desc='Should the Jacobian matrix be computed?'
 
         self.jac_lup = (None, None)  # type: Tuple[Optional[numpy.ndarray], Optional[numpy.ndarray]]
             # desc='LU decomposition of latest Jacobian matrix (if available).'
         self.jac = None  # type: Optional[numpy.ndarray]
             # desc='Latest computed Jacobian matrix (if available).'
 
-        self.add_child(RunSingleCase(self._default_driver_name))
-
     def reset_problem(self) -> None:
         """Reset mathematical problem"""
         super().reset_problem()
         self.__design_unknowns = dict()
 
     @property
     def method(self) -> NonLinearMethods:
@@ -122,17 +155,14 @@
         - desc [str, optional]:
             Sub-driver description in the context of its parent driver.
 
         Notes
         -----
         The added child will have its owner set to match the one of the current driver.
         """
-        default_driver = self._default_driver_name
-        if len(self.children) == 1 and default_driver in self.children:
-            self.pop_child(default_driver)
         self.compute_jacobian = True
         return super().add_child(child, execution_index, desc)
 
     def is_standalone(self) -> bool:
         """Is this Driver able to solve a system?
 
         Returns
@@ -187,15 +217,15 @@
                     spacing = " " * len(name)
                     msg = f"Residues [{len(self.problem.residues)}]: \n   # ({name}"
                     msg += f"\n   #  {spacing}".join(f", {v:.5g}" for v in value)
                     msg += ")\n"
                 else:
                     logger.info(f"   # ({name}, {value:.5g})")
 
-            tol = numpy.max(numpy.abs(self.problem.residues_vector))
+            tol = numpy.linalg.norm(self.problem.residue_vector(), numpy.inf)
             try:
                 option = self.__option_aliases['tol']  # should never fail, in principle
                 target = self.options[option]
             except:
                 target = 0
             logger.debug(f" # Current tolerance {tol} for target {target}")
 
@@ -206,94 +236,37 @@
                 "*" * 40,
                 "*", 
                 "* Assemble mathematical problem",
                 "*",
                 "*" * 40,
             ])
         )
-        handler = DesignProblemHandler(self.owner)
-        handler.design.extend(self._raw_problem, equations=False)
-        handler.offdesign.extend(self._raw_problem, unknowns=False)
-        handler.prune()  # resolve aliasing
-        self.__design_unknowns = handler.design.unknowns
-        self.initial_values = numpy.append(self.initial_values, self.get_init())
-        # Set of unknown names to detect design/offdesign conflicts
-        design_unknown_set = set(handler.design.unknowns)
-        # Create assembled problem
-        problem = self.problem = MathematicalProblem(self.name, self.owner)
-        problem.extend(handler.design)
-
-        run_cases: List[RunSingleCase] = []
-        for driver in self.children.values():
-            if isinstance(driver, RunSingleCase):
-                run_cases.append(driver)
-            else:
-                logger.warning(
-                    f"Including Driver {driver.name!r} without iteratives in Driver {self.name!r} is not numerically advised."
-                )
-
-        if len(run_cases) > 1:
-            # If more than one RunSingleCase drivers are present,
-            # use a name wrapper to distinguish dict entries for
-            # residues and off-design unknowns in global problem
-            get_key_wrapper = lambda case: (
-               lambda key: f"{case.name}[{key}]"
+        run_cases = list(
+            filter(
+                lambda driver: isinstance(driver, RunSingleCase),
+                self.children.values(),
             )
+        )
+        if run_cases:
+            builder = MultipointSolverBuilder(self, run_cases)
         else:
-            get_key_wrapper = lambda case: None
-
-        for case in run_cases:
-            local = case.processed_problems
-            design_unknown_set.update(local.design.unknowns)
-            common = design_unknown_set.intersection(local.offdesign.unknowns)
-            if common:
-                kind = "unknown"
-                if len(common) > 1:
-                    names = ", ".join(repr(v) for v in sorted(common))
-                    names = f"({names}) are"
-                    kind += "s"
-                else:
-                    names = f"{common.pop()!r} is"
-                raise ValueError(
-                    f"{names} defined as design and off-design {kind} in {case.name!r}"
-                )
-            self.__design_unknowns.update(local.design.unknowns)
-            # Enforce solver-level off-design problem to child case
-            case.add_offdesign_problem(handler.offdesign)
-            # Assemble case problems (design & off-design)
-            wrapper = get_key_wrapper(case)
-            problem.extend(local.design, copy=False, residue_wrapper=wrapper)
-            problem.extend(local.offdesign, copy=False, unknown_wrapper=wrapper, residue_wrapper=wrapper)
-            self.initial_values = numpy.append(self.initial_values, case.get_init(self.force_init))
-
+            builder = StandaloneSolverBuilder(self)
+        
+        builder.build_system()
+        self.problem = builder.problem
+        self.initial_values = builder.initial_values
+        self.__builder = builder
         self.touch_unknowns()
         logger.debug(
             "\n".join([
                 "Mathematical problem:",
                 f"{'<empty>' if self.problem.is_empty() else self.problem}",
             ])
         )
 
-    def get_init(self) -> numpy.ndarray:
-        """Get the System iteratives initial values for this driver.
-
-        Returns
-        -------
-        numpy.ndarray
-            The list of iteratives initial values.
-            The values should be in the same order as the unknowns in the `get_problem`.
-        """
-        full_init = numpy.empty(0)
-
-        for unknown in self.__design_unknowns.values():
-            data = copy.deepcopy(unknown.value)
-            full_init = numpy.append(full_init, data)
-
-        return full_init
-
     def _fresidues(self, x: Sequence[float]) -> numpy.ndarray:
         """
         Method used by the solver to take free variables values as input and values of residues as
         output (after running the System).
 
         Parameters
         ----------
@@ -307,39 +280,29 @@
         numpy.ndarray
             The list of residues of the `System`
         """
         x = numpy.asarray(x)
         logger.debug(f"Call fresidues with x = {x!r}")
         self.set_iteratives(x)
 
-        # Run all points
-        for child in self.children.values():
-            logger.debug(f"Call {child.name}.run_once()")
-            child.run_once()
+        if self.children:
+            for subdriver in self.children.values():
+                logger.debug(f"Call {subdriver.name}.run_once()")
+                subdriver.run_once()
+        else:
+            self.owner.run_children_drivers()
 
-        residues = self.problem.residues_vector
+        self.__builder.update_residues()
+        residues = self.problem.residue_vector()
         logger.debug(f"Residues: {residues!r}")
         return residues
 
     def set_iteratives(self, x: Sequence[float]) -> None:
         x = numpy.asarray(x)
-        counter = 0
-        for name, unknown in self.problem.unknowns.items():
-            if unknown.mask is None:
-                unknown.set_default_value(x[counter])
-                counter += 1
-            else:
-                n = numpy.count_nonzero(unknown.mask)
-                unknown.set_default_value(x[counter : counter + n])
-                counter += n
-            # Set all design variables at once
-            if name in self.__design_unknowns:
-                # Set the variable to the new x
-                if not numpy.array_equal(unknown.value, unknown.default_value):
-                    unknown.set_to_default()
+        self.__builder.update_unknowns(x)
 
     def compute(self) -> None:
         """Run the resolution method to find free vars values that zero out residues
         """
         # Reset status
         self.status = ''
         self.error_code = '0'
@@ -373,27 +336,25 @@
                 self.status = 'ERROR'
                 self.error_code = '9'
 
                 error_msg = f"The solver failed: {results.message}"
 
                 error_desc = getattr(results, 'jac_errors', {})
                 if error_desc:
-                    if len(error_desc['unknowns']) > 0:
-                        indices = error_desc['unknowns']
-                        unknown_names = [self.problem.unknowns_names[i] for i in indices]
+                    if (indices := error_desc.get('unknowns', [])):
+                        unknown_names = self.problem.unknown_names()
                         error_msg += (
                             f" \nThe {len(indices)} following parameter(s)"
-                            f" have no influence: {unknown_names} \n{indices}"
+                            f" have no influence: {[unknown_names[i] for i in indices]} \n{indices}"
                         )
-                    if len(error_desc['residues']) > 0:
-                        indices = error_desc['residues']
-                        equation_names = [self.problem.residues_names[i] for i in indices]
+                    if (indices := error_desc.get('residues', [])):
+                        residue_names = self.problem.residue_names()
                         error_msg += (
                             f" \nThe {len(indices)} following residue(s)"
-                            f" are not influenced: {equation_names}"
+                            f" are not influenced: {[residue_names[i] for i in indices]}"
                         )
 
                 if self.parent is not None:
                     raise ArithmeticError(error_msg)
                 else:
                     logger.error(error_msg)
 
@@ -401,20 +362,25 @@
                 (key, unknown.default_value)
                 for key, unknown in self.problem.unknowns.items()
             )
             self._print_solution()
 
         else:
             logger.debug('No parameters/residues to solve. Fallback to children execution.')
+            for child in self.children.values():
+                child.run_once()
             self.owner.run_children_drivers()
 
         if self._recorder is not None:
-            for child in self.children.values():
-                child.run_once()
-                self._recorder.record_state(child.name, self.status, self.error_code)
+            if self.children:
+                for child in self.children.values():
+                    child.run_once()
+                    self._recorder.record_state(child.name, self.status, self.error_code)
+            else:
+                self._recorder.record_state(self.name, self.status, self.error_code)
 
     def log_debug_message(self,
         handler: "HandlerWithContextFilters",
         record: logging.LogRecord,
         format: LogFormat = LogFormat.RAW
     ) -> bool:
         """Callback method on the driver to log more detailed information.
@@ -454,16 +420,16 @@
 
         elif activate == False:
             emit_record = False
 
             message = ""
             unknown_trace = None
             residue_trace = None
-            residue_names = self.problem.residues_names
-            unknown_names = self.problem.unknowns_names
+            residue_names = self.problem.residue_names()
+            unknown_names = self.problem.unknown_names()
             for i, record in enumerate(self.__trace):
                 if i == 0:
                     unknown_trace = record["x"]
                     residue_trace = record["residues"]
                 else:
                     unknown_trace = numpy.vstack((unknown_trace, record["x"]))
                     residue_trace = numpy.vstack((residue_trace, record["residues"]))
@@ -605,15 +571,15 @@
 
     def add_unknown(self,
         name: Union[str, Iterable[Union[dict, str]]],
         *args, **kwargs,
     ) -> MathematicalProblem:
         """Add design unknown(s).
 
-        More details in `MathematicalProblem.add_unknown`.
+        More details in `cosapp.core.MathematicalProblem.add_unknown`.
 
         Parameters
         ----------
         - name [str or Iterable of dictionary or str]:
             Name of the variable or collection of variables to be added.
         - *args, **kwargs:
             Additional arguments forwarded to `MathematicalProblem.add_unknown`.
@@ -627,22 +593,139 @@
 
     def add_equation(self,
         equation: Union[str, Iterable[Union[dict, str]]],
         *args, **kwargs,
     ) -> MathematicalProblem:
         """Add off-design equation(s).
 
-        More details in `MathematicalProblem.add_equation`.
+        More details in `cosapp.core.MathematicalProblem.add_equation`.
 
         Parameters
         ----------
         - equation [str or Iterable of str of the kind 'lhs == rhs']:
             Equation or collection of equations to be added.
         - *args, **kwargs:
             Additional arguments forwarded to `MathematicalProblem.add_equation`.
 
         Returns
         -------
         - MathematicalProblem:
             The updated problem.
         """
         return self._raw_problem.add_equation(equation, *args, **kwargs)
+
+    def add_target(self,
+        expression: Union[str, Iterable[str]],
+        *args, **kwargs,
+    ) -> MathematicalProblem:
+        """Add deferred off-design equation(s).
+
+        More details in `cosapp.core.MathematicalProblem.add_target`.
+
+        Parameters
+        ----------
+        - expression: str
+            Targetted expression
+        - *args, **kwargs : Forwarded to `MathematicalProblem.add_target`
+
+        Returns
+        -------
+        MathematicalProblem
+            The modified mathematical problem
+        """
+        return self._raw_problem.add_target(expression, *args, **kwargs)
+
+
+class StandaloneSolverBuilder(BaseSolverBuilder):
+    """System building strategy for solvers with no
+    `RunSingleCase` sub-drivers. In this case, the actual
+    mathematical problem is entirely defined by unknowns and
+    equations declared at solver level.
+    """
+    def build_system(self):
+        solver = self.solver
+        system = self.solver.owner
+        problem = self.problem
+        handler = DesignProblemHandler(system)
+        handler.design.extend(solver.raw_problem)
+        handler.offdesign.extend(system.assembled_problem())
+        handler.prune()
+        problem.clear()
+        problem.extend(handler.merged_problem(), copy=False)
+        self.initial_values = problem.unknown_vector()
+        self.is_design_unknown = dict.fromkeys(problem.unknowns, True)
+
+    def update_residues(self):
+        for residue in self.problem.residues.values():
+            residue.update()
+
+
+class MultipointSolverBuilder(BaseSolverBuilder):
+    """System building strategy for solvers with one or more
+    `RunSingleCase` sub-drivers. In this case, the actual
+    mathematical problem is a combination of unknowns and
+    equations declared at solver level, and of local design
+    and off-design problems declared at case level.
+    """
+    def __init__(self, solver: NonLinearSolver, points: List[RunSingleCase]):
+        super().__init__(solver)
+        self.points = points
+
+    def build_system(self):
+        solver = self.solver
+        system = self.solver.owner
+        problem = self.problem
+        handler = DesignProblemHandler(system)
+        handler.design.extend(solver.raw_problem, equations=False)
+        handler.offdesign.extend(solver.raw_problem, unknowns=False)
+        handler.prune()  # resolve aliasing
+        # Create assembled problem
+        problem.clear()
+        problem.extend(handler.design)
+
+        self.initial_values = handler.design.unknown_vector()
+
+        if len(self.points) > 1:
+            # If more than one `RunSingleCase` drivers are present,
+            # use a name wrapper to distinguish dict entries for
+            # residues and off-design unknowns in global problem
+            get_key_wrapper = lambda case: (
+               lambda key: f"{case.name}[{key}]"
+            )
+        else:
+            get_key_wrapper = lambda case: None
+
+        # Set of unknown names to detect design/off-design conflicts
+        design_unknown_names = set(handler.design.unknowns)
+
+        for point in self.points:
+            local = point.processed_problems
+            # Check that local problem does not introduce design/off-design conflicts
+            design_unknown_names.update(local.design.unknowns)
+            common = design_unknown_names.intersection(local.offdesign.unknowns)
+            if common:
+                kind = "unknown"
+                if len(common) > 1:
+                    names = ", ".join(map(repr, sorted(common)))
+                    names = f"({names}) are"
+                    kind += "s"
+                else:
+                    names = f"{common.pop()!r} is"
+                raise ValueError(
+                    f"{names} defined as design and off-design {kind} in {point.name!r}"
+                )
+            # Enforce solver-level off-design problem to child case
+            point.add_offdesign_problem(handler.offdesign)
+            # Assemble case problems (design & off-design)
+            wrapper = get_key_wrapper(point)
+            problem.extend(local.design, copy=False, residue_wrapper=wrapper)
+            problem.extend(local.offdesign, copy=False, unknown_wrapper=wrapper, residue_wrapper=wrapper)
+            self.initial_values = numpy.append(self.initial_values, point.get_init(solver.force_init))
+
+        self.is_design_unknown = dict.fromkeys(problem.unknowns, False)
+        for name in design_unknown_names:
+            self.is_design_unknown[name] = True
+
+    def update_residues(self):
+        # Nothing to do, since residues are updated
+        # by `RunSingleCase` sub-drivers
+        pass
```

### Comparing `cosapp-0.14.1/cosapp/drivers/optimizer.py` & `cosapp-0.15.0/cosapp/drivers/optimizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     Notes
     -----
     This optimizer is a wrapper around ``scipy.optimize.minimize`` function. For more details please
     refer to:
     https://docs.scipy.org/doc/scipy-1.0.0/reference/generated/scipy.optimize.minimize.html
 
     """
-    __slots__ = ('_constraints', '_raw_constraints', '_initial_state', '_objective')
+    __slots__ = ('_constraints', '_raw_constraints', '_initial_state', '_objective', '__current_x')
 
     def __init__(self,
         name: str,
         owner: Optional["cosapp.systems.System"] = None,
         **kwargs
     ) -> None:
         """Initialize driver
@@ -105,14 +105,15 @@
         super().__init__(name, owner, **kwargs)
 
         # TODO we need to move this in an enhanced MathematicalProblem
         self._raw_constraints: Set[str] = set()  # Human-readable constraints
         self._constraints: List[Dict] = list()   # Non-negativity constraints
         self._initial_state: Dict[str, Any] = dict()
         self._objective: EvalString = None
+        self.__current_x = numpy.empty(0)
 
         self.options.declare(
             name = 'method',
             default = None,
             values = self.available_methods(),
             desc = (
                 "Type of solver."
@@ -284,72 +285,48 @@
     def __check_owner(self, kind: str) -> None:
         if self.owner is None:
             raise AttributeError(f"Owner system is required to define optimization {kind}.")
 
     def setup_run(self):
         """Method called once before starting any simulation."""
         super().setup_run()
+        self.__current_x = numpy.empty(0)
         
         # Resolve unknown aliasing and connected unknowns
         self.problem = dealias_problem(self._raw_problem)
         self.touch_unknowns()
 
-    def _fun_wrapper(self, expression: EvalString) -> Callable[[numpy.ndarray], float]:
+    def _expression_wrapper(self, expression: EvalString) -> Callable[[numpy.ndarray], float]:
         """Wrapper around objective and constraint expression to propagate the x values in the
             `System` owner.
 
         Parameters
         ----------
         expression : EvalString
             The expression to be evaluated.
 
         Returns
         -------
         Callable[[numpy.ndarray], float]
-            Callable function usable by scipy.optimize.minimize
+            Callable objective function usable by scipy.optimize.minimize
         """
+        if self.children:
+            def wrapper(x: numpy.ndarray, *args) -> float:
+                modified = self._update_unknowns(x)
+                if modified:
+                    for driver in self.children.values():
+                        driver.run_once()
+                return expression.eval()
 
-        def wrapper(x: numpy.ndarray, *args) -> float:
-            """Wrapper around objective and constraint function to propagate the x values in the
-            `System` owner.
-
-            Parameters
-            ----------
-            x : 1D-scalar numpy.ndarray
-                Points at which the function needs to be evaluated
-            args : Tuple
-                Any additional fixed parameters needed to completely specify the function
-
-            Returns
-            -------
-            Float
-                Value of the function for x
-            """
-            # Propagate x value in the System owner, if it has changed
-            counter = 0
-            need_update = False
-            for unknown in self.problem.unknowns.values():
-                if unknown.mask is None:
-                    unknown.set_default_value(x[counter])
-                    counter += 1
-                else:
-                    n = numpy.count_nonzero(unknown.mask)
-                    unknown.set_default_value(x[counter:counter + n])
-                    counter += n
-
-                # Set the variable to the new x
-                if not numpy.array_equal(unknown.value, unknown.default_value):
-                    unknown.set_to_default()
-                    need_update = True
-
-            if need_update:
-                for driver in self.children.values():
-                    driver.run_once()
-
-            return expression.eval()
+        else:
+            def wrapper(x: numpy.ndarray, *args) -> float:
+                modified = self._update_unknowns(x)
+                if modified:
+                    self.owner.run_children_drivers()
+                return expression.eval()
 
         return wrapper
 
     def _fresidues(self, x: numpy.ndarray) -> float:
         """
         Method used by the solver to take free variables values as input and values of the objective function (after
         running the System).
@@ -364,39 +341,48 @@
         float
             Objective function value
         """
         x = numpy.asarray(x)
         logger.debug(f"Call fresidues with x = {x!r}")
         self.set_iteratives(x)
 
-        if len(self.children) > 0:
+        if self.children:
             for subdriver in self.children.values():
                 subdriver.run_once()
         else:
             self.owner.run_children_drivers()
 
         objective = self._objective.eval()
         logger.debug(f"Objective: {objective!r}")
         return objective
 
     def set_iteratives(self, x: Sequence[float]) -> None:
-        x = numpy.asarray(x)
-        counter = 0
-        for unknown in self.problem.unknowns.values():
-            if unknown.mask is None:
-                unknown.set_default_value(x[counter])
-                counter += 1
-            else:
-                n = numpy.count_nonzero(unknown.mask)
-                unknown.set_default_value(x[counter : counter + n])
-                counter += n
-            # Set variable to new x
-            if not numpy.array_equal(unknown.value, unknown.default_value):
+        self._update_unknowns(x)
+
+    def _update_unknowns(self, x: Sequence[float]) -> bool:
+        modified = not numpy.array_equal(x, self.__current_x)
+
+        if modified:
+            x = numpy.asarray(x)
+            counter = 0
+            for unknown in self.problem.unknowns.values():
+                if unknown.mask is None:
+                    unknown.set_default_value(x[counter])
+                    counter += 1
+                else:
+                    n = numpy.count_nonzero(unknown.mask)
+                    unknown.set_default_value(x[counter : counter + n])
+                    counter += n
+                # Set variable to new x
                 unknown.set_to_default()
 
+            self.__current_x = numpy.array(x)  # force copy
+
+        return modified
+
     def resolution_method(self,
         fresidues: Callable[[Sequence[float]], float],
         x0: numpy.ndarray,
         args: Tuple[Union[float, str], bool] = (),
         options: Optional[OptionsDictionary] = None,
         bounds = None,
         constraints = None,
@@ -501,15 +487,15 @@
         unique_lower = numpy.unique(limits['lower_bound'])
         unique_upper = numpy.unique(limits['upper_bound'])
         def get_bounds(lower, upper) -> tuple:
             return (
                 None if lower == -numpy.inf else lower,
                 None if upper ==  numpy.inf else upper
             )
-        if unique_lower.size == 1 and unique_upper.size == 1:
+        if unique_lower.size == unique_upper.size == 1:
             bounds = get_bounds(unique_lower[0], unique_upper[0])
             if bounds == (None, None):
                 bounds = None
         else:
             bounds = tuple()
 
         if bounds is not None:
@@ -520,15 +506,15 @@
 
         # Create nonlinear constraints
         # TODO The following is really ugly. Constraints should be merged
         # from children through MathematicalProblem extension.
         def format_constraint(constraint):
             return {
                 'type': constraint['type'],
-                'fun': self._fun_wrapper(constraint['expr'])
+                'fun': self._expression_wrapper(constraint['expr'])
             }
         constraints = tuple(map(format_constraint, self._constraints))
 
         if len(self.initial_values) > 0:
             monitored = self.options['monitor']
             BaseRecorder.paused = not monitored
             if monitored:
```

### Comparing `cosapp-0.14.1/cosapp/drivers/optionaldriver.py` & `cosapp-0.15.0/cosapp/drivers/optionaldriver.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/runonce.py` & `cosapp-0.15.0/cosapp/drivers/runonce.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         if not isinstance(modifications, dict):
             raise TypeError(
                 "Initial values must be specified through a dictionary of the kind {varname: value}."
             )
 
         for variable, value in modifications.items():
-            boundary = Boundary(self.owner, variable, default=value)
+            boundary = Boundary(self.owner, variable, default=value, inputs_only=False)
 
             # Check if boundary.name already exists
             actual = self.initial_values.setdefault(boundary.name, boundary)
 
             if actual is not boundary:
                 # Update already existing boundary with new default value and mask
                 actual.set_default_value(boundary.default_value, boundary.mask)
```

### Comparing `cosapp-0.14.1/cosapp/drivers/runsinglecase.py` & `cosapp-0.15.0/cosapp/drivers/runsinglecase.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any, Iterable, Dict, Optional, Union, List
 
 from cosapp.core.eval_str import AssignString
 from cosapp.core.numerics.basics import MathematicalProblem
 from cosapp.core.numerics.boundary import Boundary
 from cosapp.drivers.iterativecase import IterativeCase
 from cosapp.drivers.utils import DesignProblemHandler
-from cosapp.ports.enum import PortType
 from cosapp.systems import System
 from cosapp.utils.helpers import check_arg
 
 import logging
 logger = logging.getLogger(__name__)
 
 
@@ -81,20 +80,34 @@
 
     def reset_problem(self) -> None:
         """Reset design and off-design problems defined on case."""
         self.__raw_problem = DesignProblemHandler(self.owner)
         self.__processed = DesignProblemHandler(self.owner)
         self.problem = None
 
-    def merge_problems(self) -> None:
-        # Activate targets in processed problems
-        for problem in self.__processed.problems:
-            problem.activate_targets()
+    def __merge_problems(self) -> None:
+        self.__activate_targets()
         self.problem = self.merged_problem(copy=False)
 
+    def __activate_targets(self) -> None:
+        """Activate targets in processed problems"""
+        extract_targets = lambda problem: set(
+            r.target for r in problem.deferred_residues.values()
+        )
+        target_names = set.union(
+            *map(extract_targets, self.__processed.problems)
+        )
+        if target_names:
+            # Set init values corresponding to targetted variables
+            for boundary in self.initial_values.values():
+                if boundary.basename in target_names:
+                    boundary.set_to_default()
+            for problem in self.__processed.problems:
+                problem.activate_targets()
+
     def merged_problem(self, copy=True) -> MathematicalProblem:
         handler = self.__processed
         name = self.name
         try:
             return handler.merged_problem(name=name, offdesign_prefix=None, copy=copy)
         except ValueError as error:
             error.args = (f"{error.args[0]} in {name!r}",)
@@ -110,57 +123,60 @@
 
         # Add owner off-design problem to `processed.offdesign`
         owner_problem = self.owner.assembled_problem()
         processed.offdesign.extend(owner_problem)
 
         # Resolve unknown aliasing in `processed`
         self.__processed = processed.copy(prune=True)
-        self.merge_problems()
+        self.__merge_problems()
 
     def add_offdesign_problem(self, offdesign: MathematicalProblem) -> MathematicalProblem:
         """Add outer off-design problem to inner problem.
 
         Returns:
         ----------
         - `MathematicalProblem`
             The modified mathematical problem
         """
         # Unknowns & residues are duplicated to avoid side effects between points
         # Existing unknowns and equations are silently overwritten.
         if not offdesign.is_empty():
             self.__processed.offdesign.extend(offdesign, copy=True, overwrite=True)
-            self.merge_problems()
+            self.__merge_problems()
         return self.problem
 
     def _precompute(self) -> None:
         """Actions to carry out before the :py:meth:`~cosapp.drivers.runonce.RunOnce.compute` method call.
 
         It sets the boundary conditions and changes variable status.
         """
         super()._precompute()
 
         # Set boundary conditions
-        owner_changed = False
-        for assignment in self.case_values:
-            value, changed = assignment.exec()
-            if changed:
-                owner_changed = True
-
-        if owner_changed:
-            self.owner.touch()
+        self.apply_values()
 
         # Set offdesign variables
         design_unknowns = set(self.design.unknowns)
         problem = self.get_problem()
         for name, unknown in problem.unknowns.items():
             if name in design_unknowns:
                 continue
             if not numpy.array_equal(unknown.value, unknown.default_value):
                 unknown.set_to_default()
 
+    def apply_values(self) -> None:
+        owner_changed = False
+        for assignment in self.case_values:
+            value, changed = assignment.exec()
+            if changed:
+                owner_changed = True
+
+        if owner_changed:
+            self.owner.touch()
+
     def clean_run(self):
         """Method called once after any simulation."""
         self.problem = None
 
     def get_problem(self) -> MathematicalProblem:
         """Returns the full mathematical for the case.
 
@@ -212,17 +228,33 @@
         owner = self.owner
         if owner is None:
             raise AttributeError(
                 f"Driver {self.name!r} must be attached to a System to set case values."
             )
         check_arg(modifications, 'modifications', dict)
 
-        for variable, value in modifications.items():
-            Boundary.parse(owner, variable)  # checks that variable is valid
-            self.__case_values.append(AssignString(variable, value, owner))
+        init = {}
+        for varname, value in modifications.items():
+            info = Boundary.parse(owner, varname)  # checks that variable is valid
+            if info.port.is_input:
+                self.__case_values.append(AssignString(varname, value, owner))
+            else:
+                init[varname] = value
+        if init:
+            varnames = list(init)
+            if len(init) == 1:
+                head = f"Variable {varnames[0]}"
+                tail = f"has been set as initial condition"
+            else:
+                head = f"Variables {varnames}"
+                tail = f"have been set as initial conditions"
+            logger.info(
+                f"{head} declared in `{self.name}` values {tail}."
+            )
+            self.set_init(init)
 
     def add_value(self, variable: str, value: Any) -> None:
         """Add a single variable to list of case values.
 
         The variable can be contextual `child1.port2.var`. The only rule is that it should belong to
         the owner `System` of this driver or any of its descendants.
```

### Comparing `cosapp-0.14.1/cosapp/drivers/time/euler.py` & `cosapp-0.15.0/cosapp/drivers/time/euler.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/interfaces.py` & `cosapp-0.15.0/cosapp/drivers/time/interfaces.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/runge_kutta.py` & `cosapp-0.15.0/cosapp/drivers/time/runge_kutta.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/scenario.py` & `cosapp-0.15.0/cosapp/drivers/time/scenario.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     except the right-hand side is a callable function.
     """
     def __init__(self, lhs: str, rhs: Callable[[float], Any], context: System):
         if not callable(rhs):
             raise TypeError(
                 f"right-hand side must be a callable function; got {rhs!r}"
             )
-        Boundary.parse(context, lhs)  # checks that variable is valid
+        Boundary.parse(context, lhs, inputs_only=True)  # checks that variable is valid
         fname = f"BC{id(rhs)}"
         assignment = f"{context.name}.{lhs} = {fname}(t)"
         self.__locals = {fname: rhs, context.name: context, 't': 0}
         self.__code = compile(assignment, "<string>", "single")  # type: CodeType
         self.__str = f"{lhs} = {type(rhs).__name__}(t)"
         self.__rhs = rhs
 
@@ -218,19 +218,19 @@
         """
         check_arg(modifications, 'modifications', dict,
             lambda d: all(isinstance(key, str) for key in d.keys())
         )
         if self.owner is None:
             raise AttributeError(f"Driver {self.name!r} must be attached to a System to set initial values.")
 
-        for variable, value in modifications.items():
-            variable, context = self._get_alias(variable)
+        for varname, value in modifications.items():
+            varname, context = self._get_alias(varname, inputs_only=False)
             if context is None:
                 continue
-            assignment = AssignString(variable, value, context)
+            assignment = AssignString(varname, value, context)
             if assignment.constant:
                 # If assignment is constant, it is safer to insert it at the top
                 # of the list, since other initial condition assignments might use it.
                 self.__init_values.insert(0, assignment)
             else:
                 self.__init_values.append(assignment)
 
@@ -260,22 +260,22 @@
         """
         check_arg(modifications, 'modifications', dict,
             lambda d: all(isinstance(key, str) for key in d.keys())
         )
         if self.owner is None:
             raise AttributeError(f"Driver {self.name!r} must be attached to a System to set case values.")
 
-        for variable, value in modifications.items():
-            variable, context = self._get_alias(variable)
+        for varname, value in modifications.items():
+            varname, context = self._get_alias(varname, inputs_only=True)
             if context is None:
                 continue
             if callable(value):
-                assignment = InterpolAssignString(variable, value, context)
+                assignment = InterpolAssignString(varname, value, context)
             else:
-                assignment = AssignString(variable, value, context)
+                assignment = AssignString(varname, value, context)
             if assignment.constant:
                 # If assignment is constant, it can be regarded as an initial condition,
                 # rather than a time-dependent boundary condition.
                 # Moreover, it is safer to insert it at the top of the list,
                 # since other initial condition assignments might use it.
                 self.__init_values.insert(0, assignment)
             else:
@@ -303,25 +303,36 @@
         return self.__case_values
 
     @property
     def init_values(self) -> List[AssignString]:
         """List[AssignString]: list of initial conditions"""
         return self.__init_values
 
-    def _get_alias(self, lhs) -> Tuple[str, System]:
-        """Resolve potential aliasing for input `lhs`, targetted
+    def _get_alias(self, lhs: str, inputs_only=True) -> Tuple[str, System]:
+        """Resolve potential aliasing for variable `lhs`, targetted
         in an initial or a boundary condition.
 
+        Arguments:
+        ----------
+        - lhs [str]:
+            Assignment left-hand-side, i.e. targetted variable
+        - inputs_only [bool, optional]:
+            If `True` (default), only input variables are regarded as valid
+
         Returns:
         --------
         (free_lhs, context) [Tuple[str, System]]:
             Free lhs and its evaluation context, usable in `AssignString`.
         """
         context = self.__context
-        info = Boundary.parse(context, lhs)  # checks that variable is valid
+        info = Boundary.parse(context, lhs, inputs_only=inputs_only)  # checks that variable is valid
+
+        if info.port.is_output:
+            return (lhs, context)
+
         varname = natural_varname(info.basename)
         variable = info.ref
         try:
             alias = context.input_mapping[varname]
         except KeyError:
             warnings.warn(
                 f"Skip connected variable {varname!r} in time scenario."
```

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/conftest.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_BouncingBall.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_BouncingBall.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_DiscreteStepper.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_DiscreteStepper.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_EulerExplicit.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_EulerExplicit.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_InterpolAssignString.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_InterpolAssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_Interpolator.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_Interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_NewtonPendulum.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_NewtonPendulum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_RungeKutta.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_RungeKutta.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_Scenario.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_Scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,21 +155,24 @@
         {'tank1.height': 'pipe.L / 2', 'tank2.height': '10 * pipe.D', 'pipe.D': 0.25},
         dict(content=['pipe.D = 0.25', 'tank1.height = pipe.L / 2', 'tank2.height = 10 * pipe.D'], n_const=1)
     ),
     (
         {'tank1.height': 'pipe.L / 2', 'tank2.height': '10 * pipe.D'},
         dict(content=['tank1.height = pipe.L / 2', 'tank2.height = 10 * pipe.D'], n_const=0)
     ),
+    (
+        {'pipe.k': 2},  # Output variables are accepted in `set_init`
+        dict(content=['pipe.k = 2'], n_const=0),
+    ),
     # Erroneous cases:
     ({'foo.bar': 2}, dict(error=AttributeError, match=r"'foo\.bar' is not known in \w*")),
-    ({'pipe.k': 2}, dict(error=ValueError, match="Only variables in input ports can be used as boundaries")),
 ])
 def test_Scenario_set_init(scenario, init, expected):
     error = expected.get('error', None)
-
+ 
     if error is None:
         scenario.set_init(init)
         assert all(isinstance(assignment, AssignString) for assignment in scenario.init_values)
 
         n_const = expected['n_const']
         content = expected['content']
         const = content[:n_const]
```

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_SystemInterpolator.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_SystemInterpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeAssignString.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeAssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeStepManager.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeStepManager.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeUnknownDict.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeUnknownDict.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeUnknownStack.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeUnknownStack.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_TimeVarManager.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_TimeVarManager.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_event_cascades.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_event_cascades.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/tests/test_modevar_init.py` & `cosapp-0.15.0/cosapp/drivers/time/tests/test_modevar_init.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/time/utils.py` & `cosapp-0.15.0/cosapp/drivers/time/utils.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/utils.py` & `cosapp-0.15.0/cosapp/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/drivers/validitycheck.py` & `cosapp-0.15.0/cosapp/drivers/validitycheck.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/multimode/discreteStepper.py` & `cosapp-0.15.0/cosapp/multimode/discreteStepper.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/multimode/event.py` & `cosapp-0.15.0/cosapp/multimode/event.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/multimode/zeroCrossing.py` & `cosapp-0.15.0/cosapp/multimode/zeroCrossing.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/patterns/observer.py` & `cosapp-0.15.0/cosapp/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/patterns/singleton.py` & `cosapp-0.15.0/cosapp/patterns/singleton.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/patterns/visitor.py` & `cosapp-0.15.0/cosapp/patterns/visitor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/ports/connectors.py` & `cosapp-0.15.0/cosapp/ports/connectors.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/ports/enum.py` & `cosapp-0.15.0/cosapp/ports/enum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/ports/mode_variable.py` & `cosapp-0.15.0/cosapp/ports/mode_variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         check_arg(port, "port", ModeVarPort)
         init = EvalString(init, port.owner)
         init_value = init.eval()
         if value is None:
             value = init_value
         elif init_value is not None:
             if not isinstance(init_value, type(value)):
-                raise ValueError(
-                    f"Initial value {init} appears to be inconsistent with arg value={value}."
+                raise TypeError(
+                    f"Initial value {init!r} appears to be inconsistent with arg value={value!r}."
                 )
 
         super().__init__(name, port, value, unit, dtype, desc, scope)
 
         self._init = init  # type: EvalString
 
     def _repr_markdown_(self) -> str:
```

### Comparing `cosapp-0.14.1/cosapp/ports/port.py` & `cosapp-0.15.0/cosapp/ports/port.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/ports/unit_library.ini` & `cosapp-0.15.0/cosapp/ports/unit_library.ini`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/ports/units.py` & `cosapp-0.15.0/cosapp/ports/units.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/ports/variable.py` & `cosapp-0.15.0/cosapp/ports/variable.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/recorders/dataframe_recorder.py` & `cosapp-0.15.0/cosapp/recorders/dataframe_recorder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/recorders/dsv_recorder.py` & `cosapp-0.15.0/cosapp/recorders/dsv_recorder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/recorders/recorder.py` & `cosapp-0.15.0/cosapp/recorders/recorder.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,39 @@
 class SpecialColumns(NamedTuple):
     section: str
     status: str
     code: str
     reference: str
 
 
+
+def is_cosapp_object(obj: Any) -> bool:
+    """Returns `True` if `obj` is either a port,
+    a system or a driver; `False` otherwise."""
+    from cosapp.base import Port, System, Driver
+    return isinstance(obj, (Port, System, Driver))
+
+
+def any_cosapp_objects(collection: Any) -> bool:
+    """Returns `True` if argument is a cosapp object
+    or a collection thereof; `False` otherwise."""
+    if isinstance(collection, str):
+        return False
+    try:
+        return any(map(is_cosapp_object, collection))
+    except TypeError:
+        return is_cosapp_object(collection)
+
+
+def no_cosapp_objects(dict_item: tuple) -> bool:
+    """Filter function for dictionary items, to
+    exclude entries that match `any_cosapp_object`."""
+    return not any_cosapp_objects(dict_item[1])
+
+
 class BaseRecorder(abc.ABC):
     """Abstract base class for recorders.
 
     Matching pattern are case sensitive and support the following special patterns:
 
     ========  ================================
     Pattern   Meaning
@@ -238,42 +263,47 @@
 
     def __contains__(self, field: str) -> bool:
         return field in self.field_names()
 
     def __update_varlist(self) -> None:
         """Update the list of fields to be recorded"""
         includes = []
-        evaluables = []
+        evaluables = {}
         context = self.watched_object
         for expression in set(self.__includes):
             try:
-                EvalString(expression, context)
+                evaluable = EvalString(expression, context)
             except:
                 includes.append(expression)
             else:
                 if expression in context:
                     # Keep expression in search list,
                     # in case it matches an exclusion pattern
                     includes.append(expression)
                 else:
-                    evaluables.append(expression)
+                    evaluables[expression] = evaluable.eval()
         
         if self._numerical_only:
             criterion = is_numerical
         else:
             criterion = lambda x: True
         
         variables = find_variables(
             context,
             includes,
             self.__excludes,
             advanced_filter=criterion,
             include_const=True,
         )
-        variables.extend(evaluables)
+        variables.update(evaluables)
+
+        # Filter out attributes containing non-copyable CoSApp objects
+        variables = dict(
+            filter(no_cosapp_objects, variables.items())
+        )
         self.__variables = variables = sorted(variables)
         self.__expressions = EvalString(", ".join(variables).join("[]"), context)
 
     def _get_units(self, varnames: Optional[List[str]] = None) -> List[str]:
         """Generate the list of units associated with the requested variables.
 
         Parameters
```

### Comparing `cosapp-0.14.1/cosapp/systems/__init__.py` & `cosapp-0.15.0/cosapp/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/systems/externalsystem.py` & `cosapp-0.15.0/cosapp/systems/externalsystem.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/systems/metamodels.py` & `cosapp-0.15.0/cosapp/systems/metamodels.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/systems/processsystem.py` & `cosapp-0.15.0/cosapp/systems/processsystem.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/systems/structure.schema.json` & `cosapp-0.15.0/cosapp/systems/structure.schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/systems/system.py` & `cosapp-0.15.0/cosapp/systems/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,29 +339,26 @@
                 break
             system._is_tree_clean = False
 
     def __enforce_scope(self) -> None:
         """Encapsulate input ports for which some variables are out of scope."""
         if self._user_context is None:
 
-            def get_context(
-                tags: FrozenSet[str], roles: FrozenSet[FrozenSet[str]]
-            ) -> Scope:
-                """Get context depending on the matching between user roles and tags.
+            # Ensure tags is a frozenset
+            self.tags = tags = frozenset(self.tags)
 
-                If tags is empty => `PRIVATE`
-                If one role == all tags => `PRIVATE`
+            def get_scope(role_sets: FrozenSet[FrozenSet[str]]) -> Scope:
+                """Get context depending on the matching between user roles and tags:
 
-                If one group of one role matches one of the tags => `PROTECTED`
-
-                Else `PUBLIC`
+                - No tags or full match with one role => `PRIVATE`
+                - Partial match, at best, between tags and one role => `PROTECTED`
+                - Else `PUBLIC`
 
                 Parameters
                 ----------
-                tags : FrozenSet[str]
                 roles : FrozenSet[FrozenSet[str]]
 
                 Returns
                 -------
                 Scope
 
                 Examples
@@ -378,37 +375,38 @@
                 >>> tags = frozenset(['Aerodynamics', 'Compressor'])
                 >>> roles = frozenset([frozenset(['Mechanics', 'Compressor'])])
                 >>> assert get_context(tags, roles) == Scope.PROTECTED
                 >>>
                 >>> tags = frozenset(['Aerodynamics', 'Compressor'])
                 >>> roles = frozenset([frozenset(['Heat transfert', 'Turbine'])])
                 >>> assert get_context(tags, roles) == Scope.PUBLIC
-
                 """
-                if len(tags) and tags not in roles:
-                    for role in roles:
-                        for group in role:
-                            if group in tags:
-                                return Scope.PROTECTED
-                    return Scope.PUBLIC
-                else:
+                if not tags or tags in role_sets:
                     return Scope.PRIVATE
 
-            # Unsure tags is a frozenset
-            self.tags = frozenset(self.tags)
+                else:
+                    best = Scope.PUBLIC
+                    for roles in role_sets:
+                        if tags.issubset(roles):
+                            return Scope.PRIVATE
+                        if tags.intersection(roles):
+                            best = Scope.PROTECTED
+                    return best
 
             from cosapp.core.config import CoSAppConfiguration
 
-            user_roles = CoSAppConfiguration().roles
+            user_config = CoSAppConfiguration()
+            self._user_context = get_scope(user_config.roles)
+            # print(f"{tags = }", user_config.roles, self._user_context)
 
-            self._user_context = get_context(self.tags, user_roles)
+        scope = self._user_context
 
-        if self._user_context != Scope.PRIVATE:  # Some ports may be restrained
+        if scope != Scope.PRIVATE:  # Some ports may be restrained
             for port in self.inputs.values():
-                port.scope_clearance = self._user_context
+                port.scope_clearance = scope
 
     def _initialize(self, **kwargs) -> Dict[str, Any]:
         """Hook method to add `System` member before calling `setup` method.
 
         Parameters
         ----------
         **kwargs : Dict[str, Any]
```

### Comparing `cosapp-0.14.1/cosapp/systems/system.schema.json` & `cosapp-0.15.0/cosapp/systems/system.schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/systems/systemConnector.py` & `cosapp-0.15.0/cosapp/systems/systemConnector.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/systems/systemSurrogate.py` & `cosapp-0.15.0/cosapp/systems/systemSurrogate.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,35 +175,35 @@
         elif data_out is not None:
             doe_out = OrderedDict(data_out)
         elif self.owner is not None:
             if isinstance(postsynch, str):
                 postsynch = [postsynch]
             if '*' in postsynch:
                 watched = self.__get_owner_connections()
-                varlist = watched.keys()
+                varnames = watched.keys()
             else:
                 owner = self.owner
                 def writeable(var) -> bool:
                     try:
                         owner[var] = owner[var]
                     except AttributeError:
                         return False
                     else:
                         return True
-                varlist = find_variables(
+                matches = find_variables(
                     owner,
                     includes=postsynch,
                     excludes=None,
                     inputs=False,
                 )
-                varlist = set(filter(writeable, varlist))
+                varnames = set(filter(writeable, matches.keys()))
                 # Make sure varlist contains at least owner system outputs
                 for portname, port in owner.outputs.items():
-                    varlist.update(natural_varname(f"{portname}.{var}") for var in port)
-            doe_out = OrderedDict((var, []) for var in varlist)
+                    varnames.update(natural_varname(f"{portname}.{var}") for var in port)
+            doe_out = OrderedDict((name, []) for name in varnames)
         return doe_out
 
     def __get_doe_out_sizes(self) -> None:
         state = self.__state
         owner = self.__owner
         doe_out_sizes = OrderedDict.fromkeys(state.doe_out.keys(), None)
         pos = 0
```

### Comparing `cosapp-0.14.1/cosapp/systems/systemfamily.py` & `cosapp-0.15.0/cosapp/systems/systemfamily.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/all_tests.py` & `cosapp-0.15.0/cosapp/tests/all_tests.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/export_doe.json` & `cosapp-0.15.0/cosapp/tests/data/export_doe.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config.json` & `cosapp-0.15.0/cosapp/tests/data/system_config.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config_ducts.json` & `cosapp-0.15.0/cosapp/tests/data/system_config_ducts.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss11bis.json` & `cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss11bis.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss12.json` & `cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss12.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss121.json` & `cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss121.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss131.json` & `cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss131.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss22.json` & `cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss22.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss222.json` & `cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss222.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/data/system_config_pressureloss2tank.json` & `cosapp-0.15.0/cosapp/tests/data/system_config_pressureloss2tank.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/ports.py` & `cosapp-0.15.0/cosapp/tests/library/ports.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/systems/__init__.py` & `cosapp-0.15.0/cosapp/tests/library/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/systems/basicalgebra.py` & `cosapp-0.15.0/cosapp/tests/library/systems/basicalgebra.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/systems/dynamics.py` & `cosapp-0.15.0/cosapp/tests/library/systems/dynamics.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/systems/elec.py` & `cosapp-0.15.0/cosapp/tests/library/systems/elec.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/systems/multiply.py` & `cosapp-0.15.0/cosapp/tests/library/systems/multiply.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/systems/others.py` & `cosapp-0.15.0/cosapp/tests/library/systems/others.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/systems/pressurelossvarious.py` & `cosapp-0.15.0/cosapp/tests/library/systems/pressurelossvarious.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/library/systems/vectors.py` & `cosapp-0.15.0/cosapp/tests/library/systems/vectors.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/test_ComplexDuct.py` & `cosapp-0.15.0/cosapp/tests/test_ComplexDuct.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/test_MathematicalProblem_integration.py` & `cosapp-0.15.0/cosapp/tests/test_MathematicalProblem_integration.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -218,16 +218,16 @@
     }
     pattern = "\n".join([
         r"Unknowns",
         r"  b\.width = .*",
         r"  a\.p\.y = .*",
         r"  a\.p\.x = .*",
         r"Equations",
-        r"  foo\.beq: v\[::2\] == \[0, 1\] := \[.* .*\]",
         r"  b\.area == 10 := .*",
+        r"  foo\.beq: v\[::2\] == \[0, 1\] := \[.* .*\]",
     ])
     # print(pattern, problem, sep="\n")
     assert re.match(pattern, repr(problem))
 
 
 def test_MathematicalProblem_repr_3(s1: System, caplog):
     """Check unknowns and equations in a multi-point solver.
```

### Comparing `cosapp-0.14.1/cosapp/tests/test_Turbofan.py` & `cosapp-0.15.0/cosapp/tests/test_Turbofan.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/test_dynamics.py` & `cosapp-0.15.0/cosapp/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/test_electric_circuit.py` & `cosapp-0.15.0/cosapp/tests/test_electric_circuit.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/test_multimode.py` & `cosapp-0.15.0/cosapp/tests/test_multimode.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/test_system_pressureloss.py` & `cosapp-0.15.0/cosapp/tests/test_system_pressureloss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from cosapp.systems import System
-from cosapp.drivers import NonLinearSolver
+from cosapp.drivers import NonLinearSolver, RunSingleCase
 
 
 @pytest.fixture
 def PressureLossFactory(test_library, test_data):
     def factory(suffix=""):
         return System.load(test_data / f"system_config_pressureloss{suffix}.json")
     return factory
@@ -218,16 +218,17 @@
 
 def test_system121_redundant_2(system121):
     """Same as `test_system121` with redundant declaration of unknowns.
 
     Case 2: system unknown `sp.x` is redeclared as unknown at runner level.
     """
     s = system121
-    d = s.add_driver(NonLinearSolver("solver"))
-    d.runner.add_unknown("sp.x")
+    solver = s.add_driver(NonLinearSolver("solver"))
+    solver.add_child(RunSingleCase("case"))
+    solver.case.add_unknown("sp.x")
 
     with pytest.raises(ValueError, match="'sp\.x' already exists in 'offdesign'"):
         s.run_drivers()
 
 
 def test_system131(system131):
     # ! Do not suppress this unit test, it's the only one doing new computation with resetting the system
@@ -275,15 +276,16 @@
     assert s.p2.flnum_out.W == pytest.approx(10, rel=1e-5)
     assert s.p4.flnum_out.W == pytest.approx(9, rel=1e-5)
     assert s.s1.x == pytest.approx(9 / 10, rel=1e-5)
     assert s.p2.s21.x == pytest.approx(10 / 11, rel=1e-5)
 
 
 def test_system222_redundant(system222):
-    """Same as `test_system222` with redundant unknowns.
+    """Same as `test_system222` with redundant off-design unknowns.
     """
     s = system222
-    d = s.add_driver(NonLinearSolver("solver"))
-    d.runner.add_unknown(["p2.s21.x", "s1.x"])
+    solver = s.add_driver(NonLinearSolver("solver"))
+    solver.add_child(RunSingleCase("case"))
+    solver.case.add_unknown(["p2.s21.x", "s1.x"])
 
     with pytest.raises(ValueError, match="'p2\.s21\.x' already exists in 'offdesign'"):
         s.run_drivers()
```

### Comparing `cosapp-0.14.1/cosapp/tests/test_tutorials.py` & `cosapp-0.15.0/cosapp/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tests/test_unknown_aliasing.py` & `cosapp-0.15.0/cosapp/tests/test_unknown_aliasing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test problems with unknown aliased by pulling"""
 import pytest
 import logging, re
 from numpy import sqrt, cbrt
 
 from cosapp.systems import System
-from cosapp.drivers import NonLinearSolver
+from cosapp.drivers import NonLinearSolver, RunSingleCase
 
 
 class Quadratic(System):
     """System computing y = 1 + k * x**2"""
     def setup(self):
         self.add_inward('k', 0.8)
         self.add_inward('x', 1.0)
@@ -33,14 +33,15 @@
 
     Case 1: Use pulled input variable `foo.k` as unknown.
 
     Successful; log simply informs that unknown was substituted.
     """
     top = NestedQuad('top')
     solver = top.add_driver(NonLinearSolver('solver', tol=1e-9))
+    solver.add_child(RunSingleCase('runner'))
     solver.runner.add_equation('foo.y == 7').add_unknown('foo.k')
     solver.runner.set_values({
         'foo.x': 2,
         'bar.x': 0.1,
     })
     caplog.clear()
     with caplog.at_level(logging.INFO):
@@ -71,14 +72,15 @@
     top = NestedQuad('top')
     top.c = 0.1
     top.run_once()
     assert top.c == 0.1
     assert top.foo.k == top.c
 
     solver = top.foo.add_driver(NonLinearSolver('solver', tol=1e-9))
+    solver.add_child(RunSingleCase('runner'))
     solver.runner.add_unknown('k').add_equation('y == 7')
     solver.runner.set_values({'x': 2})
 
     caplog.clear()
     with caplog.at_level(logging.WARNING):
         top.run_drivers()
     
@@ -100,17 +102,16 @@
     """
     top = System('top')
     sub1 = top.add_child(Quadratic('sub1'))
     sub2 = top.add_child(NestedQuad('sub2'))
     top.connect(sub1.outwards, sub2.inwards, {'y': 'c'})  # sub2.c is no longer free
 
     solver = top.add_driver(NonLinearSolver('solver'))
-    design = solver.runner
     # Use input `bar.k` connected to an output as unknown:
-    design.add_equation('sub2.foo.y == 7').add_unknown('sub2.bar.k')
+    solver.add_equation('sub2.foo.y == 7').add_unknown('sub2.bar.k')
 
     caplog.clear()
     with pytest.raises(ArithmeticError, match="numbers of params \[0\] and residues \[1\]"):
         with caplog.at_level(logging.WARNING):
             top.run_drivers()
     
     assert len(caplog.records) > 0
@@ -146,17 +147,16 @@
     )
 
 
 def test_design_connected_unknown_1(caplog):
     """Tests that unknowns connected to an output variable are discarded"""
     top = NestedQuad('top')
     solver = top.add_driver(NonLinearSolver('solver'))
-    design = solver.runner
     # Use input `bar.k` connected to an output as unknown:
-    design.add_equation('bar.y == 7').add_unknown('bar.k')
+    solver.add_equation('bar.y == 7').add_unknown('bar.k')
 
     caplog.clear()
     with pytest.raises(ArithmeticError, match="numbers of params \[0\] and residues \[1\]"):
         with caplog.at_level(logging.WARNING):
             top.run_drivers()
     
     assert len(caplog.records) > 0
@@ -171,15 +171,15 @@
     except driver is attached to subsystem `bar`.
     
     Fails because unknown is connected.
     """
     top = NestedQuad('top')
     # Attach driver to sub-system `bar`
     solver = top.bar.add_driver(NonLinearSolver('solver', tol=1e-9))
-    solver.runner.add_unknown('k').add_equation('y == 7')
+    solver.add_unknown('k').add_equation('y == 7')
 
     caplog.clear()
     with pytest.raises(ArithmeticError, match="numbers of params \[0\] and residues \[1\]"):
         with caplog.at_level(logging.WARNING):
             top.run_drivers()
     
     assert len(caplog.records) > 0
@@ -201,15 +201,15 @@
             super().setup()
             # Use parent (free) variable 'c' as off-design unknown
             self.add_unknown('c').add_equation('c == 0')
     
     top = TopSystem('top')
     solver = top.add_driver(NonLinearSolver('solver', tol=1e-9))
     # Use pulled variable `foo.k` as design unknown:
-    solver.runner.design.add_equation('foo.y == 7').add_unknown('foo.k')
+    solver.add_equation('foo.y == 7').add_unknown('foo.k')
 
     caplog.clear()
     with pytest.raises(ValueError, match="'c' is defined as design and off-design unknown"):
         with caplog.at_level(logging.INFO):
             top.run_drivers()
     
     assert len(caplog.records) > 0
@@ -234,15 +234,15 @@
             super().setup()
             # Use pulled variable `foo.k` as off-design unknown
             self.add_unknown('foo.k').add_equation('c == 0')
     
     top = TopSystem('top')
     solver = top.add_driver(NonLinearSolver('solver', tol=1e-9))
     # Use parent variable 'c' as design unknown
-    solver.runner.design.add_equation('foo.y == 7').add_unknown('c')
+    solver.add_equation('foo.y == 7').add_unknown('c')
 
     caplog.clear()
     with pytest.raises(ValueError, match="'c' is defined as design and off-design unknown"):
         with caplog.at_level(logging.INFO):
             top.run_drivers()
     
     assert len(caplog.records) > 0
```

### Comparing `cosapp-0.14.1/cosapp/tests/test_visitor_integration.py` & `cosapp-0.15.0/cosapp/tests/test_visitor_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,11 +197,10 @@
 
     for system in top.tree():
         for driver in system.drivers.values():
             send(visitor, driver.tree())
 
     assert visitor.data['drivers'] == {
         'NonLinearSolver': 1,
-        'RunSingleCase': 1,
         'ValidityCheck': 2,
         'RunOnce': 1,
     }
```

### Comparing `cosapp-0.14.1/cosapp/tools/__init__.py` & `cosapp-0.15.0/cosapp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/fmu/exporter.py` & `cosapp-0.15.0/cosapp/tools/fmu/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -431,31 +431,39 @@
             FmuBuilder._add_variables(outputs, Fmi2Causality.output)
         )
         params["variables"].extend(
             FmuBuilder._add_variables(locals, Fmi2Causality.local)
         )
 
         if nonlinear_solver is not None:
-            children_driver = list(nonlinear_solver.children.values())
-            if len(children_driver) > 1:
-                raise ValueError("The nonlinear solver can only have one child.")
-            runSingleCase = children_driver[0]
-            if not isinstance(runSingleCase, RunSingleCase):
-                raise TypeError(
-                    "The nonlinear solver child must be of type RunSingleCase."
-                )
-            # Note:
-            #   Since `RunSingleCase` child is unique, a simple merging
-            #   of the various mathematical problems by extension works.
-            #   It would not be the case in a multi-point design problem,
-            #   for example, where off-design, design and local problems
-            #   must be assembled with care.
-            problem = nonlinear_solver.raw_problem.copy()
-            problem.extend(runSingleCase.offdesign)
-            problem.extend(runSingleCase.design)
+            subdrivers = list(nonlinear_solver.children.values())
+            error_msg = "The nonlinear solver may have at most one sub-driver, of type `RunSingleCase`"
+            if len(subdrivers) > 1:
+                names = list(map(lambda driver: driver.name, subdrivers))
+                raise ValueError(f"{error_msg}; found sub-drivers {names}")
+            # Assemble solver problem
+            try:
+                problem = nonlinear_solver.raw_problem.copy()
+            except:
+                problem = system.new_problem('design')
+            try:
+                driver = subdrivers[0]
+            except IndexError:
+                pass
+            else:
+                if not isinstance(driver, RunSingleCase):
+                    raise TypeError(f"{error_msg}; got {driver!r}")
+                # Note:
+                #   Since `RunSingleCase` child is unique, a simple merging
+                #   of the various mathematical problems by extension works.
+                #   It would not be the case in a multi-point design problem,
+                #   for example, where off-design, design and local problems
+                #   must be assembled with care.
+                problem.extend(driver.offdesign)
+                problem.extend(driver.design)
             params["problem"] = problem.to_dict()
 
         env = Environment(
             loader=PackageLoader("cosapp.tools", "templates"),
             trim_blocks=True,
             lstrip_blocks=True,
         )
```

### Comparing `cosapp-0.14.1/cosapp/tools/fmu/logging.py` & `cosapp-0.15.0/cosapp/tools/fmu/logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/fmu/tests/conftest.py` & `cosapp-0.15.0/cosapp/tools/fmu/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/fmu/tests/test_exporter.py` & `cosapp-0.15.0/cosapp/tools/fmu/tests/test_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,30 +314,29 @@
 
 def test_FMU_integration_nonlinear_design(tmp_path, iterativenonlinear):
     """Same as `test_FMU_integration_nonlinear_local` with additional
     problem defined at solver level (off-design problem).
     """
     pyfmi = pytest.importorskip("pyfmi")
 
-    solver = NonLinearSolver("solver", iterativenonlinear)
-    solver.add_unknown("nonlinear.k1").add_equation("splitter.p2_out.x == 10")
-
     # Init
     t_driver = iterativenonlinear.add_driver(
         RungeKutta(order=4, dt=0.1, time_interval=[0, 0.2])
     )
-    t_driver.add_child(solver)
+    solver = t_driver.add_child(NonLinearSolver("solver"))
+    solver.add_unknown("nonlinear.k1").add_equation("splitter.p2_out.x == 10")
 
     # Set BC
     t_driver.set_scenario(
         init = {"p_in.x": 1.0},
         values = {"p_in.x": "5 - 4 * exp(-t / 0.1)"},
     )
     recorder = t_driver.add_recorder(
-        DataFrameRecorder(includes=["p_in.x", "p_out.x", "nonlinear.k1"]), period=0.1
+        DataFrameRecorder(includes=["p_in.x", "p_out.x", "nonlinear.k1"]),
+        period=0.1
     )
     iterativenonlinear.run_drivers()
 
     # Reference
     data = recorder.export_data()
     assert_almost_equal(data["p_out.x"], numpy.full(len(data), 10.0))
 
@@ -364,24 +363,21 @@
     for column in filter(lambda c: c != "time", results.columns):
         assert results[column].values == pytest.approx(data[column].values)
 
 
 def test_FMU_integration_nonlinear_local(tmp_path, iterativenonlinear):
     pyfmi = pytest.importorskip("pyfmi")
 
-    solver = NonLinearSolver("solver", iterativenonlinear)
-    solver.runner.add_unknown("nonlinear.k1").add_equation(
-        "splitter.p2_out.x == 10"
-    )
-
     # Init
     t_driver = iterativenonlinear.add_driver(
         RungeKutta(order=4, dt=0.1, time_interval=[0, 0.2])
     )
-    t_driver.add_child(solver)
+    solver = t_driver.add_child(NonLinearSolver("solver"))
+    solver.add_child(RunSingleCase("runner"))
+    solver.runner.add_unknown("nonlinear.k1").add_equation("splitter.p2_out.x == 10")
 
     # Set BC
     t_driver.set_scenario(
         init = {"p_in.x": 1.0},
         values = {"p_in.x": "5 - 4 * exp(-t / 0.1)"},
     )
     recorder = t_driver.add_recorder(
@@ -418,19 +414,19 @@
         assert results[column].values == pytest.approx(data[column].values)
 
 
 def test_FMU_integration_vector_problem(tmp_path, vector_problem):
     pyfmi = pytest.importorskip("pyfmi")
 
     # Setup the system
-    solver = NonLinearSolver("solver", vector_problem)
+    solver = vector_problem.add_driver(NonLinearSolver("solver"))
+    
 
-    # Init
+    # Init & solve
     vector_problem.x = 1.0
-    vector_problem.add_driver(solver)
     vector_problem.run_drivers()
 
     # Convert to FMU
     fmu_file = to_fmu(
         vector_problem,
         dest=tmp_path,
         nonlinear_solver=solver,
```

### Comparing `cosapp-0.14.1/cosapp/tools/fmu/tests/test_logging.py` & `cosapp-0.15.0/cosapp/tools/fmu/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/help.py` & `cosapp-0.15.0/cosapp/tools/help.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/module_parser/package_metadata.schema.json` & `cosapp-0.15.0/cosapp/tools/module_parser/package_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/module_parser/parseModule.py` & `cosapp-0.15.0/cosapp/tools/module_parser/parseModule.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/problem_viewer.py` & `cosapp-0.15.0/cosapp/tools/problem_viewer/problem_viewer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py` & `cosapp-0.15.0/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/index.html` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/index.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/http.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/http.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/constants.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/constants.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/draw.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/draw.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/legend.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/legend.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/modal.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/modal.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/ptN2.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/ptN2.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/search.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/search.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/src/svg.js` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/src/svg.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/style/awesomplete.css` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/style/awesomplete.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/style/fontello.woff` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/style/fontello.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/problem_viewer/visualization/style/partition_tree.css` & `cosapp-0.15.0/cosapp/tools/problem_viewer/visualization/style/partition_tree.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/templates/lib/d3.min.js` & `cosapp-0.15.0/cosapp/tools/templates/lib/d3.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/templates/lib/vis.min.css` & `cosapp-0.15.0/cosapp/tools/templates/lib/vis.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/templates/lib/vis.min.js` & `cosapp-0.15.0/cosapp/tools/templates/lib/vis.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/templates/pythonfmu.j2` & `cosapp-0.15.0/cosapp/tools/templates/pythonfmu.j2`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         # Change the log level in the next line to increase verbosity
         FMUForwardHandler.add_handler(self, level=logging.WARNING)
 
         self.__master = System.load(pathlib.Path(__file__).parent / "{{ system_file }}")
-        self.__driver = {{ driver }}({% for key, value in time_options.items() %}{{key}}={{value}},{% endfor %})
-        self.__driver.owner = self.__master
+        self.__driver = self.__master.add_driver(
+            {{ driver }}({% for key, value in time_options.items() %}{{key}}={{value}},{% endfor %})
+        )
         self.__start_time = 0.
         
         {% for var in variables %}
         self.register_variable(
             {{ var.fmutype }}(
                 "{{ var.name }}", 
                 causality=Fmi2Causality.{{ var.causality }},
@@ -53,18 +54,18 @@
         self.__master.open_loops()
 
         # Add the drivers
         has_iterative = {% if local %}True{% else %}not self.__master.assembled_problem().is_empty(){% endif %}
 
         self.__driver.children.clear()
         if has_iterative:
-            self.__driver.add_child(NonLinearSolver('solver'))  {# TODO, {% for key, value in nl_options.items() %}{{key}}={{option}},{% endfor %})) #}
+            solver = self.__driver.add_child(NonLinearSolver('solver'))  {# TODO, {% for key, value in nl_options.items() %}{{key}}={{option}},{% endfor %})) #}
 
-{% if problem %}            runner = self.__driver.solver.runner
-            runner.offdesign \
+{% if problem %}
+            solver \
 {% for name, unknown in problem.unknowns.items() %}                .add_unknown("{{ unknown.name }}", {{ unknown.max_abs_step }}, {{ unknown.max_rel_step }}, {{ unknown.lower_bound }}, {{ unknown.upper_bound }}{% if unknown.mask is not none %}, {{ unknown.mask }}{% endif %}) \
             {% endfor %}
 {% for name, equation in problem.equations.items() %}                .add_equation("{{ equation.equation }}", "{{ name }}", {{ equation.reference }}) \
             {% endfor %}
             
             {% endif %}
```

### Comparing `cosapp-0.14.1/cosapp/tools/templates/src/d3_draw.js` & `cosapp-0.15.0/cosapp/tools/templates/src/d3_draw.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/templates/system_repr.html` & `cosapp-0.15.0/cosapp/tools/templates/system_repr.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/trigger.py` & `cosapp-0.15.0/cosapp/tools/trigger.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/baseRenderer.py` & `cosapp-0.15.0/cosapp/tools/views/baseRenderer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/d3js.py` & `cosapp-0.15.0/cosapp/tools/views/d3js.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/markdown.py` & `cosapp-0.15.0/cosapp/tools/views/markdown.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/prettyprint.py` & `cosapp-0.15.0/cosapp/tools/views/prettyprint.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/tests/test_VisJsRenderer.py` & `cosapp-0.15.0/cosapp/tools/views/tests/test_VisJsRenderer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/tests/test_d3.py` & `cosapp-0.15.0/cosapp/tools/views/tests/test_d3.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/tests/test_markdown.py` & `cosapp-0.15.0/cosapp/tools/views/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/tests/test_prettyprint.py` & `cosapp-0.15.0/cosapp/tools/views/tests/test_prettyprint.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tools/views/visjs.py` & `cosapp-0.15.0/cosapp/tools/views/visjs.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/00-Introduction.ipynb` & `cosapp-0.15.0/cosapp/tutorials/00-Introduction.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994318181818183%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(8, '* [File Event Triggers](04-Triggers.ipynb)\\n'), (9, '* "*

 * *            "[Replacing a sub-system on the fly](SwapSystems.ipynb)')], delete: [8]}}}"}*

```diff
@@ -78,15 +78,16 @@
                 "\n",
                 "CoSApp comes with a couple of utility tools. The following notebooks demonstrate their usage:\n",
                 "\n",
                 "* [Recording data](10-Recorders.ipynb)\n",
                 "* [Simulation log](Logging.ipynb)\n",
                 "* [System surrogates](SystemSurrogates.ipynb)\n",
                 "* [Export to FMU](FMI.ipynb)\n",
-                "* [File Event Triggers](04-Triggers.ipynb)"
+                "* [File Event Triggers](04-Triggers.ipynb)\n",
+                "* [Replacing a sub-system on the fly](SwapSystems.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Tips & Tricks\n",
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/01-Systems.ipynb` & `cosapp-0.15.0/cosapp/tutorials/01-Systems.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/02-Ports.ipynb` & `cosapp-0.15.0/cosapp/tutorials/02-Ports.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/03-Drivers.ipynb` & `cosapp-0.15.0/cosapp/tutorials/03-Drivers.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9828087843775848%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 4: "*

 * *            "{'attachments': OrderedDict()}, 5: {'attachments': OrderedDict()}, 7: {'attachments': "*

 * *            "OrderedDict()}, 8: {'attachments': OrderedDict()}, 11: {'attachments': "*

 * *            "OrderedDict()}, 14: {'attachments': OrderedDict()}, 16: {'attachments': "*

 * *            "OrderedDict()}, 17: {'source': {insert: [(2, '`RunSingleCase` sets its owner system "*

 * *            'in a given state, and executes all su […]*

```diff
@@ -1,19 +1,21 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials:"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Drivers\n",
                 "\n",
                 "## What is a `Driver`?!\n",
                 "\n",
@@ -58,21 +60,23 @@
                 "from cosapp.drivers import RunOnce\n",
                 "\n",
                 "m = MultiplySystem('mult')\n",
                 "run = m.add_driver(RunOnce('run'))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 " ![Driver in system](images/drivers_1.svg)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Implementation\n",
                 "\n",
                 "Every `System` (including sub-systems) may have one or multiple `Driver` objects. They are stored in the `drivers` attribute.\n",
                 "By default, no `Driver` is attached to a `System`.\n",
@@ -95,28 +99,30 @@
                 "m.p_in.x = 15.\n",
                 "m.run_drivers()\n",
                 "\n",
                 "print(f\"{m.p_out.x = }\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Driver chains and subdrivers\n",
                 "\n",
                 "If several drivers are attached to a system, `run_drivers` will execute them in turn, as a sequence of drivers.\n",
                 "Furthermore, like a `System`, each individual `Driver` may have children, which also inherit from base class `Driver`. Nested drivers are created with method `add_child` of class `Driver`; they are stored in attribute `children` of the parent driver.\n",
                 "\n",
                 "By construction, a `System` can have as many levels of drivers as required.\n",
                 "\n",
                 "Driver chains and nested drivers thus allow users to define complex simulation scenarios, such as workflows, multi-point design, designs of experiment, optimization, *etc.*\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "![drivers](images/drivers_2.svg)\n"
             ]
         },
         {
@@ -139,14 +145,15 @@
             "source": [
                 "subrun = run.add_child(RunOnce('subrun'))  # add a sub-driver 'subrun'\n",
                 "\n",
                 "print(f\"{run.children = }\", f\"{subrun.children = }\", sep=\"\\n\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Available Drivers\n",
                 "\n",
                 "**CoSApp** comes with a set of drivers to help users build their simulations.\n",
                 "\n",
@@ -211,14 +218,15 @@
                 "    f\"{m.p_out.x = }\",\n",
                 "    f\"residues: {list(m.residues.values())}\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### NonLinearSolver\n",
                 "\n",
                 "This `Driver` determines the parameters of your `System` declared as unknowns that satisfy its equations. It resolves the mathematical problem between free parameters and residues of its child drivers.\n",
                 "\n",
@@ -263,50 +271,47 @@
                 "    f\"{m.p_out.x = }\",\n",
                 "    f\"residues: {list(solver.problem.residues.values())}\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Resolution method\n",
                 "\n",
                 "Several resolution methods are available, through option `method`, of type `NonLinearMethods`, contained in module `cosapp.drivers`.\n",
                 "Possible choices are:\n",
                 "\n",
                 "- `NonLinearMethods.NR` (default, recommended): custom implementation of Newton-Raphson algorithm, tailored for CoSApp systems.\n",
                 "- `NonLinearMethods.POWELL`: Powell hybrid method (encapsulation of `scipy.optimize.root`).\n",
                 "- `NonLinearMethods.BROYDEN_GOOD`: Broyden's \"good\" method (encapsulation of `scipy.optimize.root`).\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### RunSingleCase\n",
                 "\n",
-                "`NonLinearSolver` is primarily designed to solve [multi-point problems](./08-Multipoints-Design.ipynb), where several [RunSingleCase](#RunSingleCase) drivers are declared as direct sub-drivers of the solver.\n",
-                "By default, a `NonLinearSolver` driver comes with one [RunSingleCase](#RunSingleCase) child, called *runner*. \n",
+                "`RunSingleCase` sets its owner system in a given state, and executes all subsystem drivers by recursively calling the `compute()` method throughout the owner system tree.\n",
                 "\n",
-                "![scipysolver](images/drivers_nonlinear.svg)\n",
-                "\n",
-                "`RunSingleCase` executes all subsystem drivers by recursively calling the `compute()` method of the top system and each of its children.\n",
-                "\n",
-                "This `Driver` does not contain a solver per se, but is helpfull to set boundary conditions, initial values, and define additional unknowns and/or equations.\n",
-                "It is primarily meant to be used as an operating point of a [NonLinearSolver](#NonLinearSolver) driver.\n",
+                "This driver does not contain a solver *per se*, but is helpfull to set boundary conditions, initial values, and define additional unknowns and/or equations.\n",
+                "It is primarily meant to be used as an operating point of a [NonLinearSolver](#NonLinearSolver) driver, to solve [multi-point problems](./08-Multipoints-Design.ipynb).\n",
                 "Therefore, `RunSingleCase` drivers are usually created as sub-drivers of `NonLinearSolver`, and are seldom directly attached to a system.\n",
                 "\n",
                 "The state of the owner `System` can be changed with two methods:\n",
                 "\n",
                 "- `set_values` will impose the value of prescribed input variables, as boundary conditions;\n",
                 "- `set_init` will change the initial value of iteratives before resolving the case.\n",
                 "\n",
-                "Both methods take as argument a dictionary of the kind `{varname: value, ...}`, where `varname` is the name of an input variable *in the context of the driver owner*.\n",
+                "Both methods take as argument a dictionary of the kind `{varname: value, ...}`, where `varname` is the name of an input variable *in the context of the owner system*.\n",
                 "For example, if the driver is attached to a system `head` possessing a child named `sub` and an inward `x`, `{'sub.k': 0.0, 'x': 0.1}` will affect variables `head.sub.k` and `head.x`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -334,21 +339,22 @@
                 "    f\"{m.p_out.x = }\",\n",
                 "    f\"residues: {list(m.residues.values())}\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Another important ability of this driver is the addition of unknowns and equations to the mathematical system.\n",
                 "There are two kinds of problems for a `RunSingleCase` driver:\n",
                 "\n",
-                "- **Design problems**: They are associated with design variables that are frozen in the final product; e.g. the diameter of a pipe. Design unknowns are uniquely defined, and shared between all design points, when several `RunSingleCase` drivers are present (see tutorial on [multi-point design](08-Multipoints-Design.ipynb)).\n",
+                "- **Design problems**: They are associated with design variables that are frozen in the final product (such as a geometrical parameter, *e.g.*). Design unknowns are uniquely defined, and shared between all design points, when several `RunSingleCase` drivers are present (see tutorial on [multi-point design](08-Multipoints-Design.ipynb)).\n",
                 "- **Local off-design problems**: They correspond to constraints imposed at the design point only. Local `RunSingleCase` unknowns will usually assume different values at different design points.\n",
                 "\n",
                 "Design and off-design problems are stored in attributes `design` and `offdesign`, respectively.\n",
                 "Unknowns and equations are added with methods `add_unknown` and `add_equation`:\n",
                 "\n",
                 "```python\n",
                 "case.design  \\\n",
@@ -395,14 +401,15 @@
                 "    f\"{m.p_in.x = }\",\n",
                 "    f\"{m.p_out.x = }\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Design methods are defined at system level, and can be activated on demand in a simulation (more info in the [Design Method tutorial](./11-DesignMethods.ipynb))."
             ]
         },
         {
@@ -458,14 +465,15 @@
                 "    \"Mathematical problem:\",\n",
                 "    solver.problem,\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "`RunSingleCase` drivers may also be used to simulate a life cycle made of states. On next example, a design point is followed by two off-design operating points. \n",
                 "\n",
                 "![metadriver](images/drivers_5.svg)"
             ]
@@ -489,14 +497,15 @@
                 "print(f\"Mathematical problem:\\n{solver.problem}\\n\")\n",
                 "\n",
                 "df = solver.recorder.export_data()  # export recorded data as a pandas DataFrame\n",
                 "df"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For advanced design methods tutorial and strategy to create a \"design model\" from a \"simulation model\", we recommend the tutorial on [Design Methods](./11-DesignMethods.ipynb).\n",
                 "\n",
                 "**Congrats!** You are now ready to launch computation on your `System` with **CoSApp**!"
             ]
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/04-Triggers.ipynb` & `cosapp-0.15.0/cosapp/tutorials/04-Triggers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/05-Validation.ipynb` & `cosapp-0.15.0/cosapp/tutorials/05-Validation.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/06-Visibility.ipynb` & `cosapp-0.15.0/cosapp/tutorials/06-Visibility.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/07-Metamodels.ipynb` & `cosapp-0.15.0/cosapp/tutorials/07-Metamodels.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/08-Multipoints-Design.ipynb` & `cosapp-0.15.0/cosapp/tutorials/08-Multipoints-Design.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9655500886524823%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 2: "*

 * *            "{'attachments': OrderedDict()}, 3: {'attachments': OrderedDict()}, 4: {'attachments': "*

 * *            "OrderedDict()}, 5: {'source': {insert: [(76, '    def make(\\n'), (77, '        "*

 * *            "cls,\\n'), (78, '        name: str,\\n'), (79, '        parent: System,\\n'), (80, "*

 * *            "'        incoming: list[Dipole]=[],\\n'), (81, '        outgoing: "*

 * *            "list[Dipole]=[],\\n'), (82, '       […]*

```diff
@@ -1,19 +1,21 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Multi-point design"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Multi-point design\n",
                 "\n",
                 "Up to now, systems have been solved in their up-and-running state, that is all inputs are set, and we want to obtain the state of the system for a given set of boundary conditions.\n",
                 "\n",
@@ -96,14 +98,15 @@
                 "* For a `RunSingleCase` design point *case*, `case.add_unknown(...)` (respectively `add_equation`, `extend`) is a shortcut to `case.offdesign.add_unknown(...)`.\n",
                 "* Fixing a parameter using `case.set_values({'x': '0.123'})` is mathematically equivalent to the trivial constaint `case.add_unknown('x').add_equation('x == 0.123')`. Thus, the local off-design problem can be viewed as an extension of `set_values` for non-trivial, nonlinear constraints.\n",
                 "* In single-point design, solver and case problems (either off-design or design) are interchangeable. However, it is good practice to follow multi-point design rules, for the sake of consistency.\n",
                 "* Equations declared at solver level are satisfied independently on each `RunSingleCase` subdriver. Thus, in multi-point problems, be aware that a single solver equation will eventually result in several equations in the assembled mathematical problem."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Example\n",
                 "## Case description\n",
                 "\n",
                 "The simple circuit test case having a constant intensity source will be used here. In addition to the off-design resolution driving the potential `V` at nodes to balance current fluxes, we seek to determine the value of two resistances from two different operating points.\n",
@@ -113,19 +116,21 @@
                 "| Operating point | Boundary conditions | Design variable | Design equation |\n",
                 "|---|---|---|---|\n",
                 "| Point 1 | $I_{source} = 0.08$ A | `R2.R` | `n2.V == 8 V` |\n",
                 "| Point 2 | $I_{source} = 0.15$ A | `R1.R` | `n1.V == 50 V` |"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": []
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Building the circuit\n",
                 "\n",
                 "The circuit is built as an assembly of elementary models. The default case is then solved to initialize all variables."
             ]
@@ -208,15 +213,22 @@
                 "        self.add_equation('sum_I_in == sum_I_out', name='current balance')\n",
                 "\n",
                 "    def compute(self):\n",
                 "        self.sum_I_in = sum(current.I for current in self.incoming_currents)\n",
                 "        self.sum_I_out = sum(current.I for current in self.outgoing_currents)\n",
                 "\n",
                 "    @classmethod\n",
-                "    def make(cls, name, parent, incoming: list[Dipole]=[], outgoing: list[Dipole]=[], pulling=None) -> Node:\n",
+                "    def make(\n",
+                "        cls,\n",
+                "        name: str,\n",
+                "        parent: System,\n",
+                "        incoming: list[Dipole]=[],\n",
+                "        outgoing: list[Dipole]=[],\n",
+                "        pulling=None,\n",
+                "    ) -> Node:\n",
                 "        \"\"\"Factory creating new node within `parent`, with\n",
                 "        appropriate connections with incoming and outgoing dipoles.\n",
                 "        \"\"\"\n",
                 "        node = cls(name, n_in=len(incoming), n_out=len(outgoing))\n",
                 "        parent.add_child(node, pulling=pulling)\n",
                 "        \n",
                 "        for dipole, current in zip(incoming, node.incoming_currents):\n",
@@ -329,14 +341,15 @@
             "source": [
                 "from cosapp.utils import get_state, set_state\n",
                 "\n",
                 "initial_state = get_state(model)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Defining the design case\n",
                 "\n",
                 "After purging all drivers, the design case can be defined. First, a numerical solver is attached to the head system. Then, for each design point, a sub-driver `RunSingleCase` is added to the solver."
             ]
@@ -431,17 +444,15 @@
                 "from cosapp.drivers import NonLinearSolver, RunSingleCase\n",
                 "from cosapp.recorders import DataFrameRecorder\n",
                 "\n",
                 "# Create and initialize new model\n",
                 "model = AssembledModel('model')\n",
                 "set_state(model, initial_state)\n",
                 "\n",
-                "# Clear all previously defined drivers and add solver\n",
-                "model.drivers.clear()\n",
-                "set_state(model, initial_state)\n",
+                "# Add solver\n",
                 "solver = model.add_driver(NonLinearSolver('solver'))\n",
                 "\n",
                 "# Define design unknwowns.\n",
                 "# A maximum relative step between iterations is requested,\n",
                 "# to stabilize the resolution.\n",
                 "solver.add_unknown(['circuit.R1.R', 'circuit.R2.R'], max_rel_step=0.5)\n",
                 "\n",
@@ -495,19 +506,139 @@
             "source": [
                 "data = solver.recorder.export_data()\n",
                 "data = data.drop(['Section', 'Status', 'Error code'], axis=1)\n",
                 "data"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Multi-point design problems involving targets\n",
+                "\n",
+                "Targets offer a convenient way to declare a dynamically changeable target value on a variable (either input or output), rather than imposing a hard-coded right-hand-side value, as in:\n",
+                "\n",
+                "```python\n",
+                "point1.add_equation('circuit.n2.V == 8')\n",
+                "```\n",
+                "\n",
+                "Further detail on targets may be found in a dedicated [tutorial](Targets.ipynb).\n",
+                "\n",
+                "In single-point design problems, target values can be redefined by simply reassigning the targetted variables prior to solver execution (see [tutorial](Targets.ipynb)).\n",
+                "In multi-point design problems, though, a variable may be assigned different target values in different design points.\n",
+                "In the last circuit design problem, for example, potential `circuit.n2.V` is required to be 8 V in `point1`, and 5 V in `point2`.\n",
+                "Setting point-wise targets can be achieved with method `set_init`.\n",
+                "\n",
+                "Let us reformulate the same design problem, using targets:"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "from cosapp.drivers import NonLinearSolver, RunSingleCase\n",
+                "from cosapp.recorders import DataFrameRecorder\n",
+                "\n",
+                "# Create and initialize new model\n",
+                "model = AssembledModel('model')\n",
+                "set_state(model, initial_state)\n",
+                "\n",
+                "# Add solver\n",
+                "solver = model.add_driver(NonLinearSolver('solver'))\n",
+                "\n",
+                "# Define design unknwowns.\n",
+                "solver.add_unknown(['circuit.R1.R', 'circuit.R2.R'], max_rel_step=0.5)\n",
+                "\n",
+                "# Set a target on node 2 voltage (will pertain to all design points)\n",
+                "solver.add_target('circuit.n2.V')\n",
+                "\n",
+                "solver.add_recorder(\n",
+                "    DataFrameRecorder(\n",
+                "        includes = ['*.n?.V', '*R', 'source.I'],\n",
+                "        excludes = 'ground.*',\n",
+                "    )\n",
+                ")\n",
+                "\n",
+                "# Define design point #1\n",
+                "point1 = solver.add_child(RunSingleCase('point1'))\n",
+                "\n",
+                "point1.set_values({\n",
+                "    'source.I': 0.08, \n",
+                "    'ground.V': 0,\n",
+                "    'circuit.R3.R': 0.5e3,\n",
+                "})\n",
+                "\n",
+                "# Define design point #2\n",
+                "point2 = solver.add_child(RunSingleCase('point2')) \n",
+                "\n",
+                "point2.add_unknown('circuit.R3.R')  # local, off-design unknown\n",
+                "point2.add_target('circuit.n1.V')   # local target on node 1 voltage\n",
+                "\n",
+                "point2.set_values({\n",
+                "    'source.I': 0.15,\n",
+                "    'ground.V': 0,\n",
+                "})"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Once the problem is defined, we can specify point-dependent target values using method `set_init`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "point1.set_init({\n",
+                "    'circuit.n2.V': 8.0,\n",
+                "})\n",
+                "point2.set_init({\n",
+                "    'circuit.n1.V': 50.0,\n",
+                "    'circuit.n2.V': 5.0,\n",
+                "})\n",
+                "\n",
+                "model.run_drivers()\n",
+                "\n",
+                "solver.problem"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Target values can now be redefined interactively, by simply changing initial values:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "point1.set_init({\n",
+                "    'circuit.n2.V': 12.0,\n",
+                "})\n",
+                "point2.set_init({\n",
+                "    'circuit.n1.V': 62.0,\n",
+                "    'circuit.n2.V': 7.5,\n",
+                "})\n",
+                "\n",
+                "model.run_drivers()\n",
+                "\n",
+                "solver.problem"
+            ]
         }
     ],
     "metadata": {
         "hide_input": false,
         "kernelspec": {
             "display_name": "cosapp",
             "language": "python",
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/09-MonteCarlo.ipynb` & `cosapp-0.15.0/cosapp/tutorials/09-MonteCarlo.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/10-Recorders.ipynb` & `cosapp-0.15.0/cosapp/tutorials/10-Recorders.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/11-DesignMethods.ipynb` & `cosapp-0.15.0/cosapp/tutorials/11-DesignMethods.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982744815097756%*

 * *Differences: {"'cells'": '{10: {\'source\': {insert: [(14, \'        """Compute `x` such that `y == 0`.\\n\')], '*

 * *            'delete: [14]}}, 12: {\'source\': {insert: [(5, \'\\n\'), (14, \'    f"Converged in '*

 * *            '{solver.results.fres_calls} iterations",\\n\')]}}, 14: {\'source\': {insert: [(3, '*

 * *            '\'\\n\'), (12, \'    f"Converged in {solver.results.fres_calls} '*

 * *            'iterations",\\n\')]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -219,15 +219,15 @@
                 "        self.add_inward('x', 1.0)\n",
                 "        self.add_outward('y', 0.0)\n",
                 "\n",
                 "    def compute(self):\n",
                 "        self.y = math.sin(self.x**2 - 2)\n",
                 "    \n",
                 "    def design_x(self, **options):\n",
-                "        \"\"\"Design method for `x`.\n",
+                "        \"\"\"Compute `x` such that `y == 0`.\n",
                 "        Additional options apply to unknown `x`.\n",
                 "        \"\"\"\n",
                 "        problem = self.new_problem()\n",
                 "        problem.add_unknown('x', **options)\n",
                 "        problem.add_equation('y == 0')\n",
                 "        return problem\n"
             ]
@@ -246,22 +246,24 @@
             "outputs": [],
             "source": [
                 "from cosapp.drivers import NonLinearSolver\n",
                 "\n",
                 "s = SystemWithDynamicDesignMethod('s')\n",
                 "\n",
                 "solver = s.add_driver(NonLinearSolver('solver'))\n",
+                "\n",
                 "solver.extend(s.design_x())\n",
                 "\n",
                 "s.x = 0.7  # initial value\n",
                 "s.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{s.x = }\",\n",
                 "    f\"{s.y = }\",\n",
+                "    f\"Converged in {solver.results.fres_calls} iterations\",\n",
                 "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -274,22 +276,24 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = SystemWithDynamicDesignMethod('s')\n",
                 "\n",
                 "solver = s.add_driver(NonLinearSolver('solver'))\n",
+                "\n",
                 "solver.extend(s.design_x(max_abs_step=0.1))\n",
                 "\n",
                 "s.x = 0.7  # initial value\n",
                 "s.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{s.x = }\",\n",
                 "    f\"{s.y = }\",\n",
+                "    f\"Converged in {solver.results.fres_calls} iterations\",\n",
                 "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -327,15 +331,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.10.12"
         },
         "vscode": {
             "interpreter": {
                 "hash": "03d8647662c9fbe9220ebb6c4a5dd3c1d557fb5efab079901b8383e5f052f0cc"
             }
         }
     },
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/CustomConnectors.ipynb` & `cosapp-0.15.0/cosapp/tutorials/CustomConnectors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/FMI.ipynb` & `cosapp-0.15.0/cosapp/tutorials/FMI.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/Guidelines.ipynb` & `cosapp-0.15.0/cosapp/tutorials/Guidelines.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/HybridSimulations.ipynb` & `cosapp-0.15.0/cosapp/tutorials/HybridSimulations.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761436480186481%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '![CoSAppLogo](images/cosapp.svg) **CoSApp** "*

 * *            "tutorials\\n'), (1, '\\n')]}}, 1: {'source': {insert: [(32, '* `<=`: expression `lhs "*

 * *            '- rhs` goes from positive to negative, meaning `lhs` becomes smaller than '*

 * *            "`rhs`;\\n'), (33, '* `>=`: expression `lhs - rhs` goes from negative to positive, "*

 * *            "meaning `lhs` becomes greater than `rhs`;\\n'), (50, 'Alternatively, events may be "*

 * *            'triggered by other events, […]*

```diff
@@ -1,20 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "![CoSAppLogo](images/cosapp.svg)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials\n",
+                "\n",
                 "# Simulations with discrete-time events\n",
                 "\n",
                 "Dynamic systems involving time derivatives can be solved using a time driver (see tutorial on [time simulations](TimeDriver.ipynb)).\n",
                 "Such simulations are referred to as *continuous time* simulations, as all quantities are expected to vary continuously with time.\n",
                 "\n",
                 "Discontinuities, however, can be introduced with the occurrence of **events**, defined within a system."
             ]
@@ -51,16 +46,16 @@
                 "Even though `\"lhs <op> rhs\"` corresponds to a Boolean expression, the event activation will *not* be triggered by the Boolean value.\n",
                 "Instead, time drivers will check for sign changes of `lhs - rhs` at each integration time step.\n",
                 "Since lhs and rhs are assumed to be continuous expressions in time, a sign change of their difference guaranties that there exists a time when lhs equals rhs.\n",
                 "This time value, determined numerically by solving a root-finding problem, will be regarded as the occurrence time of the event.\n",
                 "\n",
                 "Strict and non-strict inequalities are treated identically, so the actual discriminating cases are `==`, `<=`, and `>=`:\n",
                 "\n",
-                "* `<=`: expression `lhs - rhs` goes from positive to negative, meaning that `lhs` becomes smaller that `rhs`;\n",
-                "* `>=`: expression `lhs - rhs` goes from negative to positive, meaning that `lhs` becomes greater that `rhs`;\n",
+                "* `<=`: expression `lhs - rhs` goes from positive to negative, meaning `lhs` becomes smaller than `rhs`;\n",
+                "* `>=`: expression `lhs - rhs` goes from negative to positive, meaning `lhs` becomes greater than `rhs`;\n",
                 "* `==`: expression `lhs - rhs` simply changes sign.\n",
                 "\n",
                 "These distinctions allow one to define directional events (different events occur when *a* exceeds *b*, and when *b* exceeds *a*), as well as one-way events.\n",
                 "For example,\n",
                 "```python\n",
                 "class BreakableSystem(System):\n",
                 "    def setup(self):\n",
@@ -69,21 +64,36 @@
                 "        self.add_event('failure', trigger=\"x > x_max\")\n",
                 "```\n",
                 "indicates that if `failure` ever occurs (in which case we expect the system will change, as we will see later), there is no going back, even is `x` later returns below `x_max`.\n",
                 "\n",
                 "### Primitive and derived events\n",
                 "\n",
                 "Events triggered by a zero-crossing expression, as discussed in previous section, are said to be *primitive*, as they are self-determined.\n",
-                "Alternatively, events may be triggered by other events, in which case they are referred to as *derived events*.\n",
+                "Alternatively, events may be triggered by other events, in which case they are referred to as *secondary*, or *derived* events.\n",
                 "\n",
                 "Derived events can be either:\n",
                 "\n",
-                "* Synchronized events, simply triggered by the occurrence of another event.\n",
-                "* Filtered events, triggered by the occurrence of a distinct event *and* an additional condition, given as an evaluable Boolean expression. The syntax is `primary.filter(<condition>)`.\n",
-                "* Merged events, triggered by the occurrence of one among a list of events. Syntax is `Event.merge(event1, event2, ...)`, where `Event` is imported from module `cosapp.multimode`.\n"
+                "* **Synchronized events**, simply triggered by the occurrence of another event:\n",
+                "\n",
+                "  ```python\n",
+                "  event.trigger = other_event\n",
+                "  ```\n",
+                "\n",
+                "* **Filtered events**, triggered by the occurrence of a distinct event *and* an additional condition, given as an evaluable Boolean expression. Syntax is:\n",
+                "\n",
+                "  ```python\n",
+                "  event = other_event.filter(<condition>)\n",
+                "  ```\n",
+                "\n",
+                "* **Merged events**, triggered by the occurrence of one among a list of events. Syntax is:\n",
+                "  ```python\n",
+                "  from cosapp.multimode import Event\n",
+                "\n",
+                "  event = Event.merge(event1, event2, ...)\n",
+                "  ```\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -293,19 +303,14 @@
             "source": [
                 "## Examples\n",
                 "\n",
                 "* [Multimode ODE](multimode/MultimodeOde.ipynb)\n",
                 "* [Newton Pendulum](multimode/NewtonPendulum.ipynb)\n",
                 "* [Bouncing Ball](multimode/BouncingBall.ipynb)"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/Logging.ipynb` & `cosapp-0.15.0/cosapp/tutorials/Logging.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/Optimization.ipynb` & `cosapp-0.15.0/cosapp/tutorials/Optimization.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/SystemSurrogates.ipynb` & `cosapp-0.15.0/cosapp/tutorials/SystemSurrogates.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb` & `cosapp-0.15.0/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/Targets.ipynb` & `cosapp-0.15.0/cosapp/tutorials/Targets.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.967977791470295%*

 * *Differences: {"'cells'": "{0: {'source': ['![CoSAppLogo](images/cosapp.svg) **CoSApp** examples\\n', '\\n', '# "*

 * *            "Setting targets on output variables\\n', '\\n', 'CoSApp systems declare a directional "*

 * *            "interface, and transform inputs into outputs.\\n', 'It is good practice to design "*

 * *            'systems such that their inputs and outputs correspond to the "normal", direct '*

 * *            'behaviour of the system, without presuming how it will be used in a more complex '*

 * *            "assembly, or […]*

```diff
@@ -1,28 +1,24 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "![CoSAppLogo](images/cosapp.svg) **CoSApp** examples:"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Settings targets on output values\n",
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** examples\n",
+                "\n",
+                "# Setting targets on output variables\n",
                 "\n",
                 "CoSApp systems declare a directional interface, and transform inputs into outputs.\n",
                 "It is good practice to design systems such that their inputs and outputs correspond to the \"normal\", direct behaviour of the system, without presuming how it will be used in a more complex assembly, or what users will want to do with it.\n",
                 "\n",
-                "As it happens, it is very common to use a given system in a reverse way, when one wishes certain outputs to reach a target value.\n",
+                "As it happens, it is very common to use a given system in a reverse way, when one wishes certain outputs to reach target values.\n",
                 "\n",
                 "The first obvious way to achieve that is to setup a nonlinear problem, whereby an input is sought to satisfy an equation of the kind \"target_output == target_value\"."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -56,19 +52,20 @@
                 "\n",
                 "f.a = 2.0\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Displaying attribute `solver.problem` reveals the mathematical problem solved by the driver:"
             ]
         },
         {
@@ -77,23 +74,24 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "solver.problem"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Set target value dynamically\n",
                 "\n",
                 "In the previous example, the target value for `f.y` is hard-coded as the right-hand side of the design equation.\n",
-                "Changing this value requires the setup of a new mathematical problem, with a new equation.\n",
+                "Changing this value requires the setup of a new mathematical problem, with a new hard-coded equation.\n",
                 "\n",
-                "An alternative way is to this procedure is the use of method `add_target`:"
+                "Alternatively, method `add_target` offers a convenient way is to set targets on variables:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -103,24 +101,26 @@
                 "f = SimpleFunction('f')\n",
                 "\n",
                 "solver = f.add_driver(NonLinearSolver('solver'))\n",
                 "solver.add_unknown('x').add_target('y')\n",
                 "\n",
                 "f.a = 2.0\n",
                 "f.y = 0.0   # set target value by setting output variable\n",
+                "\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Job done!\n",
                 "Looking at attribute `problem` shows that the actual mathematical problem has not changed:"
             ]
         },
@@ -130,18 +130,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "solver.problem"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The difference, however, is that the right-hand side of the equation is now dynamically set to the current value of `f.y` before each solver execution.\n",
+                "The difference, however, is that the right-hand side of the equation is now dynamically set to the current value of `f.y`, before each solver execution.\n",
                 "Therefore, we can now update the target value interactively, by simply assigning a new value to `f.y`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -150,32 +151,112 @@
                 "f.y = -0.5  # update target value dynamically\n",
                 "\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As can be seen after each computation, `f.y` only reaches the targetted value *within solver tolerance*.\n",
                 "Indeed, if `add_target` offers a convenient way of defining target values, one must keep in mind that `f.y` remains an output, whose value is strictly determined by the actual inputs of `f`.\n",
                 "\n",
                 "As a consequence, it is up to users to control the value of targetted variables *before each solver execution*."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Controlling more strictly target values, if necessary, can be achieved by defining initial values in `RunSingleCase` sub-driver(s)."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from cosapp.drivers import NonLinearSolver, RunSingleCase\n",
+                "\n",
+                "f = SimpleFunction('f')\n",
+                "\n",
+                "solver = f.add_driver(NonLinearSolver('solver'))\n",
+                "solver.add_unknown('x').add_target('y')\n",
+                "\n",
+                "case = solver.add_child(RunSingleCase('case'))\n",
+                "case.set_init({\n",
+                "    'y': 0.5,  # will be used as equation rhs\n",
+                "})\n",
+                "\n",
+                "f.a = 2.0\n",
+                "f.x = 1.0\n",
+                "f.y = 0.0\n",
+                "\n",
+                "f.run_drivers()\n",
+                "\n",
+                "print(solver.problem)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Re-affecting `f.y` interactively will not update the mathematical problem, as the target value for `f.y` is now enforced by driver `solver.case`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "f.x = 1.0\n",
+                "f.y = 0.0\n",
+                "\n",
+                "f.run_drivers()\n",
+                "\n",
+                "print(solver.problem)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Changing the target value of `f.y` can still be done through `solver.case.set_init`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "solver.case.set_init({\n",
+                "    'x': 2.0,\n",
+                "    'y': -0.5,\n",
+                "})\n",
+                "\n",
+                "f.run_drivers()\n",
+                "\n",
+                "print(solver.problem)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Targets and design methods\n",
                 "\n",
                 "Targets can be particularly interesting to define [design methods](11-DesignMethods.ipynb) with a controllable target value."
             ]
         },
         {
             "cell_type": "code",
@@ -214,19 +295,20 @@
                 "f.a = 2.0\n",
                 "f.y = -0.5\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Without the use of `add_target`, the only way to control the design value of `y` would be to declare an additional inward `y_target`, say, used as right-hand side value of design equation:\n",
                 "```python\n",
                 "    def setup(self):\n",
                 "        self.add_inward('a', 0.0)\n",
@@ -238,14 +320,15 @@
                 "        design.add_unknown('x').add_equation('y == y_target')\n",
                 "```\n",
                 "\n",
                 "While this syntax works, it has the inconvenience of burdening the system with an inward only meaningful when design method `'y'` is activated."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Pulling a targetted variable\n",
                 "\n",
                 "Consider a system with a targetted output pulled at parent level.\n"
             ]
@@ -284,31 +367,32 @@
                 "head.x = 3.0\n",
                 "head.g.y = 5.0\n",
                 "head.f.a = 2.0\n",
                 "\n",
                 "head.run_drivers()\n",
                 "\n",
                 "print(\n",
-                "    f\"Solution:\\n\"\n",
+                "    f\"Solution:\",\n",
                 "    f\"{head.g.x = }\",\n",
                 "    f\"{head.g.y = }\",\n",
                 "    f\"\\n{solver.problem!r}\",\n",
                 "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "What just happened?!\n",
                 "\n",
                 "In this case, output `head.g.y` is pulled up at parent level. Behind the scene, an *upward* connection is created from `head.g.y` to `head.y`, such that `y` appears as a natural output of top system `head`, computed by sub-system `head.g`.\n",
                 "\n",
-                "As a consequence, it seems natural to set the targetted value in the context of system `head`, that is setting `head.y` instead of `head.g.y`, when activating `head.design('y')`.\n",
+                "As a consequence, when activating `head.design('y')`, it seems natural to set the targetted value in the context of system `head`, that is setting `head.y` instead of `head.g.y`.\n",
                 "Let's try again:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -323,23 +407,24 @@
                 "head.x = 3.0\n",
                 "head.y = 5.0    # set target value\n",
                 "head.f.a = 2.0\n",
                 "\n",
                 "head.run_drivers()\n",
                 "\n",
                 "print(\n",
-                "    f\"Solution:\\n\"\n",
+                "    f\"Solution:\",\n",
                 "    f\"{head.g.x = }\",\n",
                 "    f\"{head.g.y = }\",\n",
                 "    f\"\\n{solver.problem!r}\",\n",
                 "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Weak and strong targets\n",
                 "\n",
                 "A target is said to be *weak* if it can be disregarded in certain situations.\n",
                 "By default, targets are *strong*, meaning the target equation is always enforced.\n",
@@ -348,30 +433,32 @@
                 "\n",
                 "1. is an output;\n",
                 "2. is connected to an input.\n",
                 "\n",
                 "The second condition specifically excludes pulled outputs, which is the only admissible output-output connection.\n",
                 "\n",
                 "Weak targets may be useful when a targetted variable is transmitted through a chain of systems, and one wants to specify the target on the last system only.\n",
-                "This is typically the case in the next example, where we simulate three resistors series, and wish to determine the current between end-point voltages.\n"
+                "This is typically the case in the next example, where we simulate three resistors in series, and wish to determine the current between end-point voltages.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from cosapp.base import System, Port\n",
                 "\n",
+                "\n",
                 "class ElectricPort(Port):\n",
                 "    def setup(self):\n",
                 "        self.add_variable(\"I\", 1.0, unit=\"A\", desc=\"Current\")\n",
                 "        self.add_variable(\"V\", 0.0, unit=\"V\", desc=\"Voltage\")\n",
                 "\n",
+                "\n",
                 "class Resistor(System):\n",
                 "    def setup(self):\n",
                 "        self.add_input(ElectricPort, 'elec_in')\n",
                 "        self.add_output(ElectricPort, 'elec_out')\n",
                 "\n",
                 "        self.add_inward(\"R\", 1e2, unit=\"ohm\", desc=\"Resistance\")\n",
                 "        self.add_outward(\"deltaV\", 0.0, unit=\"V\")\n",
@@ -381,25 +468,29 @@
                 "    \n",
                 "    def compute(self):\n",
                 "        elec_in, elec_out = self.elec_in, self.elec_out\n",
                 "        self.deltaV = self.R * elec_in.I\n",
                 "        elec_out.I = elec_in.I\n",
                 "        elec_out.V = elec_in.V - self.deltaV\n",
                 "\n",
+                "\n",
                 "class ThreeResistorSeries(System):\n",
                 "    def setup(self):\n",
                 "        R1 = self.add_child(Resistor(\"R1\"), pulling=\"elec_in\")\n",
                 "        R2 = self.add_child(Resistor(\"R2\"))\n",
                 "        R3 = self.add_child(Resistor(\"R3\"), pulling=\"elec_out\")\n",
-                "        \n",
+                "\n",
+                "        self.add_property('resistances', (R1, R2, R3))  # for convenience\n",
+                "\n",
                 "        self.connect(R1.elec_out, R2.elec_in)\n",
                 "        self.connect(R2.elec_out, R3.elec_in)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Each resistor defines an inner off-design problem, in which current is unknown, and a target is set on the output voltage.\n",
                 "When several resistors are connected, local unknown currents are discarded every time they belong to a connected input port, which occurs at each node point connecting adjacent resistors.\n",
                 "Likewise, local weak targets on voltages are discarded at each connecting node, where output voltage is transmitted to the next resistor.\n",
                 "\n",
@@ -408,52 +499,61 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s = ThreeResistorSeries('s')\n",
-                "\n",
-                "s.R1.R = 100\n",
-                "s.R2.R = 50\n",
-                "s.R3.R = 250\n",
+                "circuit = ThreeResistorSeries('circuit')\n",
                 "\n",
-                "s.elec_in.V = 10\n",
-                "s.elec_out.V = -2\n",
+                "circuit.R1.R = 100\n",
+                "circuit.R2.R = 50.\n",
+                "circuit.R3.R = 250\n",
+                "\n",
+                "circuit.elec_in.I = 0.25   # initial guess\n",
+                "circuit.elec_in.V = 10\n",
+                "circuit.elec_out.V = -2\n",
                 "\n",
                 "# Set bogus target values at connection points\n",
                 "# These values will be discarded, as targets are weak\n",
-                "s.R1.elec_out.V = 1.23e4\n",
-                "s.R2.elec_out.V = -8e17\n",
-                "\n",
-                "s.add_driver(NonLinearSolver('solver'))\n",
-                "s.run_drivers()\n",
+                "circuit.R1.elec_out.V = 1.23e4\n",
+                "circuit.R2.elec_out.V = -8e17\n",
                 "\n",
-                "voltages = [s.elec_in.V]\n",
-                "voltages.extend(s[f\"R{i}.elec_out.V\"] for i in range(1, 4))\n",
+                "circuit.add_driver(NonLinearSolver('solver'))\n",
+                "circuit.run_drivers()\n",
                 "\n",
-                "print(\n",
-                "    f\"Solution:\\n\"\n",
-                "    f\"{s.elec_in.I = }\",\n",
-                "    f\"{s.elec_in.V = }\",\n",
-                "    f\"{s.elec_out.V = }\",\n",
-                "    f\"{voltages = }\",\n",
-                "    f\"\\nOverall resistance: {(s.elec_in.V - s.elec_out.V) / s.elec_in.I :.2f} Ohm\",\n",
-                "    sep = \"\\n\",\n",
-                ")\n"
+                "# Show actual problem solved\n",
+                "circuit.drivers['solver'].problem"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s.drivers['solver'].problem"
+                "voltages = [circuit.elec_in.V]\n",
+                "voltages.extend(res.elec_out.V for res in circuit.resistances)\n",
+                "\n",
+                "R_global = (circuit.elec_in.V - circuit.elec_out.V) / circuit.elec_in.I\n",
+                "\n",
+                "print(\n",
+                "    f\"Solution:\",\n",
+                "    f\"{circuit.elec_in.I = }\",\n",
+                "    f\"{circuit.elec_in.V = }\",\n",
+                "    f\"{circuit.elec_out.V = }\",\n",
+                "    f\"{voltages = }\",\n",
+                "    sep=\"\\n  \",\n",
+                ")\n",
+                "print(\n",
+                "    \"\",\n",
+                "    f\"Overall resistance: {R_global} Ohm\",\n",
+                "    f\"Sum of resistances: {sum(res.R for res in circuit.resistances)} Ohm\",\n",
+                "    sep=\"\\n\",\n",
+                ")\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -461,31 +561,38 @@
                 "import pandas as pd\n",
                 "import plotly.express as px\n",
                 "\n",
                 "df = pd.DataFrame.from_dict(\n",
                 "    {\n",
                 "        \"V\": voltages,\n",
                 "        \"index\": list(range(len(voltages))),\n",
-                "        \"node\": list('ABCD'),\n",
+                "        \"node\": list(\"ABCD\"),\n",
                 "    }\n",
                 ")\n",
                 "\n",
-                "fig = px.line(df,\n",
+                "fig = px.scatter(df,\n",
                 "    x=\"node\", y=\"V\",\n",
                 "    title=\"Voltage profile\",\n",
-                "    # markers=True,\n",
+                ")\n",
+                "fig.update_traces(\n",
+                "    mode=\"lines+markers\",\n",
+                "    marker=dict(\n",
+                "        size=10,\n",
+                "        color='#636EFA',\n",
+                "    ),\n",
                 ")\n",
                 "fig.update_layout(\n",
-                "    height=450,\n",
+                "    height=600,\n",
                 "    hovermode='x',\n",
                 ")\n",
                 "fig.show()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Targetted expressions\n",
                 "\n",
                 "A target can also be set on an evaluable expression, such as `norm(v)` or `y * (y + 1)`, as long as the expression only involves a single variable."
             ]
@@ -507,25 +614,26 @@
                 "f = CubicFunction('f')\n",
                 "\n",
                 "solver = f.add_driver(NonLinearSolver('solver'))\n",
                 "\n",
                 "solver.add_unknown('x').add_target('abs(y)')\n",
                 "\n",
                 "f.y = 8  # value used for targetted expression\n",
-                "f.x = 4  # positive initial value of unknown\n",
+                "f.x = 4  # positive initial value of unknown x\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Same computation, with a different initial guess on `f.x`:"
             ]
         },
         {
@@ -537,15 +645,15 @@
                 "f.y = 8\n",
                 "f.x = -5  # negative initial value\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/TimeDriver.ipynb` & `cosapp-0.15.0/cosapp/tutorials/TimeDriver.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666667%*

 * *Differences: {"'cells'": "{0: {'source': ['![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Time "*

 * *            "simulations\\n', '\\n', '# Time simulations\\n', '\\n', '### Declare transient "*

 * *            "variables in a system\\n', '\\n', 'CoSApp allows one to simulate the behaviour of "*

 * *            "systems with time-dependent variables, through the use of time drivers.\\n', '\\n', "*

 * *            "'Transient variables, defined by their time derivative, are declared with method "*

 * *            "`add_transient` at sy […]*

```diff
@@ -2,21 +2,16 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Time simulations"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Time simulations\n",
+                "\n",
                 "# Time simulations\n",
                 "\n",
                 "### Declare transient variables in a system\n",
                 "\n",
                 "CoSApp allows one to simulate the behaviour of systems with time-dependent variables, through the use of time drivers.\n",
                 "\n",
                 "Transient variables, defined by their time derivative, are declared with method `add_transient` at system setup.\n",
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/TimeDriverAdvanced.ipynb` & `cosapp-0.15.0/cosapp/tutorials/TimeDriverAdvanced.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9847484923245614%*

 * *Differences: {"'cells'": "{0: {'source': ['![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Advanced Time "*

 * *            "simulations\\n', '\\n', '# Time simulations - Advanced Features'], 'attachments': "*

 * *            "OrderedDict()}, 1: {'source': {insert: [(1, '\\n')]}, 'attachments': OrderedDict()}, "*

 * *            "3: {'source': {insert: [(0, 'from cosapp.drivers import RungeKutta, "*

 * *            "NonLinearSolver\\n'), (5, '\\n'), (7, 'solver = "*

 * *            'point.add_driver(NonLinearSolver("solver"))\\n\'), (8,  […]*

```diff
@@ -1,30 +1,28 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Advanced Time simulations"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Advanced Time simulations\n",
+                "\n",
                 "# Time simulations - Advanced Features"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Find the initial condition leading to a target end point\n",
+                "\n",
                 "In this example, we combine a nonlinear solver and a time driver, to compute the initial condition leading to a target point at the end of the time simulation."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -60,23 +58,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from cosapp.drivers import RungeKutta, NonLinearSolver, RunSingleCase\n",
+                "from cosapp.drivers import RungeKutta, NonLinearSolver\n",
                 "from cosapp.recorders import DataFrameRecorder\n",
                 "from time_solutions import PointMassSolution\n",
                 "\n",
                 "point = Ballistics('point')  # head system\n",
+                "\n",
                 "# Add drivers\n",
-                "solver = point.add_driver(NonLinearSolver('solver', factor=0.9))\n",
-                "target = solver.add_child(RunSingleCase('target'))\n",
-                "driver = target.add_child(RungeKutta(\"RungeKutta\", order=3))\n",
+                "solver = point.add_driver(NonLinearSolver(\"solver\"))\n",
+                "driver = solver.add_child(RungeKutta(\"RungeKutta\", order=3))\n",
+                "\n",
+                "# Define `v0` as unknown, so that the final value of `x` is a desired target point\n",
+                "# Note:\n",
+                "#   For driver `solver`, variable 'x' represents the position at the end of\n",
+                "#   each time simulation, since it is the parent of the `RungeKutta` time driver.\n",
+                "solver.add_unknown('v0').add_equation('x == [10, 0, 10]')\n",
                 "\n",
                 "# Define a simulation scenario\n",
                 "driver.time_interval = (0, 2)\n",
                 "driver.dt = 0.1\n",
                 "\n",
                 "x0 = [0, 0, 10]\n",
                 "\n",
@@ -87,22 +91,17 @@
                 "    },\n",
                 "    values = {'mass': 1.5, 'k': 0.92},\n",
                 ")\n",
                 "\n",
                 "# Add a recorder to capture time evolution in a dataframe\n",
                 "driver.add_recorder(DataFrameRecorder(includes=['x', 'v', 'a']), period=0.1)\n",
                 "\n",
-                "# Define `v0` as unknown, so that the final value of `x` is a desired target point\n",
-                "# Note:\n",
-                "#   For `RunSingleCase` driver `target`, 'x' represents the position at the end of\n",
-                "#   each time simulation, since it is the parent of the `RungeKutta` time driver.\n",
-                "target.design.add_unknown('v0').add_equation('x == [10, 0, 10]')\n",
-                "target.set_init({'v0': np.ones(3)})\n",
+                "point.v0 = np.ones(3)  # initial guess for the solver\n",
                 "\n",
-                "point.run_drivers()\n",
+                "point.run_drivers()  # solve\n",
                 "\n",
                 "solution = PointMassSolution(point, point.v0, x0)\n",
                 "\n",
                 "data = driver.recorder.export_data()\n",
                 "time = np.asarray(data['time'])\n",
                 "traj = {\n",
                 "    'exact': np.array(list(map(solution.x, time))),\n",
@@ -111,22 +110,22 @@
                 "\n",
                 "error = np.abs(traj['num'] - traj['exact'])\n",
                 "\n",
                 "print(\n",
                 "    f\"order = {driver.order}; dt = {driver.dt}\",\n",
                 "    f\"Max error on trajectory = {error.max():.2e}\",\n",
                 "    f\"End point: {traj['num'][-1].round(3)}\",\n",
+                "    f\"v0 = {point.v0.round(3)}\",\n",
                 "    sep=\"\\n\",\n",
                 ")\n",
                 "vz = point.v0[2]\n",
                 "vh = np.linalg.norm(point.v0[:2])\n",
                 "angle = np.arctan2(vz, vh)\n",
-                "print(f\"v0 = {point.v0.round(3)}\")\n",
                 "print(\n",
-                "    f\"norm = {np.linalg.norm(point.v0):.2f}\",\n",
+                "    f\"norm = {np.linalg.norm(point.v0):.2f} m/s\",\n",
                 "    f\"angle = {np.degrees(angle):.1f} deg\",\n",
                 "    sep=\"; \",\n",
                 ")\n"
             ]
         },
         {
             "cell_type": "code",
@@ -284,14 +283,15 @@
                 "    )\n",
                 ")\n",
                 "\n",
                 "go.Figure(data=traces, layout=layout)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In the next two cells, we display the recorded time and y steps, respectively.\n",
                 "At the beginning of the simulation, dy/dt is sufficiently small that the evolution of `ode.y` within time interval `driver.dt` (0.5) does not exceed the specified `max_abs_step`.\n",
                 "As time goes on, dy/dt increases and eventually becomes too large to limit the y step within `driver.dt`; time step limitation kicks in, and the actual `dt` appears to be smaller than `driver.dt`.\n",
                 "\n",
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/TipsAndTricks.ipynb` & `cosapp-0.15.0/cosapp/tutorials/TipsAndTricks.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.946529307625099%*

 * *Differences: {"'cells'": "{16: {'source': {insert: [(1, '\\n'), (7, '\\n'), (18, '\\n'), (24, '        # Create "*

 * *            "a tuple of children\\n'), (25, '        resistors = tuple(\\n'), (28, '        "*

 * *            ")\\n'), (29, '        # Store collection as a read-only property\\n'), (30, "*

 * *            '"        self.add_property(\'resistors\', resistors)\\n"), (32, \'        # Connect '*

 * *            "resistors in series\\n'), (33, '        for previous, current in zip(resistors, "*

 * *            "resistors[1:]):\\n' […]*

```diff
@@ -310,59 +310,68 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from cosapp.base import Port, System\n",
                 "\n",
+                "\n",
                 "class ElecPort(Port):\n",
                 "    def setup(self):\n",
                 "        self.add_variable(\"I\", 1.0, unit=\"A\", desc=\"Current\")\n",
                 "        self.add_variable(\"V\", 0.0, unit=\"V\", desc=\"Voltage\")\n",
                 "\n",
+                "\n",
                 "class Resistor(System):\n",
                 "    def setup(self):\n",
                 "        self.add_input(ElecPort, 'elec_in')\n",
                 "        self.add_output(ElecPort, 'elec_out')\n",
                 "        self.add_inward(\"R\", 1e2, unit=\"ohm\", desc=\"Resistance\")\n",
                 "    \n",
                 "    def compute(self):\n",
                 "        self.elec_out.I = I = self.elec_in.I\n",
                 "        self.elec_out.V = self.elec_in.V - self.R * I\n",
                 "\n",
+                "\n",
                 "class ResistorSeries(System):\n",
                 "    def setup(self, n=2):\n",
                 "        self.add_property('n', max(int(n), 2))\n",
                 "\n",
-                "        # Create a tuple of children, and store it as a property\n",
-                "        self.add_property('resistors', tuple(\n",
+                "        # Create a tuple of children\n",
+                "        resistors = tuple(\n",
                 "            self.add_child(Resistor(f\"R{i}\"))\n",
                 "            for i in range(self.n)\n",
-                "        ))\n",
-                "        R = self.resistors\n",
+                "        )\n",
+                "        # Store collection as a read-only property\n",
+                "        self.add_property('resistors', resistors)\n",
                 "        \n",
-                "        for previous, current in zip(R, R[1:]):\n",
+                "        # Connect resistors in series\n",
+                "        for previous, current in zip(resistors, resistors[1:]):\n",
                 "            self.connect(current.elec_in, previous.elec_out)\n",
                 "\n",
                 "        # Pull first `elec_in` and last `elec_out`\n",
                 "        self.add_input(ElecPort, 'elec_in')\n",
                 "        self.add_output(ElecPort, 'elec_out')\n",
                 "\n",
-                "        self.connect(self.elec_in, R[0].elec_in)\n",
-                "        self.connect(self.elec_out, R[-1].elec_out)\n"
+                "        self.connect(self.elec_in, resistors[0].elec_in)\n",
+                "        self.connect(self.elec_out, resistors[-1].elec_out)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The same trick can be used to create collections of ports, if needed.\n",
                 "\n",
-                "Use of property `resistors` makes the code clearer, and allows one to loop through the child/port collection without resorting to syntaxes of the kind `s[f\"R{i}\"] for i in range(s.n)`.\n",
+                "Use of property `resistors` makes the code clearer, and allows one to loop through the child/port collection without resorting to syntaxes of the kind\n",
+                "\n",
+                "```python\n",
+                "s[f\"R{i}\"] for i in range(s.n)\n",
+                "```\n",
                 "\n",
                 "In the next cell, for example, we show three identical ways of initializing the resistances:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -465,82 +474,84 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = MySystem('s', n=2, x=[[0, 0.1, 0.2], [-0.5, 0.9, 0.4]])\n",
                 "\n",
-                "print(s.x)"
+                "print(f\"s.x = \\n{s.x!s}\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The complexity of parsing through options at `setup` can be simplified using ad-hoc functions referred to as *factories*, declared as class methods by decorator `@classmethod`.\n",
-                "Note that the first argument of class methods is always `cls` (as opposed to `self` for traditional object methods), denoting the class itself.\n",
-                "Factories are special class method whose job is to create and return a new class instance (an object) from a specific set of arguments.\n",
+                "Factories are special class methods whose job is to create and return a new class instance (an object) from a specific set of arguments.\n",
                 "\n",
                 "Class methods are invoked with syntax `ClassName.method_name(...)`.\n",
                 "\n",
-                "In the next cell, we implement factory methods `from_data` and `from_file`, each with its own signature:\n"
+                "In the next cell, we implement factory methods `from_data` and `from_file`, each with its own signature.\n",
+                "Note that the first argument of a class method is always `cls`, denoting the class itself, as opposed to `self`, used in traditional object-bound methods.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "from cosapp.base import System\n",
                 "import numpy\n",
                 "\n",
+                "\n",
                 "class MySystem(System):\n",
                 "    def setup(self, n: int):\n",
                 "        self.add_property('n', int(n))\n",
                 "        self.add_inward('x', numpy.zeros((self.n, 3)))\n",
                 "\n",
                 "    @classmethod\n",
-                "    def from_data(cls, name: str, data) -> \"MySystem\":\n",
-                "        n = cls.check_shape(data)\n",
-                "        s = cls(name, n=n)  # newly created system\n",
-                "        s.x = numpy.array(data, dtype=float)\n",
+                "    def from_data(cls, name: str, data: numpy.ndarray) -> MySystem:\n",
+                "        \"\"\"Factory creating a new system from a numpy array.\"\"\"\n",
+                "        x = cls.reshape(data)\n",
+                "        s = cls(name, n=x.shape[0])  # newly created system\n",
+                "        s.x = numpy.asarray(data, dtype=float)\n",
                 "        return s\n",
                 "\n",
                 "    @classmethod\n",
-                "    def from_file(cls, name: str, filename) -> \"MySystem\":\n",
+                "    def from_file(cls, name: str, filename) -> MySystem:\n",
+                "        \"\"\"Factory creating a new system from data stored on file.\"\"\"\n",
                 "        data = numpy.load(filename)\n",
                 "        return cls.from_data(name, data)\n",
                 "\n",
                 "    @staticmethod\n",
-                "    def check_shape(data) -> int:\n",
-                "        \"\"\"Checks that `data` is a (N x 3) array-like object.\n",
-                "        If so, returns integer N. If not, raises `ValueError`.\n",
+                "    def reshape(data) -> numpy.ndarray:\n",
+                "        \"\"\"Checks that `data` can be reshaped into a (N x 3) array.\n",
+                "        If so, returns the reshaped array; otherwise, raises `ValueError`.\n",
                 "        \"\"\"\n",
-                "        shape = numpy.shape(data)\n",
-                "        ok = len(shape) == 2 and shape[1] == 3\n",
-                "        if not ok:\n",
-                "            raise ValueError(\"data must be a (N x 3) array-like object\")\n",
-                "        return shape[0]\n"
+                "        try:\n",
+                "            return numpy.reshape(data, (-1, 3))\n",
+                "        except ValueError:\n",
+                "            raise ValueError(\"data must be interpretable as a (N x 3) array\")\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s1 = MySystem('s1', n=4)  # usual way\n",
                 "\n",
                 "print(f\"{s1.n = }\", f\"s1.x =\\n{s1.x}\", sep=\"\\n\")\n",
                 "\n",
                 "# Create a system from existing data with `from_data`\n",
-                "s2 = MySystem.from_data('s2', [[0, 0.1, 0.2], [-0.5, 0.9, 0.4]])\n",
+                "s2 = MySystem.from_data('s2', [0, 0.1, 0.2, -0.5, 0.9, 0.4])\n",
                 "\n",
                 "print(\"\", f\"{s2.n = }\", f\"s2.x =\\n{s2.x}\", sep=\"\\n\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -559,15 +570,21 @@
                 "    )\n",
                 "else:\n",
                 "    print(f\"{s3.n = }\", f\"s3.x =\\n{s3.x}\", sep=\"\\n\")\n"
             ]
         }
     ],
     "metadata": {
+        "kernelspec": {
+            "display_name": "cosapp",
+            "language": "python",
+            "name": "python3"
+        },
         "language_info": {
-            "name": "python"
+            "name": "python",
+            "version": "3.9.16"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/Visitors.ipynb` & `cosapp-0.15.0/cosapp/tutorials/Visitors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/aa-SimpleCircuit.ipynb` & `cosapp-0.15.0/cosapp/tutorials/aa-SimpleCircuit.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9866468422543189%*

 * *Differences: {"'cells'": "{0: {'source': ['![CoSAppLogo](images/cosapp.svg) **CoSApp** examples\\n', '\\n', '# "*

 * *            "Simple circuit\\n', '\\n', 'Preliminary note:\\n', '\\n', 'This case is taken from "*

 * *            '[OpenMDAO](http://openmdao.org/twodocs/versions/latest/examples/circuit_analysis.html). '*

 * *            'OpenMDAO is an open-source computing platform for systems analysis and '*

 * *            'multidisciplinary optimization developed by the NASA. Its philosophy shares some of '*

 * *            'the goals wit […]*

```diff
@@ -2,22 +2,16 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "![CoSAppLogo](images/cosapp.svg) **CoSApp** examples:"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** examples\n",
+                "\n",
                 "# Simple circuit\n",
                 "\n",
                 "Preliminary note:\n",
                 "\n",
                 "This case is taken from [OpenMDAO](http://openmdao.org/twodocs/versions/latest/examples/circuit_analysis.html). OpenMDAO is an open-source computing platform for systems analysis and multidisciplinary optimization developed by the NASA. Its philosophy shares some of the goals with CoSApp. So this example is also an opportunity to compare both software.\n",
                 "\n",
                 "OpenMDAO is licensed under [Apache License](https://github.com/OpenMDAO/OpenMDAO/blob/master/LICENSE.txt).\n",
@@ -153,15 +147,22 @@
                 "        self.add_equation('sum_I_in == sum_I_out', name='current balance')\n",
                 "\n",
                 "    def compute(self):\n",
                 "        self.sum_I_in = sum(current.I for current in self.incoming_currents)\n",
                 "        self.sum_I_out = sum(current.I for current in self.outgoing_currents)\n",
                 "\n",
                 "    @classmethod\n",
-                "    def make(cls, name, parent, incoming: list[Dipole]=[], outgoing: list[Dipole]=[], pulling=None) -> Node:\n",
+                "    def make(\n",
+                "        cls,\n",
+                "        name: str,\n",
+                "        parent: System,\n",
+                "        incoming: list[Dipole]=[],\n",
+                "        outgoing: list[Dipole]=[],\n",
+                "        pulling=None,\n",
+                "    ) -> Node:\n",
                 "        \"\"\"Factory creating new node within `parent`, with\n",
                 "        appropriate connections with incoming and outgoing dipoles.\n",
                 "        \"\"\"\n",
                 "        node = cls(name, n_in=len(incoming), n_out=len(outgoing))\n",
                 "        parent.add_child(node, pulling=pulling)\n",
                 "        \n",
                 "        for dipole, current in zip(incoming, node.incoming_currents):\n",
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/exprampode_fmu.py` & `cosapp-0.15.0/cosapp/tutorials/exprampode_fmu.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/cosapp.svg` & `cosapp-0.15.0/cosapp/tutorials/images/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/design_circuit.svg` & `cosapp-0.15.0/cosapp/tutorials/images/design_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/drivers_1.svg` & `cosapp-0.15.0/cosapp/tutorials/images/drivers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/drivers_2.svg` & `cosapp-0.15.0/cosapp/tutorials/images/drivers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/drivers_3.svg` & `cosapp-0.15.0/cosapp/tutorials/images/drivers_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/drivers_4.svg` & `cosapp-0.15.0/cosapp/tutorials/images/drivers_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/drivers_5.svg` & `cosapp-0.15.0/cosapp/tutorials/images/drivers_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/drivers_nonlinear.svg` & `cosapp-0.15.0/cosapp/tutorials/images/drivers_nonlinear.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/experimental.svg` & `cosapp-0.15.0/cosapp/tutorials/images/experimental.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/in_progress.svg` & `cosapp-0.15.0/cosapp/tutorials/images/in_progress.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/ports_1.svg` & `cosapp-0.15.0/cosapp/tutorials/images/ports_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/ports_2.svg` & `cosapp-0.15.0/cosapp/tutorials/images/ports_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/ports_3.svg` & `cosapp-0.15.0/cosapp/tutorials/images/ports_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/simple_circuit.svg` & `cosapp-0.15.0/cosapp/tutorials/images/simple_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/systems_1.svg` & `cosapp-0.15.0/cosapp/tutorials/images/systems_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/systems_2.svg` & `cosapp-0.15.0/cosapp/tutorials/images/systems_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/systems_3.svg` & `cosapp-0.15.0/cosapp/tutorials/images/systems_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/systems_4.svg` & `cosapp-0.15.0/cosapp/tutorials/images/systems_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/systems_5.svg` & `cosapp-0.15.0/cosapp/tutorials/images/systems_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/tanks.svg` & `cosapp-0.15.0/cosapp/tutorials/images/tanks.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/triggers_1.svg` & `cosapp-0.15.0/cosapp/tutorials/images/triggers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/triggers_2.svg` & `cosapp-0.15.0/cosapp/tutorials/images/triggers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/validity.svg` & `cosapp-0.15.0/cosapp/tutorials/images/validity.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/images/visibility.svg` & `cosapp-0.15.0/cosapp/tutorials/images/visibility.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/multimode/BouncingBall.ipynb` & `cosapp-0.15.0/cosapp/tutorials/multimode/BouncingBall.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998464373464373%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(51, 'class BouncingBall(PointMassFreeFall):\\n'), (52, '    "*

 * *            '"""Extension of `PointMassFreeFall`, containing a rebound event\\n\'), (53, \'    and '*

 * *            'a rebound restitution coefficient.\\n\'), (54, \'    """\\n\'), (56, \'        '*

 * *            "super().setup()\\n')], delete: [56, 55, 54, 52, 51]}}}"}*

```diff
@@ -69,20 +69,20 @@
                 "        self.add_transient('v', der='a')\n",
                 "        self.add_transient('x', der='v')\n",
                 "\n",
                 "        self.g = np.r_[0, 0, -9.81]\n",
                 "        self.exec_order = ['friction', 'dynamics']\n",
                 "\n",
                 "\n",
-                "class BouncingBall(System):\n",
-                "    \"\"\"Bouncing point mass\"\"\"\n",
+                "class BouncingBall(PointMassFreeFall):\n",
+                "    \"\"\"Extension of `PointMassFreeFall`, containing a rebound event\n",
+                "    and a rebound restitution coefficient.\n",
+                "    \"\"\"\n",
                 "    def setup(self):\n",
-                "        self.add_child(PointMassFreeFall('point'), pulling=[\n",
-                "            'x', 'v', 'a', 'mass', 'cf', 'g',\n",
-                "        ])\n",
+                "        super().setup()\n",
                 "        self.add_event('rebound', trigger=\"x[2] <= 0\")\n",
                 "        self.add_inward('cr', 1.0, desc=\"Rebound restitution coefficient\", limits=(0, 1))\n",
                 "        self.add_outward_modevar(\"n_rebounds\", init=0, dtype=int)\n",
                 "\n",
                 "    def transition(self):\n",
                 "        if self.rebound.present:\n",
                 "            self.n_rebounds += 1\n",
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/multimode/MultimodeOde.ipynb` & `cosapp-0.15.0/cosapp/tutorials/multimode/MultimodeOde.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/multimode/NewtonPendulum.ipynb` & `cosapp-0.15.0/cosapp/tutorials/multimode/NewtonPendulum.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/optimization/BetzLimit.ipynb` & `cosapp-0.15.0/cosapp/tutorials/optimization/BetzLimit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/optimization/Sellar.ipynb` & `cosapp-0.15.0/cosapp/tutorials/optimization/Sellar.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/tutorials/quickstart.ipynb` & `cosapp-0.15.0/cosapp/tutorials/quickstart.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991859243697479%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '5 minutes?.. Challenge accepted!\\n'), (3, '\\n'), (4, "*

 * *            "'# Quickstart\\n'), (5, '\\n'), (6, '## CoSApp Overview\\n'), (7, '\\n'), (8, "*

 * *            '"<font color=\'orange\'>**CoSApp**</font> is a multidisciplinary oriented tool for '*

 * *            'the simulation and design of systems. Its goal is to provide a user-friendly and '*

 * *            'efficient environnement to build, exchange and solve physical models.\\n"), (9, '*

 * *            "'\\n'), (10, '##  […]*

```diff
@@ -5,22 +5,16 @@
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "![CoSAppLogo](images/cosapp.svg)\n",
                 "\n",
-                "5 minutes?.. Challenge accepted!"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "5 minutes?.. Challenge accepted!\n",
+                "\n",
                 "# Quickstart\n",
                 "\n",
                 "## CoSApp Overview\n",
                 "\n",
                 "<font color='orange'>**CoSApp**</font> is a multidisciplinary oriented tool for the simulation and design of systems. Its goal is to provide a user-friendly and efficient environnement to build, exchange and solve physical models.\n",
                 "\n",
                 "## Get started\n",
```

### Comparing `cosapp-0.14.1/cosapp/tutorials/time_solutions.py` & `cosapp-0.15.0/cosapp/tutorials/time_solutions.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/distributions/distribution.py` & `cosapp-0.15.0/cosapp/utils/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/distributions/normal.py` & `cosapp-0.15.0/cosapp/utils/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/distributions/tests/test_distribution.py` & `cosapp-0.15.0/cosapp/utils/distributions/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/distributions/tests/test_normal.py` & `cosapp-0.15.0/cosapp/utils/distributions/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/distributions/tests/test_triangular.py` & `cosapp-0.15.0/cosapp/utils/distributions/tests/test_triangular.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/distributions/tests/test_uniform.py` & `cosapp-0.15.0/cosapp/utils/distributions/tests/test_uniform.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/distributions/triangular.py` & `cosapp-0.15.0/cosapp/utils/distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/distributions/uniform.py` & `cosapp-0.15.0/cosapp/utils/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/find_variables.py` & `cosapp-0.15.0/cosapp/utils/find_variables.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fnmatch import fnmatchcase
-from typing import List, Any, Callable, Set, Union
+from typing import List, Any, Callable, Set, Dict, Union
 from collections.abc import Collection
 import inspect
 import itertools
 
 from cosapp.ports.port import BasePort, Port
 from cosapp.utils.naming import natural_varname, CommonPorts
 from cosapp.utils.helpers import check_arg
@@ -35,142 +35,198 @@
     return set(
         m[0] for m in inspect.getmembers(obj)
         if not m[0].startswith("_") and not callable(m[1])
     )
 
 
 def find_variables(
-    watched_object: "cosapp.systems.System",
+    system: "cosapp.systems.System",
     includes: SearchPattern,
     excludes: SearchPattern,
     advanced_filter: Callable[[Any], bool] = lambda any: True,
     inputs: bool = True,
     outputs: bool = True,
     include_const: bool = False,
-) -> List[str]:
-    """Generate the list of requested variables.
-
-    The variables are sorted in alphabetical order.
+) -> Dict[str, Any]:
+    """Generate the dictionary (name, value) of variables
+    whose names match inclusion and exclusion criteria.
 
     Parameters
     ----------
-    watched_object : cosapp.systems.System
-        Object that owns the variables searched
+    system : cosapp.systems.System
+        Object that owns the variables searched.
     includes : str or List[str]
-        Variables matching these patterns will be included
+        Variables matching these patterns will be included.
     excludes : str or List[str]
-        Variables matching these patterns will be excluded
+        Variables matching these patterns will be excluded.
     advanced_filter : Callable[[Any], bool]
-        Function taking the variable as input and returning an acceptance criteria (True if variable is valid)
+        Function taking the variable as input and returning an acceptance criteria (True if variable is valid).
     inputs : bool
-        Defines if input variables will be accepted or not
+        Defines if input variables will be accepted or not.
     outputs : bool
-        Defines if output variables will be accepted or not
+        Defines if output variables will be accepted or not.
     include_const : bool
-        Defines if read-only properties defined with `System.add_property` will be accepted or not
+        Defines if read-only properties defined with `System.add_property` will be accepted or not.
 
     Returns
     -------
-    List[str]
-        Variable names matching the includes/excludes patterns of the user in the watched object.
+    dict[str, Any]
+        Dictionary (name, value) of matches.
 
     .. note::
         Inward and outward variables will appear without the prefix `inwards.` or `outwards.`.
     """
     from cosapp.systems import System  # Local import to avoid recursion
-    check_arg(watched_object, 'watched_object', System)
+    check_arg(system, 'system', System)
 
     if not (inputs or outputs):
         # quick return, if possible
         return []
 
     includes = make_wishlist(includes)
     excludes = make_wishlist(excludes)
-    result = set()
+    result = dict()
 
     def is_valid(port: BasePort) -> bool:
         return isinstance(port, BasePort) and (
             (port.is_input and inputs) or
             (port.is_output and outputs)
         )
 
-    def find_matches(name: str, value: Any) -> Set[str]:
-        result = set()
+    def find_matches(name: str, value: Any) -> Dict[str, Any]:
+        matches = dict()
         if advanced_filter(value):
             for pattern in includes:
                 if fnmatchcase(name, pattern):
                     include = True
                     for pattern in excludes:
                         if fnmatchcase(name, pattern):
                             include = False
                             break
                     if include:
-                        result.add(name)
+                        matches[name] = value
                         break
-        return result
+        return matches
 
     ports = set()
 
-    for name, ref in watched_object.name2variable.items():
+    for name, ref in system.name2variable.items():
         # Save variable for non virtual port
         # Suppress duplicates INWARDS and OUTWARDS
         port = ref.mapping
         valid = (
             is_valid(port)
             and name == natural_varname(name)
         )
         if not valid:
             continue  # skip `name`
 
         ports.add(port)
-        result |= find_matches(name, watched_object[name])
+        result.update(find_matches(name, ref.value))
     
     # Find matches among port properties
     Port_cls_attr = get_attributes(Port)
 
     for port in ports:
         if not isinstance(port, Port):
             continue  # exclude `inwards` and `outwards` extensible ports
         port_properties = get_attributes(port) - Port_cls_attr - set(port._variables)
         port_name = port.full_name(trim_root=True)
         for name in port_properties:
-            result |= find_matches(f"{port_name}.{name}", getattr(port, name))
+            result.update(
+                find_matches(f"{port_name}.{name}", getattr(port, name))
+            )
 
     # Find matches among system properties
-    system_properties = find_system_properties(watched_object, include_const)
+    system_properties = find_system_properties(system, include_const)
     for name in system_properties:
         try:
             child, attr = name.rsplit('.', maxsplit=1)
         except ValueError:
-            owner, attr = watched_object, name
+            owner, attr = system, name
         else:
-            owner = watched_object[child]
-        result |= find_matches(name, getattr(owner, attr))
+            owner = system[child]
+        result.update(
+            find_matches(name, getattr(owner, attr))
+        )
 
-    return sorted(result)
+    return result
+
+
+def find_variable_names(
+    system: "cosapp.systems.System",
+    includes: SearchPattern,
+    excludes: SearchPattern,
+    advanced_filter: Callable[[Any], bool] = lambda any: True,
+    inputs: bool = True,
+    outputs: bool = True,
+    include_const: bool = False,
+) -> List[str]:
+    """Generate the list of requested variable names,
+    given inclusion and exclusion criteria.
+
+    Matching variable names are returned in alphabetical order.
+
+    Parameters
+    ----------
+    system : cosapp.systems.System
+        Object that owns the variables searched.
+    includes : str or List[str]
+        Variables matching these patterns will be included.
+    excludes : str or List[str]
+        Variables matching these patterns will be excluded.
+    advanced_filter : Callable[[Any], bool]
+        Function taking the variable as input and returning an acceptance criteria (True if variable is valid).
+    inputs : bool
+        Defines if input variables will be accepted or not.
+    outputs : bool
+        Defines if output variables will be accepted or not.
+    include_const : bool
+        Defines if read-only properties defined with `System.add_property` will be accepted or not.
+
+    Returns
+    -------
+    list[str]
+        Variable names in `system` matching the requested includes/excludes patterns.
+
+    .. note::
+        Inward and outward variables will appear without the prefix `inwards.` or `outwards.`.
+        This functions returns the sorted keys of the dictionary returned by `find_variables`.
+    """
+    return sorted(
+        find_variables(
+            system,
+            includes,
+            excludes,
+            advanced_filter,
+            inputs,
+            outputs,
+            include_const,
+        )
+    )
 
 
 def find_system_properties(system, include_const=False) -> Set[str]:
     """
     Returns system properties, defined either as class properties
     (with @property decorator), or with `System.add_property`.
     The latter are excluded if optional argument `include_const`
     is False (default).
 
     Parameters
     ----------
     - system [cosapp.systems.System]:
         System of interest
     - include_const [bool, optional]:
-        Defines if read-only properties defined with `System.add_property` will be accepted or not.
+        Defines if read-only properties defined with `System.add_property` will be accepted or not..
         Default: `False`.
 
     Returns
     -------
-    - Set[str]:
+    - set[str]:
         Set of property names.
     """
     from cosapp.systems import System  # Local import to avoid recursion
     check_arg(system, 'system', System)
 
     base_cls_attr = get_attributes(System)
     get_name = lambda obj: obj.name
```

### Comparing `cosapp-0.14.1/cosapp/utils/graph_analysis.py` & `cosapp-0.15.0/cosapp/utils/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/helpers.py` & `cosapp-0.15.0/cosapp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/json.py` & `cosapp-0.15.0/cosapp/utils/json.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/logging.py` & `cosapp-0.15.0/cosapp/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/naming.py` & `cosapp-0.15.0/cosapp/utils/naming.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/options_dictionary.py` & `cosapp-0.15.0/cosapp/utils/options_dictionary.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/parsing.py` & `cosapp-0.15.0/cosapp/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/pull_variables.py` & `cosapp-0.15.0/cosapp/utils/pull_variables.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/state_io.py` & `cosapp-0.15.0/cosapp/utils/state_io.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/__init__.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/base.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/base.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/kriging.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/kriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/multifi_cokriging.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/multifi_cokriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/nearest_neighbor.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/response_surface.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/response_surface.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/tests/test_kriging.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/tests/test_kriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/surrogate_models/tests/test_response_surface.py` & `cosapp-0.15.0/cosapp/utils/surrogate_models/tests/test_response_surface.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/testing.py` & `cosapp-0.15.0/cosapp/utils/testing.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp/utils/validate.py` & `cosapp-0.15.0/cosapp/utils/validate.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/cosapp.egg-info/PKG-INFO` & `cosapp-0.15.0/cosapp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosapp
-Version: 0.14.1
+Version: 0.15.0
 Summary: CoSApp, the Collaborative System Approach.
 Home-page: https://cosapp.readthedocs.io
 Author: CoSApp Development Team
 License: Apache-2.0
 Keywords: cosapp,system simulation,system design
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -55,14 +55,33 @@
 # Try it now!
 Run a Jupyter Lab instance with binder to try out CoSApp features through examples.
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cosapp%2Fcosapp/master?urlpath=lab/tree/docs/tutorials)
 
 # History
 
+## 0.15.0 (2023-07-20)
+
+### New features & API changes
+
+- Suppression of default `RunSingleCase` subdriver `runner` in `NonLinearSolver` drivers (MR [#239](https://gitlab.com/cosapp/cosapp/-/merge_requests/239)).
+- Enable target initialization in multi-point design problems (MR [#233](https://gitlab.com/cosapp/cosapp/-/merge_requests/233)).
+- New utility function `swap_system` to replace on the fly a subsystem by another `System` instance (MR [#238](https://gitlab.com/cosapp/cosapp/-/merge_requests/238)).
+
+### Bug fixes and code quality
+
+- Refactor driver `Optimizer` (MR [#240](https://gitlab.com/cosapp/cosapp/-/merge_requests/240)).
+- Various bug fixes (MRs [#234](https://gitlab.com/cosapp/cosapp/-/merge_requests/234), [#235](https://gitlab.com/cosapp/cosapp/-/merge_requests/235), [#241](https://gitlab.com/cosapp/cosapp/-/merge_requests/241)).
+
+### Documentation
+
+- New tutorial on `swap_system` (MR [#243](https://gitlab.com/cosapp/cosapp/-/merge_requests/243)).
+- General update of tutorials (MRs [#232](https://gitlab.com/cosapp/cosapp/-/merge_requests/232) and [#242](https://gitlab.com/cosapp/cosapp/-/merge_requests/242)).
+
+
 ## 0.14.1 (2023-06-08)
 
 ### Bug fixes and code quality
 
 - Fix incorrect output file name in `cosapp.tools.parse_module` (MR [#229](https://gitlab.com/cosapp/cosapp/-/merge_requests/229)).
 - Refactoring pass (MR [#230](https://gitlab.com/cosapp/cosapp/-/merge_requests/230)).
```

### Comparing `cosapp-0.14.1/cosapp.egg-info/SOURCES.txt` & `cosapp-0.15.0/cosapp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 cosapp/core/numerics/sobol_seq.py
 cosapp/core/signal/__init__.py
 cosapp/core/signal/signal.py
 cosapp/core/signal/slot.py
 cosapp/core/tests/__init__.py
 cosapp/core/tests/conftest.py
 cosapp/core/tests/test_AssignString.py
+cosapp/core/tests/test_CoSAppConfiguration.py
 cosapp/core/tests/test_ContextLocals.py
 cosapp/core/tests/test_EvalString.py
 cosapp/core/tests/test_Module.py
-cosapp/core/tests/test_coSAppConfiguration.py
 cosapp/core/tests/test_time.py
 cosapp/drivers/__init__.py
 cosapp/drivers/abstractsetofcases.py
 cosapp/drivers/abstractsolver.py
 cosapp/drivers/driver.py
 cosapp/drivers/influence.py
 cosapp/drivers/iterativecase.py
@@ -225,14 +225,15 @@
 cosapp/tutorials/11-DesignMethods.ipynb
 cosapp/tutorials/CustomConnectors.ipynb
 cosapp/tutorials/FMI.ipynb
 cosapp/tutorials/Guidelines.ipynb
 cosapp/tutorials/HybridSimulations.ipynb
 cosapp/tutorials/Logging.ipynb
 cosapp/tutorials/Optimization.ipynb
+cosapp/tutorials/SwapSystems.ipynb
 cosapp/tutorials/SystemSurrogates.ipynb
 cosapp/tutorials/SystemSurrogatesAdvanced.ipynb
 cosapp/tutorials/Targets.ipynb
 cosapp/tutorials/TimeDriver.ipynb
 cosapp/tutorials/TimeDriverAdvanced.ipynb
 cosapp/tutorials/TipsAndTricks.ipynb
 cosapp/tutorials/Visitors.ipynb
@@ -277,14 +278,15 @@
 cosapp/utils/json.py
 cosapp/utils/logging.py
 cosapp/utils/naming.py
 cosapp/utils/options_dictionary.py
 cosapp/utils/parsing.py
 cosapp/utils/pull_variables.py
 cosapp/utils/state_io.py
+cosapp/utils/swap_system.py
 cosapp/utils/testing.py
 cosapp/utils/validate.py
 cosapp/utils/distributions/__init__.py
 cosapp/utils/distributions/distribution.py
 cosapp/utils/distributions/normal.py
 cosapp/utils/distributions/triangular.py
 cosapp/utils/distributions/uniform.py
@@ -383,14 +385,15 @@
 docs/tutorials/11-DesignMethods.ipynb
 docs/tutorials/CustomConnectors.ipynb
 docs/tutorials/FMI.ipynb
 docs/tutorials/Guidelines.ipynb
 docs/tutorials/HybridSimulations.ipynb
 docs/tutorials/Logging.ipynb
 docs/tutorials/Optimization.ipynb
+docs/tutorials/SwapSystems.ipynb
 docs/tutorials/SystemSurrogates.ipynb
 docs/tutorials/SystemSurrogatesAdvanced.ipynb
 docs/tutorials/Targets.ipynb
 docs/tutorials/TimeDriver.ipynb
 docs/tutorials/TimeDriverAdvanced.ipynb
 docs/tutorials/TipsAndTricks.ipynb
 docs/tutorials/Visitors.ipynb
```

### Comparing `cosapp-0.14.1/docs/Makefile` & `cosapp-0.15.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/conf.py` & `cosapp-0.15.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/layout.html` & `cosapp-0.15.0/docs/cosapp_theme/layout.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/searchbox.html` & `cosapp-0.15.0/docs/cosapp_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/cosapp.css_t` & `cosapp-0.15.0/docs/cosapp_theme/static/cosapp.css_t`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/custom.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/font-awesome.min.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/font.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/font.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/highlight.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/highlight.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/kube.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/kube.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/kube.demo.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/kube.demo.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/kube.legenda.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/kube.legenda.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/kube.min.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/kube.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/css/master.css` & `cosapp-0.15.0/docs/cosapp_theme/static/css/master.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Black.woff` & `cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Black.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Bold.woff` & `cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-BoldItalic.woff` & `cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Italic.woff` & `cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Regular.woff` & `cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/font/Lato-Semibold.woff` & `cosapp-0.15.0/docs/cosapp_theme/static/font/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff` & `cosapp-0.15.0/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/img/cosapp.svg` & `cosapp-0.15.0/docs/cosapp_theme/static/img/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/js/jquery-2.1.4.min.js` & `cosapp-0.15.0/docs/cosapp_theme/static/js/jquery-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/js/kube.js` & `cosapp-0.15.0/docs/cosapp_theme/static/js/kube.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/js/kube.min.js` & `cosapp-0.15.0/docs/cosapp_theme/static/js/kube.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/js/tocbot.min.js` & `cosapp-0.15.0/docs/cosapp_theme/static/js/tocbot.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/static/sidebar.js_t` & `cosapp-0.15.0/docs/cosapp_theme/static/sidebar.js_t`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/cosapp_theme/theme.conf` & `cosapp-0.15.0/docs/cosapp_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/developer/installation_cases.rst` & `cosapp-0.15.0/docs/developer/installation_cases.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/developer/logger.rst` & `cosapp-0.15.0/docs/developer/logger.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/developer/project_structure.rst` & `cosapp-0.15.0/docs/developer/project_structure.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/developer/scenarii.rst` & `cosapp-0.15.0/docs/developer/scenarii.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/img/gitlab-cosapp-f4950f.svg` & `cosapp-0.15.0/docs/img/gitlab-cosapp-f4950f.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/img/website-docs-blue.svg` & `cosapp-0.15.0/docs/img/website-docs-blue.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/index.rst` & `cosapp-0.15.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/installation.rst` & `cosapp-0.15.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/make.bat` & `cosapp-0.15.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/nb_thumbnails/_images/verified.svg` & `cosapp-0.15.0/docs/nb_thumbnails/_images/verified.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/source/modules.rst` & `cosapp-0.15.0/docs/source/modules.rst`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
    cosapp.tools.trigger
    cosapp.tools.module_parser.parseModule
 
    cosapp.utils.distributions.distribution
    cosapp.utils.distributions.normal
    cosapp.utils.distributions.triangular
    cosapp.utils.distributions.uniform
+   cosapp.utils.swap_system
 
    cosapp.utils.context
    cosapp.utils.helpers
    cosapp.utils.json
    cosapp.utils.logging
    cosapp.utils.naming
    cosapp.utils.options_dictionary
```

### Comparing `cosapp-0.14.1/docs/tools/mermaid.py` & `cosapp-0.15.0/docs/tools/mermaid.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tools/mermaid_inheritance.py` & `cosapp-0.15.0/docs/tools/mermaid_inheritance.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/00-Introduction.ipynb` & `cosapp-0.15.0/docs/tutorials/00-Introduction.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994318181818183%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(8, '* [File Event Triggers](04-Triggers.ipynb)\\n'), (9, '* "*

 * *            "[Replacing a sub-system on the fly](SwapSystems.ipynb)')], delete: [8]}}}"}*

```diff
@@ -78,15 +78,16 @@
                 "\n",
                 "CoSApp comes with a couple of utility tools. The following notebooks demonstrate their usage:\n",
                 "\n",
                 "* [Recording data](10-Recorders.ipynb)\n",
                 "* [Simulation log](Logging.ipynb)\n",
                 "* [System surrogates](SystemSurrogates.ipynb)\n",
                 "* [Export to FMU](FMI.ipynb)\n",
-                "* [File Event Triggers](04-Triggers.ipynb)"
+                "* [File Event Triggers](04-Triggers.ipynb)\n",
+                "* [Replacing a sub-system on the fly](SwapSystems.ipynb)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Tips & Tricks\n",
```

### Comparing `cosapp-0.14.1/docs/tutorials/01-Systems.ipynb` & `cosapp-0.15.0/docs/tutorials/01-Systems.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/02-Ports.ipynb` & `cosapp-0.15.0/docs/tutorials/02-Ports.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/03-Drivers.ipynb` & `cosapp-0.15.0/docs/tutorials/03-Drivers.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9828087843775848%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 4: "*

 * *            "{'attachments': OrderedDict()}, 5: {'attachments': OrderedDict()}, 7: {'attachments': "*

 * *            "OrderedDict()}, 8: {'attachments': OrderedDict()}, 11: {'attachments': "*

 * *            "OrderedDict()}, 14: {'attachments': OrderedDict()}, 16: {'attachments': "*

 * *            "OrderedDict()}, 17: {'source': {insert: [(2, '`RunSingleCase` sets its owner system "*

 * *            'in a given state, and executes all su […]*

```diff
@@ -1,19 +1,21 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials:"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Drivers\n",
                 "\n",
                 "## What is a `Driver`?!\n",
                 "\n",
@@ -58,21 +60,23 @@
                 "from cosapp.drivers import RunOnce\n",
                 "\n",
                 "m = MultiplySystem('mult')\n",
                 "run = m.add_driver(RunOnce('run'))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 " ![Driver in system](images/drivers_1.svg)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Implementation\n",
                 "\n",
                 "Every `System` (including sub-systems) may have one or multiple `Driver` objects. They are stored in the `drivers` attribute.\n",
                 "By default, no `Driver` is attached to a `System`.\n",
@@ -95,28 +99,30 @@
                 "m.p_in.x = 15.\n",
                 "m.run_drivers()\n",
                 "\n",
                 "print(f\"{m.p_out.x = }\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Driver chains and subdrivers\n",
                 "\n",
                 "If several drivers are attached to a system, `run_drivers` will execute them in turn, as a sequence of drivers.\n",
                 "Furthermore, like a `System`, each individual `Driver` may have children, which also inherit from base class `Driver`. Nested drivers are created with method `add_child` of class `Driver`; they are stored in attribute `children` of the parent driver.\n",
                 "\n",
                 "By construction, a `System` can have as many levels of drivers as required.\n",
                 "\n",
                 "Driver chains and nested drivers thus allow users to define complex simulation scenarios, such as workflows, multi-point design, designs of experiment, optimization, *etc.*\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "![drivers](images/drivers_2.svg)\n"
             ]
         },
         {
@@ -139,14 +145,15 @@
             "source": [
                 "subrun = run.add_child(RunOnce('subrun'))  # add a sub-driver 'subrun'\n",
                 "\n",
                 "print(f\"{run.children = }\", f\"{subrun.children = }\", sep=\"\\n\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Available Drivers\n",
                 "\n",
                 "**CoSApp** comes with a set of drivers to help users build their simulations.\n",
                 "\n",
@@ -211,14 +218,15 @@
                 "    f\"{m.p_out.x = }\",\n",
                 "    f\"residues: {list(m.residues.values())}\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### NonLinearSolver\n",
                 "\n",
                 "This `Driver` determines the parameters of your `System` declared as unknowns that satisfy its equations. It resolves the mathematical problem between free parameters and residues of its child drivers.\n",
                 "\n",
@@ -263,50 +271,47 @@
                 "    f\"{m.p_out.x = }\",\n",
                 "    f\"residues: {list(solver.problem.residues.values())}\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Resolution method\n",
                 "\n",
                 "Several resolution methods are available, through option `method`, of type `NonLinearMethods`, contained in module `cosapp.drivers`.\n",
                 "Possible choices are:\n",
                 "\n",
                 "- `NonLinearMethods.NR` (default, recommended): custom implementation of Newton-Raphson algorithm, tailored for CoSApp systems.\n",
                 "- `NonLinearMethods.POWELL`: Powell hybrid method (encapsulation of `scipy.optimize.root`).\n",
                 "- `NonLinearMethods.BROYDEN_GOOD`: Broyden's \"good\" method (encapsulation of `scipy.optimize.root`).\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### RunSingleCase\n",
                 "\n",
-                "`NonLinearSolver` is primarily designed to solve [multi-point problems](./08-Multipoints-Design.ipynb), where several [RunSingleCase](#RunSingleCase) drivers are declared as direct sub-drivers of the solver.\n",
-                "By default, a `NonLinearSolver` driver comes with one [RunSingleCase](#RunSingleCase) child, called *runner*. \n",
+                "`RunSingleCase` sets its owner system in a given state, and executes all subsystem drivers by recursively calling the `compute()` method throughout the owner system tree.\n",
                 "\n",
-                "![scipysolver](images/drivers_nonlinear.svg)\n",
-                "\n",
-                "`RunSingleCase` executes all subsystem drivers by recursively calling the `compute()` method of the top system and each of its children.\n",
-                "\n",
-                "This `Driver` does not contain a solver per se, but is helpfull to set boundary conditions, initial values, and define additional unknowns and/or equations.\n",
-                "It is primarily meant to be used as an operating point of a [NonLinearSolver](#NonLinearSolver) driver.\n",
+                "This driver does not contain a solver *per se*, but is helpfull to set boundary conditions, initial values, and define additional unknowns and/or equations.\n",
+                "It is primarily meant to be used as an operating point of a [NonLinearSolver](#NonLinearSolver) driver, to solve [multi-point problems](./08-Multipoints-Design.ipynb).\n",
                 "Therefore, `RunSingleCase` drivers are usually created as sub-drivers of `NonLinearSolver`, and are seldom directly attached to a system.\n",
                 "\n",
                 "The state of the owner `System` can be changed with two methods:\n",
                 "\n",
                 "- `set_values` will impose the value of prescribed input variables, as boundary conditions;\n",
                 "- `set_init` will change the initial value of iteratives before resolving the case.\n",
                 "\n",
-                "Both methods take as argument a dictionary of the kind `{varname: value, ...}`, where `varname` is the name of an input variable *in the context of the driver owner*.\n",
+                "Both methods take as argument a dictionary of the kind `{varname: value, ...}`, where `varname` is the name of an input variable *in the context of the owner system*.\n",
                 "For example, if the driver is attached to a system `head` possessing a child named `sub` and an inward `x`, `{'sub.k': 0.0, 'x': 0.1}` will affect variables `head.sub.k` and `head.x`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -334,21 +339,22 @@
                 "    f\"{m.p_out.x = }\",\n",
                 "    f\"residues: {list(m.residues.values())}\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Another important ability of this driver is the addition of unknowns and equations to the mathematical system.\n",
                 "There are two kinds of problems for a `RunSingleCase` driver:\n",
                 "\n",
-                "- **Design problems**: They are associated with design variables that are frozen in the final product; e.g. the diameter of a pipe. Design unknowns are uniquely defined, and shared between all design points, when several `RunSingleCase` drivers are present (see tutorial on [multi-point design](08-Multipoints-Design.ipynb)).\n",
+                "- **Design problems**: They are associated with design variables that are frozen in the final product (such as a geometrical parameter, *e.g.*). Design unknowns are uniquely defined, and shared between all design points, when several `RunSingleCase` drivers are present (see tutorial on [multi-point design](08-Multipoints-Design.ipynb)).\n",
                 "- **Local off-design problems**: They correspond to constraints imposed at the design point only. Local `RunSingleCase` unknowns will usually assume different values at different design points.\n",
                 "\n",
                 "Design and off-design problems are stored in attributes `design` and `offdesign`, respectively.\n",
                 "Unknowns and equations are added with methods `add_unknown` and `add_equation`:\n",
                 "\n",
                 "```python\n",
                 "case.design  \\\n",
@@ -395,14 +401,15 @@
                 "    f\"{m.p_in.x = }\",\n",
                 "    f\"{m.p_out.x = }\",\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Design methods are defined at system level, and can be activated on demand in a simulation (more info in the [Design Method tutorial](./11-DesignMethods.ipynb))."
             ]
         },
         {
@@ -458,14 +465,15 @@
                 "    \"Mathematical problem:\",\n",
                 "    solver.problem,\n",
                 "    sep=\"\\n\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "`RunSingleCase` drivers may also be used to simulate a life cycle made of states. On next example, a design point is followed by two off-design operating points. \n",
                 "\n",
                 "![metadriver](images/drivers_5.svg)"
             ]
@@ -489,14 +497,15 @@
                 "print(f\"Mathematical problem:\\n{solver.problem}\\n\")\n",
                 "\n",
                 "df = solver.recorder.export_data()  # export recorded data as a pandas DataFrame\n",
                 "df"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "For advanced design methods tutorial and strategy to create a \"design model\" from a \"simulation model\", we recommend the tutorial on [Design Methods](./11-DesignMethods.ipynb).\n",
                 "\n",
                 "**Congrats!** You are now ready to launch computation on your `System` with **CoSApp**!"
             ]
```

### Comparing `cosapp-0.14.1/docs/tutorials/04-Triggers.ipynb` & `cosapp-0.15.0/docs/tutorials/04-Triggers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/05-Validation.ipynb` & `cosapp-0.15.0/docs/tutorials/05-Validation.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/06-Visibility.ipynb` & `cosapp-0.15.0/docs/tutorials/06-Visibility.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/07-Metamodels.ipynb` & `cosapp-0.15.0/docs/tutorials/07-Metamodels.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/08-Multipoints-Design.ipynb` & `cosapp-0.15.0/docs/tutorials/08-Multipoints-Design.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9655500886524823%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 2: "*

 * *            "{'attachments': OrderedDict()}, 3: {'attachments': OrderedDict()}, 4: {'attachments': "*

 * *            "OrderedDict()}, 5: {'source': {insert: [(76, '    def make(\\n'), (77, '        "*

 * *            "cls,\\n'), (78, '        name: str,\\n'), (79, '        parent: System,\\n'), (80, "*

 * *            "'        incoming: list[Dipole]=[],\\n'), (81, '        outgoing: "*

 * *            "list[Dipole]=[],\\n'), (82, '       […]*

```diff
@@ -1,19 +1,21 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Multi-point design"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Multi-point design\n",
                 "\n",
                 "Up to now, systems have been solved in their up-and-running state, that is all inputs are set, and we want to obtain the state of the system for a given set of boundary conditions.\n",
                 "\n",
@@ -96,14 +98,15 @@
                 "* For a `RunSingleCase` design point *case*, `case.add_unknown(...)` (respectively `add_equation`, `extend`) is a shortcut to `case.offdesign.add_unknown(...)`.\n",
                 "* Fixing a parameter using `case.set_values({'x': '0.123'})` is mathematically equivalent to the trivial constaint `case.add_unknown('x').add_equation('x == 0.123')`. Thus, the local off-design problem can be viewed as an extension of `set_values` for non-trivial, nonlinear constraints.\n",
                 "* In single-point design, solver and case problems (either off-design or design) are interchangeable. However, it is good practice to follow multi-point design rules, for the sake of consistency.\n",
                 "* Equations declared at solver level are satisfied independently on each `RunSingleCase` subdriver. Thus, in multi-point problems, be aware that a single solver equation will eventually result in several equations in the assembled mathematical problem."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Example\n",
                 "## Case description\n",
                 "\n",
                 "The simple circuit test case having a constant intensity source will be used here. In addition to the off-design resolution driving the potential `V` at nodes to balance current fluxes, we seek to determine the value of two resistances from two different operating points.\n",
@@ -113,19 +116,21 @@
                 "| Operating point | Boundary conditions | Design variable | Design equation |\n",
                 "|---|---|---|---|\n",
                 "| Point 1 | $I_{source} = 0.08$ A | `R2.R` | `n2.V == 8 V` |\n",
                 "| Point 2 | $I_{source} = 0.15$ A | `R1.R` | `n1.V == 50 V` |"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": []
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Building the circuit\n",
                 "\n",
                 "The circuit is built as an assembly of elementary models. The default case is then solved to initialize all variables."
             ]
@@ -208,15 +213,22 @@
                 "        self.add_equation('sum_I_in == sum_I_out', name='current balance')\n",
                 "\n",
                 "    def compute(self):\n",
                 "        self.sum_I_in = sum(current.I for current in self.incoming_currents)\n",
                 "        self.sum_I_out = sum(current.I for current in self.outgoing_currents)\n",
                 "\n",
                 "    @classmethod\n",
-                "    def make(cls, name, parent, incoming: list[Dipole]=[], outgoing: list[Dipole]=[], pulling=None) -> Node:\n",
+                "    def make(\n",
+                "        cls,\n",
+                "        name: str,\n",
+                "        parent: System,\n",
+                "        incoming: list[Dipole]=[],\n",
+                "        outgoing: list[Dipole]=[],\n",
+                "        pulling=None,\n",
+                "    ) -> Node:\n",
                 "        \"\"\"Factory creating new node within `parent`, with\n",
                 "        appropriate connections with incoming and outgoing dipoles.\n",
                 "        \"\"\"\n",
                 "        node = cls(name, n_in=len(incoming), n_out=len(outgoing))\n",
                 "        parent.add_child(node, pulling=pulling)\n",
                 "        \n",
                 "        for dipole, current in zip(incoming, node.incoming_currents):\n",
@@ -329,14 +341,15 @@
             "source": [
                 "from cosapp.utils import get_state, set_state\n",
                 "\n",
                 "initial_state = get_state(model)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Defining the design case\n",
                 "\n",
                 "After purging all drivers, the design case can be defined. First, a numerical solver is attached to the head system. Then, for each design point, a sub-driver `RunSingleCase` is added to the solver."
             ]
@@ -431,17 +444,15 @@
                 "from cosapp.drivers import NonLinearSolver, RunSingleCase\n",
                 "from cosapp.recorders import DataFrameRecorder\n",
                 "\n",
                 "# Create and initialize new model\n",
                 "model = AssembledModel('model')\n",
                 "set_state(model, initial_state)\n",
                 "\n",
-                "# Clear all previously defined drivers and add solver\n",
-                "model.drivers.clear()\n",
-                "set_state(model, initial_state)\n",
+                "# Add solver\n",
                 "solver = model.add_driver(NonLinearSolver('solver'))\n",
                 "\n",
                 "# Define design unknwowns.\n",
                 "# A maximum relative step between iterations is requested,\n",
                 "# to stabilize the resolution.\n",
                 "solver.add_unknown(['circuit.R1.R', 'circuit.R2.R'], max_rel_step=0.5)\n",
                 "\n",
@@ -495,19 +506,139 @@
             "source": [
                 "data = solver.recorder.export_data()\n",
                 "data = data.drop(['Section', 'Status', 'Error code'], axis=1)\n",
                 "data"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Multi-point design problems involving targets\n",
+                "\n",
+                "Targets offer a convenient way to declare a dynamically changeable target value on a variable (either input or output), rather than imposing a hard-coded right-hand-side value, as in:\n",
+                "\n",
+                "```python\n",
+                "point1.add_equation('circuit.n2.V == 8')\n",
+                "```\n",
+                "\n",
+                "Further detail on targets may be found in a dedicated [tutorial](Targets.ipynb).\n",
+                "\n",
+                "In single-point design problems, target values can be redefined by simply reassigning the targetted variables prior to solver execution (see [tutorial](Targets.ipynb)).\n",
+                "In multi-point design problems, though, a variable may be assigned different target values in different design points.\n",
+                "In the last circuit design problem, for example, potential `circuit.n2.V` is required to be 8 V in `point1`, and 5 V in `point2`.\n",
+                "Setting point-wise targets can be achieved with method `set_init`.\n",
+                "\n",
+                "Let us reformulate the same design problem, using targets:"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "from cosapp.drivers import NonLinearSolver, RunSingleCase\n",
+                "from cosapp.recorders import DataFrameRecorder\n",
+                "\n",
+                "# Create and initialize new model\n",
+                "model = AssembledModel('model')\n",
+                "set_state(model, initial_state)\n",
+                "\n",
+                "# Add solver\n",
+                "solver = model.add_driver(NonLinearSolver('solver'))\n",
+                "\n",
+                "# Define design unknwowns.\n",
+                "solver.add_unknown(['circuit.R1.R', 'circuit.R2.R'], max_rel_step=0.5)\n",
+                "\n",
+                "# Set a target on node 2 voltage (will pertain to all design points)\n",
+                "solver.add_target('circuit.n2.V')\n",
+                "\n",
+                "solver.add_recorder(\n",
+                "    DataFrameRecorder(\n",
+                "        includes = ['*.n?.V', '*R', 'source.I'],\n",
+                "        excludes = 'ground.*',\n",
+                "    )\n",
+                ")\n",
+                "\n",
+                "# Define design point #1\n",
+                "point1 = solver.add_child(RunSingleCase('point1'))\n",
+                "\n",
+                "point1.set_values({\n",
+                "    'source.I': 0.08, \n",
+                "    'ground.V': 0,\n",
+                "    'circuit.R3.R': 0.5e3,\n",
+                "})\n",
+                "\n",
+                "# Define design point #2\n",
+                "point2 = solver.add_child(RunSingleCase('point2')) \n",
+                "\n",
+                "point2.add_unknown('circuit.R3.R')  # local, off-design unknown\n",
+                "point2.add_target('circuit.n1.V')   # local target on node 1 voltage\n",
+                "\n",
+                "point2.set_values({\n",
+                "    'source.I': 0.15,\n",
+                "    'ground.V': 0,\n",
+                "})"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Once the problem is defined, we can specify point-dependent target values using method `set_init`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "point1.set_init({\n",
+                "    'circuit.n2.V': 8.0,\n",
+                "})\n",
+                "point2.set_init({\n",
+                "    'circuit.n1.V': 50.0,\n",
+                "    'circuit.n2.V': 5.0,\n",
+                "})\n",
+                "\n",
+                "model.run_drivers()\n",
+                "\n",
+                "solver.problem"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Target values can now be redefined interactively, by simply changing initial values:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "point1.set_init({\n",
+                "    'circuit.n2.V': 12.0,\n",
+                "})\n",
+                "point2.set_init({\n",
+                "    'circuit.n1.V': 62.0,\n",
+                "    'circuit.n2.V': 7.5,\n",
+                "})\n",
+                "\n",
+                "model.run_drivers()\n",
+                "\n",
+                "solver.problem"
+            ]
         }
     ],
     "metadata": {
         "hide_input": false,
         "kernelspec": {
             "display_name": "cosapp",
             "language": "python",
```

### Comparing `cosapp-0.14.1/docs/tutorials/09-MonteCarlo.ipynb` & `cosapp-0.15.0/docs/tutorials/09-MonteCarlo.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/10-Recorders.ipynb` & `cosapp-0.15.0/docs/tutorials/10-Recorders.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/11-DesignMethods.ipynb` & `cosapp-0.15.0/docs/tutorials/11-DesignMethods.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982744815097756%*

 * *Differences: {"'cells'": '{10: {\'source\': {insert: [(14, \'        """Compute `x` such that `y == 0`.\\n\')], '*

 * *            'delete: [14]}}, 12: {\'source\': {insert: [(5, \'\\n\'), (14, \'    f"Converged in '*

 * *            '{solver.results.fres_calls} iterations",\\n\')]}}, 14: {\'source\': {insert: [(3, '*

 * *            '\'\\n\'), (12, \'    f"Converged in {solver.results.fres_calls} '*

 * *            'iterations",\\n\')]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -219,15 +219,15 @@
                 "        self.add_inward('x', 1.0)\n",
                 "        self.add_outward('y', 0.0)\n",
                 "\n",
                 "    def compute(self):\n",
                 "        self.y = math.sin(self.x**2 - 2)\n",
                 "    \n",
                 "    def design_x(self, **options):\n",
-                "        \"\"\"Design method for `x`.\n",
+                "        \"\"\"Compute `x` such that `y == 0`.\n",
                 "        Additional options apply to unknown `x`.\n",
                 "        \"\"\"\n",
                 "        problem = self.new_problem()\n",
                 "        problem.add_unknown('x', **options)\n",
                 "        problem.add_equation('y == 0')\n",
                 "        return problem\n"
             ]
@@ -246,22 +246,24 @@
             "outputs": [],
             "source": [
                 "from cosapp.drivers import NonLinearSolver\n",
                 "\n",
                 "s = SystemWithDynamicDesignMethod('s')\n",
                 "\n",
                 "solver = s.add_driver(NonLinearSolver('solver'))\n",
+                "\n",
                 "solver.extend(s.design_x())\n",
                 "\n",
                 "s.x = 0.7  # initial value\n",
                 "s.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{s.x = }\",\n",
                 "    f\"{s.y = }\",\n",
+                "    f\"Converged in {solver.results.fres_calls} iterations\",\n",
                 "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -274,22 +276,24 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = SystemWithDynamicDesignMethod('s')\n",
                 "\n",
                 "solver = s.add_driver(NonLinearSolver('solver'))\n",
+                "\n",
                 "solver.extend(s.design_x(max_abs_step=0.1))\n",
                 "\n",
                 "s.x = 0.7  # initial value\n",
                 "s.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{s.x = }\",\n",
                 "    f\"{s.y = }\",\n",
+                "    f\"Converged in {solver.results.fres_calls} iterations\",\n",
                 "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -327,15 +331,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.10.12"
         },
         "vscode": {
             "interpreter": {
                 "hash": "03d8647662c9fbe9220ebb6c4a5dd3c1d557fb5efab079901b8383e5f052f0cc"
             }
         }
     },
```

### Comparing `cosapp-0.14.1/docs/tutorials/CustomConnectors.ipynb` & `cosapp-0.15.0/docs/tutorials/CustomConnectors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/FMI.ipynb` & `cosapp-0.15.0/docs/tutorials/FMI.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/Guidelines.ipynb` & `cosapp-0.15.0/docs/tutorials/Guidelines.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/HybridSimulations.ipynb` & `cosapp-0.15.0/docs/tutorials/HybridSimulations.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761436480186481%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '![CoSAppLogo](images/cosapp.svg) **CoSApp** "*

 * *            "tutorials\\n'), (1, '\\n')]}}, 1: {'source': {insert: [(32, '* `<=`: expression `lhs "*

 * *            '- rhs` goes from positive to negative, meaning `lhs` becomes smaller than '*

 * *            "`rhs`;\\n'), (33, '* `>=`: expression `lhs - rhs` goes from negative to positive, "*

 * *            "meaning `lhs` becomes greater than `rhs`;\\n'), (50, 'Alternatively, events may be "*

 * *            'triggered by other events, […]*

```diff
@@ -1,20 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "![CoSAppLogo](images/cosapp.svg)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials\n",
+                "\n",
                 "# Simulations with discrete-time events\n",
                 "\n",
                 "Dynamic systems involving time derivatives can be solved using a time driver (see tutorial on [time simulations](TimeDriver.ipynb)).\n",
                 "Such simulations are referred to as *continuous time* simulations, as all quantities are expected to vary continuously with time.\n",
                 "\n",
                 "Discontinuities, however, can be introduced with the occurrence of **events**, defined within a system."
             ]
@@ -51,16 +46,16 @@
                 "Even though `\"lhs <op> rhs\"` corresponds to a Boolean expression, the event activation will *not* be triggered by the Boolean value.\n",
                 "Instead, time drivers will check for sign changes of `lhs - rhs` at each integration time step.\n",
                 "Since lhs and rhs are assumed to be continuous expressions in time, a sign change of their difference guaranties that there exists a time when lhs equals rhs.\n",
                 "This time value, determined numerically by solving a root-finding problem, will be regarded as the occurrence time of the event.\n",
                 "\n",
                 "Strict and non-strict inequalities are treated identically, so the actual discriminating cases are `==`, `<=`, and `>=`:\n",
                 "\n",
-                "* `<=`: expression `lhs - rhs` goes from positive to negative, meaning that `lhs` becomes smaller that `rhs`;\n",
-                "* `>=`: expression `lhs - rhs` goes from negative to positive, meaning that `lhs` becomes greater that `rhs`;\n",
+                "* `<=`: expression `lhs - rhs` goes from positive to negative, meaning `lhs` becomes smaller than `rhs`;\n",
+                "* `>=`: expression `lhs - rhs` goes from negative to positive, meaning `lhs` becomes greater than `rhs`;\n",
                 "* `==`: expression `lhs - rhs` simply changes sign.\n",
                 "\n",
                 "These distinctions allow one to define directional events (different events occur when *a* exceeds *b*, and when *b* exceeds *a*), as well as one-way events.\n",
                 "For example,\n",
                 "```python\n",
                 "class BreakableSystem(System):\n",
                 "    def setup(self):\n",
@@ -69,21 +64,36 @@
                 "        self.add_event('failure', trigger=\"x > x_max\")\n",
                 "```\n",
                 "indicates that if `failure` ever occurs (in which case we expect the system will change, as we will see later), there is no going back, even is `x` later returns below `x_max`.\n",
                 "\n",
                 "### Primitive and derived events\n",
                 "\n",
                 "Events triggered by a zero-crossing expression, as discussed in previous section, are said to be *primitive*, as they are self-determined.\n",
-                "Alternatively, events may be triggered by other events, in which case they are referred to as *derived events*.\n",
+                "Alternatively, events may be triggered by other events, in which case they are referred to as *secondary*, or *derived* events.\n",
                 "\n",
                 "Derived events can be either:\n",
                 "\n",
-                "* Synchronized events, simply triggered by the occurrence of another event.\n",
-                "* Filtered events, triggered by the occurrence of a distinct event *and* an additional condition, given as an evaluable Boolean expression. The syntax is `primary.filter(<condition>)`.\n",
-                "* Merged events, triggered by the occurrence of one among a list of events. Syntax is `Event.merge(event1, event2, ...)`, where `Event` is imported from module `cosapp.multimode`.\n"
+                "* **Synchronized events**, simply triggered by the occurrence of another event:\n",
+                "\n",
+                "  ```python\n",
+                "  event.trigger = other_event\n",
+                "  ```\n",
+                "\n",
+                "* **Filtered events**, triggered by the occurrence of a distinct event *and* an additional condition, given as an evaluable Boolean expression. Syntax is:\n",
+                "\n",
+                "  ```python\n",
+                "  event = other_event.filter(<condition>)\n",
+                "  ```\n",
+                "\n",
+                "* **Merged events**, triggered by the occurrence of one among a list of events. Syntax is:\n",
+                "  ```python\n",
+                "  from cosapp.multimode import Event\n",
+                "\n",
+                "  event = Event.merge(event1, event2, ...)\n",
+                "  ```\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -293,19 +303,14 @@
             "source": [
                 "## Examples\n",
                 "\n",
                 "* [Multimode ODE](multimode/MultimodeOde.ipynb)\n",
                 "* [Newton Pendulum](multimode/NewtonPendulum.ipynb)\n",
                 "* [Bouncing Ball](multimode/BouncingBall.ipynb)"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `cosapp-0.14.1/docs/tutorials/Logging.ipynb` & `cosapp-0.15.0/docs/tutorials/Logging.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/Optimization.ipynb` & `cosapp-0.15.0/docs/tutorials/Optimization.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/SystemSurrogates.ipynb` & `cosapp-0.15.0/docs/tutorials/SystemSurrogates.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/SystemSurrogatesAdvanced.ipynb` & `cosapp-0.15.0/docs/tutorials/SystemSurrogatesAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/Targets.ipynb` & `cosapp-0.15.0/docs/tutorials/Targets.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.967977791470295%*

 * *Differences: {"'cells'": "{0: {'source': ['![CoSAppLogo](images/cosapp.svg) **CoSApp** examples\\n', '\\n', '# "*

 * *            "Setting targets on output variables\\n', '\\n', 'CoSApp systems declare a directional "*

 * *            "interface, and transform inputs into outputs.\\n', 'It is good practice to design "*

 * *            'systems such that their inputs and outputs correspond to the "normal", direct '*

 * *            'behaviour of the system, without presuming how it will be used in a more complex '*

 * *            "assembly, or […]*

```diff
@@ -1,28 +1,24 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "![CoSAppLogo](images/cosapp.svg) **CoSApp** examples:"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# Settings targets on output values\n",
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** examples\n",
+                "\n",
+                "# Setting targets on output variables\n",
                 "\n",
                 "CoSApp systems declare a directional interface, and transform inputs into outputs.\n",
                 "It is good practice to design systems such that their inputs and outputs correspond to the \"normal\", direct behaviour of the system, without presuming how it will be used in a more complex assembly, or what users will want to do with it.\n",
                 "\n",
-                "As it happens, it is very common to use a given system in a reverse way, when one wishes certain outputs to reach a target value.\n",
+                "As it happens, it is very common to use a given system in a reverse way, when one wishes certain outputs to reach target values.\n",
                 "\n",
                 "The first obvious way to achieve that is to setup a nonlinear problem, whereby an input is sought to satisfy an equation of the kind \"target_output == target_value\"."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -56,19 +52,20 @@
                 "\n",
                 "f.a = 2.0\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Displaying attribute `solver.problem` reveals the mathematical problem solved by the driver:"
             ]
         },
         {
@@ -77,23 +74,24 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "solver.problem"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Set target value dynamically\n",
                 "\n",
                 "In the previous example, the target value for `f.y` is hard-coded as the right-hand side of the design equation.\n",
-                "Changing this value requires the setup of a new mathematical problem, with a new equation.\n",
+                "Changing this value requires the setup of a new mathematical problem, with a new hard-coded equation.\n",
                 "\n",
-                "An alternative way is to this procedure is the use of method `add_target`:"
+                "Alternatively, method `add_target` offers a convenient way is to set targets on variables:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -103,24 +101,26 @@
                 "f = SimpleFunction('f')\n",
                 "\n",
                 "solver = f.add_driver(NonLinearSolver('solver'))\n",
                 "solver.add_unknown('x').add_target('y')\n",
                 "\n",
                 "f.a = 2.0\n",
                 "f.y = 0.0   # set target value by setting output variable\n",
+                "\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Job done!\n",
                 "Looking at attribute `problem` shows that the actual mathematical problem has not changed:"
             ]
         },
@@ -130,18 +130,19 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "solver.problem"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The difference, however, is that the right-hand side of the equation is now dynamically set to the current value of `f.y` before each solver execution.\n",
+                "The difference, however, is that the right-hand side of the equation is now dynamically set to the current value of `f.y`, before each solver execution.\n",
                 "Therefore, we can now update the target value interactively, by simply assigning a new value to `f.y`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -150,32 +151,112 @@
                 "f.y = -0.5  # update target value dynamically\n",
                 "\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As can be seen after each computation, `f.y` only reaches the targetted value *within solver tolerance*.\n",
                 "Indeed, if `add_target` offers a convenient way of defining target values, one must keep in mind that `f.y` remains an output, whose value is strictly determined by the actual inputs of `f`.\n",
                 "\n",
                 "As a consequence, it is up to users to control the value of targetted variables *before each solver execution*."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "Controlling more strictly target values, if necessary, can be achieved by defining initial values in `RunSingleCase` sub-driver(s)."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from cosapp.drivers import NonLinearSolver, RunSingleCase\n",
+                "\n",
+                "f = SimpleFunction('f')\n",
+                "\n",
+                "solver = f.add_driver(NonLinearSolver('solver'))\n",
+                "solver.add_unknown('x').add_target('y')\n",
+                "\n",
+                "case = solver.add_child(RunSingleCase('case'))\n",
+                "case.set_init({\n",
+                "    'y': 0.5,  # will be used as equation rhs\n",
+                "})\n",
+                "\n",
+                "f.a = 2.0\n",
+                "f.x = 1.0\n",
+                "f.y = 0.0\n",
+                "\n",
+                "f.run_drivers()\n",
+                "\n",
+                "print(solver.problem)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Re-affecting `f.y` interactively will not update the mathematical problem, as the target value for `f.y` is now enforced by driver `solver.case`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "f.x = 1.0\n",
+                "f.y = 0.0\n",
+                "\n",
+                "f.run_drivers()\n",
+                "\n",
+                "print(solver.problem)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Changing the target value of `f.y` can still be done through `solver.case.set_init`:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "solver.case.set_init({\n",
+                "    'x': 2.0,\n",
+                "    'y': -0.5,\n",
+                "})\n",
+                "\n",
+                "f.run_drivers()\n",
+                "\n",
+                "print(solver.problem)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Targets and design methods\n",
                 "\n",
                 "Targets can be particularly interesting to define [design methods](11-DesignMethods.ipynb) with a controllable target value."
             ]
         },
         {
             "cell_type": "code",
@@ -214,19 +295,20 @@
                 "f.a = 2.0\n",
                 "f.y = -0.5\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Without the use of `add_target`, the only way to control the design value of `y` would be to declare an additional inward `y_target`, say, used as right-hand side value of design equation:\n",
                 "```python\n",
                 "    def setup(self):\n",
                 "        self.add_inward('a', 0.0)\n",
@@ -238,14 +320,15 @@
                 "        design.add_unknown('x').add_equation('y == y_target')\n",
                 "```\n",
                 "\n",
                 "While this syntax works, it has the inconvenience of burdening the system with an inward only meaningful when design method `'y'` is activated."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Pulling a targetted variable\n",
                 "\n",
                 "Consider a system with a targetted output pulled at parent level.\n"
             ]
@@ -284,31 +367,32 @@
                 "head.x = 3.0\n",
                 "head.g.y = 5.0\n",
                 "head.f.a = 2.0\n",
                 "\n",
                 "head.run_drivers()\n",
                 "\n",
                 "print(\n",
-                "    f\"Solution:\\n\"\n",
+                "    f\"Solution:\",\n",
                 "    f\"{head.g.x = }\",\n",
                 "    f\"{head.g.y = }\",\n",
                 "    f\"\\n{solver.problem!r}\",\n",
                 "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "What just happened?!\n",
                 "\n",
                 "In this case, output `head.g.y` is pulled up at parent level. Behind the scene, an *upward* connection is created from `head.g.y` to `head.y`, such that `y` appears as a natural output of top system `head`, computed by sub-system `head.g`.\n",
                 "\n",
-                "As a consequence, it seems natural to set the targetted value in the context of system `head`, that is setting `head.y` instead of `head.g.y`, when activating `head.design('y')`.\n",
+                "As a consequence, when activating `head.design('y')`, it seems natural to set the targetted value in the context of system `head`, that is setting `head.y` instead of `head.g.y`.\n",
                 "Let's try again:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -323,23 +407,24 @@
                 "head.x = 3.0\n",
                 "head.y = 5.0    # set target value\n",
                 "head.f.a = 2.0\n",
                 "\n",
                 "head.run_drivers()\n",
                 "\n",
                 "print(\n",
-                "    f\"Solution:\\n\"\n",
+                "    f\"Solution:\",\n",
                 "    f\"{head.g.x = }\",\n",
                 "    f\"{head.g.y = }\",\n",
                 "    f\"\\n{solver.problem!r}\",\n",
                 "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Weak and strong targets\n",
                 "\n",
                 "A target is said to be *weak* if it can be disregarded in certain situations.\n",
                 "By default, targets are *strong*, meaning the target equation is always enforced.\n",
@@ -348,30 +433,32 @@
                 "\n",
                 "1. is an output;\n",
                 "2. is connected to an input.\n",
                 "\n",
                 "The second condition specifically excludes pulled outputs, which is the only admissible output-output connection.\n",
                 "\n",
                 "Weak targets may be useful when a targetted variable is transmitted through a chain of systems, and one wants to specify the target on the last system only.\n",
-                "This is typically the case in the next example, where we simulate three resistors series, and wish to determine the current between end-point voltages.\n"
+                "This is typically the case in the next example, where we simulate three resistors in series, and wish to determine the current between end-point voltages.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from cosapp.base import System, Port\n",
                 "\n",
+                "\n",
                 "class ElectricPort(Port):\n",
                 "    def setup(self):\n",
                 "        self.add_variable(\"I\", 1.0, unit=\"A\", desc=\"Current\")\n",
                 "        self.add_variable(\"V\", 0.0, unit=\"V\", desc=\"Voltage\")\n",
                 "\n",
+                "\n",
                 "class Resistor(System):\n",
                 "    def setup(self):\n",
                 "        self.add_input(ElectricPort, 'elec_in')\n",
                 "        self.add_output(ElectricPort, 'elec_out')\n",
                 "\n",
                 "        self.add_inward(\"R\", 1e2, unit=\"ohm\", desc=\"Resistance\")\n",
                 "        self.add_outward(\"deltaV\", 0.0, unit=\"V\")\n",
@@ -381,25 +468,29 @@
                 "    \n",
                 "    def compute(self):\n",
                 "        elec_in, elec_out = self.elec_in, self.elec_out\n",
                 "        self.deltaV = self.R * elec_in.I\n",
                 "        elec_out.I = elec_in.I\n",
                 "        elec_out.V = elec_in.V - self.deltaV\n",
                 "\n",
+                "\n",
                 "class ThreeResistorSeries(System):\n",
                 "    def setup(self):\n",
                 "        R1 = self.add_child(Resistor(\"R1\"), pulling=\"elec_in\")\n",
                 "        R2 = self.add_child(Resistor(\"R2\"))\n",
                 "        R3 = self.add_child(Resistor(\"R3\"), pulling=\"elec_out\")\n",
-                "        \n",
+                "\n",
+                "        self.add_property('resistances', (R1, R2, R3))  # for convenience\n",
+                "\n",
                 "        self.connect(R1.elec_out, R2.elec_in)\n",
                 "        self.connect(R2.elec_out, R3.elec_in)\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Each resistor defines an inner off-design problem, in which current is unknown, and a target is set on the output voltage.\n",
                 "When several resistors are connected, local unknown currents are discarded every time they belong to a connected input port, which occurs at each node point connecting adjacent resistors.\n",
                 "Likewise, local weak targets on voltages are discarded at each connecting node, where output voltage is transmitted to the next resistor.\n",
                 "\n",
@@ -408,52 +499,61 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s = ThreeResistorSeries('s')\n",
-                "\n",
-                "s.R1.R = 100\n",
-                "s.R2.R = 50\n",
-                "s.R3.R = 250\n",
+                "circuit = ThreeResistorSeries('circuit')\n",
                 "\n",
-                "s.elec_in.V = 10\n",
-                "s.elec_out.V = -2\n",
+                "circuit.R1.R = 100\n",
+                "circuit.R2.R = 50.\n",
+                "circuit.R3.R = 250\n",
+                "\n",
+                "circuit.elec_in.I = 0.25   # initial guess\n",
+                "circuit.elec_in.V = 10\n",
+                "circuit.elec_out.V = -2\n",
                 "\n",
                 "# Set bogus target values at connection points\n",
                 "# These values will be discarded, as targets are weak\n",
-                "s.R1.elec_out.V = 1.23e4\n",
-                "s.R2.elec_out.V = -8e17\n",
-                "\n",
-                "s.add_driver(NonLinearSolver('solver'))\n",
-                "s.run_drivers()\n",
+                "circuit.R1.elec_out.V = 1.23e4\n",
+                "circuit.R2.elec_out.V = -8e17\n",
                 "\n",
-                "voltages = [s.elec_in.V]\n",
-                "voltages.extend(s[f\"R{i}.elec_out.V\"] for i in range(1, 4))\n",
+                "circuit.add_driver(NonLinearSolver('solver'))\n",
+                "circuit.run_drivers()\n",
                 "\n",
-                "print(\n",
-                "    f\"Solution:\\n\"\n",
-                "    f\"{s.elec_in.I = }\",\n",
-                "    f\"{s.elec_in.V = }\",\n",
-                "    f\"{s.elec_out.V = }\",\n",
-                "    f\"{voltages = }\",\n",
-                "    f\"\\nOverall resistance: {(s.elec_in.V - s.elec_out.V) / s.elec_in.I :.2f} Ohm\",\n",
-                "    sep = \"\\n\",\n",
-                ")\n"
+                "# Show actual problem solved\n",
+                "circuit.drivers['solver'].problem"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "s.drivers['solver'].problem"
+                "voltages = [circuit.elec_in.V]\n",
+                "voltages.extend(res.elec_out.V for res in circuit.resistances)\n",
+                "\n",
+                "R_global = (circuit.elec_in.V - circuit.elec_out.V) / circuit.elec_in.I\n",
+                "\n",
+                "print(\n",
+                "    f\"Solution:\",\n",
+                "    f\"{circuit.elec_in.I = }\",\n",
+                "    f\"{circuit.elec_in.V = }\",\n",
+                "    f\"{circuit.elec_out.V = }\",\n",
+                "    f\"{voltages = }\",\n",
+                "    sep=\"\\n  \",\n",
+                ")\n",
+                "print(\n",
+                "    \"\",\n",
+                "    f\"Overall resistance: {R_global} Ohm\",\n",
+                "    f\"Sum of resistances: {sum(res.R for res in circuit.resistances)} Ohm\",\n",
+                "    sep=\"\\n\",\n",
+                ")\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -461,31 +561,38 @@
                 "import pandas as pd\n",
                 "import plotly.express as px\n",
                 "\n",
                 "df = pd.DataFrame.from_dict(\n",
                 "    {\n",
                 "        \"V\": voltages,\n",
                 "        \"index\": list(range(len(voltages))),\n",
-                "        \"node\": list('ABCD'),\n",
+                "        \"node\": list(\"ABCD\"),\n",
                 "    }\n",
                 ")\n",
                 "\n",
-                "fig = px.line(df,\n",
+                "fig = px.scatter(df,\n",
                 "    x=\"node\", y=\"V\",\n",
                 "    title=\"Voltage profile\",\n",
-                "    # markers=True,\n",
+                ")\n",
+                "fig.update_traces(\n",
+                "    mode=\"lines+markers\",\n",
+                "    marker=dict(\n",
+                "        size=10,\n",
+                "        color='#636EFA',\n",
+                "    ),\n",
                 ")\n",
                 "fig.update_layout(\n",
-                "    height=450,\n",
+                "    height=600,\n",
                 "    hovermode='x',\n",
                 ")\n",
                 "fig.show()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Targetted expressions\n",
                 "\n",
                 "A target can also be set on an evaluable expression, such as `norm(v)` or `y * (y + 1)`, as long as the expression only involves a single variable."
             ]
@@ -507,25 +614,26 @@
                 "f = CubicFunction('f')\n",
                 "\n",
                 "solver = f.add_driver(NonLinearSolver('solver'))\n",
                 "\n",
                 "solver.add_unknown('x').add_target('abs(y)')\n",
                 "\n",
                 "f.y = 8  # value used for targetted expression\n",
-                "f.x = 4  # positive initial value of unknown\n",
+                "f.x = 4  # positive initial value of unknown x\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Same computation, with a different initial guess on `f.x`:"
             ]
         },
         {
@@ -537,15 +645,15 @@
                 "f.y = 8\n",
                 "f.x = -5  # negative initial value\n",
                 "f.run_drivers()\n",
                 "\n",
                 "print(\n",
                 "    f\"{f.x = }\",\n",
                 "    f\"{f.y = }\",\n",
-                "    sep = \"\\n\",\n",
+                "    sep=\"\\n\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `cosapp-0.14.1/docs/tutorials/TimeDriver.ipynb` & `cosapp-0.15.0/docs/tutorials/TimeDriver.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666667%*

 * *Differences: {"'cells'": "{0: {'source': ['![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Time "*

 * *            "simulations\\n', '\\n', '# Time simulations\\n', '\\n', '### Declare transient "*

 * *            "variables in a system\\n', '\\n', 'CoSApp allows one to simulate the behaviour of "*

 * *            "systems with time-dependent variables, through the use of time drivers.\\n', '\\n', "*

 * *            "'Transient variables, defined by their time derivative, are declared with method "*

 * *            "`add_transient` at sy […]*

```diff
@@ -2,21 +2,16 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Time simulations"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Time simulations\n",
+                "\n",
                 "# Time simulations\n",
                 "\n",
                 "### Declare transient variables in a system\n",
                 "\n",
                 "CoSApp allows one to simulate the behaviour of systems with time-dependent variables, through the use of time drivers.\n",
                 "\n",
                 "Transient variables, defined by their time derivative, are declared with method `add_transient` at system setup.\n",
```

### Comparing `cosapp-0.14.1/docs/tutorials/TimeDriverAdvanced.ipynb` & `cosapp-0.15.0/docs/tutorials/TimeDriverAdvanced.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9847484923245614%*

 * *Differences: {"'cells'": "{0: {'source': ['![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Advanced Time "*

 * *            "simulations\\n', '\\n', '# Time simulations - Advanced Features'], 'attachments': "*

 * *            "OrderedDict()}, 1: {'source': {insert: [(1, '\\n')]}, 'attachments': OrderedDict()}, "*

 * *            "3: {'source': {insert: [(0, 'from cosapp.drivers import RungeKutta, "*

 * *            "NonLinearSolver\\n'), (5, '\\n'), (7, 'solver = "*

 * *            'point.add_driver(NonLinearSolver("solver"))\\n\'), (8,  […]*

```diff
@@ -1,30 +1,28 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Advanced Time simulations"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** tutorials: Advanced Time simulations\n",
+                "\n",
                 "# Time simulations - Advanced Features"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Find the initial condition leading to a target end point\n",
+                "\n",
                 "In this example, we combine a nonlinear solver and a time driver, to compute the initial condition leading to a target point at the end of the time simulation."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -60,23 +58,29 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from cosapp.drivers import RungeKutta, NonLinearSolver, RunSingleCase\n",
+                "from cosapp.drivers import RungeKutta, NonLinearSolver\n",
                 "from cosapp.recorders import DataFrameRecorder\n",
                 "from time_solutions import PointMassSolution\n",
                 "\n",
                 "point = Ballistics('point')  # head system\n",
+                "\n",
                 "# Add drivers\n",
-                "solver = point.add_driver(NonLinearSolver('solver', factor=0.9))\n",
-                "target = solver.add_child(RunSingleCase('target'))\n",
-                "driver = target.add_child(RungeKutta(\"RungeKutta\", order=3))\n",
+                "solver = point.add_driver(NonLinearSolver(\"solver\"))\n",
+                "driver = solver.add_child(RungeKutta(\"RungeKutta\", order=3))\n",
+                "\n",
+                "# Define `v0` as unknown, so that the final value of `x` is a desired target point\n",
+                "# Note:\n",
+                "#   For driver `solver`, variable 'x' represents the position at the end of\n",
+                "#   each time simulation, since it is the parent of the `RungeKutta` time driver.\n",
+                "solver.add_unknown('v0').add_equation('x == [10, 0, 10]')\n",
                 "\n",
                 "# Define a simulation scenario\n",
                 "driver.time_interval = (0, 2)\n",
                 "driver.dt = 0.1\n",
                 "\n",
                 "x0 = [0, 0, 10]\n",
                 "\n",
@@ -87,22 +91,17 @@
                 "    },\n",
                 "    values = {'mass': 1.5, 'k': 0.92},\n",
                 ")\n",
                 "\n",
                 "# Add a recorder to capture time evolution in a dataframe\n",
                 "driver.add_recorder(DataFrameRecorder(includes=['x', 'v', 'a']), period=0.1)\n",
                 "\n",
-                "# Define `v0` as unknown, so that the final value of `x` is a desired target point\n",
-                "# Note:\n",
-                "#   For `RunSingleCase` driver `target`, 'x' represents the position at the end of\n",
-                "#   each time simulation, since it is the parent of the `RungeKutta` time driver.\n",
-                "target.design.add_unknown('v0').add_equation('x == [10, 0, 10]')\n",
-                "target.set_init({'v0': np.ones(3)})\n",
+                "point.v0 = np.ones(3)  # initial guess for the solver\n",
                 "\n",
-                "point.run_drivers()\n",
+                "point.run_drivers()  # solve\n",
                 "\n",
                 "solution = PointMassSolution(point, point.v0, x0)\n",
                 "\n",
                 "data = driver.recorder.export_data()\n",
                 "time = np.asarray(data['time'])\n",
                 "traj = {\n",
                 "    'exact': np.array(list(map(solution.x, time))),\n",
@@ -111,22 +110,22 @@
                 "\n",
                 "error = np.abs(traj['num'] - traj['exact'])\n",
                 "\n",
                 "print(\n",
                 "    f\"order = {driver.order}; dt = {driver.dt}\",\n",
                 "    f\"Max error on trajectory = {error.max():.2e}\",\n",
                 "    f\"End point: {traj['num'][-1].round(3)}\",\n",
+                "    f\"v0 = {point.v0.round(3)}\",\n",
                 "    sep=\"\\n\",\n",
                 ")\n",
                 "vz = point.v0[2]\n",
                 "vh = np.linalg.norm(point.v0[:2])\n",
                 "angle = np.arctan2(vz, vh)\n",
-                "print(f\"v0 = {point.v0.round(3)}\")\n",
                 "print(\n",
-                "    f\"norm = {np.linalg.norm(point.v0):.2f}\",\n",
+                "    f\"norm = {np.linalg.norm(point.v0):.2f} m/s\",\n",
                 "    f\"angle = {np.degrees(angle):.1f} deg\",\n",
                 "    sep=\"; \",\n",
                 ")\n"
             ]
         },
         {
             "cell_type": "code",
@@ -284,14 +283,15 @@
                 "    )\n",
                 ")\n",
                 "\n",
                 "go.Figure(data=traces, layout=layout)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In the next two cells, we display the recorded time and y steps, respectively.\n",
                 "At the beginning of the simulation, dy/dt is sufficiently small that the evolution of `ode.y` within time interval `driver.dt` (0.5) does not exceed the specified `max_abs_step`.\n",
                 "As time goes on, dy/dt increases and eventually becomes too large to limit the y step within `driver.dt`; time step limitation kicks in, and the actual `dt` appears to be smaller than `driver.dt`.\n",
                 "\n",
```

### Comparing `cosapp-0.14.1/docs/tutorials/TipsAndTricks.ipynb` & `cosapp-0.15.0/docs/tutorials/TipsAndTricks.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.946529307625099%*

 * *Differences: {"'cells'": "{16: {'source': {insert: [(1, '\\n'), (7, '\\n'), (18, '\\n'), (24, '        # Create "*

 * *            "a tuple of children\\n'), (25, '        resistors = tuple(\\n'), (28, '        "*

 * *            ")\\n'), (29, '        # Store collection as a read-only property\\n'), (30, "*

 * *            '"        self.add_property(\'resistors\', resistors)\\n"), (32, \'        # Connect '*

 * *            "resistors in series\\n'), (33, '        for previous, current in zip(resistors, "*

 * *            "resistors[1:]):\\n' […]*

```diff
@@ -310,59 +310,68 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from cosapp.base import Port, System\n",
                 "\n",
+                "\n",
                 "class ElecPort(Port):\n",
                 "    def setup(self):\n",
                 "        self.add_variable(\"I\", 1.0, unit=\"A\", desc=\"Current\")\n",
                 "        self.add_variable(\"V\", 0.0, unit=\"V\", desc=\"Voltage\")\n",
                 "\n",
+                "\n",
                 "class Resistor(System):\n",
                 "    def setup(self):\n",
                 "        self.add_input(ElecPort, 'elec_in')\n",
                 "        self.add_output(ElecPort, 'elec_out')\n",
                 "        self.add_inward(\"R\", 1e2, unit=\"ohm\", desc=\"Resistance\")\n",
                 "    \n",
                 "    def compute(self):\n",
                 "        self.elec_out.I = I = self.elec_in.I\n",
                 "        self.elec_out.V = self.elec_in.V - self.R * I\n",
                 "\n",
+                "\n",
                 "class ResistorSeries(System):\n",
                 "    def setup(self, n=2):\n",
                 "        self.add_property('n', max(int(n), 2))\n",
                 "\n",
-                "        # Create a tuple of children, and store it as a property\n",
-                "        self.add_property('resistors', tuple(\n",
+                "        # Create a tuple of children\n",
+                "        resistors = tuple(\n",
                 "            self.add_child(Resistor(f\"R{i}\"))\n",
                 "            for i in range(self.n)\n",
-                "        ))\n",
-                "        R = self.resistors\n",
+                "        )\n",
+                "        # Store collection as a read-only property\n",
+                "        self.add_property('resistors', resistors)\n",
                 "        \n",
-                "        for previous, current in zip(R, R[1:]):\n",
+                "        # Connect resistors in series\n",
+                "        for previous, current in zip(resistors, resistors[1:]):\n",
                 "            self.connect(current.elec_in, previous.elec_out)\n",
                 "\n",
                 "        # Pull first `elec_in` and last `elec_out`\n",
                 "        self.add_input(ElecPort, 'elec_in')\n",
                 "        self.add_output(ElecPort, 'elec_out')\n",
                 "\n",
-                "        self.connect(self.elec_in, R[0].elec_in)\n",
-                "        self.connect(self.elec_out, R[-1].elec_out)\n"
+                "        self.connect(self.elec_in, resistors[0].elec_in)\n",
+                "        self.connect(self.elec_out, resistors[-1].elec_out)\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The same trick can be used to create collections of ports, if needed.\n",
                 "\n",
-                "Use of property `resistors` makes the code clearer, and allows one to loop through the child/port collection without resorting to syntaxes of the kind `s[f\"R{i}\"] for i in range(s.n)`.\n",
+                "Use of property `resistors` makes the code clearer, and allows one to loop through the child/port collection without resorting to syntaxes of the kind\n",
+                "\n",
+                "```python\n",
+                "s[f\"R{i}\"] for i in range(s.n)\n",
+                "```\n",
                 "\n",
                 "In the next cell, for example, we show three identical ways of initializing the resistances:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -465,82 +474,84 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s = MySystem('s', n=2, x=[[0, 0.1, 0.2], [-0.5, 0.9, 0.4]])\n",
                 "\n",
-                "print(s.x)"
+                "print(f\"s.x = \\n{s.x!s}\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The complexity of parsing through options at `setup` can be simplified using ad-hoc functions referred to as *factories*, declared as class methods by decorator `@classmethod`.\n",
-                "Note that the first argument of class methods is always `cls` (as opposed to `self` for traditional object methods), denoting the class itself.\n",
-                "Factories are special class method whose job is to create and return a new class instance (an object) from a specific set of arguments.\n",
+                "Factories are special class methods whose job is to create and return a new class instance (an object) from a specific set of arguments.\n",
                 "\n",
                 "Class methods are invoked with syntax `ClassName.method_name(...)`.\n",
                 "\n",
-                "In the next cell, we implement factory methods `from_data` and `from_file`, each with its own signature:\n"
+                "In the next cell, we implement factory methods `from_data` and `from_file`, each with its own signature.\n",
+                "Note that the first argument of a class method is always `cls`, denoting the class itself, as opposed to `self`, used in traditional object-bound methods.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "from cosapp.base import System\n",
                 "import numpy\n",
                 "\n",
+                "\n",
                 "class MySystem(System):\n",
                 "    def setup(self, n: int):\n",
                 "        self.add_property('n', int(n))\n",
                 "        self.add_inward('x', numpy.zeros((self.n, 3)))\n",
                 "\n",
                 "    @classmethod\n",
-                "    def from_data(cls, name: str, data) -> \"MySystem\":\n",
-                "        n = cls.check_shape(data)\n",
-                "        s = cls(name, n=n)  # newly created system\n",
-                "        s.x = numpy.array(data, dtype=float)\n",
+                "    def from_data(cls, name: str, data: numpy.ndarray) -> MySystem:\n",
+                "        \"\"\"Factory creating a new system from a numpy array.\"\"\"\n",
+                "        x = cls.reshape(data)\n",
+                "        s = cls(name, n=x.shape[0])  # newly created system\n",
+                "        s.x = numpy.asarray(data, dtype=float)\n",
                 "        return s\n",
                 "\n",
                 "    @classmethod\n",
-                "    def from_file(cls, name: str, filename) -> \"MySystem\":\n",
+                "    def from_file(cls, name: str, filename) -> MySystem:\n",
+                "        \"\"\"Factory creating a new system from data stored on file.\"\"\"\n",
                 "        data = numpy.load(filename)\n",
                 "        return cls.from_data(name, data)\n",
                 "\n",
                 "    @staticmethod\n",
-                "    def check_shape(data) -> int:\n",
-                "        \"\"\"Checks that `data` is a (N x 3) array-like object.\n",
-                "        If so, returns integer N. If not, raises `ValueError`.\n",
+                "    def reshape(data) -> numpy.ndarray:\n",
+                "        \"\"\"Checks that `data` can be reshaped into a (N x 3) array.\n",
+                "        If so, returns the reshaped array; otherwise, raises `ValueError`.\n",
                 "        \"\"\"\n",
-                "        shape = numpy.shape(data)\n",
-                "        ok = len(shape) == 2 and shape[1] == 3\n",
-                "        if not ok:\n",
-                "            raise ValueError(\"data must be a (N x 3) array-like object\")\n",
-                "        return shape[0]\n"
+                "        try:\n",
+                "            return numpy.reshape(data, (-1, 3))\n",
+                "        except ValueError:\n",
+                "            raise ValueError(\"data must be interpretable as a (N x 3) array\")\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "s1 = MySystem('s1', n=4)  # usual way\n",
                 "\n",
                 "print(f\"{s1.n = }\", f\"s1.x =\\n{s1.x}\", sep=\"\\n\")\n",
                 "\n",
                 "# Create a system from existing data with `from_data`\n",
-                "s2 = MySystem.from_data('s2', [[0, 0.1, 0.2], [-0.5, 0.9, 0.4]])\n",
+                "s2 = MySystem.from_data('s2', [0, 0.1, 0.2, -0.5, 0.9, 0.4])\n",
                 "\n",
                 "print(\"\", f\"{s2.n = }\", f\"s2.x =\\n{s2.x}\", sep=\"\\n\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -559,15 +570,21 @@
                 "    )\n",
                 "else:\n",
                 "    print(f\"{s3.n = }\", f\"s3.x =\\n{s3.x}\", sep=\"\\n\")\n"
             ]
         }
     ],
     "metadata": {
+        "kernelspec": {
+            "display_name": "cosapp",
+            "language": "python",
+            "name": "python3"
+        },
         "language_info": {
-            "name": "python"
+            "name": "python",
+            "version": "3.9.16"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `cosapp-0.14.1/docs/tutorials/Visitors.ipynb` & `cosapp-0.15.0/docs/tutorials/Visitors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/aa-SimpleCircuit.ipynb` & `cosapp-0.15.0/docs/tutorials/aa-SimpleCircuit.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9866468422543189%*

 * *Differences: {"'cells'": "{0: {'source': ['![CoSAppLogo](images/cosapp.svg) **CoSApp** examples\\n', '\\n', '# "*

 * *            "Simple circuit\\n', '\\n', 'Preliminary note:\\n', '\\n', 'This case is taken from "*

 * *            '[OpenMDAO](http://openmdao.org/twodocs/versions/latest/examples/circuit_analysis.html). '*

 * *            'OpenMDAO is an open-source computing platform for systems analysis and '*

 * *            'multidisciplinary optimization developed by the NASA. Its philosophy shares some of '*

 * *            'the goals wit […]*

```diff
@@ -2,22 +2,16 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
-                "![CoSAppLogo](images/cosapp.svg) **CoSApp** examples:"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "![CoSAppLogo](images/cosapp.svg) **CoSApp** examples\n",
+                "\n",
                 "# Simple circuit\n",
                 "\n",
                 "Preliminary note:\n",
                 "\n",
                 "This case is taken from [OpenMDAO](http://openmdao.org/twodocs/versions/latest/examples/circuit_analysis.html). OpenMDAO is an open-source computing platform for systems analysis and multidisciplinary optimization developed by the NASA. Its philosophy shares some of the goals with CoSApp. So this example is also an opportunity to compare both software.\n",
                 "\n",
                 "OpenMDAO is licensed under [Apache License](https://github.com/OpenMDAO/OpenMDAO/blob/master/LICENSE.txt).\n",
@@ -153,15 +147,22 @@
                 "        self.add_equation('sum_I_in == sum_I_out', name='current balance')\n",
                 "\n",
                 "    def compute(self):\n",
                 "        self.sum_I_in = sum(current.I for current in self.incoming_currents)\n",
                 "        self.sum_I_out = sum(current.I for current in self.outgoing_currents)\n",
                 "\n",
                 "    @classmethod\n",
-                "    def make(cls, name, parent, incoming: list[Dipole]=[], outgoing: list[Dipole]=[], pulling=None) -> Node:\n",
+                "    def make(\n",
+                "        cls,\n",
+                "        name: str,\n",
+                "        parent: System,\n",
+                "        incoming: list[Dipole]=[],\n",
+                "        outgoing: list[Dipole]=[],\n",
+                "        pulling=None,\n",
+                "    ) -> Node:\n",
                 "        \"\"\"Factory creating new node within `parent`, with\n",
                 "        appropriate connections with incoming and outgoing dipoles.\n",
                 "        \"\"\"\n",
                 "        node = cls(name, n_in=len(incoming), n_out=len(outgoing))\n",
                 "        parent.add_child(node, pulling=pulling)\n",
                 "        \n",
                 "        for dipole, current in zip(incoming, node.incoming_currents):\n",
```

### Comparing `cosapp-0.14.1/docs/tutorials/exprampode_fmu.py` & `cosapp-0.15.0/docs/tutorials/exprampode_fmu.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/Moise_tables_loi.jpg` & `cosapp-0.15.0/docs/tutorials/images/Moise_tables_loi.jpg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/cosapp.svg` & `cosapp-0.15.0/docs/tutorials/images/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/design_circuit.svg` & `cosapp-0.15.0/docs/tutorials/images/design_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/drivers_1.svg` & `cosapp-0.15.0/docs/tutorials/images/drivers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/drivers_2.svg` & `cosapp-0.15.0/docs/tutorials/images/drivers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/drivers_3.svg` & `cosapp-0.15.0/docs/tutorials/images/drivers_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/drivers_4.svg` & `cosapp-0.15.0/docs/tutorials/images/drivers_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/drivers_5.svg` & `cosapp-0.15.0/docs/tutorials/images/drivers_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/drivers_nonlinear.svg` & `cosapp-0.15.0/docs/tutorials/images/drivers_nonlinear.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/experimental.svg` & `cosapp-0.15.0/docs/tutorials/images/experimental.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/in_progress.svg` & `cosapp-0.15.0/docs/tutorials/images/in_progress.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/ports_1.svg` & `cosapp-0.15.0/docs/tutorials/images/ports_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/ports_2.svg` & `cosapp-0.15.0/docs/tutorials/images/ports_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/ports_3.svg` & `cosapp-0.15.0/docs/tutorials/images/ports_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/simple_circuit.svg` & `cosapp-0.15.0/docs/tutorials/images/simple_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/systems_1.svg` & `cosapp-0.15.0/docs/tutorials/images/systems_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/systems_2.svg` & `cosapp-0.15.0/docs/tutorials/images/systems_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/systems_3.svg` & `cosapp-0.15.0/docs/tutorials/images/systems_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/systems_4.svg` & `cosapp-0.15.0/docs/tutorials/images/systems_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/systems_5.svg` & `cosapp-0.15.0/docs/tutorials/images/systems_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/tanks.svg` & `cosapp-0.15.0/docs/tutorials/images/tanks.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/triggers_1.svg` & `cosapp-0.15.0/docs/tutorials/images/triggers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/triggers_2.svg` & `cosapp-0.15.0/docs/tutorials/images/triggers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/validity.svg` & `cosapp-0.15.0/docs/tutorials/images/validity.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/images/visibility.svg` & `cosapp-0.15.0/docs/tutorials/images/visibility.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/multimode/BouncingBall.ipynb` & `cosapp-0.15.0/docs/tutorials/multimode/BouncingBall.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998464373464373%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(51, 'class BouncingBall(PointMassFreeFall):\\n'), (52, '    "*

 * *            '"""Extension of `PointMassFreeFall`, containing a rebound event\\n\'), (53, \'    and '*

 * *            'a rebound restitution coefficient.\\n\'), (54, \'    """\\n\'), (56, \'        '*

 * *            "super().setup()\\n')], delete: [56, 55, 54, 52, 51]}}}"}*

```diff
@@ -69,20 +69,20 @@
                 "        self.add_transient('v', der='a')\n",
                 "        self.add_transient('x', der='v')\n",
                 "\n",
                 "        self.g = np.r_[0, 0, -9.81]\n",
                 "        self.exec_order = ['friction', 'dynamics']\n",
                 "\n",
                 "\n",
-                "class BouncingBall(System):\n",
-                "    \"\"\"Bouncing point mass\"\"\"\n",
+                "class BouncingBall(PointMassFreeFall):\n",
+                "    \"\"\"Extension of `PointMassFreeFall`, containing a rebound event\n",
+                "    and a rebound restitution coefficient.\n",
+                "    \"\"\"\n",
                 "    def setup(self):\n",
-                "        self.add_child(PointMassFreeFall('point'), pulling=[\n",
-                "            'x', 'v', 'a', 'mass', 'cf', 'g',\n",
-                "        ])\n",
+                "        super().setup()\n",
                 "        self.add_event('rebound', trigger=\"x[2] <= 0\")\n",
                 "        self.add_inward('cr', 1.0, desc=\"Rebound restitution coefficient\", limits=(0, 1))\n",
                 "        self.add_outward_modevar(\"n_rebounds\", init=0, dtype=int)\n",
                 "\n",
                 "    def transition(self):\n",
                 "        if self.rebound.present:\n",
                 "            self.n_rebounds += 1\n",
```

### Comparing `cosapp-0.14.1/docs/tutorials/multimode/MultimodeOde.ipynb` & `cosapp-0.15.0/docs/tutorials/multimode/MultimodeOde.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/multimode/NewtonPendulum.ipynb` & `cosapp-0.15.0/docs/tutorials/multimode/NewtonPendulum.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/optimization/BetzLimit.ipynb` & `cosapp-0.15.0/docs/tutorials/optimization/BetzLimit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/optimization/Sellar.ipynb` & `cosapp-0.15.0/docs/tutorials/optimization/Sellar.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/docs/tutorials/quickstart.ipynb` & `cosapp-0.15.0/docs/tutorials/quickstart.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.991859243697479%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, '5 minutes?.. Challenge accepted!\\n'), (3, '\\n'), (4, "*

 * *            "'# Quickstart\\n'), (5, '\\n'), (6, '## CoSApp Overview\\n'), (7, '\\n'), (8, "*

 * *            '"<font color=\'orange\'>**CoSApp**</font> is a multidisciplinary oriented tool for '*

 * *            'the simulation and design of systems. Its goal is to provide a user-friendly and '*

 * *            'efficient environnement to build, exchange and solve physical models.\\n"), (9, '*

 * *            "'\\n'), (10, '##  […]*

```diff
@@ -5,22 +5,16 @@
             "cell_type": "markdown",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "source": [
                 "![CoSAppLogo](images/cosapp.svg)\n",
                 "\n",
-                "5 minutes?.. Challenge accepted!"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
+                "5 minutes?.. Challenge accepted!\n",
+                "\n",
                 "# Quickstart\n",
                 "\n",
                 "## CoSApp Overview\n",
                 "\n",
                 "<font color='orange'>**CoSApp**</font> is a multidisciplinary oriented tool for the simulation and design of systems. Its goal is to provide a user-friendly and efficient environnement to build, exchange and solve physical models.\n",
                 "\n",
                 "## Get started\n",
```

### Comparing `cosapp-0.14.1/docs/tutorials/time_solutions.py` & `cosapp-0.15.0/docs/tutorials/time_solutions.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/setup.cfg` & `cosapp-0.15.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cosapp-0.14.1/setup.py` & `cosapp-0.15.0/setup.py`

 * *Files identical despite different names*

