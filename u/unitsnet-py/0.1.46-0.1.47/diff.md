# Comparing `tmp/unitsnet-py-0.1.46.tar.gz` & `tmp/unitsnet-py-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitsnet-py-0.1.46.tar", last modified: Mon Jul 17 18:41:41 2023, max compression
+gzip compressed data, was "unitsnet-py-0.1.47.tar", last modified: Thu Jul 20 17:29:31 2023, max compression
```

## Comparing `unitsnet-py-0.1.46.tar` & `unitsnet-py-0.1.47.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:41:41.455574 unitsnet-py-0.1.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-17 18:40:49.000000 unitsnet-py-0.1.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-17 18:41:41.455574 unitsnet-py-0.1.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27203 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-17 18:41:34.000000 unitsnet-py-0.1.46/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 18:41:41.455574 unitsnet-py-0.1.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-17 18:41:35.000000 unitsnet-py-0.1.46/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:41:41.439574 unitsnet-py-0.1.46/unitsnet_py/
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:41:41.455574 unitsnet-py-0.1.46/unitsnet_py/units/
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/amount_of_substance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/amplitude_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-17 18:41:30.000000 unitsnet-py-0.1.46/unitsnet_py/units/apparent_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/apparent_power.py
--rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/area.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/area_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/area_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/bit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/brake_specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/capacitance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/coefficient_of_thermal_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/compressibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    77189 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/density.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/dynamic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_admittance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_conductance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_current_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_current_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_inductance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_resistivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/electric_surface_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    51805 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/energy_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/force.py
--rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/force_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    62708 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/force_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/fuel_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/heat_transfer_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/illuminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/impulse.py
--rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/information.py
--rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/irradiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/jerk.py
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/kinematic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/leak_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/linear_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    42257 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/linear_power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/luminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/luminosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/luminous_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/luminous_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/magnetic_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/magnetic_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/magnetization.py
--rw-r--r--   0 runner    (1001) docker     (123)    40535 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    80144 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-07-17 18:41:31.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_fraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    48955 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/mass_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molar_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molar_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molar_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molar_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/molarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/permittivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/porous_medium_permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/power.py
--rw-r--r--   0 runner    (1001) docker     (123)    69959 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/power_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)    73652 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)    34511 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/pressure_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/ratio_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/reactive_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/reactive_power.py
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/reciprocal_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    18523 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/reciprocal_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/relative_humidity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/rotational_acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/rotational_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    61867 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/rotational_stiffness.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/rotational_stiffness_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/solid_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    50352 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    32699 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/specific_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    48511 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/standard_volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/temperature_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/temperature_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/temperature_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/thermal_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/thermal_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/torque_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/turbidity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/vitamin_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    71514 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    99718 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume_flow_per_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volume_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    22169 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/volumetric_heat_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-17 18:41:32.000000 unitsnet-py-0.1.46/unitsnet_py/units/warping_moment_of_inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:41:41.439574 unitsnet-py-0.1.46/unitsnet_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-17 18:41:41.000000 unitsnet-py-0.1.46/unitsnet_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-17 18:41:41.000000 unitsnet-py-0.1.46/unitsnet_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:41:41.000000 unitsnet-py-0.1.46/unitsnet_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 18:41:41.000000 unitsnet-py-0.1.46/unitsnet_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:31.237998 unitsnet-py-0.1.47/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 17:28:32.000000 unitsnet-py-0.1.47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-20 17:29:31.237998 unitsnet-py-0.1.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27203 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-20 17:29:24.000000 unitsnet-py-0.1.47/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:29:31.237998 unitsnet-py-0.1.47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-20 17:29:24.000000 unitsnet-py-0.1.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:31.221998 unitsnet-py-0.1.47/unitsnet_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:31.237998 unitsnet-py-0.1.47/unitsnet_py/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/amount_of_substance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/amplitude_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/apparent_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/apparent_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/area_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/area_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/bit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/brake_specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/capacitance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/coefficient_of_thermal_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/compressibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77189 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/dynamic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_admittance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_conductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_current_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_current_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_inductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_potential_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_potential_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_potential_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_resistivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/electric_surface_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51805 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/energy_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-20 17:29:20.000000 unitsnet-py-0.1.47/unitsnet_py/units/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/force_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62708 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/force_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/fuel_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/heat_transfer_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/irradiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/jerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/kinematic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/leak_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/linear_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42257 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/linear_power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/luminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/luminous_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/luminous_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/magnetic_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/magnetic_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40535 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80144 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/mass_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/mass_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/mass_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/mass_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48955 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/mass_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/molar_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/molar_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/molar_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/molar_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/molarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/permittivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/porous_medium_permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69959 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/power_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73652 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34511 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/pressure_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/ratio_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/reactive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/reactive_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/reciprocal_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18523 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/reciprocal_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/relative_humidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/rotational_acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/rotational_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61867 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/rotational_stiffness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/rotational_stiffness_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/solid_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50352 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/specific_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-20 17:29:21.000000 unitsnet-py-0.1.47/unitsnet_py/units/specific_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/specific_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32699 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/specific_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48511 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/standard_volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/temperature_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/temperature_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/temperature_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/thermal_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/thermal_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/torque_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/turbidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/vitamin_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71514 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/volume_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99718 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/volume_flow_per_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/volume_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22169 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/volumetric_heat_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-20 17:29:22.000000 unitsnet-py-0.1.47/unitsnet_py/units/warping_moment_of_inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:31.221998 unitsnet-py-0.1.47/unitsnet_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-20 17:29:31.000000 unitsnet-py-0.1.47/unitsnet_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-20 17:29:31.000000 unitsnet-py-0.1.47/unitsnet_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:29:31.000000 unitsnet-py-0.1.47/unitsnet_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 17:29:31.000000 unitsnet-py-0.1.47/unitsnet_py.egg-info/top_level.txt
```

### Comparing `unitsnet-py-0.1.46/LICENSE` & `unitsnet-py-0.1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/PKG-INFO` & `unitsnet-py-0.1.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.46
+Version: 0.1.47
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 Keywords: conversion,units-of-measure,units,quantities,unit-converter,converter,unit,measure,measures,measurement,measurements
```

### Comparing `unitsnet-py-0.1.46/README.md` & `unitsnet-py-0.1.47/README.md`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/pyproject.toml` & `unitsnet-py-0.1.47/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitsnet_py"
-version = "0.1.46"
+version = "0.1.47"
 description = "A better way to hold unit variables and easily convert to the destination unit"
 repository = "https://github.com/haimkastner/unitsnet-py"
 authors = ["Haim Kastner <haim.kastner@gmail.com>"]
 maintainers = [
     "Haim Kastner <haim.kastner@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `unitsnet-py-0.1.46/setup.py` & `unitsnet-py-0.1.47/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['unitsnet_py', 'unitsnet_py.units']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'unitsnet-py',
-    'version': '0.1.46',
+    'version': '0.1.47',
     'keywords': 'conversion, units-of-measure, units, quantities, unit-converter, converter, unit, measure, measures, measurement, measurements',
     'description': 'A better way to hold unit variables and easily convert to the destination unit',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Haim Kastner',
     'author_email': 'haim.kastner@gmail.com',
     'maintainer': 'Haim Kastner',
```

### Comparing `unitsnet-py-0.1.46/unitsnet_py/__init__.py` & `unitsnet-py-0.1.47/unitsnet_py/__init__.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py` & `unitsnet-py-0.1.47/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/acceleration.py` & `unitsnet-py-0.1.47/unitsnet_py/units/acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/amount_of_substance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/amount_of_substance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/amplitude_ratio.py` & `unitsnet-py-0.1.47/unitsnet_py/units/amplitude_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/angle.py` & `unitsnet-py-0.1.47/unitsnet_py/units/angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/apparent_energy.py` & `unitsnet-py-0.1.47/unitsnet_py/units/apparent_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/apparent_power.py` & `unitsnet-py-0.1.47/unitsnet_py/units/apparent_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/area.py` & `unitsnet-py-0.1.47/unitsnet_py/units/area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/area_density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/area_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/area_moment_of_inertia.py` & `unitsnet-py-0.1.47/unitsnet_py/units/area_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/bit_rate.py` & `unitsnet-py-0.1.47/unitsnet_py/units/bit_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/brake_specific_fuel_consumption.py` & `unitsnet-py-0.1.47/unitsnet_py/units/brake_specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/capacitance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/capacitance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/coefficient_of_thermal_expansion.py` & `unitsnet-py-0.1.47/unitsnet_py/units/coefficient_of_thermal_expansion.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,197 +4,332 @@
 
 
 class CoefficientOfThermalExpansionUnits(Enum):
         """
             CoefficientOfThermalExpansionUnits enumeration
         """
         
-        InverseKelvin = 'inverse_kelvin'
+        PerKelvin = 'per_kelvin'
         """
             
         """
         
-        InverseDegreeCelsius = 'inverse_degree_celsius'
+        PerDegreeCelsius = 'per_degree_celsius'
         """
             
         """
         
-        InverseDegreeFahrenheit = 'inverse_degree_fahrenheit'
+        PerDegreeFahrenheit = 'per_degree_fahrenheit'
+        """
+            
+        """
+        
+        PpmPerKelvin = 'ppm_per_kelvin'
+        """
+            
+        """
+        
+        PpmPerDegreeCelsius = 'ppm_per_degree_celsius'
+        """
+            
+        """
+        
+        PpmPerDegreeFahrenheit = 'ppm_per_degree_fahrenheit'
         """
             
         """
         
 
 class CoefficientOfThermalExpansion:
     """
     A unit that represents a fractional change in size in response to a change in temperature.
 
     Args:
         value (float): The value.
-        from_unit (CoefficientOfThermalExpansionUnits): The CoefficientOfThermalExpansion unit to create from, The default unit is InverseKelvin
+        from_unit (CoefficientOfThermalExpansionUnits): The CoefficientOfThermalExpansion unit to create from, The default unit is PerKelvin
     """
-    def __init__(self, value: float, from_unit: CoefficientOfThermalExpansionUnits = CoefficientOfThermalExpansionUnits.InverseKelvin):
+    def __init__(self, value: float, from_unit: CoefficientOfThermalExpansionUnits = CoefficientOfThermalExpansionUnits.PerKelvin):
         if math.isnan(value):
             raise ValueError('Invalid unit: value is NaN')
         self.__value = self.__convert_to_base(value, from_unit)
         
-        self.__inverse_kelvin = None
+        self.__per_kelvin = None
+        
+        self.__per_degree_celsius = None
+        
+        self.__per_degree_fahrenheit = None
+        
+        self.__ppm_per_kelvin = None
         
-        self.__inverse_degree_celsius = None
+        self.__ppm_per_degree_celsius = None
         
-        self.__inverse_degree_fahrenheit = None
+        self.__ppm_per_degree_fahrenheit = None
         
 
     def __convert_from_base(self, from_unit: CoefficientOfThermalExpansionUnits) -> float:
         value = self.__value
         
-        if from_unit == CoefficientOfThermalExpansionUnits.InverseKelvin:
+        if from_unit == CoefficientOfThermalExpansionUnits.PerKelvin:
             return (value)
         
-        if from_unit == CoefficientOfThermalExpansionUnits.InverseDegreeCelsius:
+        if from_unit == CoefficientOfThermalExpansionUnits.PerDegreeCelsius:
             return (value)
         
-        if from_unit == CoefficientOfThermalExpansionUnits.InverseDegreeFahrenheit:
+        if from_unit == CoefficientOfThermalExpansionUnits.PerDegreeFahrenheit:
             return (value * 5 / 9)
         
+        if from_unit == CoefficientOfThermalExpansionUnits.PpmPerKelvin:
+            return (value * 1e6)
+        
+        if from_unit == CoefficientOfThermalExpansionUnits.PpmPerDegreeCelsius:
+            return (value * 1e6)
+        
+        if from_unit == CoefficientOfThermalExpansionUnits.PpmPerDegreeFahrenheit:
+            return (value * 5e6 / 9)
+        
         return None
 
 
     def __convert_to_base(self, value: float, to_unit: CoefficientOfThermalExpansionUnits) -> float:
         
-        if to_unit == CoefficientOfThermalExpansionUnits.InverseKelvin:
+        if to_unit == CoefficientOfThermalExpansionUnits.PerKelvin:
             return (value)
         
-        if to_unit == CoefficientOfThermalExpansionUnits.InverseDegreeCelsius:
+        if to_unit == CoefficientOfThermalExpansionUnits.PerDegreeCelsius:
             return (value)
         
-        if to_unit == CoefficientOfThermalExpansionUnits.InverseDegreeFahrenheit:
+        if to_unit == CoefficientOfThermalExpansionUnits.PerDegreeFahrenheit:
             return (value * 9 / 5)
         
+        if to_unit == CoefficientOfThermalExpansionUnits.PpmPerKelvin:
+            return (value / 1e6)
+        
+        if to_unit == CoefficientOfThermalExpansionUnits.PpmPerDegreeCelsius:
+            return (value / 1e6)
+        
+        if to_unit == CoefficientOfThermalExpansionUnits.PpmPerDegreeFahrenheit:
+            return (value * 9 / 5e6)
+        
         return None
 
 
     @property
     def base_value(self) -> float:
         return self.__value
 
     
     @staticmethod
-    def from_inverse_kelvin(inverse_kelvin: float):
+    def from_per_kelvin(per_kelvin: float):
         """
-        Create a new instance of CoefficientOfThermalExpansion from a value in inverse_kelvin.
+        Create a new instance of CoefficientOfThermalExpansion from a value in per_kelvin.
 
         
 
-        :param meters: The CoefficientOfThermalExpansion value in inverse_kelvin.
-        :type inverse_kelvin: float
+        :param meters: The CoefficientOfThermalExpansion value in per_kelvin.
+        :type per_kelvin: float
         :return: A new instance of CoefficientOfThermalExpansion.
         :rtype: CoefficientOfThermalExpansion
         """
-        return CoefficientOfThermalExpansion(inverse_kelvin, CoefficientOfThermalExpansionUnits.InverseKelvin)
+        return CoefficientOfThermalExpansion(per_kelvin, CoefficientOfThermalExpansionUnits.PerKelvin)
 
     
     @staticmethod
-    def from_inverse_degree_celsius(inverse_degree_celsius: float):
+    def from_per_degree_celsius(per_degree_celsius: float):
         """
-        Create a new instance of CoefficientOfThermalExpansion from a value in inverse_degree_celsius.
+        Create a new instance of CoefficientOfThermalExpansion from a value in per_degree_celsius.
 
         
 
-        :param meters: The CoefficientOfThermalExpansion value in inverse_degree_celsius.
-        :type inverse_degree_celsius: float
+        :param meters: The CoefficientOfThermalExpansion value in per_degree_celsius.
+        :type per_degree_celsius: float
         :return: A new instance of CoefficientOfThermalExpansion.
         :rtype: CoefficientOfThermalExpansion
         """
-        return CoefficientOfThermalExpansion(inverse_degree_celsius, CoefficientOfThermalExpansionUnits.InverseDegreeCelsius)
+        return CoefficientOfThermalExpansion(per_degree_celsius, CoefficientOfThermalExpansionUnits.PerDegreeCelsius)
 
     
     @staticmethod
-    def from_inverse_degree_fahrenheit(inverse_degree_fahrenheit: float):
+    def from_per_degree_fahrenheit(per_degree_fahrenheit: float):
         """
-        Create a new instance of CoefficientOfThermalExpansion from a value in inverse_degree_fahrenheit.
+        Create a new instance of CoefficientOfThermalExpansion from a value in per_degree_fahrenheit.
 
         
 
-        :param meters: The CoefficientOfThermalExpansion value in inverse_degree_fahrenheit.
-        :type inverse_degree_fahrenheit: float
+        :param meters: The CoefficientOfThermalExpansion value in per_degree_fahrenheit.
+        :type per_degree_fahrenheit: float
         :return: A new instance of CoefficientOfThermalExpansion.
         :rtype: CoefficientOfThermalExpansion
         """
-        return CoefficientOfThermalExpansion(inverse_degree_fahrenheit, CoefficientOfThermalExpansionUnits.InverseDegreeFahrenheit)
+        return CoefficientOfThermalExpansion(per_degree_fahrenheit, CoefficientOfThermalExpansionUnits.PerDegreeFahrenheit)
+
+    
+    @staticmethod
+    def from_ppm_per_kelvin(ppm_per_kelvin: float):
+        """
+        Create a new instance of CoefficientOfThermalExpansion from a value in ppm_per_kelvin.
+
+        
+
+        :param meters: The CoefficientOfThermalExpansion value in ppm_per_kelvin.
+        :type ppm_per_kelvin: float
+        :return: A new instance of CoefficientOfThermalExpansion.
+        :rtype: CoefficientOfThermalExpansion
+        """
+        return CoefficientOfThermalExpansion(ppm_per_kelvin, CoefficientOfThermalExpansionUnits.PpmPerKelvin)
+
+    
+    @staticmethod
+    def from_ppm_per_degree_celsius(ppm_per_degree_celsius: float):
+        """
+        Create a new instance of CoefficientOfThermalExpansion from a value in ppm_per_degree_celsius.
+
+        
+
+        :param meters: The CoefficientOfThermalExpansion value in ppm_per_degree_celsius.
+        :type ppm_per_degree_celsius: float
+        :return: A new instance of CoefficientOfThermalExpansion.
+        :rtype: CoefficientOfThermalExpansion
+        """
+        return CoefficientOfThermalExpansion(ppm_per_degree_celsius, CoefficientOfThermalExpansionUnits.PpmPerDegreeCelsius)
+
+    
+    @staticmethod
+    def from_ppm_per_degree_fahrenheit(ppm_per_degree_fahrenheit: float):
+        """
+        Create a new instance of CoefficientOfThermalExpansion from a value in ppm_per_degree_fahrenheit.
+
+        
+
+        :param meters: The CoefficientOfThermalExpansion value in ppm_per_degree_fahrenheit.
+        :type ppm_per_degree_fahrenheit: float
+        :return: A new instance of CoefficientOfThermalExpansion.
+        :rtype: CoefficientOfThermalExpansion
+        """
+        return CoefficientOfThermalExpansion(ppm_per_degree_fahrenheit, CoefficientOfThermalExpansionUnits.PpmPerDegreeFahrenheit)
 
     
     @property
-    def inverse_kelvin(self) -> float:
+    def per_kelvin(self) -> float:
         """
         
         """
-        if self.__inverse_kelvin != None:
-            return self.__inverse_kelvin
-        self.__inverse_kelvin = self.__convert_from_base(CoefficientOfThermalExpansionUnits.InverseKelvin)
-        return self.__inverse_kelvin
+        if self.__per_kelvin != None:
+            return self.__per_kelvin
+        self.__per_kelvin = self.__convert_from_base(CoefficientOfThermalExpansionUnits.PerKelvin)
+        return self.__per_kelvin
 
     
     @property
-    def inverse_degree_celsius(self) -> float:
+    def per_degree_celsius(self) -> float:
         """
         
         """
-        if self.__inverse_degree_celsius != None:
-            return self.__inverse_degree_celsius
-        self.__inverse_degree_celsius = self.__convert_from_base(CoefficientOfThermalExpansionUnits.InverseDegreeCelsius)
-        return self.__inverse_degree_celsius
+        if self.__per_degree_celsius != None:
+            return self.__per_degree_celsius
+        self.__per_degree_celsius = self.__convert_from_base(CoefficientOfThermalExpansionUnits.PerDegreeCelsius)
+        return self.__per_degree_celsius
 
     
     @property
-    def inverse_degree_fahrenheit(self) -> float:
+    def per_degree_fahrenheit(self) -> float:
         """
         
         """
-        if self.__inverse_degree_fahrenheit != None:
-            return self.__inverse_degree_fahrenheit
-        self.__inverse_degree_fahrenheit = self.__convert_from_base(CoefficientOfThermalExpansionUnits.InverseDegreeFahrenheit)
-        return self.__inverse_degree_fahrenheit
+        if self.__per_degree_fahrenheit != None:
+            return self.__per_degree_fahrenheit
+        self.__per_degree_fahrenheit = self.__convert_from_base(CoefficientOfThermalExpansionUnits.PerDegreeFahrenheit)
+        return self.__per_degree_fahrenheit
 
     
-    def to_string(self, unit: CoefficientOfThermalExpansionUnits = CoefficientOfThermalExpansionUnits.InverseKelvin) -> string:
+    @property
+    def ppm_per_kelvin(self) -> float:
+        """
+        
+        """
+        if self.__ppm_per_kelvin != None:
+            return self.__ppm_per_kelvin
+        self.__ppm_per_kelvin = self.__convert_from_base(CoefficientOfThermalExpansionUnits.PpmPerKelvin)
+        return self.__ppm_per_kelvin
+
+    
+    @property
+    def ppm_per_degree_celsius(self) -> float:
+        """
+        
+        """
+        if self.__ppm_per_degree_celsius != None:
+            return self.__ppm_per_degree_celsius
+        self.__ppm_per_degree_celsius = self.__convert_from_base(CoefficientOfThermalExpansionUnits.PpmPerDegreeCelsius)
+        return self.__ppm_per_degree_celsius
+
+    
+    @property
+    def ppm_per_degree_fahrenheit(self) -> float:
+        """
+        
+        """
+        if self.__ppm_per_degree_fahrenheit != None:
+            return self.__ppm_per_degree_fahrenheit
+        self.__ppm_per_degree_fahrenheit = self.__convert_from_base(CoefficientOfThermalExpansionUnits.PpmPerDegreeFahrenheit)
+        return self.__ppm_per_degree_fahrenheit
+
+    
+    def to_string(self, unit: CoefficientOfThermalExpansionUnits = CoefficientOfThermalExpansionUnits.PerKelvin) -> string:
         """
         Format the CoefficientOfThermalExpansion to string.
-        Note! the default format for CoefficientOfThermalExpansion is InverseKelvin.
+        Note! the default format for CoefficientOfThermalExpansion is PerKelvin.
         To specify the unit format set the 'unit' parameter.
         """
         
-        if unit == CoefficientOfThermalExpansionUnits.InverseKelvin:
-            return f"""{self.inverse_kelvin} K⁻¹"""
+        if unit == CoefficientOfThermalExpansionUnits.PerKelvin:
+            return f"""{self.per_kelvin} K⁻¹"""
+        
+        if unit == CoefficientOfThermalExpansionUnits.PerDegreeCelsius:
+            return f"""{self.per_degree_celsius} °C⁻¹"""
+        
+        if unit == CoefficientOfThermalExpansionUnits.PerDegreeFahrenheit:
+            return f"""{self.per_degree_fahrenheit} °F⁻¹"""
         
-        if unit == CoefficientOfThermalExpansionUnits.InverseDegreeCelsius:
-            return f"""{self.inverse_degree_celsius} °C⁻¹"""
+        if unit == CoefficientOfThermalExpansionUnits.PpmPerKelvin:
+            return f"""{self.ppm_per_kelvin} ppm/K"""
         
-        if unit == CoefficientOfThermalExpansionUnits.InverseDegreeFahrenheit:
-            return f"""{self.inverse_degree_fahrenheit} °F⁻¹"""
+        if unit == CoefficientOfThermalExpansionUnits.PpmPerDegreeCelsius:
+            return f"""{self.ppm_per_degree_celsius} ppm/°C"""
+        
+        if unit == CoefficientOfThermalExpansionUnits.PpmPerDegreeFahrenheit:
+            return f"""{self.ppm_per_degree_fahrenheit} ppm/°F"""
         
         return f'{self.__value}'
 
 
-    def get_unit_abbreviation(self, unit_abbreviation: CoefficientOfThermalExpansionUnits = CoefficientOfThermalExpansionUnits.InverseKelvin) -> string:
+    def get_unit_abbreviation(self, unit_abbreviation: CoefficientOfThermalExpansionUnits = CoefficientOfThermalExpansionUnits.PerKelvin) -> string:
         """
         Get CoefficientOfThermalExpansion unit abbreviation.
-        Note! the default abbreviation for CoefficientOfThermalExpansion is InverseKelvin.
+        Note! the default abbreviation for CoefficientOfThermalExpansion is PerKelvin.
         To specify the unit abbreviation set the 'unit_abbreviation' parameter.
         """
         
-        if unit_abbreviation == CoefficientOfThermalExpansionUnits.InverseKelvin:
+        if unit_abbreviation == CoefficientOfThermalExpansionUnits.PerKelvin:
             return """K⁻¹"""
         
-        if unit_abbreviation == CoefficientOfThermalExpansionUnits.InverseDegreeCelsius:
+        if unit_abbreviation == CoefficientOfThermalExpansionUnits.PerDegreeCelsius:
             return """°C⁻¹"""
         
-        if unit_abbreviation == CoefficientOfThermalExpansionUnits.InverseDegreeFahrenheit:
+        if unit_abbreviation == CoefficientOfThermalExpansionUnits.PerDegreeFahrenheit:
             return """°F⁻¹"""
         
+        if unit_abbreviation == CoefficientOfThermalExpansionUnits.PpmPerKelvin:
+            return """ppm/K"""
+        
+        if unit_abbreviation == CoefficientOfThermalExpansionUnits.PpmPerDegreeCelsius:
+            return """ppm/°C"""
+        
+        if unit_abbreviation == CoefficientOfThermalExpansionUnits.PpmPerDegreeFahrenheit:
+            return """ppm/°F"""
+        
 
     def __str__(self):
         return self.to_string()
 
 
     def __add__(self, other):
         if not isinstance(other, CoefficientOfThermalExpansion):
```

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/compressibility.py` & `unitsnet-py-0.1.47/unitsnet_py/units/compressibility.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/duration.py` & `unitsnet-py-0.1.47/unitsnet_py/units/duration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/dynamic_viscosity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/dynamic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_admittance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_admittance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_charge.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_charge.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_charge_density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_conductance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_conductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_conductivity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_current.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_current.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_current_density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_current_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_current_gradient.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_current_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_field.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_inductance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_inductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_potential.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_potential.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_ac.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_potential_ac.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_change_rate.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_potential_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_potential_dc.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_potential_dc.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_resistance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_resistivity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_resistivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/electric_surface_charge_density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/electric_surface_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/energy.py` & `unitsnet-py-0.1.47/unitsnet_py/units/energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/energy_density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/energy_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/entropy.py` & `unitsnet-py-0.1.47/unitsnet_py/units/entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/force.py` & `unitsnet-py-0.1.47/unitsnet_py/units/force.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/force_change_rate.py` & `unitsnet-py-0.1.47/unitsnet_py/units/force_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/force_per_length.py` & `unitsnet-py-0.1.47/unitsnet_py/units/force_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/frequency.py` & `unitsnet-py-0.1.47/unitsnet_py/units/frequency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/fuel_efficiency.py` & `unitsnet-py-0.1.47/unitsnet_py/units/fuel_efficiency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/heat_flux.py` & `unitsnet-py-0.1.47/unitsnet_py/units/heat_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/heat_transfer_coefficient.py` & `unitsnet-py-0.1.47/unitsnet_py/units/heat_transfer_coefficient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/illuminance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/illuminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/impulse.py` & `unitsnet-py-0.1.47/unitsnet_py/units/impulse.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/information.py` & `unitsnet-py-0.1.47/unitsnet_py/units/information.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/irradiance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/irradiance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/irradiation.py` & `unitsnet-py-0.1.47/unitsnet_py/units/irradiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/jerk.py` & `unitsnet-py-0.1.47/unitsnet_py/units/jerk.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/kinematic_viscosity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/kinematic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/leak_rate.py` & `unitsnet-py-0.1.47/unitsnet_py/units/leak_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/length.py` & `unitsnet-py-0.1.47/unitsnet_py/units/length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/level.py` & `unitsnet-py-0.1.47/unitsnet_py/units/level.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/linear_density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/linear_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/linear_power_density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/linear_power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/luminance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/luminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/luminosity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/luminosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/luminous_flux.py` & `unitsnet-py-0.1.47/unitsnet_py/units/luminous_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/luminous_intensity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/luminous_intensity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/magnetic_field.py` & `unitsnet-py-0.1.47/unitsnet_py/units/magnetic_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/magnetic_flux.py` & `unitsnet-py-0.1.47/unitsnet_py/units/magnetic_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/magnetization.py` & `unitsnet-py-0.1.47/unitsnet_py/units/magnetization.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/mass.py` & `unitsnet-py-0.1.47/unitsnet_py/units/mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/mass_concentration.py` & `unitsnet-py-0.1.47/unitsnet_py/units/mass_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/mass_flow.py` & `unitsnet-py-0.1.47/unitsnet_py/units/mass_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/mass_flux.py` & `unitsnet-py-0.1.47/unitsnet_py/units/mass_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/mass_fraction.py` & `unitsnet-py-0.1.47/unitsnet_py/units/mass_fraction.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/mass_moment_of_inertia.py` & `unitsnet-py-0.1.47/unitsnet_py/units/mass_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/molar_energy.py` & `unitsnet-py-0.1.47/unitsnet_py/units/molar_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/molar_entropy.py` & `unitsnet-py-0.1.47/unitsnet_py/units/molar_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/molar_flow.py` & `unitsnet-py-0.1.47/unitsnet_py/units/molar_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/molar_mass.py` & `unitsnet-py-0.1.47/unitsnet_py/units/molar_mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/molarity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/molarity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/permeability.py` & `unitsnet-py-0.1.47/unitsnet_py/units/permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/permittivity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/permittivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/porous_medium_permeability.py` & `unitsnet-py-0.1.47/unitsnet_py/units/porous_medium_permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/power.py` & `unitsnet-py-0.1.47/unitsnet_py/units/power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/power_density.py` & `unitsnet-py-0.1.47/unitsnet_py/units/power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/power_ratio.py` & `unitsnet-py-0.1.47/unitsnet_py/units/power_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/pressure.py` & `unitsnet-py-0.1.47/unitsnet_py/units/pressure.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/pressure_change_rate.py` & `unitsnet-py-0.1.47/unitsnet_py/units/pressure_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/ratio.py` & `unitsnet-py-0.1.47/unitsnet_py/units/ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/ratio_change_rate.py` & `unitsnet-py-0.1.47/unitsnet_py/units/ratio_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/reactive_energy.py` & `unitsnet-py-0.1.47/unitsnet_py/units/reactive_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/reactive_power.py` & `unitsnet-py-0.1.47/unitsnet_py/units/reactive_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/reciprocal_area.py` & `unitsnet-py-0.1.47/unitsnet_py/units/reciprocal_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/reciprocal_length.py` & `unitsnet-py-0.1.47/unitsnet_py/units/reciprocal_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/relative_humidity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/relative_humidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/rotational_acceleration.py` & `unitsnet-py-0.1.47/unitsnet_py/units/rotational_acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/rotational_speed.py` & `unitsnet-py-0.1.47/unitsnet_py/units/rotational_speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/rotational_stiffness.py` & `unitsnet-py-0.1.47/unitsnet_py/units/rotational_stiffness.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/rotational_stiffness_per_length.py` & `unitsnet-py-0.1.47/unitsnet_py/units/rotational_stiffness_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/scalar.py` & `unitsnet-py-0.1.47/unitsnet_py/units/scalar.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/solid_angle.py` & `unitsnet-py-0.1.47/unitsnet_py/units/solid_angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/specific_energy.py` & `unitsnet-py-0.1.47/unitsnet_py/units/specific_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/specific_entropy.py` & `unitsnet-py-0.1.47/unitsnet_py/units/specific_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/specific_fuel_consumption.py` & `unitsnet-py-0.1.47/unitsnet_py/units/specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/specific_volume.py` & `unitsnet-py-0.1.47/unitsnet_py/units/specific_volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/specific_weight.py` & `unitsnet-py-0.1.47/unitsnet_py/units/specific_weight.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/speed.py` & `unitsnet-py-0.1.47/unitsnet_py/units/speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/standard_volume_flow.py` & `unitsnet-py-0.1.47/unitsnet_py/units/standard_volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/temperature.py` & `unitsnet-py-0.1.47/unitsnet_py/units/temperature.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/temperature_change_rate.py` & `unitsnet-py-0.1.47/unitsnet_py/units/temperature_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/temperature_delta.py` & `unitsnet-py-0.1.47/unitsnet_py/units/temperature_delta.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/temperature_gradient.py` & `unitsnet-py-0.1.47/unitsnet_py/units/temperature_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/thermal_conductivity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/thermal_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/thermal_resistance.py` & `unitsnet-py-0.1.47/unitsnet_py/units/thermal_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/torque.py` & `unitsnet-py-0.1.47/unitsnet_py/units/torque.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/torque_per_length.py` & `unitsnet-py-0.1.47/unitsnet_py/units/torque_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/turbidity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/turbidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/vitamin_a.py` & `unitsnet-py-0.1.47/unitsnet_py/units/vitamin_a.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/volume.py` & `unitsnet-py-0.1.47/unitsnet_py/units/volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/volume_concentration.py` & `unitsnet-py-0.1.47/unitsnet_py/units/volume_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/volume_flow.py` & `unitsnet-py-0.1.47/unitsnet_py/units/volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/volume_flow_per_area.py` & `unitsnet-py-0.1.47/unitsnet_py/units/volume_flow_per_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/volume_per_length.py` & `unitsnet-py-0.1.47/unitsnet_py/units/volume_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/volumetric_heat_capacity.py` & `unitsnet-py-0.1.47/unitsnet_py/units/volumetric_heat_capacity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py/units/warping_moment_of_inertia.py` & `unitsnet-py-0.1.47/unitsnet_py/units/warping_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.46/unitsnet_py.egg-info/PKG-INFO` & `unitsnet-py-0.1.47/unitsnet_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.46
+Version: 0.1.47
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 Keywords: conversion,units-of-measure,units,quantities,unit-converter,converter,unit,measure,measures,measurement,measurements
```

### Comparing `unitsnet-py-0.1.46/unitsnet_py.egg-info/SOURCES.txt` & `unitsnet-py-0.1.47/unitsnet_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

