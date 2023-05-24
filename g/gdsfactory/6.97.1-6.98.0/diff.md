# Comparing `tmp/gdsfactory-6.97.1.tar.gz` & `tmp/gdsfactory-6.98.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-6.97.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gdsfactory-6.98.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gdsfactory-6.97.1.tar` & `gdsfactory-6.98.0.tar`

### file list

```diff
@@ -1,693 +1,693 @@
--rw-r--r--   0        0        0     1072 2023-05-22 15:57:46.231794 gdsfactory-6.97.1/LICENSE
--rw-r--r--   0        0        0    14319 2023-05-22 15:57:46.231794 gdsfactory-6.97.1/README.md
--rw-r--r--   0        0        0     3583 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/__init__.py
--rw-r--r--   0        0        0     2104 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12629 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3711 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5054 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    15639 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14700 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2884 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2257 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1831 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1856 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/asserts.py
--rw-r--r--   0        0        0    17589 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/cell.py
--rw-r--r--   0        0        0    16040 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/circuitviz.py
--rw-r--r--   0        0        0     5718 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/cli.py
--rw-r--r--   0        0        0   101901 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/component.py
--rw-r--r--   0        0        0    23424 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    29879 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1205 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1144 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/L.py
--rw-r--r--   0        0        0    20964 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2621 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    14087 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3207 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2622 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4705 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4322 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1269 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     2851 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2649 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     7903 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2682 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3787 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5373 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5766 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2929 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1631 2023-05-22 15:57:46.243795 gdsfactory-6.97.1/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1412 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1565 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5722 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8922 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5043 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6118 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2548 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9876 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0     7174 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2113 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     3970 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     3414 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1848 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    12873 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5272 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6450 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3765 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2721 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4288 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2486 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3177 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3245 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4319 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1226 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3471 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2975 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2863 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     8015 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4112 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1214 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1800 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7988 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3290 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     1063 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4682 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7110 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7222 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4961 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4592 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1773 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9058 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1786 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4142 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4685 2023-05-22 15:57:46.247796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3887 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1579 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8811 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3687 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1825 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1244 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1304 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     3873 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2814 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3858 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3299 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4947 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3265 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7579 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2499 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5835 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12214 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4025 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1064 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6342 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3502 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6047 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6327 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3860 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1890 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3833 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1147 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1508 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2972 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1508 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3302 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2642 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1273 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4143 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3272 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2267 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     2846 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_double_bend_coupler.py
--rw-r--r--   0        0        0     3846 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7757 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12137 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2740 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1968 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6868 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2714 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4018 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5267 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2282 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3758 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5871 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16692 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9181 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1733 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5327 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2451 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7914 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     7891 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8090 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     5686 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2809 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3974 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      655 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      820 2023-05-22 15:57:46.251796 gdsfactory-6.97.1/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7730 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3530 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2457 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1215 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1635 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2913 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3821 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3160 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3943 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2468 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2436 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3060 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15612 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4430 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4944 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1088 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     2542 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0     8145 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/config.py
--rw-r--r--   0        0        0      481 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/conftest.py
--rw-r--r--   0        0        0    38409 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/constants.py
--rw-r--r--   0        0        0     1476 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/containers.py
--rw-r--r--   0        0        0    83060 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2982 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/decorators.py
--rw-r--r--   0        0        0     7312 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/difftest.py
--rw-r--r--   0        0        0     1020 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/events.py
--rw-r--r--   0        0        0      267 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     7599 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/export/to_gerber.py
--rw-r--r--   0        0        0     1940 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3058 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0     2976 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/filestorage.py
--rw-r--r--   0        0        0    11890 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/fill.py
--rw-r--r--   0        0        0     7799 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/font.py
--rw-r--r--   0        0        0     8073 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/functions.py
--rw-r--r--   0        0        0       20 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/gdsdiff/.gitattributes
--rw-r--r--   0        0        0       83 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/gdsdiff/.gitconfig
--rw-r--r--   0        0        0       72 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/gdsdiff/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/gdsdiff/gds_diff_git.py
--rw-r--r--   0        0        0     2935 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/gdsdiff/gdsdiff.py
--rw-r--r--   0        0        0      708 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/gdsdiff/install.py
--rw-r--r--   0        0        0      271 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/gdsdiff/sample.py
--rw-r--r--   0        0        0     1059 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/gdsdiff/test_xor.py
--rw-r--r--   0        0        0     1100 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1722 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0      169 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8142 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0      161 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0     6193 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0       27 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/.gitignore
--rw-r--r--   0        0        0      494 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/Makefile
--rw-r--r--   0        0        0     4062 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/README.md
--rw-r--r--   0        0        0     2419 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
--rw-r--r--   0        0        0     9696 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
--rw-r--r--   0        0        0    12379 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
--rw-r--r--   0        0        0     7235 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
--rw-r--r--   0        0        0     3446 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
--rw-r--r--   0        0        0      479 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
--rw-r--r--   0        0        0      582 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
--rw-r--r--   0        0        0      108 2023-05-22 15:57:46.255796 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
--rw-r--r--   0        0        0      186 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
--rw-r--r--   0        0        0      398 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
--rw-r--r--   0        0        0      574 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
--rw-r--r--   0        0        0     6034 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
--rw-r--r--   0        0        0    10704 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
--rw-r--r--   0        0        0      477 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
--rw-r--r--   0        0        0     4337 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
--rw-r--r--   0        0        0      926 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
--rw-r--r--   0        0        0    10945 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      710 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4311 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1854 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
--rw-r--r--   0        0        0     1519 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    41073 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0    40616 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/layers.lyp
--rw-r--r--   0        0        0     5977 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/tech.lyt
--rw-r--r--   0        0        0     4258 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1883 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0     6511 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10780 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0      158 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3814 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1904 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      598 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2719 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2829 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3566 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1904 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     5015 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7084 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1697 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6664 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3685 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3054 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4192 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4812 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3250 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3842 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2510 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2948 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     3023 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/write_connectivity.py
--rw-r--r--   0        0        0    10532 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1158 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23569 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14446 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0      682 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/get_netlist_klayout.py
--rw-r--r--   0        0        0     9745 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/grid.py
--rw-r--r--   0        0        0     4393 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/install.py
--rw-r--r--   0        0        0     1970 2023-05-22 15:57:46.259797 gdsfactory-6.97.1/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3563 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3847 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3810 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4668 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4847 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     1149 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/materials.py
--rw-r--r--   0        0        0     5247 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/name.py
--rw-r--r--   0        0        0    11586 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/pack.py
--rw-r--r--   0        0        0    50930 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/path.py
--rw-r--r--   0        0        0    27294 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6220 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5068 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/pixelate.py
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/dagster/__init__.py
--rw-r--r--   0        0        0      976 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/database/README.md
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/database/__init__.py
--rw-r--r--   0        0        0     6216 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/database/db_upload.py
--rw-r--r--   0        0        0    16143 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/database/models.py
--rw-r--r--   0        0        0       32 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/web/Makefile
--rw-r--r--   0        0        0       23 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/web/__init__.py
--rw-r--r--   0        0        0     4080 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/web/main.py
--rwxr-xr-x   0        0        0     7511 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/web/server.py
--rwxr-xr-x   0        0        0      594 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/web/server_jupyter.py
--rw-r--r--   0        0        0     1299 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/plugins/web/static/client.css
--rw-r--r--   0        0        0    32235 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/port.py
--rw-r--r--   0        0        0    37817 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1285 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1953 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2813 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0    38082 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5897 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5688 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3407 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     3769 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2920 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3015 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3035 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8715 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10624 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     8967 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38948 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3916 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      982 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4415 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2800 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    24342 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8652 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6910 2023-05-22 15:57:46.263797 gdsfactory-6.97.1/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12949 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5284 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1937 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17064 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1510 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9233 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10872 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6119 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2766 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3311 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1854 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34394 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10081 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22568 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8679 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18132 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4379 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14370 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10167 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5072 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2477 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2897 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0     1109 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      710 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      931 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1082 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1631 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2245 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0      955 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1636 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1680 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0      965 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      489 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      533 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      507 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      493 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      569 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      848 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0     1588 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/23_reticle_passives.py
--rw-r--r--   0        0        0      457 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      687 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      692 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1412 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1307 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-05-22 15:57:46.267798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     1988 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      622 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      569 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2260 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0     1014 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4530 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      364 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0     1062 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     4235 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      475 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1880 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1715 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     2206 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     1879 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1283 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     1632 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     1617 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     4497 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     4455 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     2297 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0      316 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/schematic.py
--rw-r--r--   0        0        0    17862 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/schematic_editor.py
--rw-r--r--   0        0        0     4194 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1612 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/show.py
--rw-r--r--   0        0        0      724 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     4369 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/add_simulation_markers.py
--rw-r--r--   0        0        0     2476 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/convert_sparameters.py
--rw-r--r--   0        0        0      547 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/devsim/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/devsim/doping.py
--rw-r--r--   0        0        0    11977 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/devsim/get_simulation.py
--rw-r--r--   0        0        0    23687 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19756 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/devsim/get_solver.py
--rw-r--r--   0        0        0     1644 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/devsim/test_devsim.py
--rw-r--r--   0        0        0      189 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/disable_print.py
--rw-r--r--   0        0        0       79 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/eme/__init__.py
--rw-r--r--   0        0        0    14784 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/eme/meow_eme.py
--rw-r--r--   0        0        0     1787 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/eme/test_meow_simulation.py
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/fem/__init__.py
--rw-r--r--   0        0        0     8968 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/fem/mode_solver.py
--rw-r--r--   0        0        0     2221 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/fem/test_mode_solver.py
--rw-r--r--   0        0        0     3455 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/get_effective_indices.py
--rw-r--r--   0        0        0     3109 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/get_modes_path.py
--rw-r--r--   0        0        0     3888 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/get_sparameters_path.py
--rw-r--r--   0        0        0     2003 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/__init__.py
--rw-r--r--   0        0        0     3194 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_material.py
--rw-r--r--   0        0        0     6137 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6054 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    11014 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15915 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    18182 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12312 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11914 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      832 2023-05-22 15:57:46.271798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6642 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    14053 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21281 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8143 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9577 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1246 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11250 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/mesh.py
--rw-r--r--   0        0        0    11824 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7752 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3605 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/refine.py
--rw-r--r--   0        0        0    10851 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     2513 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14168 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7441 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0    16334 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0     1624 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/get_results.py
--rw-r--r--   0        0        0    20009 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/get_simulation.py
--rw-r--r--   0        0        0    21071 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     2821 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/materials.py
--rw-r--r--   0        0        0    27439 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/modes.py
--rw-r--r--   0        0        0     8941 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/sim_run.yaml
--rw-r--r--   0        0        0     8114 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
--rw-r--r--   0        0        0     8114 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
--rw-r--r--   0        0        0      744 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      879 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_results.py
--rw-r--r--   0        0        0     1505 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
--rw-r--r--   0        0        0     1270 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
--rw-r--r--   0        0        0     9297 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
--rw-r--r--   0        0        0     1732 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1224 2023-05-22 15:57:46.275798 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/utils.py
--rw-r--r--   0        0        0    11034 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/write_sparameters.py
--rw-r--r--   0        0        0     7695 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      588 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/lumerical/__init__.py
--rw-r--r--   0        0        0    16091 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/lumerical/interconnect.py
--rw-r--r--   0        0        0     4286 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/lumerical/settings.py
--rw-r--r--   0        0        0     2368 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/lumerical/test_read_sparameters.py
--rw-r--r--   0        0        0    19865 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1504 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0      932 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/__init__.py
--rw-r--r--   0        0        0     1618 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/coupler.py
--rw-r--r--   0        0        0     4166 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2773 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8924 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/find_modes.py
--rwxr-xr-x   0        0        0     7032 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4458 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2728 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     7148 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4462 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5411 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     8023 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2469 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/overlap.py
--rw-r--r--   0        0        0      418 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0      548 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1137 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      649 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      354 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0    15492 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/types.py
--rw-r--r--   0        0        0     1169 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/modes/waveguide.py
--rw-r--r--   0        0        0     2013 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3069 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0     7332 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/plot.py
--rw-r--r--   0        0        0     2480 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/plot_csv.py
--rw-r--r--   0        0        0      703 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/port_symmetries.py
--rw-r--r--   0        0        0     4685 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/process/diffusion.py
--rw-r--r--   0        0        0     5317 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/process/implant_tables.py
--rw-r--r--   0        0        0     6800 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      191 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/__init__.py
--rw-r--r--   0        0        0    14848 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/build_model.py
--rw-r--r--   0        0        0     7449 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/femwell_waveguide_model.py
--rw-r--r--   0        0        0     1571 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/interpolators.py
--rw-r--r--   0        0        0     6755 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/meep_FDTD_model.py
--rw-r--r--   0        0        0     4528 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/meow_eme_model.py
--rw-r--r--   0        0        0     5613 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/mlp.py
--rw-r--r--   0        0        0     7358 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/models.py
--rw-r--r--   0        0        0    13894 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/parameter.py
--rwxr-xr-x   0        0        0     2225 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/plot_model.py
--rw-r--r--   0        0        0     6805 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/read.py
--rw-r--r--   0        0        0     1350 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2220 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0     1405 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/sax/tests/test_parameters.py
--rw-r--r--   0        0        0     1357 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/add_gc.py
--rw-r--r--   0        0        0     3383 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/circuit.py
--rw-r--r--   0        0        0      891 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/__init__.py
--rw-r--r--   0        0        0     1295 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/bend_circular.py
--rw-r--r--   0        0        0     1388 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/bend_euler.py
--rw-r--r--   0        0        0     2560 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler.py
--rw-r--r--   0        0        0     1046 2023-05-22 15:57:46.279799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler_fdtd.py
--rw-r--r--   0        0        0     1848 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler_ring.py
--rw-r--r--   0        0        0     1329 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
--rw-r--r--   0        0        0      589 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
--rw-r--r--   0        0        0      913 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/gc.py
--rw-r--r--   0        0        0     2032 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mmi1x2.py
--rw-r--r--   0        0        0     1910 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mmi2x2.py
--rw-r--r--   0        0        0     2618 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mzi.py
--rw-r--r--   0        0        0     1759 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mzi_siepic.py
--rw-r--r--   0        0        0      487 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mzi_thermal.py
--rw-r--r--   0        0        0     2597 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/ring_double.py
--rw-r--r--   0        0        0     1665 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/ring_double_siepic.py
--rw-r--r--   0        0        0     1782 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/ring_single.py
--rw-r--r--   0        0        0     1416 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/ring_single_siepic.py
--rw-r--r--   0        0        0     1099 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/straight.py
--rw-r--r--   0        0        0      800 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/get_transmission.py
--rw-r--r--   0        0        0     2516 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/model_from_gdsfactory.py
--rw-r--r--   0        0        0     3841 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/model_from_sparameters.py
--rw-r--r--   0        0        0     2438 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/plot_circuit.py
--rw-r--r--   0        0        0     1798 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
--rw-r--r--   0        0        0     2773 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/plot_model.py
--rw-r--r--   0        0        0     1261 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_circuit.py
--rw-r--r--   0        0        0       90 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
--rw-r--r--   0        0        0     1109 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components.py
--rw-r--r--   0        0        0       66 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
--rw-r--r--   0        0        0       69 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
--rw-r--r--   0        0        0       69 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
--rw-r--r--   0        0        0       92 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
--rw-r--r--   0        0        0       92 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
--rw-r--r--   0        0        0      412 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
--rw-r--r--   0        0        0      412 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
--rw-r--r--   0        0        0      114 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
--rw-r--r--   0        0        0      256 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
--rw-r--r--   0        0        0      460 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
--rw-r--r--   0        0        0      104 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
--rw-r--r--   0        0        0      166 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/simphony/types.py
--rw-r--r--   0        0        0      471 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/sipann/__init__.py
--rw-r--r--   0        0        0     1376 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/sipann/bend_circular.py
--rw-r--r--   0        0        0     1465 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/sipann/bend_euler.py
--rw-r--r--   0        0        0     2508 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/sipann/coupler.py
--rw-r--r--   0        0        0     1892 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/sipann/coupler_ring.py
--rw-r--r--   0        0        0      736 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/sipann/straight.py
--rw-r--r--   0        0        0      100 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/thermal/__init__.py
--rw-r--r--   0        0        0     7789 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/simulation/thermal/heater.py
--rw-r--r--   0        0        0     1744 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/snap.py
--rw-r--r--   0        0        0     4245 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/symbols.py
--rw-r--r--   0        0        0      524 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0     7607 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1078 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    16139 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    42133 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0     1984 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/technology/simulation_settings.py
--rw-r--r--   0        0        0     1635 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/types.py
--rw-r--r--   0        0        0    10008 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/typings.py
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/utils/__init__.py
--rw-r--r--   0        0        0     1342 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/utils/async_utils.py
--rw-r--r--   0        0        0      376 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/utils/color_utils.py
--rw-r--r--   0        0        0      558 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/utils/file_utils.py
--rw-r--r--   0        0        0      185 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/utils/function_utils.py
--rw-r--r--   0        0        0      684 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/utils/xml_utils.py
--rw-r--r--   0        0        0     1453 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/utils/yaml_utils.py
--rw-r--r--   0        0        0     4865 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/watch.py
--rw-r--r--   0        0        0        0 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/widgets/__init__.py
--rw-r--r--   0        0        0     7969 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/widgets/layout_viewer.py
--rw-r--r--   0        0        0     7480 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     5687 2023-05-22 15:57:46.283799 gdsfactory-6.97.1/pyproject.toml
--rw-r--r--   0        0        0    18772 1970-01-01 00:00:00.000000 gdsfactory-6.97.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-24 15:56:43.935856 gdsfactory-6.98.0/LICENSE
+-rw-r--r--   0        0        0    14381 2023-05-24 15:56:43.935856 gdsfactory-6.98.0/README.md
+-rw-r--r--   0        0        0     3583 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     2104 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12629 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3711 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5054 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    15639 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14700 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2884 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2257 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1831 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1856 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    17589 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/cell.py
+-rw-r--r--   0        0        0    16040 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/circuitviz.py
+-rw-r--r--   0        0        0     5718 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/cli.py
+-rw-r--r--   0        0        0   101901 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/component.py
+-rw-r--r--   0        0        0    23424 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    29879 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1205 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1144 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    20964 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2621 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    14087 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3207 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2622 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4705 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4322 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1269 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     2851 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2649 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     7903 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2682 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3787 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5373 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5766 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2929 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1631 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1412 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1565 2023-05-24 15:56:43.947857 gdsfactory-6.98.0/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5722 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8922 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5043 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6118 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2548 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9876 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0     7174 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2113 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     3970 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     3414 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1848 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    12873 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5272 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6450 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3765 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2721 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4288 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2486 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3177 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3245 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4319 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1226 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3471 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2975 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2863 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     8015 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4112 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1214 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1800 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7988 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3290 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     1063 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4682 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7110 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7222 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4961 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4592 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1773 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9058 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1786 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4142 2023-05-24 15:56:43.951856 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4685 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3887 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1579 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8811 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3687 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1825 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1244 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1304 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     3873 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2814 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3858 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3299 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4947 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3265 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7579 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2499 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5835 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12214 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4025 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1064 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6342 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3502 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6047 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6327 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3860 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1890 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3833 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1147 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1508 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2972 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1508 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3302 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2642 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1273 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4143 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3272 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2267 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     2846 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_double_bend_coupler.py
+-rw-r--r--   0        0        0     3846 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7757 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12137 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2740 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1968 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6868 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2714 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4018 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5267 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2282 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3758 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5871 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16692 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9181 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1733 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5327 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2451 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7914 2023-05-24 15:56:43.955857 gdsfactory-6.98.0/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     7891 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8090 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     5686 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2809 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3974 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      655 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      820 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7730 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3530 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2457 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1215 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1635 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2913 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3821 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3160 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3943 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2468 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2436 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3060 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15612 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4430 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4944 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1088 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     2542 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0     8145 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/config.py
+-rw-r--r--   0        0        0      481 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/conftest.py
+-rw-r--r--   0        0        0    38409 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/constants.py
+-rw-r--r--   0        0        0     1476 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/containers.py
+-rw-r--r--   0        0        0    83060 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2982 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     7312 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/difftest.py
+-rw-r--r--   0        0        0     1020 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/events.py
+-rw-r--r--   0        0        0      267 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     7599 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/export/to_gerber.py
+-rw-r--r--   0        0        0     1940 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3058 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0     2976 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/filestorage.py
+-rw-r--r--   0        0        0    11890 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7799 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/font.py
+-rw-r--r--   0        0        0     8073 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/functions.py
+-rw-r--r--   0        0        0       20 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/gdsdiff/.gitattributes
+-rw-r--r--   0        0        0       83 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/gdsdiff/.gitconfig
+-rw-r--r--   0        0        0       72 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/gdsdiff/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/gdsdiff/gds_diff_git.py
+-rw-r--r--   0        0        0     2935 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/gdsdiff/gdsdiff.py
+-rw-r--r--   0        0        0      708 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/gdsdiff/install.py
+-rw-r--r--   0        0        0      271 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/gdsdiff/sample.py
+-rw-r--r--   0        0        0     1059 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/gdsdiff/test_xor.py
+-rw-r--r--   0        0        0     1100 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1722 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8142 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0      161 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0     6193 2023-05-24 15:56:43.959857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0       27 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/.gitignore
+-rw-r--r--   0        0        0      494 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/Makefile
+-rw-r--r--   0        0        0     4062 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12379 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7235 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3446 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    10704 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      477 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0     4337 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
+-rw-r--r--   0        0        0      926 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      710 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4311 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1854 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
+-rw-r--r--   0        0        0     1519 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    41073 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0    40616 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/layers.lyp
+-rw-r--r--   0        0        0     5977 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/tech.lyt
+-rw-r--r--   0        0        0     4258 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1883 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0     6511 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10780 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0      158 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3814 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1904 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      598 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2719 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2829 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3566 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1904 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     5010 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7032 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1697 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6664 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3685 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3054 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4192 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4814 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3250 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3842 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2510 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2948 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     3609 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/write_connectivity.py
+-rw-r--r--   0        0        0    10532 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1158 2023-05-24 15:56:43.963857 gdsfactory-6.98.0/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23569 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14446 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0      682 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/get_netlist_klayout.py
+-rw-r--r--   0        0        0     9745 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/grid.py
+-rw-r--r--   0        0        0     4393 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/install.py
+-rw-r--r--   0        0        0     1970 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3563 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3847 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3810 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4668 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4847 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     1149 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/materials.py
+-rw-r--r--   0        0        0     5247 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/name.py
+-rw-r--r--   0        0        0    11586 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/pack.py
+-rw-r--r--   0        0        0    50930 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/path.py
+-rw-r--r--   0        0        0    27294 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6220 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5068 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/dagster/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/database/README.md
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/database/__init__.py
+-rw-r--r--   0        0        0     6216 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/database/db_upload.py
+-rw-r--r--   0        0        0    16143 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/database/models.py
+-rw-r--r--   0        0        0       32 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/web/Makefile
+-rw-r--r--   0        0        0       23 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/web/__init__.py
+-rw-r--r--   0        0        0     4080 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/web/main.py
+-rwxr-xr-x   0        0        0     7511 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/web/server.py
+-rwxr-xr-x   0        0        0      594 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/web/server_jupyter.py
+-rw-r--r--   0        0        0     1299 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/plugins/web/static/client.css
+-rw-r--r--   0        0        0    32235 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/port.py
+-rw-r--r--   0        0        0    37817 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1285 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1953 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2813 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0    38082 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5897 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5688 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3407 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     3769 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2920 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3015 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3035 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8715 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10624 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     8967 2023-05-24 15:56:43.967857 gdsfactory-6.98.0/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38948 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3916 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      982 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4415 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2800 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    24342 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8652 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6910 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12949 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5284 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1937 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17064 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1510 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9233 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10872 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6119 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2766 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3311 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1854 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34394 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10081 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22568 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8679 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18132 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4379 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14370 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10167 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5072 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2477 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2897 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0     1109 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      710 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      931 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1082 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1631 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2245 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0      955 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1636 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1680 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0      965 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      489 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      533 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      507 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      493 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      569 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      848 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0     1588 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/23_reticle_passives.py
+-rw-r--r--   0        0        0      457 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      687 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      692 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1412 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1307 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-05-24 15:56:43.971857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     1988 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      622 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      569 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2260 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0     1014 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4530 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      364 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0     1065 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     4235 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      475 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1880 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1715 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     2206 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     1879 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1283 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     1632 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     1617 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     4497 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     4455 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     2297 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0      316 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/schematic.py
+-rw-r--r--   0        0        0    17862 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/schematic_editor.py
+-rw-r--r--   0        0        0     4194 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1612 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/show.py
+-rw-r--r--   0        0        0      724 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     4369 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/add_simulation_markers.py
+-rw-r--r--   0        0        0     2476 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/convert_sparameters.py
+-rw-r--r--   0        0        0      547 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/devsim/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/devsim/doping.py
+-rw-r--r--   0        0        0    11977 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/devsim/get_simulation.py
+-rw-r--r--   0        0        0    23687 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19756 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/devsim/get_solver.py
+-rw-r--r--   0        0        0     1644 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/devsim/test_devsim.py
+-rw-r--r--   0        0        0      189 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/disable_print.py
+-rw-r--r--   0        0        0       79 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/eme/__init__.py
+-rw-r--r--   0        0        0    14784 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/eme/meow_eme.py
+-rw-r--r--   0        0        0     1787 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/eme/test_meow_simulation.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/fem/__init__.py
+-rw-r--r--   0        0        0     8968 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/fem/mode_solver.py
+-rw-r--r--   0        0        0     2221 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/fem/test_mode_solver.py
+-rw-r--r--   0        0        0     3455 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/get_effective_indices.py
+-rw-r--r--   0        0        0     3109 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/get_modes_path.py
+-rw-r--r--   0        0        0     3888 2023-05-24 15:56:43.975857 gdsfactory-6.98.0/gdsfactory/simulation/get_sparameters_path.py
+-rw-r--r--   0        0        0     2003 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_material.py
+-rw-r--r--   0        0        0     6137 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6054 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    11014 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15915 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18182 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12312 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11914 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      832 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6642 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    14053 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21281 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8143 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9577 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1246 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11250 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/mesh.py
+-rw-r--r--   0        0        0    11824 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7752 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3605 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/refine.py
+-rw-r--r--   0        0        0    10851 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     2513 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14168 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7441 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0    16334 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0     1624 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/get_results.py
+-rw-r--r--   0        0        0    20009 2023-05-24 15:56:43.979857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21071 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     2821 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/materials.py
+-rw-r--r--   0        0        0    27439 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/modes.py
+-rw-r--r--   0        0        0     8941 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
+-rw-r--r--   0        0        0     8114 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
+-rw-r--r--   0        0        0     8114 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
+-rw-r--r--   0        0        0      744 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      879 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     1505 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
+-rw-r--r--   0        0        0     1655 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
+-rw-r--r--   0        0        0     9297 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     1732 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1224 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/utils.py
+-rw-r--r--   0        0        0    10841 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     7695 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0      588 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/lumerical/__init__.py
+-rw-r--r--   0        0        0    16091 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4286 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/lumerical/settings.py
+-rw-r--r--   0        0        0     2368 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
+-rw-r--r--   0        0        0    19865 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1504 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0      932 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/__init__.py
+-rw-r--r--   0        0        0     1618 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/coupler.py
+-rw-r--r--   0        0        0     4166 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2773 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8924 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/find_modes.py
+-rwxr-xr-x   0        0        0     7032 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4458 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2728 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7148 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4462 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5411 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     8023 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2469 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/overlap.py
+-rw-r--r--   0        0        0      418 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0      548 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1137 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      649 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      354 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0    15492 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/types.py
+-rw-r--r--   0        0        0     1169 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/modes/waveguide.py
+-rw-r--r--   0        0        0     2013 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3069 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0     7332 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/plot.py
+-rw-r--r--   0        0        0     2480 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/plot_csv.py
+-rw-r--r--   0        0        0      613 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/port_symmetries.py
+-rw-r--r--   0        0        0     4685 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/process/diffusion.py
+-rw-r--r--   0        0        0     5317 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/process/implant_tables.py
+-rw-r--r--   0        0        0     6800 2023-05-24 15:56:43.983857 gdsfactory-6.98.0/gdsfactory/simulation/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      191 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/__init__.py
+-rw-r--r--   0        0        0    14848 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/build_model.py
+-rw-r--r--   0        0        0     7449 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     1571 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/interpolators.py
+-rw-r--r--   0        0        0     6755 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4528 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/meow_eme_model.py
+-rw-r--r--   0        0        0     5613 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/mlp.py
+-rw-r--r--   0        0        0     7358 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/models.py
+-rw-r--r--   0        0        0    13894 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/parameter.py
+-rwxr-xr-x   0        0        0     2225 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/plot_model.py
+-rw-r--r--   0        0        0     6805 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/read.py
+-rw-r--r--   0        0        0     1350 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2220 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0     1405 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0     1357 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/add_gc.py
+-rw-r--r--   0        0        0     3383 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/circuit.py
+-rw-r--r--   0        0        0      891 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/__init__.py
+-rw-r--r--   0        0        0     1295 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/bend_circular.py
+-rw-r--r--   0        0        0     1388 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/bend_euler.py
+-rw-r--r--   0        0        0     2560 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler.py
+-rw-r--r--   0        0        0     1046 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
+-rw-r--r--   0        0        0     1848 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler_ring.py
+-rw-r--r--   0        0        0     1329 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
+-rw-r--r--   0        0        0      589 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
+-rw-r--r--   0        0        0      913 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/gc.py
+-rw-r--r--   0        0        0     2032 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mmi1x2.py
+-rw-r--r--   0        0        0     1910 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mmi2x2.py
+-rw-r--r--   0        0        0     2618 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mzi.py
+-rw-r--r--   0        0        0     1759 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
+-rw-r--r--   0        0        0      487 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
+-rw-r--r--   0        0        0     2597 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/ring_double.py
+-rw-r--r--   0        0        0     1665 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
+-rw-r--r--   0        0        0     1782 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/ring_single.py
+-rw-r--r--   0        0        0     1416 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
+-rw-r--r--   0        0        0     1099 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/straight.py
+-rw-r--r--   0        0        0      800 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/get_transmission.py
+-rw-r--r--   0        0        0     2516 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
+-rw-r--r--   0        0        0     3841 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/model_from_sparameters.py
+-rw-r--r--   0        0        0     2438 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/plot_circuit.py
+-rw-r--r--   0        0        0     1798 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
+-rw-r--r--   0        0        0     2773 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/plot_model.py
+-rw-r--r--   0        0        0     1261 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_circuit.py
+-rw-r--r--   0        0        0       90 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
+-rw-r--r--   0        0        0     1109 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components.py
+-rw-r--r--   0        0        0       66 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
+-rw-r--r--   0        0        0       69 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
+-rw-r--r--   0        0        0       69 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
+-rw-r--r--   0        0        0       92 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
+-rw-r--r--   0        0        0       92 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
+-rw-r--r--   0        0        0      412 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
+-rw-r--r--   0        0        0      412 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
+-rw-r--r--   0        0        0      114 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
+-rw-r--r--   0        0        0      256 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
+-rw-r--r--   0        0        0      460 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
+-rw-r--r--   0        0        0      104 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
+-rw-r--r--   0        0        0      166 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/simphony/types.py
+-rw-r--r--   0        0        0      471 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sipann/__init__.py
+-rw-r--r--   0        0        0     1376 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sipann/bend_circular.py
+-rw-r--r--   0        0        0     1465 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sipann/bend_euler.py
+-rw-r--r--   0        0        0     2508 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sipann/coupler.py
+-rw-r--r--   0        0        0     1892 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sipann/coupler_ring.py
+-rw-r--r--   0        0        0      736 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/sipann/straight.py
+-rw-r--r--   0        0        0      100 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/thermal/__init__.py
+-rw-r--r--   0        0        0     7789 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/simulation/thermal/heater.py
+-rw-r--r--   0        0        0     1744 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4245 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      524 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0     7607 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1078 2023-05-24 15:56:43.987857 gdsfactory-6.98.0/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    16139 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    42133 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0     1984 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/technology/simulation_settings.py
+-rw-r--r--   0        0        0     1635 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/types.py
+-rw-r--r--   0        0        0    10008 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/typings.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/utils/__init__.py
+-rw-r--r--   0        0        0     1342 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/utils/async_utils.py
+-rw-r--r--   0        0        0      376 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/utils/color_utils.py
+-rw-r--r--   0        0        0      558 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/utils/file_utils.py
+-rw-r--r--   0        0        0      185 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/utils/function_utils.py
+-rw-r--r--   0        0        0      684 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/utils/xml_utils.py
+-rw-r--r--   0        0        0     1453 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/utils/yaml_utils.py
+-rw-r--r--   0        0        0     4865 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/watch.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/widgets/__init__.py
+-rw-r--r--   0        0        0     7969 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/widgets/layout_viewer.py
+-rw-r--r--   0        0        0     7480 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     5706 2023-05-24 15:56:43.991857 gdsfactory-6.98.0/pyproject.toml
+-rw-r--r--   0        0        0    18870 1970-01-01 00:00:00.000000 gdsfactory-6.98.0/PKG-INFO
```

### Comparing `gdsfactory-6.97.1/LICENSE` & `gdsfactory-6.98.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/README.md` & `gdsfactory-6.98.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gdsfactory 6.97.1
+# gdsfactory 6.98.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
@@ -100,15 +100,15 @@
 ![anaconda prompt](https://i.imgur.com/Fyal5sT.png)
 
 ```
 pip install gdsfactory --upgrade
 gf install klayout-integration
 ```
 
-Then you need to restart Klayout to make sure you activate the klayout gdsfactory integration.
+Then you can install Klayout-live `klive` integration in the klayout GUI `Tools --> Manage Packages --> Install New Packages --> Klive` and restart klayout.
 
 ### 2. Installation for developers
 
 For developers you need to fork the GitHub repository, git clone it (download it), git add, git commit, git push your improvement. Then pull request your changes to the main branch from the GitHub website.
 For that you can install gdsfactory locally on your computer in `-e` edit mode.
 
 ```
```

### Comparing `gdsfactory-6.97.1/gdsfactory/__init__.py` & `gdsfactory-6.98.0/gdsfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,8 +148,8 @@
     "snap",
     "typings",
     "technology",
     "write_cells",
     "xsection",
     "PATH",
 )
-__version__ = "6.97.1"
+__version__ = "6.98.0"
```

### Comparing `gdsfactory-6.97.1/gdsfactory/add_keepout.py` & `gdsfactory-6.98.0/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/add_labels.py` & `gdsfactory-6.98.0/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/add_loopback.py` & `gdsfactory-6.98.0/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/add_padding.py` & `gdsfactory-6.98.0/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/add_pins.py` & `gdsfactory-6.98.0/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/add_ports.py` & `gdsfactory-6.98.0/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/add_tapers.py` & `gdsfactory-6.98.0/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-6.98.0/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/add_termination.py` & `gdsfactory-6.98.0/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/asserts.py` & `gdsfactory-6.98.0/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/cell.py` & `gdsfactory-6.98.0/gdsfactory/cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/circuitviz.py` & `gdsfactory-6.98.0/gdsfactory/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/cli.py` & `gdsfactory-6.98.0/gdsfactory/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "6.97.1"
+VERSION = "6.98.0"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `gdsfactory-6.97.1/gdsfactory/component.py` & `gdsfactory-6.98.0/gdsfactory/component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/component_layout.py` & `gdsfactory-6.98.0/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/component_reference.py` & `gdsfactory-6.98.0/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/C.py` & `gdsfactory-6.98.0/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/L.py` & `gdsfactory-6.98.0/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/__init__.py` & `gdsfactory-6.98.0/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/add_fiducials.py` & `gdsfactory-6.98.0/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-6.98.0/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/add_trenches.py` & `gdsfactory-6.98.0/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/align.py` & `gdsfactory-6.98.0/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/array_component.py` & `gdsfactory-6.98.0/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/array_with_fanout.py` & `gdsfactory-6.98.0/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/array_with_via.py` & `gdsfactory-6.98.0/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/awg.py` & `gdsfactory-6.98.0/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/bbox.py` & `gdsfactory-6.98.0/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/bend_circular.py` & `gdsfactory-6.98.0/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-6.98.0/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/bend_euler.py` & `gdsfactory-6.98.0/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/bend_port.py` & `gdsfactory-6.98.0/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/bend_s.py` & `gdsfactory-6.98.0/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/bezier.py` & `gdsfactory-6.98.0/gdsfactory/components/bezier.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cavity.py` & `gdsfactory-6.98.0/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cdc.py` & `gdsfactory-6.98.0/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cdsem_all.py` & `gdsfactory-6.98.0/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-6.98.0/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-6.98.0/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cdsem_straight.py` & `gdsfactory-6.98.0/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-6.98.0/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/circle.py` & `gdsfactory-6.98.0/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-6.98.0/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-6.98.0/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-6.98.0/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-6.98.0/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/compass.py` & `gdsfactory-6.98.0/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/component_lattice.py` & `gdsfactory-6.98.0/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/component_sequence.py` & `gdsfactory-6.98.0/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/copy_layers.py` & `gdsfactory-6.98.0/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler90.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler90bend.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler_full.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler_ring.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler_straight.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-6.98.0/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cross.py` & `gdsfactory-6.98.0/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-6.98.0/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-6.98.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-6.98.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cutback_2x2.py` & `gdsfactory-6.98.0/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cutback_bend.py` & `gdsfactory-6.98.0/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cutback_component.py` & `gdsfactory-6.98.0/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/cutback_splitter.py` & `gdsfactory-6.98.0/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/dbr.py` & `gdsfactory-6.98.0/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/dbr_tapered.py` & `gdsfactory-6.98.0/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/delay_snake.py` & `gdsfactory-6.98.0/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/delay_snake2.py` & `gdsfactory-6.98.0/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/delay_snake3.py` & `gdsfactory-6.98.0/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-6.98.0/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/dicing_lane.py` & `gdsfactory-6.98.0/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/die.py` & `gdsfactory-6.98.0/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/die_bbox.py` & `gdsfactory-6.98.0/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-6.98.0/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/disk.py` & `gdsfactory-6.98.0/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-6.98.0/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ellipse.py` & `gdsfactory-6.98.0/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/extend_ports_list.py` & `gdsfactory-6.98.0/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/extension.py` & `gdsfactory-6.98.0/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/fiber.py` & `gdsfactory-6.98.0/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/fiber_array.py` & `gdsfactory-6.98.0/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/fiducial_squares.py` & `gdsfactory-6.98.0/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-6.98.0/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_elliptical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-6.98.0/gdsfactory/components/grating_coupler_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/greek_cross.py` & `gdsfactory-6.98.0/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/hline.py` & `gdsfactory-6.98.0/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-6.98.0/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/litho_calipers.py` & `gdsfactory-6.98.0/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/litho_ruler.py` & `gdsfactory-6.98.0/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/litho_steps.py` & `gdsfactory-6.98.0/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/logo.py` & `gdsfactory-6.98.0/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/loop_mirror.py` & `gdsfactory-6.98.0/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mmi1x2.py` & `gdsfactory-6.98.0/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-6.98.0/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mmi2x2.py` & `gdsfactory-6.98.0/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-6.98.0/gdsfactory/components/mmi2x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-6.98.0/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mode_converter.py` & `gdsfactory-6.98.0/gdsfactory/components/mode_converter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzi.py` & `gdsfactory-6.98.0/gdsfactory/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzi_arm.py` & `gdsfactory-6.98.0/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzi_arms.py` & `gdsfactory-6.98.0/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzi_lattice.py` & `gdsfactory-6.98.0/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-6.98.0/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-6.98.0/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzit.py` & `gdsfactory-6.98.0/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzit_lattice.py` & `gdsfactory-6.98.0/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/mzm.py` & `gdsfactory-6.98.0/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/nxn.py` & `gdsfactory-6.98.0/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/optimal_90deg.py` & `gdsfactory-6.98.0/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-6.98.0/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/optimal_step.py` & `gdsfactory-6.98.0/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/pack_doe.py` & `gdsfactory-6.98.0/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/pad.py` & `gdsfactory-6.98.0/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/pad_gsg.py` & `gdsfactory-6.98.0/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/pads_shorted.py` & `gdsfactory-6.98.0/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-6.98.0/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ramp.py` & `gdsfactory-6.98.0/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/rectangle.py` & `gdsfactory-6.98.0/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-6.98.0/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/regular_polygon.py` & `gdsfactory-6.98.0/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/resistance_meander.py` & `gdsfactory-6.98.0/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/resistance_sheet.py` & `gdsfactory-6.98.0/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring.py` & `gdsfactory-6.98.0/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_crow.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_double.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_double_bend_coupler.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_double_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_double_heater.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_double_pn.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_section_based.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_single.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_single_array.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_single_dut.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_single_heater.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/ring_single_pn.py` & `gdsfactory-6.98.0/gdsfactory/components/ring_single_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/seal_ring.py` & `gdsfactory-6.98.0/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/snspd.py` & `gdsfactory-6.98.0/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/spiral_double.py` & `gdsfactory-6.98.0/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/spiral_external_io.py` & `gdsfactory-6.98.0/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/spiral_heater.py` & `gdsfactory-6.98.0/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-6.98.0/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/splitter_chain.py` & `gdsfactory-6.98.0/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/splitter_tree.py` & `gdsfactory-6.98.0/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight.py` & `gdsfactory-6.98.0/gdsfactory/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_array.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_pin.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/straight_rib.py` & `gdsfactory-6.98.0/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/switch_tree.py` & `gdsfactory-6.98.0/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/taper.py` & `gdsfactory-6.98.0/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-6.98.0/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/taper_cross_section.py` & `gdsfactory-6.98.0/gdsfactory/components/taper_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/taper_from_csv.py` & `gdsfactory-6.98.0/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/taper_parabolic.py` & `gdsfactory-6.98.0/gdsfactory/components/taper_parabolic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/terminator.py` & `gdsfactory-6.98.0/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/text.py` & `gdsfactory-6.98.0/gdsfactory/components/text.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/text_freetype.py` & `gdsfactory-6.98.0/gdsfactory/components/text_freetype.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/text_rectangular.py` & `gdsfactory-6.98.0/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-6.98.0/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/triangles.py` & `gdsfactory-6.98.0/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/verniers.py` & `gdsfactory-6.98.0/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/version_stamp.py` & `gdsfactory-6.98.0/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/via.py` & `gdsfactory-6.98.0/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/via_corner.py` & `gdsfactory-6.98.0/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/via_cutback.py` & `gdsfactory-6.98.0/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/via_stack.py` & `gdsfactory-6.98.0/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/via_stack_slot.py` & `gdsfactory-6.98.0/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-6.98.0/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/wafer.py` & `gdsfactory-6.98.0/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/wire.py` & `gdsfactory-6.98.0/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/components/wire_sbend.py` & `gdsfactory-6.98.0/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/config.py` & `gdsfactory-6.98.0/gdsfactory/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from loguru import logger
 import omegaconf
 from omegaconf import OmegaConf
 
 from rich.console import Console
 from rich.table import Table
 
-__version__ = "6.97.1"
+__version__ = "6.98.0"
 PathType = Union[str, pathlib.Path]
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
```

### Comparing `gdsfactory-6.97.1/gdsfactory/constants.py` & `gdsfactory-6.98.0/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/containers.py` & `gdsfactory-6.98.0/gdsfactory/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/cross_section.py` & `gdsfactory-6.98.0/gdsfactory/cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/decorators.py` & `gdsfactory-6.98.0/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/difftest.py` & `gdsfactory-6.98.0/gdsfactory/difftest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/events.py` & `gdsfactory-6.98.0/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/export/to_3d.py` & `gdsfactory-6.98.0/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/export/to_gerber.py` & `gdsfactory-6.98.0/gdsfactory/export/to_gerber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/export/to_np.py` & `gdsfactory-6.98.0/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/export/to_stl.py` & `gdsfactory-6.98.0/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/filestorage.py` & `gdsfactory-6.98.0/gdsfactory/filestorage.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/fill.py` & `gdsfactory-6.98.0/gdsfactory/fill.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/font.py` & `gdsfactory-6.98.0/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/functions.py` & `gdsfactory-6.98.0/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/gdsdiff/gds_diff_git.py` & `gdsfactory-6.98.0/gdsfactory/gdsdiff/gds_diff_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/gdsdiff/gdsdiff.py` & `gdsfactory-6.98.0/gdsfactory/gdsdiff/gdsdiff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/gdsdiff/install.py` & `gdsfactory-6.98.0/gdsfactory/gdsdiff/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/gdsdiff/test_xor.py` & `gdsfactory-6.98.0/gdsfactory/gdsdiff/test_xor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/README.md` & `gdsfactory-6.98.0/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/__init__.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 1% similar despite different names*

#### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>6.97.1</version>
+  <version>6.98.0</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/README.md` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/run_lvs.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 16% similar despite different names*

#### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;6.97.1&quot;
+__version__ = &quot;6.98.0&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/layers.lyp` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/layers.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/tech.lyt` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-6.98.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/layer_stack.py` & `gdsfactory-6.98.0/gdsfactory/generic_tech/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-6.98.0/gdsfactory/generic_tech/layer_views.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/__init__.py` & `gdsfactory-6.98.0/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/boolean.py` & `gdsfactory-6.98.0/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-6.98.0/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-6.98.0/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-6.98.0/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-6.98.0/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-6.98.0/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/check_space.py` & `gdsfactory-6.98.0/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/check_width.py` & `gdsfactory-6.98.0/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-6.98.0/gdsfactory/geometry/fill_klayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         fill_spacing: fill pitch in x and y.
         fill_name: name of the cell containing all fill cells. Defaults to Cell_fill.
         gdspath_out: Optional GDS output. Defaults to input.
     """
     import kfactory as kf
     import klayout.db as kdb
 
-    lib = kf.klib
+    lib = kf.kcl
     lib.read(filename=str(gdspath))
     cell = lib[cell_name or 0]
     fill_name = fill_name or f"{cell.name}_fill"
 
     c = kf.KCell(fill_name)
 
     if create_new_fill_cell:
@@ -56,36 +56,36 @@
         if not fill_layers:
             raise ValueError(
                 "You need to pass fill_layers if create_new_fill_cell=True"
             )
         fill_cell = kf.KCell(fill_cell_name)
         for layer in fill_layers:
             layer = gf.get_layer(layer)
-            layer = kf.klib.layer(*layer)
-            fill_cell << kf.pcells.waveguide.waveguide(
+            layer = kf.kcl.layer(*layer)
+            fill_cell << kf.cells.waveguide.waveguide(
                 width=fill_size[0], length=fill_size[1], layer=layer
             )
     else:
         fill_cell = lib[fill_cell_name]
 
     fill_cell_index = fill_cell.cell_index()  # fill cell index
     fill_cell_box = fill_cell.bbox().enlarged(
         fill_spacing[0] / 2 * 1e3, fill_spacing[1] / 2 * 1e3
     )
     fill_margin = kf.kdb.Point(0, 0)
 
     layer_to_fill = gf.get_layer(layer_to_fill)
-    layer_to_fill = cell.klib.layer(*layer_to_fill)
+    layer_to_fill = cell.kcl.layer(*layer_to_fill)
     region = kdb.Region()
     region_avoid_all = kdb.Region()
 
     if layers_to_avoid:
         for layer, margin in layers_to_avoid:
             layer = gf.get_layer(layer)
-            layer = kf.klib.layer(*layer)
+            layer = kf.kcl.layer(*layer)
             region_avoid = kdb.Region()
             region_avoid.insert(
                 cell.begin_shapes_rec(layer)
             ) if layer != layer_to_fill else None
             region_avoid = region_avoid.size(margin * 1e3)
             region_avoid_all = region_avoid_all + region_avoid
```

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-6.98.0/gdsfactory/geometry/fill_tiled.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Iterable, Optional
 
 try:
     import kfactory as kf
-    from kfactory import KCell, KLib, LayerEnum, kdb
+    from kfactory import KCell, KCLayout, LayerEnum, kdb
     from kfactory.config import logger
 except ImportError as e:
     print(
         "You can install `pip install gdsfactory[full]` for using maskprep. "
         "And make sure you use python >= 3.10"
     )
     raise e
 
 
 class FillOperator(kdb.TileOutputReceiver):
     def __init__(
         self,
-        klib: KLib,
+        kcl: KCLayout,
         top_cell: KCell,
         fill_cell_index: int,
         fc_bbox: kdb.Box,
         row_step: kdb.Vector,
         column_step: kdb.Vector,
         fill_margin: kdb.Vector = kdb.Vector(0, 0),
         remaining_polygons: Optional[kdb.Region] = None,
     ) -> None:
-        self.klib = klib
+        self.kcl = kcl
         self.top_cell = top_cell
         self.fill_cell_index = fill_cell_index
         self.fc_bbox = fc_bbox
         self.row_step = row_step
         self.column_step = column_step
         self.fill_margin = fill_margin
         self.remaining_polygons = remaining_polygons
@@ -67,89 +67,87 @@
     exclude_regions: Iterable[tuple[kdb.Region, int]] = [],
     n_threads: int = 4,
     tile_size: Optional[tuple[float, float]] = None,
     x_space: float = 0,
     y_space: float = 0,
 ) -> None:
     tp = kdb.TilingProcessor()
-    tp.frame = c.bbox().to_dtype(c.klib.dbu)  # type: ignore
-    tp.dbu = c.klib.dbu
+    tp.frame = c.bbox().to_dtype(c.kcl.dbu)  # type: ignore
+    tp.dbu = c.kcl.dbu
     tp.threads = n_threads
 
     if tile_size is None:
         tile_size = (
             100 * (fill_cell.dbbox().width() + x_space),
             100 * (fill_cell.dbbox().height() + y_space),
         )
     tp.tile_size(*tile_size)
 
     layer_names: list[str] = []
     for layer, _ in fill_layers:
         layer_name = f"layer{layer}"
-        tp.input(layer_name, c.klib, c.cell_index(), c.klib.get_info(layer))
+        tp.input(layer_name, c.kcl, c.cell_index(), c.kcl.get_info(layer))
         layer_names.append(layer_name)
 
     region_names: list[str] = []
     for i, (r, _) in enumerate(fill_regions):
         region_name = f"region{i}"
         tp.input(region_name, r)
         region_names.append(region_name)
 
     exlayer_names: list[str] = []
     for layer, _ in exclude_layers:
         layer_name = f"layer{layer}"
-        tp.input(layer_name, c.klib, c.cell_index(), c.klib.get_info(layer))
+        tp.input(layer_name, c.kcl, c.cell_index(), c.kcl.get_info(layer))
         exlayer_names.append(layer_name)
 
     exregion_names: list[str] = []
     for i, (r, _) in enumerate(exclude_regions):
         region_name = f"region{i}"
         tp.input(region_name, r)
         exregion_names.append(region_name)
 
     tp.output(
         "to_fill",
         FillOperator(
-            c.klib,
+            c.kcl,
             c,
             fill_cell.cell_index(),
             fc_bbox=fill_cell.bbox(),
-            row_step=kdb.Vector(
-                fill_cell.bbox().width() + int(x_space / c.klib.dbu), 0
-            ),
+            row_step=kdb.Vector(fill_cell.bbox().width() + int(x_space / c.kcl.dbu), 0),
             column_step=kdb.Vector(
-                0, fill_cell.bbox().height() + int(y_space / c.klib.dbu)
+                0, fill_cell.bbox().height() + int(y_space / c.kcl.dbu)
             ),
         ),
     )
 
     if layer_names or region_names:
         exlayers = " + ".join(
             [
-                layer_name + f".sized({int(size / c.klib.dbu)})" if size else layer_name
+                layer_name + f".sized({int(size / c.kcl.dbu)})" if size else layer_name
                 for layer_name, (_, size) in zip(exlayer_names, exclude_layers)
             ]
         )
         exregions = " + ".join(
             [
-                region_name + f".sized({int(size / c.klib.dbu)})"
+                region_name + f".sized({int(size / c.kcl.dbu)})"
                 if size
                 else region_name
                 for region_name, (_, size) in zip(exregion_names, exclude_regions)
             ]
         )
         layers = " + ".join(
             [
-                layer_name + f".sized({int(size / c.klib.dbu)})" if size else layer_name
+                layer_name + f".sized({int(size / c.kcl.dbu)})" if size else layer_name
                 for layer_name, (_, size) in zip(layer_names, fill_layers)
             ]
         )
         regions = " + ".join(
             [
-                region_name + f".sized({int(size / c.klib.dbu)})"
+                region_name + f".sized({int(size / c.kcl.dbu)})"
                 if size
                 else region_name
                 for region_name, (_, size) in zip(region_names, fill_regions)
             ]
         )
 
         if exlayer_names or exregion_names:
@@ -175,51 +173,51 @@
                     " + ".join([layers, regions])
                     if regions and layers
                     else regions + layers
                 )
                 + "; var fill_region = _tile & _frame & fill; _output(to_fill, fill_region)"
             )
         tp.queue(queue_str)
-        c.klib.start_changes()
+        c.kcl.start_changes()
         try:
             logger.info("filling {} with {}", c.name, fill_cell.name)
             logger.debug("fill string: '{}'", queue_str)
             tp.execute(f"Fill {c.name}")
             logger.info("done with filling {}", c.name)
         finally:
-            c.klib.end_changes()
+            c.kcl.end_changes()
 
 
 if __name__ == "__main__":
     import gdsfactory.geometry.fill_tiled as fill
     import gdsfactory as gf
 
     c = kf.KCell("ToFill")
-    c.shapes(kf.klib.layer(1, 0)).insert(
+    c.shapes(kf.kcl.layer(1, 0)).insert(
         kf.kdb.DPolygon.ellipse(kf.kdb.DBox(5000, 3000), 512)
     )
-    c.shapes(kf.klib.layer(10, 0)).insert(
+    c.shapes(kf.kcl.layer(10, 0)).insert(
         kf.kdb.DPolygon(
             [kf.kdb.DPoint(0, 0), kf.kdb.DPoint(5000, 0), kf.kdb.DPoint(5000, 3000)]
         )
     )
 
     fc = kf.KCell("fill")
-    fc.shapes(fc.klib.layer(2, 0)).insert(kf.kdb.DBox(20, 40))
-    fc.shapes(fc.klib.layer(3, 0)).insert(kf.kdb.DBox(30, 15))
+    fc.shapes(fc.kcl.layer(2, 0)).insert(kf.kdb.DBox(20, 40))
+    fc.shapes(fc.kcl.layer(3, 0)).insert(kf.kdb.DBox(30, 15))
 
-    # fill.fill_tiled(c, fc, [(kf.klib.layer(1,0), 0)], exclude_layers = [(kf.klib.layer(10,0), 100), (kf.klib.layer(2,0), 0), (kf.klib.layer(3,0),0)], x_space=5, y_space=5)
+    # fill.fill_tiled(c, fc, [(kf.kcl.layer(1,0), 0)], exclude_layers = [(kf.kcl.layer(10,0), 100), (kf.kcl.layer(2,0), 0), (kf.kcl.layer(3,0),0)], x_space=5, y_space=5)
     fill.fill_tiled(
         c,
         fc,
-        [(kf.klib.layer(1, 0), 0)],
+        [(kf.kcl.layer(1, 0), 0)],
         exclude_layers=[
-            (kf.klib.layer(10, 0), 100),
-            (kf.klib.layer(2, 0), 0),
-            (kf.klib.layer(3, 0), 0),
+            (kf.kcl.layer(10, 0), 100),
+            (kf.kcl.layer(2, 0), 0),
+            (kf.kcl.layer(3, 0), 0),
         ],
         x_space=5,
         y_space=5,
     )
 
     gdspath = "mzi_fill.gds"
     c.write(gdspath)
```

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/fillet.py` & `gdsfactory-6.98.0/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/functions.py` & `gdsfactory-6.98.0/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/invert.py` & `gdsfactory-6.98.0/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/layer_priority.py` & `gdsfactory-6.98.0/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/manhattanize.py` & `gdsfactory-6.98.0/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/maskprep.py` & `gdsfactory-6.98.0/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-6.98.0/gdsfactory/geometry/maskprep_flat.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         layermap: dict of layernames to layer numbers {'WG': (1, 0)}
         filepath: to read GDS from.
     """
 
     def __init__(
         self, layermap: Dict[str, Layer], filepath: Optional[PathType] = None
     ) -> None:
-        lib = kf.kcell.KLib()
+        lib = kf.kcell.KCLayout()
         lib.read(filename=str(filepath))
         c = lib[0]
 
         for layername, layer in layermap.items():
             region = Region()
             layer = lib.layer(layer[0], layer[1])
             region.insert(c.begin_shapes_rec(layer))
@@ -123,16 +123,16 @@
             fill_layers: layers of the fill cell (can be multiple).
             fill_name: fill cell name.
             fill_cell_name: fill cell name.
         """
 
         fill_cell = kf.KCell(fill_cell_name)
         for layer in fill_layers:
-            layer = kf.klib.layer(*layer)
-            fill_cell << kf.pcells.waveguide.waveguide(
+            layer = kf.kcl.layer(*layer)
+            fill_cell << kf.cells.waveguide.waveguide(
                 width=size[0], length=size[1], layer=layer
             )
 
         fc_index = fill_cell.cell_index()  # fill cell index
         fc_box = fill_cell.bbox().enlarged(spacing[0] / 2 * 1e3, spacing[1] / 2 * 1e3)
         fill_margin = kf.kdb.Point(0, 0)
```

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/offset.py` & `gdsfactory-6.98.0/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/outline.py` & `gdsfactory-6.98.0/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/trim.py` & `gdsfactory-6.98.0/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/union.py` & `gdsfactory-6.98.0/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/write_connectivity.py` & `gdsfactory-6.98.0/gdsfactory/geometry/write_connectivity.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,65 +2,77 @@
 
 from __future__ import annotations
 
 from typing import List
 from pydantic import BaseModel
 
 import gdsfactory as gf
-from gdsfactory.typings import CrossSectionSpec, Dict, Layer
+from gdsfactory.typings import CrossSectionSpec, Dict, Layer, LayerSpec
 from gdsfactory.geometry.write_drc import write_drc_deck_macro
 
 layer_name_to_min_width: Dict[str, float]
 
 nm = 1e-3
 
 
 class ConnectivyCheck(BaseModel):
     cross_section: CrossSectionSpec
     pin_length: float
     pin_layer: Layer
 
 
 def write_connectivity_checks(
-    pin_widths: List[float], pin_layer: Layer, pin_length: float = 1 * nm
+    pin_widths: List[float],
+    pin_layer: Layer,
+    pin_length: float = 1 * nm,
+    device_layer: LayerSpec = "DEVREC",
 ):
     """Return script for port connectivity check.
     Assumes the port pins are inside the Component.
 
     Args:
         pin_widths: list of pin widths allowed.
         pin_layer: for the pin markers.
         pin_length: in um.
+        device_layer: device recognizion layer.
     """
+    device_layer = gf.get_layer(device_layer)
 
     script = f"""pin = input{pin_layer}
 pin = pin.merged\n
 pin2 = pin.rectangles.without_area({pin_widths[0]} * {2 * pin_length})"""
 
     for w in pin_widths[1:]:
         script += f" - pin.rectangles.with_area({w} * {2 * pin_length})"
 
     script += """\npin2.output(\"port alignment error\")\n
 pin2 = pin.sized(0.0).merged\n
 pin2.non_rectangles.output(\"port width check\")\n\n"""
 
+    script += f"""DEVREC = input{device_layer}.raw.merged(2)\n
+DEVREC.overlapping(DEVREC).output("Component overlap")\n
+    """
+
     return script
 
 
 def write_connectivity_checks_per_section(
     connectivity_checks: List[ConnectivyCheck],
+    device_layer: LayerSpec = None,
 ) -> str:
     """Return script for port connectivity check.
     Assumes the port pins are inside the Component and each cross_section has pins on a different layer.
     This is not the recommended way as it only supports two widths per cross_section (cross_section.width and cross_section.width_wide)
 
     Args:
         connectivity_checks: list of connectivity objects to check for.
+        device_layer: device recognizion layer.
     """
     script = ""
+    device_layer = gf.get_layer(device_layer)
 
     for cc in connectivity_checks:
         xs = gf.get_cross_section(cc.cross_section)
         if not xs.name:
             raise ValueError("You need to define cross_section name")
         script += f"""{xs.name}_pin = input{cc.pin_layer}
 {xs.name}_pin = {xs.name}_pin.merged\n
@@ -69,14 +81,19 @@
         if xs.width_wide:
             script += f" - {xs.name}_pin.rectangles.with_area({xs.width_wide} * {2 * cc.pin_length})"
 
         script += f"""\n{xs.name}_pin2.output(\"port alignment error\")\n
 {xs.name}_pin2 = {xs.name}_pin.sized(0.0).merged\n
 {xs.name}_pin2.non_rectangles.output(\"port width check\")\n\n"""
 
+    if device_layer:
+        script += f"""DEVREC = input{device_layer}.raw.merged(2)\n
+DEVREC.overlapping(DEVREC).output("Component overlap")\n
+    """
+
     return script
 
 
 if __name__ == "__main__":
     from gdsfactory.generic_tech import LAYER
 
     nm = 1e-3
@@ -84,15 +101,16 @@
     connectivity_checks = [
         # ConnectivyCheck(cross_section="strip", pin_length=1 * nm, pin_layer=(1, 10))
         ConnectivyCheck(
             cross_section="strip_auto_widen", pin_length=1 * nm, pin_layer=(1, 10)
         )
     ]
     rules = [
-        write_connectivity_checks_per_section(connectivity_checks=connectivity_checks)
+        write_connectivity_checks_per_section(connectivity_checks=connectivity_checks),
+        "DEVREC",
     ]
 
     rules = [
         write_connectivity_checks(pin_widths=[0.5, 0.9, 0.45], pin_layer=LAYER.PORT)
     ]
     script = write_drc_deck_macro(rules=rules, layers=None)
     print(script)
```

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/write_drc.py` & `gdsfactory-6.98.0/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/geometry/xor_diff.py` & `gdsfactory-6.98.0/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/get_factories.py` & `gdsfactory-6.98.0/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/get_netlist.py` & `gdsfactory-6.98.0/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/get_netlist_flat.py` & `gdsfactory-6.98.0/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/get_netlist_klayout.py` & `gdsfactory-6.98.0/gdsfactory/get_netlist_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/grid.py` & `gdsfactory-6.98.0/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/install.py` & `gdsfactory-6.98.0/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/klive.py` & `gdsfactory-6.98.0/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/labels/__init__.py` & `gdsfactory-6.98.0/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-6.98.0/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/labels/ehva.py` & `gdsfactory-6.98.0/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-6.98.0/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/labels/siepic.py` & `gdsfactory-6.98.0/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/labels/write_labels.py` & `gdsfactory-6.98.0/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/materials.py` & `gdsfactory-6.98.0/gdsfactory/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/name.py` & `gdsfactory-6.98.0/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/pack.py` & `gdsfactory-6.98.0/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/path.py` & `gdsfactory-6.98.0/gdsfactory/path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/pdk.py` & `gdsfactory-6.98.0/gdsfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/picmodel.py` & `gdsfactory-6.98.0/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/pixelate.py` & `gdsfactory-6.98.0/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/plugins/dagster/workflow.py` & `gdsfactory-6.98.0/gdsfactory/plugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/plugins/database/README.md` & `gdsfactory-6.98.0/gdsfactory/plugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/plugins/database/db_upload.py` & `gdsfactory-6.98.0/gdsfactory/plugins/database/db_upload.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/plugins/database/models.py` & `gdsfactory-6.98.0/gdsfactory/plugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/plugins/web/main.py` & `gdsfactory-6.98.0/gdsfactory/plugins/web/main.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/plugins/web/server.py` & `gdsfactory-6.98.0/gdsfactory/plugins/web/server.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/plugins/web/server_jupyter.py` & `gdsfactory-6.98.0/gdsfactory/plugins/web/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/plugins/web/static/client.css` & `gdsfactory-6.98.0/gdsfactory/plugins/web/static/client.css`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/port.py` & `gdsfactory-6.98.0/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/quickplotter.py` & `gdsfactory-6.98.0/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/__init__.py` & `gdsfactory-6.98.0/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/from_dphox.py` & `gdsfactory-6.98.0/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/from_gdspaths.py` & `gdsfactory-6.98.0/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/from_np.py` & `gdsfactory-6.98.0/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/from_phidl.py` & `gdsfactory-6.98.0/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/from_yaml.py` & `gdsfactory-6.98.0/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/from_yaml_template.py` & `gdsfactory-6.98.0/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/import_gds.py` & `gdsfactory-6.98.0/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/read/labels.py` & `gdsfactory-6.98.0/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/__init__.py` & `gdsfactory-6.98.0/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-6.98.0/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-6.98.0/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-6.98.0/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-6.98.0/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-6.98.0/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/add_pads.py` & `gdsfactory-6.98.0/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/all_angle.py` & `gdsfactory-6.98.0/gdsfactory/routing/all_angle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/auto_taper.py` & `gdsfactory-6.98.0/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/factories.py` & `gdsfactory-6.98.0/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/fanout.py` & `gdsfactory-6.98.0/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/fanout2x2.py` & `gdsfactory-6.98.0/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_bundle.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_input_labels.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_route.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_route.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_route_astar.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_route_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-6.98.0/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/manhattan.py` & `gdsfactory-6.98.0/gdsfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/path_length_matching.py` & `gdsfactory-6.98.0/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-6.98.0/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-6.98.0/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-6.98.0/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/route_quad.py` & `gdsfactory-6.98.0/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/route_sharp.py` & `gdsfactory-6.98.0/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/route_south.py` & `gdsfactory-6.98.0/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/sort_ports.py` & `gdsfactory-6.98.0/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/routing/utils.py` & `gdsfactory-6.98.0/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-6.98.0/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-6.98.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-6.98.0/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-6.98.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/03_move.py` & `gdsfactory-6.98.0/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/04_connect.py` & `gdsfactory-6.98.0/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-6.98.0/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-6.98.0/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-6.98.0/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/11_component_layout.py` & `gdsfactory-6.98.0/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/12_component_refs.py` & `gdsfactory-6.98.0/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-6.98.0/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/14_component_connectivity.py` & `gdsfactory-6.98.0/gdsfactory/samples/14_component_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-6.98.0/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-6.98.0/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/17_ports.py` & `gdsfactory-6.98.0/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/20_components.py` & `gdsfactory-6.98.0/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/22_add_pads.py` & `gdsfactory-6.98.0/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/23_reticle.py` & `gdsfactory-6.98.0/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/23_reticle_passives.py` & `gdsfactory-6.98.0/gdsfactory/samples/23_reticle_passives.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/24_doe_2.py` & `gdsfactory-6.98.0/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/24_doe_3.py` & `gdsfactory-6.98.0/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/30_lidar.py` & `gdsfactory-6.98.0/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-6.98.0/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-6.98.0/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/big_device.py` & `gdsfactory-6.98.0/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-6.98.0/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-6.98.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-6.98.0/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-6.98.0/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/layers.py` & `gdsfactory-6.98.0/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/lvs.py` & `gdsfactory-6.98.0/gdsfactory/samples/demo/lvs.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 if __name__ == "__main__":
     c = pads_with_routes(radius=100)
     c.show(show_ports=True)
     gdspath = c.write_gds()
 
     import kfactory as kf
 
-    lib = kf.kcell.KLib()
+    lib = kf.kcell.KCLayout()
     lib.read(filename=str(gdspath))
     c = lib[0]
 
     l2n = kf.kdb.LayoutToNetlist(c.begin_shapes_rec(0))
-    for l_idx in c.klib.layer_indices():
+    for l_idx in c.kcl.layer_indices():
         l2n.connect(l2n.make_layer(l_idx, f"layer{l_idx}"))
     l2n.extract_netlist()
     print(l2n.netlist().to_s())
```

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/demo/pcell.py` & `gdsfactory-6.98.0/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-6.98.0/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-6.98.0/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-6.98.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/schematic_editor.py` & `gdsfactory-6.98.0/gdsfactory/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/serialization.py` & `gdsfactory-6.98.0/gdsfactory/serialization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/show.py` & `gdsfactory-6.98.0/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/add_simulation_markers.py` & `gdsfactory-6.98.0/gdsfactory/simulation/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/convert_sparameters.py` & `gdsfactory-6.98.0/gdsfactory/simulation/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/devsim/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/devsim/doping.py` & `gdsfactory-6.98.0/gdsfactory/simulation/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/devsim/get_simulation.py` & `gdsfactory-6.98.0/gdsfactory/simulation/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/devsim/get_simulation_xsection.py` & `gdsfactory-6.98.0/gdsfactory/simulation/devsim/get_simulation_xsection.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/devsim/get_solver.py` & `gdsfactory-6.98.0/gdsfactory/simulation/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/devsim/test_devsim.py` & `gdsfactory-6.98.0/gdsfactory/simulation/devsim/test_devsim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/eme/meow_eme.py` & `gdsfactory-6.98.0/gdsfactory/simulation/eme/meow_eme.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/eme/test_meow_simulation.py` & `gdsfactory-6.98.0/gdsfactory/simulation/eme/test_meow_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/fem/mode_solver.py` & `gdsfactory-6.98.0/gdsfactory/simulation/fem/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/fem/test_mode_solver.py` & `gdsfactory-6.98.0/gdsfactory/simulation/fem/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/get_effective_indices.py` & `gdsfactory-6.98.0/gdsfactory/simulation/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/get_modes_path.py` & `gdsfactory-6.98.0/gdsfactory/simulation/get_modes_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/get_sparameters_path.py` & `gdsfactory-6.98.0/gdsfactory/simulation/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_material.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_meep_geometry.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_port_eigenmode.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_simulation.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_eigenmode.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_materials.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/write_sparameters_grating.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/write_sparameters_meep.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/break_geometry.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/mesh.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/meshtracker.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/parse_component.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/parse_gds.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/parse_layerstack.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/parse_layerstack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/refine.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/scratch/mesh3D.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/tests/test_meshing.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/uz_xsection_mesh.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/xy_xsection_mesh.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gmsh/xyz_mesh.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gmsh/xyz_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/get_results.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/get_simulation.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/materials.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/modes.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/sim_run.yaml` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_modes.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_results.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_simulation.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,34 +2,43 @@
 
 import numpy as np
 
 import gdsfactory as gf
 import gdsfactory.simulation.gtidy3d as gt
 
 
-def test_sparameters_straight(overwrite=True) -> None:
+def test_sparameters_straight_3d(overwrite=True) -> None:
     """Checks Sparameters for a straight waveguide in 2D."""
     c = gf.components.straight(length=2)
-    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=False)
+    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=True)
 
-    # Check reasonable reflection/transmission
     assert 1 > np.abs(sp["o1@0,o2@0"]).min() > 0.8, np.abs(sp["o1@0,o2@0"]).min()
     assert 0 < np.abs(sp["o1@0,o1@0"]).max() < 0.1, np.abs(sp["o1@0,o1@0"]).max()
 
+
+def test_sparameters_straight_2d(overwrite=True) -> None:
+    """Checks Sparameters for a straight waveguide in 2D."""
+    c = gf.components.straight(length=2)
+    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=False)
+
+    assert 1 > np.abs(sp["o1@0,o2@0"]).min() > 0.7, np.abs(sp["o1@0,o2@0"]).min()
+    assert 0 < np.abs(sp["o1@0,o1@0"]).max() < 0.1, np.abs(sp["o1@0,o1@0"]).max()
+
     # assert np.allclose(sp["o2@0,o1@0"], 1, atol=1e-02), sp["o2@0,o1@0"]
     # assert np.allclose(sp["o1@0,o1@0"], 0, atol=5e-02), sp["o1@0,o1@0"]
     # assert np.allclose(sp["o2@0,o2@0"], 0, atol=5e-02), sp["o2@0,o2@0"]
 
     # if dataframe_regression:
     #     dataframe_regression.check(sp)
 
 
 if __name__ == "__main__":
     # test_sparameters_straight()
 
+    overwrite = False
     overwrite = True
     c = gf.components.straight(length=3)
-    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=False)
+    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=False, run=True)
 
     # Check reasonable reflection/transmission
     assert 1 > np.abs(sp["o1@0,o2@0"]).min() > 0.8, np.abs(sp["o1@0,o2@0"]).min()
     assert 0 < np.abs(sp["o1@0,o1@0"]).max() < 0.1, np.abs(sp["o1@0,o1@0"]).max()
```

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/utils.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/write_sparameters.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/write_sparameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,24 +167,27 @@
         logger.info(f"Simulation loaded from {filepath!r}")
         return dict(np.load(filepath))
 
     port_symmetries = port_symmetries or {}
     component_ref = component.ref()
     ports = component_ref.ports
     port_names = [port.name for port in list(ports.values())]
+    port_symmetries_sources = [key.split("@")[0] for key in port_symmetries]
 
     sims = []
     sp = {}
 
     port_source_names = port_source_names or port_names
 
     for port_name in port_source_names:
-        if port_name in port_symmetries or not port_symmetries:
+        if port_name not in port_symmetries_sources:
             sim = get_simulation(component, port_source_name=port_name, **kwargs)
             sims.append(sim)
+        else:
+            print(f"leveraging port_symmetries for {port_name!r}")
 
     if not run:
         sim = sims[0]
         plot_simulation(sim)
         return sp
 
     start = time.time()
@@ -195,15 +198,15 @@
         sim_data: td.SimulationData,
         port_symmetries=port_symmetries,
         **kwargs,
     ) -> Dict[str, np.ndarray]:
         """Return Component sparameter for a particular port Index n.
 
         Args:
-            port_name: source port name.
+            port_name_source: source port name.
             sim_data: simulation data.
             port_symmetries: to save simulations.
             kwargs: simulation settings.
         """
         source_entering, source_exiting = parse_port_eigenmode_coeff(
             port_name=port_name_source, ports=component_ref.ports, sim_data=sim_data
         )
@@ -213,39 +216,29 @@
                 port_name=port_name, ports=ports, sim_data=sim_data
             )
             sij = monitor_exiting / source_entering
             key = f"{port_name}@0,{port_name_source}@0"
             sp[key] = sij
             sp["wavelengths"] = get_wavelengths(port_name=port_name, sim_data=sim_data)
 
-        def convert_old_fmt(s_name):
-            if len(s_name) == 3 and s_name[0] == "s":
-                s_name = (
-                    f"{port_names[int(s_name[1])-1]}@0,{port_names[int(s_name[2])-1]}@0"
-                )
-            return s_name
-
         if bool(port_symmetries):
             for key, symmetries in port_symmetries.items():
                 for sym in symmetries:
-                    n_key = convert_old_fmt(key)
-                    n_sym = convert_old_fmt(sym)
-                    if n_key in sp:
-                        sp[n_sym] = sp[n_key]
+                    if key in sp:
+                        sp[sym] = sp[key]
 
         return sp
 
     for port_source_name, (_sim_name, sim_data) in zip(
         port_source_names, batch_data.items()
     ):
         sp.update(
             get_sparameter(
                 port_source_name,
                 sim_data,
-                port_symmetries=port_symmetries.get(port_source_name, {}),
             )
         )
 
     end = time.time()
     np.savez_compressed(filepath, **sp)
     kwargs.update(compute_time_seconds=end - start)
     kwargs.update(compute_time_minutes=(end - start) / 60)
@@ -280,19 +273,20 @@
 
 write_sparameters_batch_1x1 = gf.partial(
     write_sparameters_batch, port_symmetries=port_symmetries.port_symmetries_1x1
 )
 
 
 if __name__ == "__main__":
-    import gdsfactory.simulation as gs
-
     # c = gf.components.straight(length=2.1)
-    c = gf.c.straight(length=2.123)
+    # c = gf.c.straight(length=2.123)
     # c = gf.components.mmi1x2()
-    sp = write_sparameters(c, is_3d=True, port_source_names=None, overwrite=False)
-    gs.plot.plot_sparameters(sp)
+    # sp = write_sparameters(c, is_3d=True, port_source_names=None, overwrite=False)
+    # gs.plot.plot_sparameters(sp)
+    c = gf.components.straight(length=3)
+    sp = write_sparameters_1x1(c, overwrite=True, is_3d=False)
+    print(sp)
 
     # t = sp.o1@0,o2@0
     # print(f"Transmission = {t}")
     # cs = [gf.c.straight(length=1.11 + i) for i in [1, 2]]
     # sps = write_sparameters_batch_1x1(cs)
```

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/lumerical/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/lumerical/interconnect.py` & `gdsfactory-6.98.0/gdsfactory/simulation/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/lumerical/read.py` & `gdsfactory-6.98.0/gdsfactory/simulation/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/lumerical/settings.py` & `gdsfactory-6.98.0/gdsfactory/simulation/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/lumerical/test_read_sparameters.py` & `gdsfactory-6.98.0/gdsfactory/simulation/lumerical/test_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py` & `gdsfactory-6.98.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py` & `gdsfactory-6.98.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/coupler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/find_coupling_vs_gap.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/find_mode_dispersion.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/find_modes.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/find_modes_cross_section.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/find_neff_vs_width.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/get_mode_solver_coupler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/get_mode_solver_cross_section.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/get_mode_solver_rib.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/neff_convergence_test.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/overlap.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_find_modes.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/types.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/modes/waveguide.py` & `gdsfactory-6.98.0/gdsfactory/simulation/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/coupler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/mzi.py` & `gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/photonic_circuit_models/ring.py` & `gdsfactory-6.98.0/gdsfactory/simulation/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/plot.py` & `gdsfactory-6.98.0/gdsfactory/simulation/plot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/plot_csv.py` & `gdsfactory-6.98.0/gdsfactory/simulation/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/port_symmetries.py` & `gdsfactory-6.98.0/gdsfactory/simulation/port_symmetries.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 port_symmetries_1x1 = {
-    "o1@0,o1@0": ["o2@0,o2@0"],
     "o2@0,o1@0": ["o1@0,o2@0"],
 }
 
 
 port_symmetries_crossing = {
-    "o1@0,o1@0": ["o2@0,o2@0", "o3@0,o3@0", "o4@0,o4@0"],
     "o2@0,o1@0": ["o1@0,o2@0", "o3@0,o4@0", "o4@0,o3@0"],
     "o3@0,o1@0": ["o1@0,o3@0", "o2@0,o4@0", "o4@0,o2@0"],
     "o4@0,o1@0": ["o1@0,o4@0", "o2@0,o3@0", "o3@0,o2@0"],
 }
 
 
 if __name__ == "__main__":
```

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/process/diffusion.py` & `gdsfactory-6.98.0/gdsfactory/simulation/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/process/implant_tables.py` & `gdsfactory-6.98.0/gdsfactory/simulation/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/process/pysrim.py` & `gdsfactory-6.98.0/gdsfactory/simulation/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/process/silicon.py` & `gdsfactory-6.98.0/gdsfactory/simulation/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/process/skew/antimony_si_skew.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/process/skew/arsenic_si_skew.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/process/skew/boron_si_skew.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv` & `gdsfactory-6.98.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/build_model.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/femwell_waveguide_model.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/interpolators.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/meep_FDTD_model.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/meow_eme_model.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/mlp.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/models.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/parameter.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/plot_model.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/read.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/tests/test_mzi.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/tests/test_mzi_lattice.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sax/tests/test_parameters.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/add_gc.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/add_gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/circuit.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/__init__.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/bend_circular.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/bend_euler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler_fdtd.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler_ring.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/gc.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mmi1x2.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mmi2x2.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mzi.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/mzi_siepic.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/mzi_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/ring_double.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/ring_double_siepic.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/ring_single.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/ring_single_siepic.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/components/straight.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/get_transmission.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/get_transmission.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/model_from_gdsfactory.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/model_from_sparameters.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/model_from_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/plot_circuit.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/plot_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/plot_model.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_circuit.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/simphony/tests/test_components.py` & `gdsfactory-6.98.0/gdsfactory/simulation/simphony/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sipann/bend_circular.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sipann/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sipann/bend_euler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sipann/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sipann/coupler.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sipann/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sipann/coupler_ring.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sipann/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/sipann/straight.py` & `gdsfactory-6.98.0/gdsfactory/simulation/sipann/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/simulation/thermal/heater.py` & `gdsfactory-6.98.0/gdsfactory/simulation/thermal/heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/snap.py` & `gdsfactory-6.98.0/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/symbols.py` & `gdsfactory-6.98.0/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/technology/__init__.py` & `gdsfactory-6.98.0/gdsfactory/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/technology/klayout_tech.py` & `gdsfactory-6.98.0/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/technology/layer_map.py` & `gdsfactory-6.98.0/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/technology/layer_stack.py` & `gdsfactory-6.98.0/gdsfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/technology/layer_views.py` & `gdsfactory-6.98.0/gdsfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/technology/simulation_settings.py` & `gdsfactory-6.98.0/gdsfactory/technology/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/types.py` & `gdsfactory-6.98.0/gdsfactory/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/typings.py` & `gdsfactory-6.98.0/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/utils/async_utils.py` & `gdsfactory-6.98.0/gdsfactory/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/utils/file_utils.py` & `gdsfactory-6.98.0/gdsfactory/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/utils/xml_utils.py` & `gdsfactory-6.98.0/gdsfactory/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/utils/yaml_utils.py` & `gdsfactory-6.98.0/gdsfactory/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/watch.py` & `gdsfactory-6.98.0/gdsfactory/watch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/widgets/layout_viewer.py` & `gdsfactory-6.98.0/gdsfactory/widgets/layout_viewer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/gdsfactory/write_cells.py` & `gdsfactory-6.98.0/gdsfactory/write_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.97.1/pyproject.toml` & `gdsfactory-6.98.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
 ]
-version = "6.97.1"
+version = "6.98.0"
 authors = [
 {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 keywords = ["eda", "photonics", "python"]
 license = {file = "LICENSE"}
 dependencies = [
   "click",
@@ -64,24 +64,24 @@
     "pygmsh",
     "scikit-fem",
     "scikit-image",
     "scikit-learn",
     "trimesh",
     "jupytext",
     "klayout",
-    "kfactory",
     "ipytree",
     "rich-click",
     "ipycytoscape",
     "kweb>=0.0.11,<0.1",
     "jinja2",
     "python-multipart",
     "fastapi",
     "uvicorn[standard]",
     ]
+    kfactory = ["kfactory==0.7.0"]
     femwell = ["femwell==0.0.18"]
     database = [
     "sqlalchemy",
     "sqlalchemy-utils",
     "dagster",
     "dagit",
     "sqlmodel",
@@ -94,15 +94,15 @@
       "mapbox_earcut",
       "meshio",
       "pygmsh",
       "pyvista",
       "trimesh",
       "shapely",
     ]
-    tidy3d = ["tidy3d==2.1.1"]
+    tidy3d = ["tidy3d==2.2.1"]
     devsim = [
       "devsim",
       "mkl",
       "pyvista",
       "tidy3d",
     ]
     meow = ["meow-sim"]
```

### Comparing `gdsfactory-6.97.1/PKG-INFO` & `gdsfactory-6.98.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 6.97.1
+Version: 6.98.0
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -78,15 +78,14 @@
 Requires-Dist: pygmsh ; extra == "full"
 Requires-Dist: scikit-fem ; extra == "full"
 Requires-Dist: scikit-image ; extra == "full"
 Requires-Dist: scikit-learn ; extra == "full"
 Requires-Dist: trimesh ; extra == "full"
 Requires-Dist: jupytext ; extra == "full"
 Requires-Dist: klayout ; extra == "full"
-Requires-Dist: kfactory ; extra == "full"
 Requires-Dist: ipytree ; extra == "full"
 Requires-Dist: rich-click ; extra == "full"
 Requires-Dist: ipycytoscape ; extra == "full"
 Requires-Dist: kweb>=0.0.11,<0.1 ; extra == "full"
 Requires-Dist: jinja2 ; extra == "full"
 Requires-Dist: python-multipart ; extra == "full"
 Requires-Dist: fastapi ; extra == "full"
@@ -95,34 +94,36 @@
 Requires-Dist: h5py ; extra == "gmsh"
 Requires-Dist: mapbox_earcut ; extra == "gmsh"
 Requires-Dist: meshio ; extra == "gmsh"
 Requires-Dist: pygmsh ; extra == "gmsh"
 Requires-Dist: pyvista ; extra == "gmsh"
 Requires-Dist: trimesh ; extra == "gmsh"
 Requires-Dist: shapely ; extra == "gmsh"
+Requires-Dist: kfactory==0.7.0 ; extra == "kfactory"
 Requires-Dist: meow-sim ; extra == "meow"
 Requires-Dist: ray[tune,air] ; extra == "ray"
 Requires-Dist: hyperopt ; extra == "ray"
 Requires-Dist: sax>=0.8.6 ; extra == "sax"
 Requires-Dist: jaxlib ; extra == "sax"
 Requires-Dist: jax ; extra == "sax"
-Requires-Dist: tidy3d==2.1.1 ; extra == "tidy3d"
+Requires-Dist: tidy3d==2.2.1 ; extra == "tidy3d"
 Provides-Extra: database
 Provides-Extra: dev
 Provides-Extra: devsim
 Provides-Extra: docs
 Provides-Extra: femwell
 Provides-Extra: full
 Provides-Extra: gmsh
+Provides-Extra: kfactory
 Provides-Extra: meow
 Provides-Extra: ray
 Provides-Extra: sax
 Provides-Extra: tidy3d
 
-# gdsfactory 6.97.1
+# gdsfactory 6.98.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
@@ -220,15 +221,15 @@
 ![anaconda prompt](https://i.imgur.com/Fyal5sT.png)
 
 ```
 pip install gdsfactory --upgrade
 gf install klayout-integration
 ```
 
-Then you need to restart Klayout to make sure you activate the klayout gdsfactory integration.
+Then you can install Klayout-live `klive` integration in the klayout GUI `Tools --> Manage Packages --> Install New Packages --> Klive` and restart klayout.
 
 ### 2. Installation for developers
 
 For developers you need to fork the GitHub repository, git clone it (download it), git add, git commit, git push your improvement. Then pull request your changes to the main branch from the GitHub website.
 For that you can install gdsfactory locally on your computer in `-e` edit mode.
 
 ```
```

