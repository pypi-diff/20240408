# Comparing `tmp/whitecanvas-0.2.5.tar.gz` & `tmp/whitecanvas-0.2.6.tar.gz`

## Comparing `whitecanvas-0.2.5.tar` & `whitecanvas-0.2.6.tar`

### file list

```diff
@@ -1,230 +1,240 @@
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/mkdocs.yml
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/.github/workflows/test.yml
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/index.md
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/quick_start.md
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/_scripts/_hooks.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/_scripts/_screenshots.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/api/canvas.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/api/core.md
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/canvas/basics.md
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/canvas/grid.md
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/canvas/index.md
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/canvas/inset_second.md
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/canvas/joint_grid.md
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/canvas/legend.md
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/canvas/namespaces.md
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/canvas/native_objects.md
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/categorical/aggregation.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/categorical/cat_cat.md
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/categorical/cat_num.md
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/categorical/index.md
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/categorical/num_num.md
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/categorical/stacking.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/events/canvas_events.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/events/index.md
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/events/layer_events.md
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/events/mouse_events.md
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/layers/distribution.md
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/layers/face_layers.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/layers/index.md
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/layers/layer_groups.md
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/layers/lines.md
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/layers/markers.md
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/layers/mouse.md
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/docs/layers/texts.md
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/boxplot_with_outliers.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/curve_fit.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/draw_with_mouse.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/fit_layer.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/heatmap_with_text.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/image_profile.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/integral.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/joint_grid.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/layer_clicked_event.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/line_with_error.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/line_with_spans.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/lines.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/markers_hover_text.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/markers_multicolor.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/markers_with_legend.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/plotly_in_qt.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/raincloud_plot.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/show_image_on_pick.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/stack_bars.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/examples/superplot.py
--rw-r--r--   0        0        0    93685 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/images/curve_fit.png
--rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/images/heatmap.png
--rw-r--r--   0        0        0   205151 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/images/jointgrid.png
--rw-r--r--   0        0        0    45190 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/images/raincloud.png
--rw-r--r--   0        0        0    41392 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/images/superplot.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/_utils.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/test_canvas.py
--rw-r--r--   0        0        0    11716 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/test_categorical.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/test_grouping.py
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/test_layers.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/test_logics.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/test_plt.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/tests/test_theme.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/__init__.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/_axis.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/_exceptions.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/_signal.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/animation.py
--rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/core.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/__init__.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/_app.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/_instance.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/_not_implemented.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/_window/__init__.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/_window/_qt.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/_window/_tk.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/__init__.py
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/_base.py
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/_labels.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/_legend.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/band.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/bars.py
--rw-r--r--   0        0        0    14101 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/canvas.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/image.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/line.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/markers.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/bokeh/text.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/__init__.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/_base.py
--rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/_labels.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/_legend.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/band.py
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/bars.py
--rw-r--r--   0        0        0    14991 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/canvas.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/image.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/line.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/markers.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/matplotlib/text.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/mock/__init__.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/mock/_base.py
--rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/mock/canvas.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/mock/layers.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/__init__.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/_base.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/_labels.py
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/_legend.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/band.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/bars.py
--rw-r--r--   0        0        0    12986 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/canvas.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/image.py
--rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/line.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/markers.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/plotly/text.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/__init__.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/_base.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/_labels.py
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/_legend.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/_qt_utils.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/band.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/bars.py
--rw-r--r--   0        0        0    14193 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/canvas.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/image.py
--rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/line.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/markers.py
--rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/text.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/__init__.py
--rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/_label.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/band.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/bars.py
--rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/canvas.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/image.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/line.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/markers.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/backend/vispy/text.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/__init__.py
--rw-r--r--   0        0        0    67301 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_base.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_between.py
--rw-r--r--   0        0        0    18249 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_dims.py
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_fit.py
--rw-r--r--   0        0        0    14012 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_grid.py
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_imageref.py
--rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_joint.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_linker.py
--rw-r--r--   0        0        0    10765 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_namespaces.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_palette.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/_stacked.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/layerlist.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/dataframe/__init__.py
--rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_base.py
--rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_both_cat.py
--rw-r--r--   0        0        0    18971 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_feature_cat.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_joint_cat.py
--rw-r--r--   0        0        0    35906 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_one_cat.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_stacked_cat.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/__init__.py
--rw-r--r--   0        0        0    11908 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_base.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_legend.py
--rw-r--r--   0        0        0    34989 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_mixin.py
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_ndim.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_sizehint.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_text_utils.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/__init__.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/band.py
--rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/bars.py
--rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/errorbars.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/image.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/inf_curve.py
--rw-r--r--   0        0        0    23189 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/line.py
--rw-r--r--   0        0        0    25150 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/markers.py
--rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/rug.py
--rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/spans.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/_primitive/text.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/_cat_utils.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/_collections.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/_offsets.py
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/band_collection.py
--rw-r--r--   0        0        0    12099 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/boxplot.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/colorbar.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/graph.py
--rw-r--r--   0        0        0    25082 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/labeled.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/line_band.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/line_collection.py
--rw-r--r--   0        0        0    14529 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/line_fill.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/line_markers.py
--rw-r--r--   0        0        0    16196 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/marker_collection.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/stemplot.py
--rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/group/textinfo.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/__init__.py
--rw-r--r--   0        0        0    40606 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/_box_like.py
--rw-r--r--   0        0        0    26904 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/_dataframe.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/_df_compat.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/_jitter.py
--rw-r--r--   0        0        0    31694 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/_marker_like.py
--rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/_plans.py
--rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/_shared.py
--rw-r--r--   0        0        0    14768 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/layers/tabular/_stackable.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/plot/__init__.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/plot/_canvases.py
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/plot/_methods.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/protocols/__init__.py
--rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/protocols/canvas_protocol.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/protocols/layer_protocols.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/theme/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/theme/_api.py
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/theme/_dataclasses.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/types/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/types/_alias.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/types/_enums.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/types/_mouse.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/types/_tuples.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/utils/__init__.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/utils/collections.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/utils/hist.py
--rw-r--r--   0        0        0    14353 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/utils/kde.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/utils/normalize.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/whitecanvas/utils/type_check.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/LICENSE
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/README.md
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 whitecanvas-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/mkdocs.yml
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/index.md
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/quick_start.md
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/_scripts/_hooks.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/_scripts/_screenshots.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/api/canvas.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/api/core.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/api/tools.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/api/types.md
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/basics.md
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/grid.md
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/index.md
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/inset_second.md
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/joint_grid.md
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/legend.md
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/namespaces.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/canvas/native_objects.md
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/aggregation.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/cat_cat.md
+-rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/cat_num.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/index.md
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/num_num.md
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/categorical/stacking.md
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/events/canvas_events.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/events/index.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/events/layer_events.md
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/events/mouse_events.md
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/distribution.md
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/face_layers.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/index.md
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/layer_groups.md
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/lines.md
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/markers.md
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/mouse.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/layers/texts.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/tools/index.md
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/docs/tools/selection.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/boxplot_with_outliers.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/curve_fit.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/draw_with_mouse.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/fit_layer.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/heatmap_with_text.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/image_profile.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/integral.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/joint_grid.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/layer_clicked_event.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/line_with_error.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/line_with_spans.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/lines.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/markers_hover_text.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/markers_multicolor.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/markers_with_legend.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/plotly_in_qt.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/raincloud_plot.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/show_image_on_pick.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/stack_bars.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/examples/superplot.py
+-rw-r--r--   0        0        0    93685 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/curve_fit.png
+-rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/heatmap.png
+-rw-r--r--   0        0        0   205151 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/jointgrid.png
+-rw-r--r--   0        0        0    45190 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/raincloud.png
+-rw-r--r--   0        0        0    41392 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/images/superplot.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/_utils.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/conftest.py
+-rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_canvas.py
+-rw-r--r--   0        0        0    11908 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_categorical.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_grouping.py
+-rw-r--r--   0        0        0    12476 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_layers.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_logics.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_plt.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_theme.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/tests/test_tools.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/__init__.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/_axis.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/_exceptions.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/_signal.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/animation.py
+-rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/core.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/__init__.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_app.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_instance.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_not_implemented.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_window/__init__.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_window/_qt.py
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/_window/_tk.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/__init__.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/_base.py
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/_labels.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/_legend.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/band.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/bars.py
+-rw-r--r--   0        0        0    14323 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/canvas.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/image.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/line.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/markers.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/bokeh/text.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/__init__.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_base.py
+-rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_labels.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_legend.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/band.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/bars.py
+-rw-r--r--   0        0        0    15742 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/canvas.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/image.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/line.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/markers.py
+-rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/matplotlib/text.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/mock/__init__.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/mock/_base.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/mock/canvas.py
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/mock/layers.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/__init__.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/_base.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/_labels.py
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/_legend.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/band.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/bars.py
+-rw-r--r--   0        0        0    13248 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/canvas.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/image.py
+-rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/line.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/markers.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/plotly/text.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/__init__.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_base.py
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_labels.py
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_legend.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_qt_utils.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/band.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/bars.py
+-rw-r--r--   0        0        0    15158 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/canvas.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/image.py
+-rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/line.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/markers.py
+-rw-r--r--   0        0        0     7951 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/text.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/_gridlines.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/_label.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/band.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/bars.py
+-rw-r--r--   0        0        0    12258 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/canvas.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/image.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/line.py
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/markers.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/backend/vispy/text.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/__init__.py
+-rw-r--r--   0        0        0    69749 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_base.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_between.py
+-rw-r--r--   0        0        0    18261 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_dims.py
+-rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_fit.py
+-rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_grid.py
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_imageref.py
+-rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_joint.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_linker.py
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_namespaces.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_palette.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/_stacked.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/layerlist.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/__init__.py
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_base.py
+-rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_both_cat.py
+-rw-r--r--   0        0        0    18971 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_feature_cat.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_joint_cat.py
+-rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_one_cat.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_stacked_cat.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/__init__.py
+-rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_base.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_legend.py
+-rw-r--r--   0        0        0    36394 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_mixin.py
+-rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_ndim.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_sizehint.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_text_utils.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/__init__.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/band.py
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/bars.py
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/errorbars.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/image.py
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/inf_curve.py
+-rw-r--r--   0        0        0    23189 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/line.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/markers.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/rects.py
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/rug.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/spans.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/_primitive/text.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/_cat_utils.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/_collections.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/_offsets.py
+-rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/band_collection.py
+-rw-r--r--   0        0        0    12099 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/boxplot.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/colorbar.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/graph.py
+-rw-r--r--   0        0        0    25093 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/labeled.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/line_band.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/line_collection.py
+-rw-r--r--   0        0        0    14529 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/line_fill.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/line_markers.py
+-rw-r--r--   0        0        0    16196 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/marker_collection.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/stemplot.py
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/group/textinfo.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/__init__.py
+-rw-r--r--   0        0        0    41141 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_box_like.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_dataframe.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_df_compat.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_jitter.py
+-rw-r--r--   0        0        0    33317 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_marker_like.py
+-rw-r--r--   0        0        0    15921 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_plans.py
+-rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_shared.py
+-rw-r--r--   0        0        0    14768 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/layers/tabular/_stackable.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/plot/__init__.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/plot/_canvases.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/plot/_methods.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/protocols/__init__.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/protocols/canvas_protocol.py
+-rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/protocols/layer_protocols.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/theme/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/theme/_api.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/theme/_dataclasses.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/tools/__init__.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/tools/_polygon_utils.py
+-rw-r--r--   0        0        0    24164 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/tools/_selection.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/_alias.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/_enums.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/_mouse.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/types/_tuples.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/__init__.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/collections.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/hist.py
+-rw-r--r--   0        0        0    14353 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/kde.py
+-rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/normalize.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/whitecanvas/utils/type_check.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/README.md
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 whitecanvas-0.2.6/PKG-INFO
```

### Comparing `whitecanvas-0.2.5/mkdocs.yml` & `whitecanvas-0.2.6/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,22 @@
     - Aggregation: categorical/aggregation.md
     - Stacking: categorical/stacking.md
   - Event Handling:
     - Overview: events/index.md
     - Canvas Events: events/canvas_events.md
     - Layer Events: events/layer_events.md
     - Mouse Events: events/mouse_events.md
+  - Tools:
+    - Overview: tools/index.md
+    - Mouse Selection: tools/selection.md
   - API Reference:
     - api/core.md
     - api/canvas.md
+    - api/tools.md
+    - api/types.md
 
 plugins:
   - search
   - autorefs
   - mkdocstrings:
       handlers:
         python:
```

### Comparing `whitecanvas-0.2.5/.github/workflows/docs.yml` & `whitecanvas-0.2.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/.github/workflows/test.yml` & `whitecanvas-0.2.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/index.md` & `whitecanvas-0.2.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/quick_start.md` & `whitecanvas-0.2.6/docs/quick_start.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 The `new_canvas` function creates a new canvas, in which you can add many graphical
 elements. Created canvas can be shown by calling `show`.
 
 ``` python
 #!name: quick_start_empty_canvas
 from whitecanvas import new_canvas
 
-canvas = new_canvas()  # create a canvas
-canvas.show()  # show the canvas
+# create a canvas
+canvas = new_canvas()
+
+# show the canvas
+canvas.show()
 ```
 
 As `whitecanvas` is backend independent, you can specify a plotting backend when
 creating the canvas.
 
 ``` python
 #!skip
```

### Comparing `whitecanvas-0.2.5/docs/_scripts/_hooks.py` & `whitecanvas-0.2.6/docs/_scripts/_hooks.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/_scripts/_screenshots.py` & `whitecanvas-0.2.6/docs/_scripts/_screenshots.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/canvas/basics.md` & `whitecanvas-0.2.6/docs/canvas/basics.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/canvas/grid.md` & `whitecanvas-0.2.6/docs/canvas/grid.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/canvas/inset_second.md` & `whitecanvas-0.2.6/docs/canvas/inset_second.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/canvas/joint_grid.md` & `whitecanvas-0.2.6/docs/canvas/joint_grid.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/canvas/legend.md` & `whitecanvas-0.2.6/docs/canvas/legend.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/canvas/namespaces.md` & `whitecanvas-0.2.6/docs/canvas/namespaces.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/canvas/native_objects.md` & `whitecanvas-0.2.6/docs/canvas/native_objects.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Working with the Backend Objects
 
 ## Convert a backend object to `whitecanvas` canvas
 
-The `wrap_canvas`{.interpreted-text role="func"} converts a backend
-object to a `whitecanvas`{.interpreted-text role="mod"} canvas.
+The `wrap_canvas` converts a backend object to a `whitecanvas` canvas.
 
 ``` python
 #!skip
 from whitecanvas import wrap_canvas
 import matplotlib.pyplot as plt
 
 fig, axes = plt.subplots()
```

### Comparing `whitecanvas-0.2.5/docs/categorical/aggregation.md` & `whitecanvas-0.2.6/docs/categorical/aggregation.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/categorical/cat_cat.md` & `whitecanvas-0.2.6/docs/categorical/cat_cat.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/categorical/cat_num.md` & `whitecanvas-0.2.6/docs/categorical/cat_num.md`

 * *Files 2% similar despite different names*

```diff
@@ -225,25 +225,25 @@
     .cat_x(df, x="category", y="observation")
     .add_stripplot(color="replicate", dodge=True)
     .with_hover_template("{category} (rep={replicate})")
 )
 canvas.show()
 ```
 
-Each marker size can represent a numerical value. `with_size` will map the numerical
+Each marker size can represent a numerical value. `update_size` will map the numerical
 values of a column to the size of the markers.
 
-``` python
+``` python hl_lines="6"
 #!name: categorical_axis_stripplot_by_size
 canvas = new_canvas("matplotlib")
 (
     canvas
     .cat_x(df, x="category", y="observation")
     .add_stripplot()
-    .with_size("temperature")
+    .update_size("temperature")
 )
 canvas.show()
 ```
 
 Similarly, each marker color can represent a numerical value. `update_colormap` will map
 the value with an arbitrary colormap.
```

### Comparing `whitecanvas-0.2.5/docs/categorical/index.md` & `whitecanvas-0.2.6/docs/categorical/index.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/categorical/num_num.md` & `whitecanvas-0.2.6/docs/categorical/num_num.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/categorical/stacking.md` & `whitecanvas-0.2.6/docs/categorical/stacking.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/events/index.md` & `whitecanvas-0.2.6/docs/events/index.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/layers/distribution.md` & `whitecanvas-0.2.6/docs/layers/distribution.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/layers/face_layers.md` & `whitecanvas-0.2.6/docs/layers/face_layers.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/layers/layer_groups.md` & `whitecanvas-0.2.6/docs/layers/layer_groups.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/layers/lines.md` & `whitecanvas-0.2.6/docs/layers/lines.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/layers/markers.md` & `whitecanvas-0.2.6/docs/layers/markers.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/layers/mouse.md` & `whitecanvas-0.2.6/docs/layers/mouse.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/docs/layers/texts.md` & `whitecanvas-0.2.6/docs/layers/texts.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/curve_fit.py` & `whitecanvas-0.2.6/examples/curve_fit.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/draw_with_mouse.py` & `whitecanvas-0.2.6/examples/draw_with_mouse.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 
 def main():
     canvas = new_canvas("matplotlib:qt")
     x, y = np.indices((10, 10)).reshape(2, -1)
     canvas.add_markers(x, y, color="gray")
 
-    @canvas.events.mouse_moved.connect
+    @canvas.mouse.moved.connect
     def _add_line(e: MouseEvent):
         if e.button != "left" or e.modifiers != ():
             return
         pos0 = e.pos
         line = canvas.add_line(np.array([pos0, pos0]), color="blue")
         dragged = False
         while e.type != "release":
             data = np.array([pos0, e.pos])
             line.data = data
             yield
             dragged = True
         if not dragged:
             canvas.layers.remove(line)
 
-    @canvas.events.mouse_moved.connect
+    @canvas.mouse.moved.connect
     def _add_spans(e: MouseEvent):
         if e.button != "left" or e.modifiers != ("shift",):
             return
         x0 = e.pos[0]
         span = canvas.add_spans([[x0, x0]], color="pink")
         dragged = False
         while e.type != "release":
```

### Comparing `whitecanvas-0.2.5/examples/fit_layer.py` & `whitecanvas-0.2.6/examples/fit_layer.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/image_profile.py` & `whitecanvas-0.2.6/examples/image_profile.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/joint_grid.py` & `whitecanvas-0.2.6/examples/joint_grid.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/layer_clicked_event.py` & `whitecanvas-0.2.6/examples/layer_clicked_event.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/line_with_error.py` & `whitecanvas-0.2.6/examples/line_with_error.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/line_with_spans.py` & `whitecanvas-0.2.6/examples/line_with_spans.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/markers_hover_text.py` & `whitecanvas-0.2.6/examples/markers_hover_text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/markers_multicolor.py` & `whitecanvas-0.2.6/examples/markers_multicolor.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/raincloud_plot.py` & `whitecanvas-0.2.6/examples/raincloud_plot.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/show_image_on_pick.py` & `whitecanvas-0.2.6/examples/show_image_on_pick.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/examples/superplot.py` & `whitecanvas-0.2.6/examples/superplot.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/images/curve_fit.png` & `whitecanvas-0.2.6/images/curve_fit.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/images/heatmap.png` & `whitecanvas-0.2.6/images/heatmap.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/images/jointgrid.png` & `whitecanvas-0.2.6/images/jointgrid.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/images/raincloud.png` & `whitecanvas-0.2.6/images/raincloud.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/images/superplot.png` & `whitecanvas-0.2.6/images/superplot.png`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/tests/_utils.py` & `whitecanvas-0.2.6/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/tests/conftest.py` & `whitecanvas-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/tests/test_canvas.py` & `whitecanvas-0.2.6/tests/test_canvas.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import tempfile
 import numpy as np
 from numpy.testing import assert_allclose
 
 import pytest
 import whitecanvas as wc
 from whitecanvas import new_canvas, wrap_canvas
+from whitecanvas.types import Point, MouseEvent
 
 from ._utils import assert_color_equal, filter_warning
 
 
 def test_namespaces(backend: str):
     canvas = new_canvas(backend=backend)
     canvas.aspect_ratio
@@ -323,7 +324,53 @@
         pytest.skip(f"{backend} does not support screenshot")
     if backend == "vispy":
         backend += ":qt"
     canvas = new_canvas(backend=backend)
     canvas.add_line([0, 1, 2], [0, 1, 2], name="line")
     if sys.platform != "win32":  # NOTE: testing in GitHub Actions fails for some reason
         canvas._repr_png_()
+
+def test_emulating_mouse_click():
+    canvas = new_canvas("mock")
+
+    clicked_history: list[Point] = []
+    double_clicked_history: list[Point] = []
+
+    @canvas.mouse.clicked.connect
+    def _clicked(ev: MouseEvent):
+        clicked_history.append(ev.pos)
+
+    @canvas.mouse.double_clicked.connect
+    def _double_clicked(ev: MouseEvent):
+        double_clicked_history.append(ev.pos)
+
+    canvas.mouse.emulate_click((1, 1))
+    assert clicked_history == [(1, 1)]
+    assert double_clicked_history == []
+
+    canvas.mouse.emulate_click((1, 2))
+    assert clicked_history == [(1, 1), (1, 2)]
+    assert double_clicked_history == []
+
+    canvas.mouse.emulate_double_click((-1, -1))
+    assert clicked_history == [(1, 1), (1, 2)]
+    assert double_clicked_history == [(-1, -1)]
+
+def test_emulating_mouse_move():
+    canvas = new_canvas("mock")
+    history: list[str] = []
+
+    @canvas.mouse.moved.connect
+    def _move(ev: MouseEvent):
+        if ev.button != "right":
+            return
+        history.append("press")
+        yield
+        while ev.type != "release":
+            history.append("move")
+            yield
+        history.append("release")
+
+    canvas.mouse.emulate_drag([(1, 1), (1, 2), (1, 3)], button="left")
+    assert history == []
+    canvas.mouse.emulate_drag([(1, 1), (1, 2), (1, 3)], button="right")
+    assert history == ["press", "move", "move", "release"]
```

### Comparing `whitecanvas-0.2.5/tests/test_categorical.py` & `whitecanvas-0.2.6/tests/test_categorical.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,21 +50,22 @@
 @pytest.mark.parametrize("orient", ["v", "h"])
 def test_cat_plots(backend: str, orient: str):
     canvas = new_canvas(backend=backend)
     df = {
         "y": np.arange(30),
         "label": np.repeat(["A", "B", "C"], 10),
         "c": ["P", "Q"] * 15,
+        "val": np.cos(np.arange(30) / 10),
     }
     if orient == "v":
         cat_plt = canvas.cat_x(df, "label", "y")
     else:
         cat_plt = canvas.cat_y(df, "y", "label")
-    cat_plt.add_stripplot(color="c").move(0.1)
-    cat_plt.add_swarmplot(color="c").move(0.1)
+    cat_plt.add_stripplot(color="c", alpha=0.8).move(0.1)
+    cat_plt.add_swarmplot(color="c", alpha="val").move(0.1)
     cat_plt.add_boxplot(color="c").with_edge().with_outliers(ratio=0.5)
     with filter_warning(backend, "plotly"):
         box = cat_plt.add_boxplot(color="c").as_edge_only().move(0.1)
         box.update_color_palette(["blue", "red"], alpha=0.9, cycle_by="c")
         box = cat_plt.add_boxplot(hatch="c").as_edge_only().move(0.1)
         box.update_hatch_palette(["/", "x"])
         box.update_const(color="black", hatch="+")
@@ -154,22 +155,22 @@
         "label": np.repeat(["A", "B", "C"], 10),
         "c": ["P", "Q"] * 15,
     }
     if orient == "v":
         cat_plt = canvas.cat_x(df, "label", "y")
     else:
         cat_plt = canvas.cat_y(df, "y", "label")
-    cat_plt.mean().add_line(color="c")
-    cat_plt.mean().add_markers(color="c")
-    cat_plt.mean().add_bars(color="c")
-    cat_plt.std().add_line(color="c")
-    cat_plt.sum().add_line(color="c")
-    cat_plt.median().add_line(color="c")
-    cat_plt.max().add_line(color="c")
-    cat_plt.min().add_line(color="c")
+    cat_plt.mean().add_line(color="c", alpha=0.8)
+    cat_plt.mean().add_markers(color="c", alpha=0.8)
+    cat_plt.mean().add_bars(color="c", alpha=0.8).as_edge_only()
+    cat_plt.std().add_line(color="c", width=2.5)
+    cat_plt.sum().add_line()
+    cat_plt.median().add_bars(color="c").update_width(1.5)
+    cat_plt.max().add_markers()
+    cat_plt.min().add_bars(color="c").update_hatch("/")
     cat_plt.first().add_line(color="c")
     if orient == "v":
         canvas.cat_x(df, x="label").count().add_line(color="c")
     else:
         canvas.cat_y(df, y="label").count().add_line(color="c")
 
     cat_plt.mean_for_each("c").add_stripplot()
@@ -200,18 +201,18 @@
     canvas = new_canvas(backend=backend)
     df = {
         "x": ["P", "Q"] * 15,
         "y": np.arange(30),
         "label": np.repeat(["A", "B", "C"], 10),
     }
     _c = canvas.cat_x(df, "x", "y")
-    _c.add_boxplot(color="label")
-    _c.add_violinplot(color="label").with_rug()
-    _c.add_pointplot(color="label").err_by_se()
-    _c.add_barplot(color="label")
+    _c.add_boxplot(color="label", alpha=0.8)
+    _c.add_violinplot(color="label", alpha=0.8).with_rug()
+    _c.add_pointplot(color="label", alpha=0.8).err_by_se()
+    _c.add_barplot(color="label", alpha=0.8)
     canvas.add_legend()
 
 def test_marker_legend():
     canvas = new_canvas("mock")
     df = {
         "x": ["P", "Q"] * 15,
         "y": np.arange(30),
```

### Comparing `whitecanvas-0.2.5/tests/test_grouping.py` & `whitecanvas-0.2.6/tests/test_grouping.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/tests/test_layers.py` & `whitecanvas-0.2.6/tests/test_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     layer.visible = False
     layer.visible = True
 
 def test_line(backend: str):
     canvas = new_canvas(backend=backend)
     canvas.add_line(np.arange(10), np.zeros(10))
     layer = canvas.add_line(np.zeros(10))
+    canvas.add_line(layer.data)
 
     repr(layer)
     layer.color
     layer.color = [1.0, 0.0, 0.0, 1.0]
     assert_color_equal(layer.color, "red")
     layer.style
     layer.style = ":"
@@ -367,7 +368,20 @@
     layer.data = [[6, 11], [18, 25]]
 
     layer.with_edge("black")
 
     if backend != "vispy":
         canvas.add_legend()
     canvas.autoscale(xpad=0.01, ypad=0.01)
+
+
+def test_rects(backend: str):
+    canvas = new_canvas(backend=backend)
+
+    layer = canvas.add_rects([[5, 10, 18, 30], [15, 20, 18, 21]])
+    layer.data
+    assert layer.ndata == 2
+    layer.data = [5, 10, 18, 30]
+    layer.data = [[5, 10, 18, 30], [15, 20, 18, 21]]
+    layer.rects
+    layer.as_edge_only()
+    layer.with_hover_template("x={left:.2f}, y={bottom:.2f}")
```

### Comparing `whitecanvas-0.2.5/tests/test_logics.py` & `whitecanvas-0.2.6/tests/test_logics.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/tests/test_theme.py` & `whitecanvas-0.2.6/tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/__init__.py` & `whitecanvas-0.2.6/whitecanvas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 from whitecanvas import theme
 from whitecanvas.canvas import link_axes
 from whitecanvas.core import (
     new_canvas,
     new_col,
     new_grid,
```

### Comparing `whitecanvas-0.2.5/whitecanvas/_axis.py` & `whitecanvas-0.2.6/whitecanvas/_axis.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/animation.py` & `whitecanvas-0.2.6/whitecanvas/animation.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/core.py` & `whitecanvas-0.2.6/whitecanvas/core.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/_app.py` & `whitecanvas-0.2.6/whitecanvas/backend/_app.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/_instance.py` & `whitecanvas-0.2.6/whitecanvas/backend/_instance.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/_not_implemented.py` & `whitecanvas-0.2.6/whitecanvas/backend/_not_implemented.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/_window/__init__.py` & `whitecanvas-0.2.6/whitecanvas/backend/_window/__init__.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/_window/_qt.py` & `whitecanvas-0.2.6/whitecanvas/backend/_window/_qt.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self.setWindowTitle("whitecanvas")
         self._widget = QtCanvas(canvas)
         self.setCentralWidget(self._widget)
         sl = QtDimSliders.from_canvas(canvas[0, 0], self)
         dock = QtW.QDockWidget("Dimensions", self)
         dock.setWidget(sl)
         self.addDockWidget(QtCore.Qt.DockWidgetArea.BottomDockWidgetArea, dock)
-        canvas.events.drawn.connect(self._widget._update_widget_state)
+        canvas.events.drawn.connect(self._widget._update_widget_state, max_args=0)
         self.__class__._instance = self
 
 
 class QtDimSliders(QtW.QWidget):
     changed = QtCore.Signal(object)
 
     def __init__(self, parent=None):
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/_window/_tk.py` & `whitecanvas-0.2.6/whitecanvas/backend/_window/_tk.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def __init__(self, canvas: CanvasGrid):
         super().__init__()
         tkcanvas = TkCanvas(canvas)
         tkcanvas.pack(fill="both", expand=True)
         sl = TkDimSliders(self)
         sl.pack(fill="both", expand=True)
         self.__class__._instance = self
-        canvas.events.drawn.connect(tkcanvas._update_imagetk)
+        canvas.events.drawn.connect(tkcanvas._update_imagetk, max_args=0)
 
 
 class TkSlider(ttk.Scale):
     changed = Signal(int)
 
     def __init__(self, parent=None, **kwargs):
         kwargs["command"] = lambda value: self.changed.emit(int(value))
@@ -94,15 +94,15 @@
                 )
                 slider.pack(fill="both", expand=True)
             else:
                 raise ValueError(f"Unknown axis type {axis}")
             self._widgets[axis.name] = slider
 
     def connect_changed(self, callback: Callable[[dict[str, object]], None]):
-        self.changed.connect(callback)
+        self.changed.connect(callback, max_args=1)
 
     def _emit_changed(self):
         values = {}
         for name, widget in self._widgets.items():
             if isinstance(widget, TkSlider):
                 values[name] = int(widget.get())
             elif isinstance(widget, TkComboBox):
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/_base.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/_labels.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/_labels.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/_legend.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/band.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/bars.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/bars.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,12 +46,24 @@
             self._data.data["x1"],
             self._data.data["y0"],
             self._data.data["y1"],
         )
 
     def _plt_set_data(self, x0, x1, y0, y1):
         cur_data = self._data.data.copy()
+        ndata: int = cur_data["x0"].size
         cur_data.update({"x0": x0, "x1": x1, "y0": y0, "y1": y1})
+        cols_to_update = [
+            "face_color", "edge_color", "width", "pattern", "style", "hovertexts"
+        ]  # fmt: skip
+        if x0.size < ndata:
+            for key in cols_to_update:
+                cur_data[key] = cur_data[key][: x0.size]
+        elif x0.size > ndata:
+            for key in cols_to_update:
+                cur_data[key] = np.concatenate(
+                    [cur_data[key], np.full(x0.size - ndata, cur_data[key][-1])]
+                )
         self._data.data = cur_data
 
     def _plt_get_ndata(self) -> int:
         return len(self._data.data["x0"])
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/canvas.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
         def _cb(event: bk_events.Press):
             self._set_mouse_down(MouseButton.LEFT)
             ev = MouseEvent(
                 button=MouseButton.LEFT,
                 modifiers=_translate_modifiers(event.modifiers),
                 pos=(event.x, event.y),
-                type=MouseEventType.CLICK,
+                type=MouseEventType.PRESS,
             )
             callback(ev)
 
         self._plot.on_event(bk_events.Tap, _cb)
         self._plot.on_event(bk_events.Press, _cb)
 
     def _plt_connect_mouse_drag(self, callback: Callable[[MouseEvent], None]):
@@ -246,14 +246,20 @@
             "start",
             lambda attr, old, new: callback((rng.start, rng.end)),  # noqa: ARG005
         )
 
     def _plt_draw(self):
         pass
 
+    def _plt_get_mouse_enabled(self):
+        return self._plot.toolbar.active_drag is None
+
+    def _plt_set_mouse_enabled(self, enabled: bool):
+        self._plot.toolbar.active_drag = "auto" if enabled else None
+
     def _plt_twinx(self):
         self._plot.extra_y_ranges[SECOND_Y] = bk_models.DataRange1d()
         self._plot.add_layout(
             bk_models.LinearAxis(y_range_name=SECOND_Y),
             "right",
         )
         return Canvas(self._plot, second_y=True)
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/image.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/line.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/markers.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/bokeh/text.py` & `whitecanvas-0.2.6/whitecanvas/backend/bokeh/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/_base.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/_labels.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_labels.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/_legend.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/band.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/bars.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/bars.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,31 +8,38 @@
 from whitecanvas.backend.matplotlib._base import MplMouseEventsMixin
 from whitecanvas.protocols import BarProtocol, check_protocol
 from whitecanvas.types import Hatch, LineStyle
 from whitecanvas.utils.normalize import as_color_array
 from whitecanvas.utils.type_check import is_not_array
 
 
+def _rectangle(x, y, dx, dy) -> Rectangle:
+    r = Rectangle(xy=(x, y), width=dx, height=dy, linestyle="-", picker=True)
+    r.get_path()._interpolation_steps = 100
+    return r
+
+
 @check_protocol(BarProtocol)
 class Bars(BarContainer, MplMouseEventsMixin):
     def __init__(self, xlow, xhigh, ylow, yhigh):
         patches = []
         width = xhigh - xlow
         height = yhigh - ylow
         for x, y, dx, dy in zip(xlow, ylow, width, height):
-            r = Rectangle(xy=(x, y), width=dx, height=dy, linestyle="-", picker=True)
-            r.get_path()._interpolation_steps = 100
-            patches.append(r)
+            patches.append(_rectangle(x, y, dx, dy))
         super().__init__(patches)
         self._visible = True
         MplMouseEventsMixin.__init__(self)
 
     def _plt_get_visible(self):
         return self._visible
 
+    def __iter__(self):
+        return iter(self.patches)
+
     def _plt_set_visible(self, visible):
         for patch in self.patches:
             patch.set_visible(visible)
         self._visible = visible
 
     def _plt_set_zorder(self, zorder: int):
         for patch in self.patches:
@@ -54,24 +61,31 @@
             x0[i] = patch.get_x()
             x1[i] = patch.get_x() + patch.get_width()
             y0[i] = patch.get_y()
             y1[i] = patch.get_y() + patch.get_height()
         return x0, x1, y0, y1
 
     def _plt_set_data(self, x0, x1, y0, y1):
+        for _ in range(x0.size - len(self.patches)):
+            rect = _rectangle(0, 0, 1, 1)
+            self.patches.append(rect)
+            rect.set_visible(self._visible)
+        for _ in range(len(self.patches) - x0.size):
+            self.patches.pop()
         for patch, x0i, x1i, y0i, y1i in zip(self.patches, x0, x1, y0, y1):
             patch.set_x(x0i)
             patch.set_width(x1i - x0i)
             patch.set_y(y0i)
             patch.set_height(y1i - y0i)
-        # TODO: longer or shorter
 
     ##### HasFace protocol #####
 
     def _plt_get_face_color(self) -> NDArray[np.float32]:
+        if len(self.patches) == 0:
+            return np.empty((0, 4), dtype=np.float32)
         return np.stack([patch.get_facecolor() for patch in self.patches], axis=0)
 
     def _plt_set_face_color(self, color: NDArray[np.float32]):
         color = as_color_array(color, size=len(self.patches))
         for patch, c in zip(self.patches, color):
             patch.set_facecolor(c)
 
@@ -83,14 +97,16 @@
             pattern = [pattern] * len(self.patches)
         for pat, patch in zip(pattern, self.patches):
             patch.set_hatch(None if pat is Hatch.SOLID else pat.value)
 
     ##### HasEdges protocol #####
 
     def _plt_get_edge_color(self) -> NDArray[np.float32]:
+        if len(self.patches) == 0:
+            return np.empty((0, 4), dtype=np.float32)
         return np.stack([patch.get_edgecolor() for patch in self.patches], axis=0)
 
     def _plt_set_edge_color(self, color: NDArray[np.float32]):
         color = as_color_array(color, size=len(self.patches))
         for patch, c in zip(self.patches, color):
             patch.set_edgecolor(c)
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/canvas.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/canvas.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 
     def _plt_connect_mouse_click(self, callback: Callable[[MouseEvent], None]):
         """Connect callback to clicked event"""
 
         def _cb(ev: mplMouseEvent):
             if ev.inaxes is not self._axes or ev.dblclick:
                 return
-            callback(self._translate_mouse_event(ev, MouseEventType.CLICK))
+            callback(self._translate_mouse_event(ev, MouseEventType.PRESS))
 
         self._axes.figure.canvas.mpl_connect("button_press_event", _cb)
 
     def _plt_connect_mouse_drag(self, callback: Callable[[MouseEvent], None]):
         """Connect callback to clicked event"""
 
         def _cb(ev: mplMouseEvent):
@@ -250,14 +250,24 @@
 
         self._axes.figure.canvas.mpl_connect("button_release_event", _cb)
 
     def _plt_draw(self):
         if fig := self._axes.get_figure():
             fig.canvas.draw_idle()
 
+    def _plt_get_mouse_enabled(self):
+        return self._axes.get_navigate()
+
+    def _plt_set_mouse_enabled(self, enable: bool):
+        if fig := self._axes.get_figure():
+            if toolbar := getattr(fig.canvas, "toolbar", None):
+                toolbar._update_buttons_checked()
+                return
+        return self._axes.set_navigate(enable)
+
     def _translate_mouse_event(
         self, ev: mplMouseEvent, typ: MouseEventType
     ) -> MouseEvent:
         if ev.key is None:
             modifiers = ()
         else:
             modifiers = []
@@ -301,15 +311,19 @@
             else:
                 sample = make_sample_item(item)
                 if sample is not None:
                     artists.append(sample)
                     names.append(name)
         if artists:
             loc, bbox_to_anchor = _LEGEND_LOC_MAP[anchor]
-            self._axes.legend(artists, names, loc=loc, bbox_to_anchor=bbox_to_anchor)
+            font_size = self._plt_get_xticks()._plt_get_size()
+            self._axes.legend(
+                artists, names, loc=loc, bbox_to_anchor=bbox_to_anchor,
+                prop={"size": font_size},
+            )  # fmt: skip
             if anchor.is_side:
                 self._axes.figure.tight_layout()
 
 
 _MOUSE_BUTTON_MAP = {
     mplMouseButton.LEFT: MouseButton.LEFT,
     mplMouseButton.MIDDLE: MouseButton.MIDDLE,
@@ -396,16 +410,20 @@
         import io
 
         fig = self._fig
         with io.BytesIO() as buff:
             fig.savefig(buff, format="raw")
             buff.seek(0)
             data = np.frombuffer(buff.getvalue(), dtype=np.uint8)
-        w, h = fig.canvas.get_width_height()
-        img = data.reshape((int(h), int(w), -1))
+        # NOTE: fig.canvas.get_width_height() fails if the device pixel ratio is such
+        # as 175%.
+        wmax, hmax = fig.bbox.max
+        width = int(round(wmax / fig.canvas.device_pixel_ratio))
+        height = int(round(hmax / fig.canvas.device_pixel_ratio))
+        img = data.reshape((height, width, -1))
         return img
 
     def _plt_set_figsize(self, width: int, height: int):
         dpi = self._fig.get_dpi()
         self._fig.set_size_inches(width / dpi, height / dpi)
         with warnings.catch_warnings():
             # if the size is small, tight_layout may raise a warning
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/image.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/line.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/markers.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/matplotlib/text.py` & `whitecanvas-0.2.6/whitecanvas/backend/matplotlib/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/mock/_base.py` & `whitecanvas-0.2.6/whitecanvas/backend/mock/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/mock/canvas.py` & `whitecanvas-0.2.6/whitecanvas/backend/mock/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self._xaxis = Axis()
         self._yaxis = Axis()
         self._title = Title()
         self._xticks = Ticks()
         self._yticks = Ticks()
         self._aspect_ratio = None
         self._visible = True
+        self._mouse_enabled = True
         self._obj = MockObject()
 
     def _plt_get_native(self):
         return self._obj
 
     def _plt_get_title(self):
         return self._title
@@ -118,24 +119,30 @@
 
     def _plt_draw(self):
         pass
 
     def _plt_connect_xlim_changed(
         self, callback: Callable[[tuple[float, float]], None]
     ):
-        self._xaxis.lim_changed.connect(callback)
+        self._xaxis.lim_changed.connect(callback, max_args=1)
 
     def _plt_connect_ylim_changed(
         self, callback: Callable[[tuple[float, float]], None]
     ):
-        self._yaxis.lim_changed.connect(callback)
+        self._yaxis.lim_changed.connect(callback, max_args=1)
 
     def _plt_make_legend(self, *args, **kwargs):
         pass
 
+    def _plt_get_mouse_enabled(self):
+        return self._mouse_enabled
+
+    def _plt_set_mouse_enabled(self, enabled: bool):
+        self._mouse_enabled = enabled
+
 
 @protocols.check_protocol(protocols.CanvasGridProtocol)
 class CanvasGrid:
     def __init__(self, heights: list[float], widths: list[float], app: str = "default"):
         self._background_color = np.array([1, 1, 1, 1], dtype=np.float32)
         self._figsize = (100, 100)
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/mock/layers.py` & `whitecanvas-0.2.6/whitecanvas/backend/mock/layers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/_base.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/_labels.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,11 +170,11 @@
     def _plt_get_color(self):
         return np.array(self._plt_get_axis().tickfont.color)
 
     def _plt_set_color(self, color):
         self._plt_get_axis().tickfont.color = rgba_str_color(color)
 
     def _plt_get_text_rotation(self) -> float:
-        return self._plt_get_axis().tickangle
+        return -self._plt_get_axis().tickangle
 
     def _plt_set_text_rotation(self, angle: float):
-        self._plt_get_axis().tickangle = angle
+        self._plt_get_axis().tickangle = -angle
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/_legend.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/band.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/bars.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/bars.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     ##### XXYYDataProtocol #####
     def _plt_get_data(self):
         half_width = self._props["width"] / 2
         x = self._props["x"]
         yhigh = self._props["y"]
         # for some reason, the base property is dtype=object
         ylow = self._props["base"].astype(yhigh.dtype, copy=False)
-        xlow = x - half_width / 2
-        xhigh = x + half_width / 2
+        xlow = x - half_width
+        xhigh = x + half_width
         return xlow, xhigh, ylow, yhigh
 
     def _plt_set_data(self, x0, x1, y0, y1):
         self._props["x"] = (x0 + x1) / 2
         self._props["y"] = y1 - y0
         self._props["width"] = x1 - x0
         self._props["base"] = y0
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/canvas.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,21 @@
 
     def _plt_connect_mouse_release(self, callback: Callable[[MouseEvent], None]):
         """Connect callback to clicked event"""
 
     def _plt_draw(self):
         pass
 
+    def _plt_get_mouse_enabled(self):
+        return self._fig.layout.xaxis.fixedrange
+
+    def _plt_set_mouse_enabled(self, enabled: bool):
+        self._fig.layout.xaxis.fixedrange = not enabled
+        self._fig.layout.yaxis.fixedrange = not enabled
+
     def _plt_twinx(self):
         from plotly._subplots import SubplotRef
 
         # count axis numbers
         y_id = 1
         for _c in self._fig._grid_ref:
             for _r in _c:
@@ -366,15 +373,15 @@
             fig_class = go.Figure
         self._figs = fig_class(
             make_subplots(
                 rows=len(heights),
                 cols=len(widths),
                 row_heights=heights,
                 column_widths=widths,
-            )
+            ),
         )
         self._figs.update_layout(margin={"l": 6, "r": 6, "t": 30, "b": 6})
         self._app = app
         self._heights = heights
         self._widths = widths
 
     def _plt_add_canvas(self, row: int, col: int, rowspan: int, colspan: int) -> Canvas:
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/image.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/line.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/markers.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/plotly/text.py` & `whitecanvas-0.2.6/whitecanvas/backend/plotly/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/_labels.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 from typing import TYPE_CHECKING
 
 import numpy as np
 from cmap import Color
 from qtpy import QtCore
 from qtpy.QtGui import QFont, QPen
 
+from whitecanvas.backend.pyqtgraph._base import PyQtAxis
 from whitecanvas.backend.pyqtgraph._qt_utils import array_to_qcolor
 from whitecanvas.types import LineStyle
 
 if TYPE_CHECKING:
     import pyqtgraph as pg
     from qtpy import QtWidgets as QtW
 
     from whitecanvas.backend.pyqtgraph.canvas import Canvas
 
+_X_AXIS = ("bottom", "top")
+
 
 class _CanvasComponent:
     def __init__(self, canvas: Canvas):
         self._canvas = weakref.ref(canvas)
 
 
 class Title(_CanvasComponent):
@@ -127,30 +130,30 @@
     def _plt_get_axis(self) -> pg.AxisItem:
         return self._canvas()._plot_item.getAxis(self._axis)
 
     def _plt_get_limits(self) -> tuple[float, float]:
         return tuple(self._plt_get_axis().range)
 
     def _plt_set_limits(self, limits: tuple[float, float]):
-        if self._axis == "bottom":
+        if self._axis in _X_AXIS:
             self._canvas()._viewbox().setXRange(*limits, padding=0)
         else:
             self._canvas()._viewbox().setYRange(*limits, padding=0)
 
     def _plt_get_color(self):
         return np.array(self._pen.color().getRgbF())
 
     def _plt_set_color(self, color):
         self._pen.setColor(array_to_qcolor(color))
         self._plt_get_axis().setTextPen(self._pen)
         self._plt_get_axis().setPen(self._pen)
 
     def _plt_flip(self) -> None:
         viewbox: pg.ViewBox = self._plt_get_axis().linkedView()
-        if self._axis == "bottom":
+        if self._axis in _X_AXIS:
             viewbox.invertX()
         elif self._axis == "left":
             viewbox.invertY()
 
     def _plt_set_grid_state(self, visible: bool, color, width: float, style: LineStyle):
         if visible:
             grid = color[3] * 255
@@ -201,20 +204,28 @@
 
     def _plt_reset_override(self):
         self._plt_get_axis().setTicks(None)
 
     def _plt_get_visible(self) -> bool:
         return self._visible
 
+    def _plt_set_fixed_size(self, size: float | None):
+        if self._axis in _X_AXIS:
+            self._plt_get_axis().setHeight(size)
+        else:
+            self._plt_get_axis().setWidth(size)
+
     def _plt_set_visible(self, visible: bool):
         axis = self._plt_get_axis()
         if visible:
             pen = self._pen
+            self._plt_set_fixed_size(None)
         else:
             pen = QPen(array_to_qcolor(np.zeros(4)))
+            self._plt_set_fixed_size(0)
         axis.setTickPen(pen)
         axis.setTextPen(pen)
         self._visible = visible
 
     def _get_font(self) -> QFont:
         return self._plt_get_axis().style["tickFont"]
 
@@ -240,11 +251,16 @@
     def _plt_set_color(self, color):
         pen = self._pen
         pen.setColor(array_to_qcolor(color))
         self._plt_get_axis().setTickPen(pen)
         self._plt_get_axis().setTextPen(pen)
 
     def _plt_get_text_rotation(self) -> float:
-        return 0
+        axis = self._plt_get_axis()
+        if isinstance(axis, PyQtAxis):
+            return axis.style["tickRotation"]
+        return 0.0
 
     def _plt_set_text_rotation(self, rotation: float):
-        raise NotImplementedError
+        axis = self._plt_get_axis()
+        if isinstance(axis, PyQtAxis):
+            axis.setTickRotation(rotation)
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/_legend.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/_qt_utils.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/_qt_utils.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/band.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/bars.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/bars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/canvas.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/canvas.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import qtpy
 from pyqtgraph.GraphicsScene.mouseEvents import HoverEvent as pgHoverEvent
 from pyqtgraph.GraphicsScene.mouseEvents import MouseClickEvent as pgMouseClickEvent
 from qtpy import QtCore, QtGui
 from qtpy.QtCore import Signal
 
 from whitecanvas import protocols
-from whitecanvas.backend.pyqtgraph._base import InsetPlotItem, PyQtLayer
+from whitecanvas.backend.pyqtgraph._base import InsetPlotItem, PyQtAxis, PyQtLayer
 from whitecanvas.backend.pyqtgraph._labels import Axis, AxisLabel, Ticks, Title
 from whitecanvas.backend.pyqtgraph._legend import QtItemSampleBase, make_sample_item
 from whitecanvas.backend.pyqtgraph._qt_utils import from_qt_button, from_qt_modifiers
 from whitecanvas.layers._legend import LegendItem, LegendItemCollection
 from whitecanvas.types import (
     Location,
     MouseButton,
@@ -108,77 +108,90 @@
 
     def _plt_set_visible(self, visible: bool):
         """Set visibility of canvas"""
         self._plot_item.setVisible(visible)
 
     def _plt_twinx(self) -> Canvas:
         """Create a twinx canvas"""
-        plotitem = self._plot_item
-        vb1 = plotitem.vb
+        vb1 = self._plot_item.vb
         vb2 = pg.ViewBox()
-        canvas = Canvas(pg.PlotItem(viewBox=vb2), yaxis="right")
+        new_item = pg.PlotItem(
+            viewBox=vb2,
+            axisItems={"right": PyQtAxis("right"), "bottom": PyQtAxis("bottom")},
+        )
+        canvas = Canvas(new_item, yaxis="right")
 
         self._get_scene().addItem(vb2)
-        plotitem.getAxis("right").linkToView(vb2)
-        vb2.setXLink(plotitem)
+        self._plot_item.getAxis("right").linkToView(vb2)
+        self._plot_item.showAxis("right")
+        vb2.setXLink(self._plot_item)
 
         def _update_views():
             vb2.setGeometry(vb1.sceneBoundingRect())
             vb2.linkedViewChanged(vb1, vb2.XAxis)
 
         _update_views()
         vb1.sigResized.connect(_update_views)
 
         return canvas
 
     def _plt_twiny(self) -> Canvas:
-        plotitem = self._plot_item
-        vb1 = plotitem.vb
+        vb1 = self._plot_item.vb
         vb2 = pg.ViewBox()
-        canvas = Canvas(pg.PlotItem(viewBox=vb2), xaxis="top")
+        new_item = pg.PlotItem(
+            viewBox=vb2, axisItems={"left": PyQtAxis("left"), "top": PyQtAxis("top")}
+        )
+        canvas = Canvas(new_item, xaxis="top")
 
         self._get_scene().addItem(vb2)
-        plotitem.getAxis("bottom").linkToView(vb2)
-        vb2.setYLink(plotitem)
+        self._plot_item.getAxis("bottom").linkToView(vb2)
+        self._plot_item.showAxis("top")
+        vb2.setYLink(self._plot_item)
 
         def _update_views():
             vb2.setGeometry(vb1.sceneBoundingRect())
             vb2.linkedViewChanged(vb1, vb2.YAxis)
 
         _update_views()
         vb1.sigResized.connect(_update_views)
 
         return canvas
 
     def _plt_inset(self, rect: Rect) -> Canvas:
         vb = pg.ViewBox()
-        item = pg.PlotItem(viewBox=vb)
+        item = pg.PlotItem(
+            viewBox=vb,
+            axisItems={"left": PyQtAxis("left"), "bottom": PyQtAxis("bottom")},
+        )
         canvas = Canvas(item)
         inset_item = InsetPlotItem(item, rect)
         inset_item.setParentItem(self._plot_item.vb)
         return canvas
 
     def _get_scene(self) -> pg.GraphicsScene:
         return self._plot_item.scene()
 
     def _plt_connect_mouse_click(self, callback: Callable[[MouseEvent], None]):
         """Connect callback to clicked event"""
 
         def _cb(ev):
-            mev = self._translate_mouse_event(ev, MouseEventType.CLICK)
+            mev = self._translate_mouse_event(ev, MouseEventType.PRESS)
             callback(mev)
 
         self._signals.pressed.connect(_cb)
 
     def _plt_connect_mouse_drag(self, callback: Callable[[MouseEvent], None]):
         """Connect callback to clicked event"""
 
         def _cb(qpoint: QtCore.QPointF):
             mev = self._translate_mouse_event(qpoint, MouseEventType.MOVE)
             callback(mev)
+            if not self._plt_get_mouse_enabled():
+                # for some reason, plot items are not updated when mouse is disabled
+                self._viewbox().update()
 
         self._signals.moved.connect(_cb)
 
     def _plt_connect_mouse_double_click(self, callback: Callable[[MouseEvent], None]):
         """Connect callback to clicked event"""
 
         def _cb(ev):
@@ -228,14 +241,20 @@
                     if sample is not None:
                         legend.addItem(sample, sub_label)
             else:
                 sample = make_sample_item(item)
                 if sample is not None:
                     legend.addItem(sample, label)
 
+    def _plt_get_mouse_enabled(self):
+        return self._viewbox().mouseEnabled()[0]
+
+    def _plt_set_mouse_enabled(self, enabled: bool):
+        self._viewbox().setMouseEnabled(enabled, enabled)
+
     def _translate_mouse_event(
         self,
         ev: QtGui.QMouseEvent | QtCore.QPointF,
         typ: MouseEventType,
     ) -> MouseEvent:
         """Translate a mouse event from pyqtgraph to whitecanvas."""
         if isinstance(ev, QtCore.QPointF):
@@ -308,25 +327,29 @@
         if app == "notebook":
             from pyqtgraph.jupyter import GraphicsLayoutWidget
         elif app in ("default", "qt"):
             from pyqtgraph import GraphicsLayoutWidget
         else:
             raise ValueError(f"pyqtgraph does not support {app!r}")
         self._layoutwidget = GraphicsLayoutWidget()
-        self._heights = heights  # TODO: not used
+        self._heights = heights
         self._widths = widths
 
     def _plt_add_canvas(self, row: int, col: int, rowspan: int, colspan: int) -> Canvas:
         vb = pg.ViewBox()
         item = pg.PlotItem(viewBox=vb)
-        self._layoutwidget.addItem(item, row, col)
-        if rowspan != 1:
-            self._layoutwidget.ci.layout.setRowStretchFactor(row, rowspan)
-        if colspan != 1:
-            self._layoutwidget.ci.layout.setColumnStretchFactor(col, colspan)
+        rspan = sum(self._heights[row : row + rowspan])
+        cspan = sum(self._widths[col : col + colspan])
+        r = sum(self._heights[:row])
+        c = sum(self._widths[:col])
+        self._layoutwidget.addItem(item, r, c)
+        if rspan != 1:
+            self._layoutwidget.ci.layout.setRowStretchFactor(row, rspan)
+        if cspan != 1:
+            self._layoutwidget.ci.layout.setColumnStretchFactor(col, cspan)
         canvas = Canvas(item)
         return canvas
 
     def _plt_show(self) -> bool:
         self._layoutwidget.setVisible(True)
 
     def _get_background_brush(self) -> QtGui.QBrush:
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/image.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/line.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/markers.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/pyqtgraph/text.py` & `whitecanvas-0.2.6/whitecanvas/backend/pyqtgraph/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/vispy/_label.py` & `whitecanvas-0.2.6/whitecanvas/backend/vispy/_label.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from whitecanvas.types import LineStyle
 
 if TYPE_CHECKING:
     from vispy.visuals import LineVisual, TextVisual
 
     from whitecanvas.backend.vispy.canvas import Camera, Canvas
 
-FONT_SIZE_FACTOR = 2.0
-
 
 class TextLabel(scene.Label):
     _text_visual: TextVisual
 
     def _plt_get_visible(self) -> bool:
         return self.visible
 
@@ -35,18 +33,18 @@
     def _plt_get_color(self):
         return np.array(self._text_visual.color).ravel()
 
     def _plt_set_color(self, color):
         self._text_visual.color = color
 
     def _plt_get_size(self) -> int:
-        return self._text_visual.font_size * FONT_SIZE_FACTOR
+        return self._text_visual.font_size
 
     def _plt_set_size(self, size: int):
-        self._text_visual.font_size = size / FONT_SIZE_FACTOR
+        self._text_visual.font_size = size
 
     def _plt_get_fontfamily(self) -> str:
         return self._text_visual.face
 
     def _plt_set_fontfamily(self, family: str):
         self._text_visual.face = family
 
@@ -101,20 +99,19 @@
         camera = self._plt_camera()
         flipped = list(camera.flip)
         axis = 1 - self._dim
         flipped[axis] = not flipped[axis]
         camera.flip = tuple(flipped)
 
     def _plt_set_grid_state(self, visible: bool, color, width: float, style: LineStyle):
-        # if visible:
-        #     self._canvas()._gridlines.visible = True
-        #     self._canvas()._gridlines._grid_color_fn['color'] = color
-        # else:
-        #     self._canvas()._gridlines.visible = False
-        pass  # TODO: implement this
+        grid_lines = self._canvas_ref()._grid_lines
+        if self._dim == 0:  # y
+            grid_lines.set_y_grid_lines(visible, color, width, style)
+        else:
+            grid_lines.set_x_grid_lines(visible, color, width, style)
 
 
 class Ticks:
     def __init__(self, axis: Axis):
         self._axis = weakref.ref(axis)
         axis.axis.ticker = VispyTicker(axis.axis)
 
@@ -148,32 +145,37 @@
         self._axis().axis.tick_color = color
 
     def _plt_get_visible(self) -> bool:
         return self._get_ticker().visible
 
     def _plt_set_visible(self, visible: bool):
         self._get_ticker().visible = visible
+        # axis = self._axis()
+        # if axis._dim == 0:  # y
+        #     axis.width_min = axis.width_max = 40 if visible else 0
+        # else:
+        #     axis.height_min = axis.height_max = 50 if visible else 0
 
     def _plt_get_size(self) -> float:
-        return self._text.font_size * FONT_SIZE_FACTOR
+        return self._text.font_size
 
     def _plt_set_size(self, size: float):
-        self._text.font_size = size / FONT_SIZE_FACTOR
+        self._text.font_size = size
 
     def _plt_get_fontfamily(self) -> str:
         return self._text.face
 
     def _plt_set_fontfamily(self, font):
         self._text.face = font
 
     def _plt_get_text_rotation(self) -> float:
-        return self._text.rotation
+        return -self._text.rotation
 
     def _plt_set_text_rotation(self, rotation: float):
-        self._text.rotation = rotation
+        self._text.rotation = -rotation
 
 
 class VispyTicker(Ticker):
     """Ticker that supports categorical axes"""
 
     axis: AxisVisual
 
@@ -181,25 +183,29 @@
         anchors = axis.ticker._anchors
         super().__init__(axis, anchors)
         self._categorical_labels: tuple[list[float], list[str]] | None = None
         self._visible = True
 
     def _get_tick_frac_labels(self):
         if not self._visible:
-            return np.zeros(0), np.zeros(0), np.zeros(0)
-        if self._categorical_labels is None:
-            return super()._get_tick_frac_labels()
-        pos, labels = self._categorical_labels
-        domain = self.axis.domain
-        scale = domain[1] - domain[0]
-        major_tick_fractions = (np.asarray(pos) - domain[0]) / scale
-        minor_tick_fractions = np.zeros(0)
-        ok = (0 <= major_tick_fractions) & (major_tick_fractions <= 1)
-        tick_labels = np.asarray(labels)[ok]
-        return major_tick_fractions[ok], minor_tick_fractions, tick_labels
+            major, minor, labels = np.zeros(0), np.zeros(0), np.zeros(0)
+        elif self._categorical_labels is None:
+            major, minor, labels = super()._get_tick_frac_labels()
+        else:
+            pos, labels = self._categorical_labels
+            domain = self.axis.domain
+            scale = domain[1] - domain[0]
+            major_tick_fractions = (np.asarray(pos) - domain[0]) / scale
+            minor_tick_fractions = np.zeros(0)
+            ok = (0 <= major_tick_fractions) & (major_tick_fractions <= 1)
+            tick_labels = np.asarray(labels)[ok]
+            major = major_tick_fractions[ok]
+            minor = minor_tick_fractions
+            labels = tick_labels
+        return major, minor, labels
 
     @property
     def visible(self):
         return self._visible
 
     @visible.setter
     def visible(self, visible: bool):
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/vispy/band.py` & `whitecanvas-0.2.6/whitecanvas/backend/vispy/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/vispy/bars.py` & `whitecanvas-0.2.6/whitecanvas/backend/vispy/bars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/vispy/canvas.py` & `whitecanvas-0.2.6/whitecanvas/backend/vispy/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from numpy.typing import NDArray
 from psygnal import Signal
 from vispy import use as vispy_use
 from vispy.scene import PanZoomCamera, SceneCanvas, ViewBox, visuals
 from vispy.util import keys
 
 from whitecanvas import protocols
+from whitecanvas.backend.vispy._gridlines import GridLines
 from whitecanvas.backend.vispy._label import Axis, TextLabel, Ticks
 from whitecanvas.types import Modifier, MouseButton, MouseEvent, MouseEventType
 
 if TYPE_CHECKING:
     from vispy.app.canvas import MouseEvent as vispyMouseEvent
     from vispy.scene import Grid
     from vispy.scene.subscene import SubScene
@@ -68,19 +69,19 @@
             tick_label_margin=5,
             axis_label="",
         )
 
         y_axis.stretch = (0.1, 1)
         grid.add_widget(y_axis, row=1, col=0)
         y_axis.link_view(self._viewbox)
+        self._grid_lines = GridLines(self)
         self._xaxis = x_axis
         self._yaxis = y_axis
         self._xticks = Ticks(x_axis)
         self._yticks = Ticks(y_axis)
-        self._title = TextLabel("")
         self._xlabel = TextLabel("")
         self._ylabel = TextLabel("")
         self._grid = grid
         self._mouse_click_callbacks: list[Callable[[MouseEvent], None]] = []
         self._mouse_move_callbacks: list[Callable[[MouseEvent], None]] = []
         self._mouse_double_click_callbacks: list[Callable[[MouseEvent], None]] = []
         self._mouse_release_callbacks: list[Callable[[MouseEvent], None]] = []
@@ -201,14 +202,20 @@
     def _plt_make_legend(self, *args, **kwargs):
         warnings.warn(
             "Legend is not supported in vispy backend",
             UserWarning,
             stacklevel=2,
         )
 
+    def _plt_get_mouse_enabled(self) -> bool:
+        return self._camera.interactive
+
+    def _plt_set_mouse_enabled(self, enabled: bool):
+        self._camera.interactive = enabled
+
 
 @protocols.check_protocol(protocols.CanvasGridProtocol)
 class CanvasGrid:
     def __init__(self, heights: list[float], widths: list[float], app: str = "default"):
         if app == "qt":  # pragma: no cover
             import importlib
 
@@ -272,30 +279,30 @@
     scene: SubScene
 
     def on_mouse_press(self, event: vispyMouseEvent):
         visual = self.visual_at(event.pos)
         if isinstance(visual, ViewBox) and hasattr(visual, "_canvas_ref"):
             canvas: Canvas = visual._canvas_ref()
             tr = self.scene.node_transform(visual.scene)
-            pos = tr.map(event.pos)[:2] - 0.5
+            pos = tr.map(event.pos)[:2]
             ev = MouseEvent(
                 button=_VISPY_BUTTON_MAP.get(event.button, MouseButton.NONE),
                 modifiers=tuple(_VISPY_KEY_MAP[mod] for mod in event.modifiers),
                 pos=pos,
-                type=MouseEventType.CLICK,
+                type=MouseEventType.PRESS,
             )
             for callback in canvas._mouse_click_callbacks:
                 callback(ev)
 
     def on_mouse_move(self, event: vispyMouseEvent):
         visual = self.visual_at(event.pos)
         if isinstance(visual, ViewBox) and hasattr(visual, "_canvas_ref"):
             canvas: Canvas = visual._canvas_ref()
             tr = self.scene.node_transform(visual.scene)
-            pos = tr.map(event.pos)[:2] - 0.5
+            pos = tr.map(event.pos)[:2]
             ev = MouseEvent(
                 button=_VISPY_BUTTON_MAP.get(event.button, MouseButton.NONE),
                 modifiers=tuple(_VISPY_KEY_MAP[mod] for mod in event.modifiers),
                 pos=pos,
                 type=MouseEventType.MOVE,
             )
 
@@ -303,15 +310,15 @@
                 callback(ev)
 
     def on_mouse_double_click(self, event: vispyMouseEvent):
         visual = self.visual_at(event.pos)
         if isinstance(visual, ViewBox) and hasattr(visual, "_canvas_ref"):
             canvas: Canvas = visual._canvas_ref()
             tr = self.scene.node_transform(visual.scene)
-            pos = tr.map(event.pos)[:2] - 0.5
+            pos = tr.map(event.pos)[:2]
             ev = MouseEvent(
                 button=_VISPY_BUTTON_MAP.get(event.button, MouseButton.NONE),
                 modifiers=tuple(_VISPY_KEY_MAP[mod] for mod in event.modifiers),
                 pos=pos,
                 type=MouseEventType.DOUBLE_CLICK,
             )
 
@@ -344,11 +351,13 @@
     keys.SHIFT: Modifier.SHIFT,
     keys.CONTROL: Modifier.CTRL,
     keys.ALT: Modifier.ALT,
     keys.META: Modifier.META,
 }
 
 _VISPY_BUTTON_MAP = {
-    0: MouseButton.LEFT,
-    1: MouseButton.RIGHT,
-    2: MouseButton.MIDDLE,
+    1: MouseButton.LEFT,
+    2: MouseButton.RIGHT,
+    3: MouseButton.MIDDLE,
+    4: MouseButton.BACK,
+    5: MouseButton.FORWARD,
 }
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/vispy/image.py` & `whitecanvas-0.2.6/whitecanvas/backend/vispy/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/vispy/line.py` & `whitecanvas-0.2.6/whitecanvas/backend/vispy/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/vispy/markers.py` & `whitecanvas-0.2.6/whitecanvas/backend/vispy/markers.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             edge_color = edge_color[: xdata.size]
         self.set_data(
             pos=np.stack([xdata, ydata], axis=1),
             size=size,
             edge_width=edge_width,
             face_color=face_color,
             edge_color=edge_color,
-            symbol=self._plt_get_symbol(),
+            symbol=self.symbol[0],
         )
 
     ##### HasSymbol protocol #####
     def _plt_get_symbol(self) -> Symbol:
         if self._data["a_position"].shape[0] == 0:
             return Symbol.CIRCLE
         sym = self.symbol[0]
@@ -105,15 +105,15 @@
             return
         self.set_data(
             pos=self._data["a_position"],
             size=size,
             edge_width=self._plt_get_edge_width(),
             face_color=self._plt_get_face_color(),
             edge_color=self._plt_get_edge_color(),
-            symbol=self._plt_get_symbol(),
+            symbol=self.symbol,
         )
 
     ##### HasFace protocol #####
     def _plt_get_face_color(self) -> NDArray[np.float32]:
         return self._data["a_bg_color"]
 
     def _plt_set_face_color(self, color: NDArray[np.float32]):
@@ -122,15 +122,15 @@
             return
         self.set_data(
             pos=self._data["a_position"],
             size=self._plt_get_symbol_size(),
             edge_width=self._plt_get_edge_width(),
             face_color=color,
             edge_color=self._plt_get_edge_color(),
-            symbol=self._plt_get_symbol(),
+            symbol=self.symbol,
         )
 
     _plt_get_face_hatch, _plt_set_face_hatch = _not_implemented.face_patterns()
 
     ##### HasEdges protocol #####
     def _plt_get_edge_color(self) -> NDArray[np.float32]:
         return self._data["a_fg_color"]
@@ -141,15 +141,15 @@
             return
         self.set_data(
             pos=self._data["a_position"],
             size=self._plt_get_symbol_size(),
             edge_width=self._plt_get_edge_width(),
             face_color=self._plt_get_face_color(),
             edge_color=color,
-            symbol=self._plt_get_symbol(),
+            symbol=self.symbol,
         )
 
     def _plt_get_edge_width(self) -> NDArray[np.floating]:
         return self._data["a_edgewidth"]
 
     def _plt_set_edge_width(self, width: float):
         if isinstance(width, float):
@@ -158,15 +158,15 @@
             return
         self.set_data(
             pos=self._data["a_position"],
             size=self._plt_get_symbol_size(),
             edge_width=width,
             face_color=self._plt_get_face_color(),
             edge_color=self._plt_get_edge_color(),
-            symbol=self._plt_get_symbol(),
+            symbol=self.symbol,
         )
 
     _plt_get_edge_style, _plt_set_edge_style = _not_implemented.edge_styles()
 
     def _plt_connect_pick_event(self, callback):
         # TODO: implement this
         # https://github.com/napari/napari/blob/main/napari/layers/points/points.py#L1617
```

### Comparing `whitecanvas-0.2.5/whitecanvas/backend/vispy/text.py` & `whitecanvas-0.2.6/whitecanvas/backend/vispy/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 from whitecanvas.backend import _not_implemented
 from whitecanvas.protocols import TextProtocol, check_protocol
 from whitecanvas.types import Alignment, LineStyle
 from whitecanvas.utils.normalize import as_color_array
 from whitecanvas.utils.type_check import is_real_number
 
-FONT_SIZE_FACTOR = 2.0
-
 
 @check_protocol(TextProtocol)
 class Texts(visuals.Text):
     def __init__(
         self, x: NDArray[np.floating], y: NDArray[np.floating], text: list[str]
     ):
         if x.size > 0:
@@ -61,33 +59,33 @@
 
     def _plt_set_text_color(self, color):
         col = as_color_array(color, self._plt_get_ndata())
         if not self._is_empty:
             self.color = col
 
     def _plt_get_text_size(self) -> NDArray[np.floating]:
-        return np.full(self._plt_get_ndata(), self.font_size * FONT_SIZE_FACTOR)
+        return np.full(self._plt_get_ndata(), self.font_size)
 
     def _plt_set_text_size(self, size: float | NDArray[np.floating]):
         if is_real_number(size):
-            self.font_size = size / FONT_SIZE_FACTOR
+            self.font_size = size
         else:
             candidates = np.unique(size)
             if candidates.size == 1:
-                self.font_size = candidates[0] / FONT_SIZE_FACTOR
+                self.font_size = candidates[0]
             elif candidates.size == 0:
                 pass
             else:
                 warnings.warn(
                     "vispy Text layer does not support different font sizes. Set to "
                     "the average size.",
                     UserWarning,
                     stacklevel=4,
                 )
-                self.font_size = np.mean(size) / FONT_SIZE_FACTOR
+                self.font_size = np.mean(size)
 
     def _plt_get_text_position(
         self,
     ) -> tuple[NDArray[np.floating], NDArray[np.floating]]:
         if self._is_empty:
             return np.array([], dtype=np.float32), np.array([], dtype=np.float32)
         return self.pos[:, 0], self.pos[:, 1]
```

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_base.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import warnings
 from abc import ABC, abstractmethod
+from contextlib import contextmanager
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
     Iterator,
     Literal,
@@ -17,25 +19,18 @@
 from cmap import Color
 from numpy.typing import ArrayLike
 from psygnal import Signal, SignalGroup
 from typing_extensions import deprecated
 
 from whitecanvas import layers as _l
 from whitecanvas import protocols, theme
-from whitecanvas._signal import MouseMoveSignal, MouseSignal
 from whitecanvas.backend import Backend, patch_dummy_backend
-from whitecanvas.canvas import (
-    _namespaces as _ns,
-)
-from whitecanvas.canvas import (
-    dataframe as _df,
-)
-from whitecanvas.canvas import (
-    layerlist as _ll,
-)
+from whitecanvas.canvas import _namespaces as _ns
+from whitecanvas.canvas import dataframe as _df
+from whitecanvas.canvas import layerlist as _ll
 from whitecanvas.canvas._between import BetweenPlotter
 from whitecanvas.canvas._dims import Dims
 from whitecanvas.canvas._fit import FitPlotter
 from whitecanvas.canvas._palette import ColorPalette
 from whitecanvas.canvas._stacked import StackOverPlotter
 from whitecanvas.layers import _legend, _mixin
 from whitecanvas.layers import group as _lg
@@ -69,28 +64,26 @@
 _L0 = TypeVar("_L0", _l.Bars, _l.Band)
 _void = _Void()
 
 
 class CanvasEvents(SignalGroup):
     lims = Signal(Rect)
     drawn = Signal()
-    mouse_clicked = MouseSignal(object)
-    mouse_moved = MouseMoveSignal()
-    mouse_double_clicked = MouseSignal(object)
 
 
 class CanvasBase(ABC):
     """Base class for any canvas object."""
 
     title = _ns.TitleNamespace()
     x = _ns.XAxisNamespace()
     y = _ns.YAxisNamespace()
     dims = Dims()
     layers = _ll.LayerList()
     overlays = _ll.LayerList()
+    mouse = _ns.MouseNamespace()
     events: CanvasEvents
 
     def __init__(self, palette: ColormapType | None = None):
         if palette is None:
             palette = theme.get_theme().palette
         self._color_palette = ColorPalette(palette)
         self.events = CanvasEvents()
@@ -108,58 +101,109 @@
         self.x.label.update(family=_ft.family, color=_ft.color, size=_ft.size)
         self.y.label.update(family=_ft.family, color=_ft.color, size=_ft.size)
         self.title.update(family=_ft.family, color=_ft.color, size=_ft.size)
         self.x.ticks.update(family=_ft.family, color=_ft.color, size=_ft.size)
         self.y.ticks.update(family=_ft.family, color=_ft.color, size=_ft.size)
 
         # connect layer events
-        self.layers.events.inserted.connect(self._cb_inserted, unique=True)
-        self.layers.events.removed.connect(self._cb_removed, unique=True)
-        self.layers.events.reordered.connect(self._cb_reordered, unique=True)
-        self.layers.events.connect(self._draw_canvas, unique=True)
-
-        self.overlays.events.inserted.connect(self._cb_overlay_inserted, unique=True)
-        self.overlays.events.removed.connect(self._cb_removed, unique=True)
-        self.overlays.events.connect(self._draw_canvas, unique=True)
+        self.layers.events.inserted.connect(
+            self._cb_inserted, unique=True, max_args=None
+        )
+        self.layers.events.removed.connect(self._cb_removed, unique=True, max_args=None)
+        self.layers.events.reordered.connect(
+            self._cb_reordered, unique=True, max_args=None
+        )
+        self.layers.events.connect(self._draw_canvas, unique=True, max_args=None)
+
+        self.overlays.events.inserted.connect(
+            self._cb_overlay_inserted, unique=True, max_args=None
+        )
+        self.overlays.events.removed.connect(
+            self._cb_removed, unique=True, max_args=None
+        )
+        self.overlays.events.connect(self._draw_canvas, unique=True, max_args=None)
 
         canvas = self._canvas()
         canvas._plt_connect_xlim_changed(self._emit_xlim_changed)
         canvas._plt_connect_ylim_changed(self._emit_ylim_changed)
 
         if hasattr(canvas, "_plt_canvas_hook"):
             canvas._plt_canvas_hook(self)
 
     def _install_mouse_events(self):
         canvas = self._canvas()
-        canvas._plt_connect_mouse_click(self.events.mouse_clicked.emit)
-        canvas._plt_connect_mouse_click(self.events.mouse_moved.emit)
-        canvas._plt_connect_mouse_drag(self.events.mouse_moved.emit)
-        canvas._plt_connect_mouse_release(self.events.mouse_moved.emit)
-        canvas._plt_connect_mouse_double_click(self.events.mouse_double_clicked.emit)
-        canvas._plt_connect_mouse_double_click(self.events.mouse_moved.emit)
+        canvas._plt_connect_mouse_click(self.mouse.clicked.emit)
+        canvas._plt_connect_mouse_click(self.mouse.moved.emit)
+        canvas._plt_connect_mouse_drag(self.mouse.moved.emit)
+        canvas._plt_connect_mouse_release(self.mouse.moved.emit)
+        canvas._plt_connect_mouse_double_click(self.mouse.double_clicked.emit)
+        canvas._plt_connect_mouse_double_click(self.mouse.moved.emit)
 
     def _emit_xlim_changed(self, lim):
         self.x.events.lim.emit(lim)
         self.events.lims.emit(Rect(*lim, *self.y.lim))
 
     def _emit_ylim_changed(self, lim):
         self.y.events.lim.emit(lim)
         self.events.lims.emit(Rect(*self.x.lim, *lim))
 
     def _emit_mouse_moved(self, ev):
         """Emit mouse moved event with autoscaling blocked"""
-        _was_enabled = self._autoscale_enabled
-        # If new layers are added during the mouse move event, the canvas
-        # should not be autoscaled, otherwise unexpected values will be
-        # passed to the callback functions.
-        self._autoscale_enabled = False
+        self.mouse.moved.emit(ev)
+
+    @property
+    def mouse_clicked(self):
+        warnings.warn(
+            "`canvas.events.mouse_clicked` is deprecated. Use `canvas.mouse.clicked` "
+            "instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.mouse.clicked
+
+    @property
+    def mouse_moved(self):
+        warnings.warn(
+            "`canvas.events.mouse_moved` is deprecated. Use `canvas.mouse.moved` "
+            "instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.mouse.clicked
+
+    @property
+    def mouse_double_clicked(self):
+        warnings.warn(
+            "`canvas.events.mouse_double_clicked` is deprecated. Use "
+            "`canvas.mouse.double_clicked` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.mouse.clicked
+
+    @property
+    def autoscale_enabled(self) -> bool:
+        """Return whether autoscale is enabled."""
+        return self._autoscale_enabled
+
+    @autoscale_enabled.setter
+    def autoscale_enabled(self, enabled: bool):
+        if not isinstance(enabled, bool):
+            raise TypeError(f"Expected a bool, got {type(enabled)}.")
+        self._autoscale_enabled = enabled
+
+    @contextmanager
+    def autoscale_context(self, enabled: bool):
+        """Context manager to temporarily change the autoscale state."""
+        _was_enabled = self.autoscale_enabled
+        self.autoscale_enabled = enabled
         try:
-            self.events.mouse_moved.emit(ev)
+            yield
         finally:
-            self._autoscale_enabled = _was_enabled
+            self.autoscale_enabled = _was_enabled
 
     @abstractmethod
     def _get_backend(self) -> Backend:
         """Return the backend."""
 
     @abstractmethod
     def _canvas(self) -> protocols.CanvasProtocol:
@@ -181,14 +225,32 @@
 
     @aspect_ratio.setter
     def aspect_ratio(self, ratio: float | None):
         if ratio is not None:
             ratio = float(ratio)
         self._canvas()._plt_set_aspect_ratio(ratio)
 
+    @property
+    def mouse_enabled(self) -> bool:
+        warnings.warn(
+            "`canvas.mouse_enabled` is deprecated. Use `canvas.mouse.enabled` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.mouse.enabled
+
+    @mouse_enabled.setter
+    def mouse_enabled(self, enabled: bool):
+        warnings.warn(
+            "`canvas.mouse_enabled` is deprecated. Use `canvas.mouse.enabled` instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        self.mouse.enabled = enabled
+
     def autoscale(
         self,
         xpad: float | tuple[float, float] | None = None,
         ypad: float | tuple[float, float] | None = None,
     ) -> tuple[float, float, float, float]:
         """
         Autoscale the canvas to fit the contents.
@@ -966,14 +1028,32 @@
         """
         layer = _l.Image.build_hist(
             x, y, bins=bins, range=(rangex, rangey), density=density, name=name,
             cmap=cmap, backend=self._get_backend(),
         )  # fmt: skip
         return self.add_layer(layer)
 
+    def add_rects(
+        self,
+        coords: ArrayLike,
+        *,
+        name=None,
+        color: ColorType | None = None,
+        alpha: float = 1.0,
+        hatch: str | Hatch | None = None,
+    ) -> _l.Rects[_mixin.ConstFace, _mixin.ConstEdge]:
+        name = self._coerce_name(_l.Rects, name)
+        color = self._generate_colors(color)
+        hatch = theme._default("bars.hatch", hatch)
+        layer = _l.Rects(
+            coords, name=name, color=color, alpha=alpha, hatch=hatch,
+            backend=self._get_backend()
+        )  # fmt: skip
+        return self.add_layer(layer)
+
     def add_cdf(
         self,
         data: ArrayLike1D,
         *,
         name: str | None = None,
         orient: OrientationLike = "vertical",
         color: ColorType | None = None,
@@ -1670,20 +1750,20 @@
         return layer
 
     @overload
     def group_layers(
         self,
         layers: Iterable[_l.Layer],
         name: str | None = None,
-    ) -> _l.LayerGroup:
-        ...
+    ) -> _l.LayerGroup: ...
 
     @overload
-    def group_layers(self, *layers: _l.Layer, name: str | None = None) -> _l.LayerGroup:
-        ...
+    def group_layers(
+        self, *layers: _l.Layer, name: str | None = None
+    ) -> _l.LayerGroup: ...
 
     def group_layers(self, layers, *more_layers, name=None):
         """
         Group layers.
 
         Parameters
         ----------
@@ -1718,18 +1798,18 @@
     def _autoscale_for_layer(
         self,
         layer: _l.Layer,
         pad_rel: float | None = None,
         maybe_empty: bool = True,
     ):
         """This function will be called when a layer is inserted to the canvas."""
+        if not self.autoscale_enabled:
+            return
         if pad_rel is None:
             pad_rel = 0 if layer._NO_PADDING_NEEDED else 0.025
-        if not self._autoscale_enabled:
-            return
         xmin, xmax, ymin, ymax = layer.bbox_hint()
         if len(self.layers) > 1 or not maybe_empty:
             # NOTE: if there was no layer, so backend may not have xlim/ylim,
             # or they may be set to a default value.
             _xmin, _xmax = self.x.lim
             _ymin, _ymax = self.y.lim
             _dx = (_xmax - _xmin) * pad_rel
```

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_between.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_between.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_dims.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_dims.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     def __init__(self, canvas: CanvasBase | None = None):
         self._instances: dict[int, Self] = {}
         self._axes: list[DimAxis] = []
         self.events = DimsEvents()
         if canvas is not None:
             self._canvas_ref = weakref.ref(canvas)
-            self.events.indices.connect(canvas._draw_canvas, unique=True)
+            self.events.indices.connect(canvas._draw_canvas, unique=True, max_args=0)
         else:
             self._canvas_ref = lambda: None
 
     def __get__(self, canvas, owner) -> Self:
         if canvas is None:
             return self
         _id = id(canvas)
```

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_fit.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_fit.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_grid.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         canvas._install_mouse_events()
 
         # link axes if needed
         if self._x_linked:
             self._x_linker_ref.link(canvas.x)
         if self._y_linked:
             self._y_linker_ref.link(canvas.y)
-        canvas.events.drawn.connect(self.events.drawn.emit, unique=True)
+        canvas.events.drawn.connect(self.events.drawn.emit, unique=True, max_args=None)
         return canvas
 
     def _iter_add_canvas(self, **kwargs) -> Iterator[Canvas]:
         for row in range(len(self._heights)):
             for col in range(len(self._widths)):
                 yield self.add_canvas(row, col, **kwargs)
 
@@ -405,9 +405,12 @@
             raise ValueError("Grid must have only one canvas")
         self._main_canvas = canvas
         super().__init__(canvas, grid)
 
         # NOTE: events, dims etc are not shared between the main canvas and the
         # SingleCanvas instance. To avoid confusion, the first and the only canvas
         # should be replaces with the SingleCanvas instance.
+        self.mouse = grid[0, 0].mouse
         grid._canvas_array[0, 0] = self
-        self.events.drawn.connect(self._main_canvas.events.drawn.emit, unique=True)
+        self.events.drawn.connect(
+            self._main_canvas.events.drawn.emit, unique=True, max_args=None
+        )
```

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_imageref.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_imageref.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_joint.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_joint.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_linker.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def link(self, axis: AxisNamespace):
         """Link an axis."""
         axis._get_canvas()  # raise error if the parent canvas is deleted.
         if axis in self._axis_set:
             warnings.warn(f"Axis {axis} already linked", RuntimeWarning, stacklevel=2)
             return
         self._axis_set.add(axis)
-        axis.events.lim.connect(self.set_limits)
+        axis.events.lim.connect(self.set_limits, max_args=1)
 
     def unlink(self, axis: AxisNamespace):
         """Unlink an axis."""
         if axis not in self._axis_set:
             warnings.warn(f"Axis {axis} was not linked", RuntimeWarning, stacklevel=2)
         self._axis_set.discard(axis)
         axis.events.lim.disconnect(self.set_limits)
```

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_namespaces.py` & `whitecanvas-0.2.6/whitecanvas/layers/_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,347 +1,324 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Generic, Iterable, TypeVar
+import weakref
+from abc import ABC, abstractmethod, abstractproperty
+from typing import TYPE_CHECKING, Any, Generic, Iterable, Iterator, TypeVar
 
 import numpy as np
-from cmap import Color
 from numpy.typing import NDArray
 from psygnal import Signal, SignalGroup
 
-from whitecanvas import protocols
-from whitecanvas._exceptions import ReferenceDeletedError
-from whitecanvas.types import ColorType, LineStyle
-from whitecanvas.utils.normalize import arr_color
+from whitecanvas.backend import Backend
+from whitecanvas.layers._legend import EmptyLegendItem, LegendItem
+from whitecanvas.protocols import BaseProtocol
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
-    from whitecanvas.canvas._base import CanvasBase
+    from whitecanvas.canvas import CanvasBase
 
-_no_canvas = object()
+_P = TypeVar("_P", bound=BaseProtocol)
+_L = TypeVar("_L", bound="Layer")
 _T = TypeVar("_T")
 
 
-class AxisSignals(SignalGroup):
-    """Signals emitted by an axis."""
-
-    lim = Signal(tuple)
-
-
-class StrongRef(Generic[_T]):
-    """Strong reference to an object."""
-
-    def __init__(self, obj: _T):
-        self._obj = obj
-
-    def __call__(self) -> _T:
-        return self._obj
-
-
-class Namespace:
-    _attrs: tuple[str, ...] = ()
-
-    def __init__(self, canvas: CanvasBase | None = None):
-        if canvas is not None:
-            # This line *should* be an weak reference, but canvas is sometimes deleted
-            # for some reason. Just use a strong reference for now.
-            self._canvas_ref = StrongRef(canvas)
+class LayerEvents(SignalGroup):
+    data = Signal(check_nargs_on_connect=False)  # (data)
+    name = Signal(str)
+    visible = Signal(bool)
+    _layer_grouped = Signal(object)  # (group)
+
+
+class Layer(ABC):
+    events: LayerEvents
+    _events_class: type[LayerEvents]
+    _ATTACH_TO_AXIS = False
+    _NO_PADDING_NEEDED = False
+
+    def __init__(self, name: str | None = None):
+        if not hasattr(self.__class__, "_events_class"):
+            self.events = LayerEvents()
         else:
-            self._canvas_ref = StrongRef(_no_canvas)
-        self._instances: dict[int, Self] = {}
-
-    def __get__(self, canvas, owner=None) -> Self:
-        if canvas is None:
-            return self
-        while isinstance(canvas, Namespace):
-            canvas = canvas._canvas_ref()
-        id_ = id(canvas)
-        if (ns := self._instances.get(id_)) is None:
-            ns = self._instances[id_] = type(self)(canvas)
-        return ns
-
-    def _get_canvas(self) -> protocols.CanvasProtocol:
-        l = self._canvas_ref()
-        if l is None:
-            raise ReferenceDeletedError("Canvas has been deleted.")
-        elif l is _no_canvas:
-            raise TypeError("No canvas is associated with the class itself.")
-        return l._canvas()
-
-    def __repr__(self) -> str:
-        cname = type(self).__name__
-        l = self._canvas_ref()
-        if l is None:
-            return f"<{cname} of deleted canvas>"
-        elif l is _no_canvas:
-            return f"<{cname}>"
-        props = [f"canvas={l!r}"]
-        for k in self._attrs:
-            v = getattr(self, k)
-            props.append(f"{k}={v!r}")
-        return f"{cname}({', '.join(props)})"
-
-    def update(self, d: dict[str, Any] = {}, **kwargs):
-        values = dict(d, **kwargs)
-        invalid_args = set(values) - set(self._attrs)
-        if invalid_args:
-            raise TypeError(f"Cannot set {invalid_args!r} on {type(self).__name__}")
-        for k, v in values.items():
-            setattr(self, k, v)
-
+            self.events = self.__class__._events_class()
+        self._name = name if name is not None else self.__class__.__name__
+        self._x_hint = self._y_hint = None
+        self._group_layer_ref: weakref.ReferenceType[LayerGroup] | None = None
+        self._canvas_ref = lambda: None
 
-class _TextBoundNamespace(Namespace):
-    _attrs = ("color", "size", "family", "visible")
+    @abstractproperty
+    def visible(self) -> bool:
+        """Return true if the layer is visible"""
 
-    def _get_object(self) -> protocols.TextLabelProtocol:
-        raise NotImplementedError
+    @visible.setter
+    def visible(self, visible: bool):
+        """Set the visibility of the layer"""
 
     @property
-    def color(self):
-        """Text color"""
-        return self._get_object()._plt_get_color()
-
-    @color.setter
-    def color(self, color):
-        self._get_object()._plt_set_color(np.array(Color(color)))
+    def name(self) -> str:
+        """Name of this layer."""
+        return self._name
+
+    @name.setter
+    def name(self, name: str):
+        """Set the name of this layer."""
+        self._name = str(name)
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}<{self.name!r}>"
+
+    def _connect_canvas(self, canvas: CanvasBase):
+        """If needed, do something when layer is added to a canvas."""
+        self.events._layer_grouped.connect(
+            canvas._cb_layer_grouped, unique=True, max_args=1
+        )
+        self.events.connect(canvas._draw_canvas, unique=True, max_args=0)
+        self._canvas_ref = weakref.ref(canvas)
+
+    def _disconnect_canvas(self, canvas: CanvasBase):
+        """If needed, do something when layer is removed from a canvas."""
+        self.events._layer_grouped.disconnect(canvas._cb_layer_grouped)
+        self.events.disconnect(canvas._draw_canvas)
+        self._canvas_ref = lambda: None
 
-    @property
-    def size(self) -> float:
-        """Text font size"""
-        return self._get_object()._plt_get_size()
-
-    @size.setter
-    def size(self, size: float):
-        self._get_object()._plt_set_size(size)
+    def _canvas(self) -> CanvasBase:
+        canvas = self._canvas_ref()
+        if canvas is None:
+            raise ValueError("Layer is not in any canvas.")
+        return canvas
 
-    @property
-    def family(self) -> str:
-        """Text font family."""
-        return self._get_object()._plt_get_fontfamily()
-
-    @family.setter
-    def family(self, font):
-        self._get_object()._plt_set_fontfamily(font)
+    @abstractmethod
+    def bbox_hint(self) -> NDArray[np.float64]:
+        """Return the bounding box hint (xmin, xmax, ymin, ymax) of this layer."""
+
+    def as_overlay(self) -> Self:
+        """Move this layer to the overlay level."""
+        canvas = self._canvas()
+        canvas.layers.remove(self)
+        canvas.overlays.append(self)
+        return self
+
+    def _as_legend_item(self) -> LegendItem:
+        """Return the legend item for this layer."""
+        return EmptyLegendItem()
+
+
+class PrimitiveLayer(Layer, Generic[_P]):
+    """Layers that are composed of a single component."""
+
+    _backend: _P
+    _backend_name: str
+    _backend_class_name = None
 
     @property
     def visible(self) -> bool:
-        """Text visibility."""
-        return self._get_object()._plt_get_visible()
+        """Return true if the layer is visible"""
+        return self._backend._plt_get_visible()
 
     @visible.setter
     def visible(self, visible: bool):
-        self._get_object()._plt_set_visible(visible)
-
-
-class _TextLabelNamespace(_TextBoundNamespace):
-    def __repr__(self) -> str:
-        cname = type(self).__name__
-        l = self._canvas_ref()
-        if l is None:
-            return f"<{cname} of deleted canvas>"
-        elif l is _no_canvas:
-            return f"<{cname}>"
-        text = self.text
-        color = self.color
-        size = self.size
-        family = self.family
-        return f"{cname}({text=!r}, {color=!r}, {size=!r}, {family=!r})"
-
-    @property
-    def text(self) -> str:
-        """Text content."""
-        return self._get_object()._plt_get_text()
-
-    @text.setter
-    def text(self, text: str):
-        self._get_object()._plt_set_text(text)
-
-    def __set__(self, instance, value):
-        # allow canvas.x.label = "X" as a shortcut for canvas.x.label.text = "X"
-        obj = self.__get__(instance)
-        if isinstance(value, str):
-            obj.text = value
-        elif isinstance(value, dict):
-            obj.update(value)
+        """Set the visibility of the layer"""
+        self._backend._plt_set_visible(visible)
+        self.events.visible.emit(visible)
+
+    def _create_backend(self, backend: Backend, *args) -> _P:
+        """Create a backend object."""
+        if self._backend_class_name is not None:
+            self._backend_name = backend.name
+            return backend.get(self._backend_class_name)(*args)
+        for mro in reversed(type(self).__mro__):
+            name = mro.__name__
+            if (
+                issubclass(mro, PrimitiveLayer)
+                and mro is not PrimitiveLayer
+                and backend.has(name)
+            ):
+                self._backend_name = backend.name
+                return backend.get(name)(*args)
+        raise TypeError(
+            f"Cannot create a {backend.name} backend for {type(self).__name__}"
+        )
+
+    def bbox_hint(self) -> NDArray[np.float64]:
+        """Return the bounding box hint (xmin, xmax, ymin, ymax) of this layer."""
+        if self._x_hint is None:
+            _x = (np.nan, np.nan)
         else:
-            raise TypeError(f"Cannot set {value!r} to {type(obj)}.")
+            _x = self._x_hint
+        if self._y_hint is None:
+            _y = (np.nan, np.nan)
+        else:
+            _y = self._y_hint
+        return np.array(_x + _y, dtype=np.float64)
 
 
-class _TicksNamespace(_TextBoundNamespace):
-    def __repr__(self) -> str:
-        cname = type(self).__name__
-        l = self._canvas_ref()
-        if l is None:
-            return f"<{cname} of deleted canvas>"
-        elif l is _no_canvas:
-            return f"<{cname}>"
-        pos, labels = self._get_object()._plt_get_tick_labels()
-        pos = list(pos)
-        color = self.color
-        size = self.size
-        family = self.family
-        return f"{cname}({pos=!r}, {labels=}, {color=!r}, {size=!r}, {family=!r})"
+class DataBoundLayer(PrimitiveLayer[_P], Generic[_P, _T]):
+    @abstractmethod
+    def _get_layer_data(self) -> _T:
+        """Get the data for this layer."""
 
-    def _get_object(self) -> protocols.TicksProtocol:
-        raise NotImplementedError
+    @abstractmethod
+    def _set_layer_data(self, data: _T):
+        """Set the data for this layer."""
 
-    @property
-    def pos(self) -> NDArray[np.floating]:
-        pos, _ = self._get_object()._plt_get_tick_labels()
-        return np.asarray(pos)
+    def _norm_layer_data(self, data: Any) -> _T:
+        """Normalize the data for this layer."""
+        return data
 
     @property
-    def labels(self) -> list[str]:
-        _, labels = self._get_object()._plt_get_tick_labels()
-        return labels
+    def data(self) -> _T:
+        """Data for this layer."""
+        return self._get_layer_data()
 
-    def set_labels(self, pos: Iterable[float], labels: Iterable[str] | None = None):
-        """
-        Override tick labels.
+    @data.setter
+    def data(self, data):
+        """Set the data for this layer."""
+        data_normed = self._norm_layer_data(data)
+        self._set_layer_data(data_normed)
+        self.events.data.emit(data_normed)
 
-        >>> canvas.x.ticks.set_labels([0, 1, 2], ["a", "b", "c"])
 
-        Parameters
-        ----------
-        pos : iterable of float
-            The positions of the ticks.
-        labels : iterable of str, optional
-            The label strings of the ticks. If None, the labels are set to the
-            `pos` values.
-        """
-        _pos = list(pos)
-        # test sorted
-        if len(_pos) > 0 and np.any(np.diff(_pos) <= 0):
-            raise ValueError(f"pos must be strictly increasing, got {pos}.")
-        if labels is not None:
-            _labels = [str(l) for l in labels]
+class HoverableDataBoundLayer(DataBoundLayer[_P, _T]):
+    def with_hover_text(self, text: str | Iterable[Any]) -> Self:
+        """Add hover text to the data points."""
+        if isinstance(text, str):
+            texts = [text] * self.ndata
         else:
-            ndigits = int(np.log10(_pos[-1] - _pos[0])) + 1
-            _labels = [str(round(p, ndigits)) for p in _pos]
-        if len(_pos) != len(_labels):
-            raise ValueError("pos and labels must have the same length.")
-        self._get_object()._plt_override_labels(_pos, _labels)
-        self._get_canvas()._plt_draw()
-
-    def reset_labels(self) -> None:
-        """Reset the tick labels to the default."""
-        self._get_object()._plt_reset_override()
-        self._get_canvas()._plt_draw()
-
-    @property
-    def rotation(self) -> float:
-        """Tick label rotation in degrees."""
-        return self._get_object()._plt_get_text_rotation()
-
-    @rotation.setter
-    def rotation(self, rotation: float):
-        self._get_object()._plt_set_text_rotation(rotation)
-
-
-class XTickNamespace(_TicksNamespace):
-    def _get_object(self):
-        return self._get_canvas()._plt_get_xticks()
-
-
-class YTickNamespace(_TicksNamespace):
-    def _get_object(self):
-        return self._get_canvas()._plt_get_yticks()
+            texts = [str(t) for t in text]
+        if len(texts) != self.ndata:
+            raise ValueError(
+                "Expected text to have the same size as the data, "
+                f"got {len(texts)} and {self.ndata}"
+            )
+        self._backend._plt_set_hover_text(texts)
+        return self
 
+    @abstractproperty
+    def ndata(self) -> int:
+        """Number of data points."""
+
+
+class LayerGroup(Layer):
+    """
+    A group of layers that will be treated as a single layer in the canvas.
+    """
+
+    def __init__(self, name: str | None = None):
+        super().__init__(name)
+        self._visible = True
+
+    @abstractmethod
+    def iter_children(self) -> Iterator[Layer]:
+        """Iterate over all children."""
+
+    def iter_primitive(self) -> Iterator[PrimitiveLayer[BaseProtocol]]:
+        for child in self.iter_children():
+            if isinstance(child, LayerGroup):
+                yield from child.iter_primitive()
+            elif isinstance(child, LayerWrapper):
+                if isinstance(child._base_layer, LayerGroup):
+                    yield from child._base_layer.iter_primitive()
+                else:
+                    yield child._base_layer
+            else:
+                yield child
+
+    def _emit_layer_grouped(self):
+        """Emit all the grouped signal."""
+        for c in self.iter_children():
+            c.events._layer_grouped.emit(self)
 
-class TitleNamespace(_TextLabelNamespace):
-    def _get_object(self):
-        return self._get_canvas()._plt_get_title()
+    @property
+    def visible(self) -> bool:
+        """Return true if the layer is visible"""
+        return self._visible
 
+    @visible.setter
+    def visible(self, visible: bool):
+        """Set the visibility of the layer"""
+        self._visible = visible
+        for child in self.iter_children():
+            child.visible = visible
+        self.events.visible.emit(visible)
 
-class XLabelNamespace(_TextLabelNamespace):
-    def _get_object(self):
-        return self._get_canvas()._plt_get_xlabel()
+    @property
+    def _backend_name(self) -> str:
+        """The backend name of this layer group."""
+        for child in self.iter_children():
+            return child._backend_name
+        raise RuntimeError(f"No backend name found for {self!r}")
 
+    def bbox_hint(self) -> NDArray[np.float64]:
+        """
+        Return the bounding box hint (xmin, xmax, ymin, ymax) of this group.
 
-class YLabelNamespace(_TextLabelNamespace):
-    def _get_object(self):
-        return self._get_canvas()._plt_get_ylabel()
+        Note that unless children notifies the change of their bounding box hint, bbox
+        hint needs recalculation.
+        """
+        hints = [child.bbox_hint() for child in self.iter_children()]
+        if len(hints) == 0:
+            return np.array([np.nan, np.nan, np.nan, np.nan], dtype=np.float64)
+        ar = np.stack(hints, axis=1)
+        # Any of the four corners could be all-nan. In that case, we should return nan.
+        # Otherwise, we should return the known min/max.
+        allnan = np.isnan(ar).all(axis=1)
+        xmin = np.nan if allnan[0] else np.nanmin(ar[0, :])
+        xmax = np.nan if allnan[1] else np.nanmax(ar[1, :])
+        ymin = np.nan if allnan[2] else np.nanmin(ar[2, :])
+        ymax = np.nan if allnan[3] else np.nanmax(ar[3, :])
+        return np.array([xmin, xmax, ymin, ymax], dtype=np.float64)
 
 
-class AxisNamespace(Namespace):
-    events: AxisSignals
-    _attrs = ("lim", "color", "flipped")
+class LayerWrapper(Layer, Generic[_L]):
+    def __init__(
+        self,
+        base_layer: _L,
+    ):
+        self._base_layer = base_layer
+        super().__init__(base_layer.name)
 
-    def __init__(self, canvas: CanvasBase | None = None):
-        super().__init__(canvas)
-        self.events = AxisSignals()
-        self._flipped = False
+    @property
+    def visible(self) -> bool:
+        """Whether the layer is visible."""
+        return self._base_layer.visible
 
-    def _get_object(self) -> protocols.AxisProtocol:
-        raise NotImplementedError
+    @visible.setter
+    def visible(self, visible: bool):
+        self._base_layer.visible = visible
 
     @property
-    def lim(self) -> tuple[float, float]:
-        """Limits of the axis."""
-        return self._get_object()._plt_get_limits()
-
-    @lim.setter
-    def lim(self, lim: tuple[float, float]):
-        low, high = lim
-        if low >= high:
-            a = type(self).__name__[0].lower()
-            raise ValueError(
-                f"low must be less than high, but got {lim!r}. If you "
-                f"want to flip the axis, use `canvas.{a}.flipped = True`."
-            )
-        # Manually emit signal. This is needed when the plot backend is
-        # implemented in JS (such as bokeh) and the python callback is not
-        # enabled. Otherwise axis linking fails.
-        with self.events.blocked():
-            self._get_object()._plt_set_limits(lim)
-        self.events.lim.emit(lim)
-        return None
+    def name(self) -> str:
+        """Name of the layer."""
+        return self._base_layer.name
 
-    @property
-    def color(self):
-        """Color of the axis."""
-        return self._get_object()._plt_get_color()
-
-    @color.setter
-    def color(self, color):
-        self._get_object()._plt_set_color(np.array(Color(color)))
+    @name.setter
+    def name(self, name: str):
+        self._base_layer.name = name
 
     @property
-    def flipped(self) -> bool:
-        """Return true if the axis is flipped."""
-        return self._flipped
-
-    @flipped.setter
-    def flipped(self, flipped: bool):
-        """Set the axis to be flipped."""
-        if flipped != self._flipped:
-            self._get_object()._plt_flip()
-            self._flipped = flipped
-
-    def set_gridlines(
-        self,
-        visible: bool = True,
-        color: ColorType = "gray",
-        width: float = 1.0,
-        style: str | LineStyle = LineStyle.SOLID,
-    ):
-        color = arr_color(color)
-        style = LineStyle(style)
-        if width < 0:
-            raise ValueError("width must be non-negative.")
-        self._get_object()._plt_set_grid_state(visible, color, width, style)
+    def base(self) -> _L:
+        """The base layer."""
+        return self._base_layer
 
+    def bbox_hint(self) -> NDArray[np.floating]:
+        """Return the bounding box hint using the base layer."""
+        return self._base_layer.bbox_hint()
 
-class XAxisNamespace(AxisNamespace):
-    label = XLabelNamespace()
-    ticks = XTickNamespace()
+    def _connect_canvas(self, canvas: CanvasBase):
+        self._base_layer._connect_canvas(canvas)
+        return super()._connect_canvas(canvas)
 
-    def _get_object(self):
-        return self._get_canvas()._plt_get_xaxis()
+    def _disconnect_canvas(self, canvas: CanvasBase):
+        self._base_layer._disconnect_canvas(canvas)
+        return super()._disconnect_canvas(canvas)
 
+    @property
+    def _ATTACH_TO_AXIS(self) -> bool:
+        return self._base_layer._ATTACH_TO_AXIS
 
-class YAxisNamespace(AxisNamespace):
-    label = YLabelNamespace()
-    ticks = YTickNamespace()
+    @property
+    def _NO_PADDING_NEEDED(self) -> bool:
+        return self._base_layer._NO_PADDING_NEEDED
 
-    def _get_object(self):
-        return self._get_canvas()._plt_get_yaxis()
+    def _as_legend_item(self) -> LegendItem:
+        """Return the legend item for this layer."""
+        return self._base_layer._as_legend_item()
```

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_palette.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_palette.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/_stacked.py` & `whitecanvas-0.2.6/whitecanvas/canvas/_stacked.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/layerlist.py` & `whitecanvas-0.2.6/whitecanvas/canvas/layerlist.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_base.py` & `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_base.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_both_cat.py` & `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_both_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_feature_cat.py` & `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_feature_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_joint_cat.py` & `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_joint_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_one_cat.py` & `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_one_cat.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,22 @@
     def __get__(self, ins: _C, owner) -> Self:
         return _Aggregator(self._method, ins)
 
     def __repr__(self) -> str:
         return f"Aggregator<{self._method}>"
 
     def __call__(self) -> OneAxisCatAggPlotter[_C, _DF]:
-        """Aggregate the values before plotting it."""
+        """
+        Aggregate the values before plotting it.
+
+        Examples
+        --------
+        Calculate mean of "value" for each "group" and connect them with lines.
+        >>> canvas.cat_x(df, "group", "value").mean().add_line()
+        """
         plotter = self._plotter
         if plotter is None:
             raise TypeError("Cannot call this method from a class.")
         if self._method == "size":
             value = "size"
         elif plotter._value is None:
             raise ValueError("Value column is not specified.")
@@ -241,14 +248,15 @@
     ### 1-D categorical ###
 
     def add_violinplot(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | None = None,
         hatch: NStr | None = None,
         dodge: NStr | bool = True,
         extent: float = 0.8,
         shape: str = "both",
     ) -> _lt.DFViolinPlot[_DF]:
         """
         Add a categorical violin plot.
@@ -263,14 +271,16 @@
 
         Parameters
         ----------
         name : str, optional
             Name of the layer.
         color : str or sequence of str, optional
             Column name(s) for coloring the lines. Must be categorical.
+        alpha : float, optional
+            Opacity of the layer.
         hatch : str or sequence of str, optional
             Column name(s) for hatches. Must be categorical.
         dodge : str, sequence of str or bool, optional
             Column name(s) for dodging. If True, column name(s) for splitting the data
             will all be used for dodging to avoid overlap.
         extent : float, default 0.8
             Width of the violins. Usually in range (0, 1].
@@ -284,22 +294,23 @@
         """
         canvas = self._canvas()
         layer = _lt.DFViolinPlot(
             self._cat_iter, self._get_value(), name=name, color=color, hatch=hatch,
             dodge=dodge, extent=extent, shape=shape, orient=self._orient,
             backend=canvas._get_backend(),
         )  # fmt: skip
-        self._post_add_boxlike(layer, color)
+        self._post_add_boxlike(layer, color, alpha)
         return canvas.add_layer(layer)
 
     def add_boxplot(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | None = None,
         hatch: NStr | None = None,
         dodge: NStr | bool = True,
         capsize: float = 0.1,
         extent: float = 0.8,
     ) -> _lt.DFBoxPlot[_DF]:
         """
         Add a categorical box plot.
@@ -314,14 +325,16 @@
 
         Parameters
         ----------
         name : str, optional
             Name of the layer.
         color : str or sequence of str, optional
             Column name(s) for coloring the lines. Must be categorical.
+        alpha : float, optional
+            Opacity of the layer.
         hatch : str or sequence of str, optional
             Column name(s) for hatches. Must be categorical.
         dodge : str, sequence of str or bool, optional
             Column name(s) for dodging. If True, column name(s) for splitting the data
             will all be used for dodging to avoid overlap.
         capsize : float, default 0.1
             Length of the caps as a fraction of the width of the box.
@@ -335,22 +348,23 @@
         """
         canvas = self._canvas()
         layer = _lt.DFBoxPlot(
             self._cat_iter, self._get_value(), name=name, color=color, hatch=hatch,
             dodge=dodge, orient=self._orient, capsize=capsize, extent=extent,
             backend=canvas._get_backend(),
         )  # fmt: skip
-        self._post_add_boxlike(layer, color)
+        self._post_add_boxlike(layer, color, alpha)
         return canvas.add_layer(layer)
 
     def add_pointplot(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | None = None,
         hatch: NStr | None = None,
         dodge: NStr | bool = True,
         capsize: float = 0.1,
     ) -> _lt.DFPointPlot[_DF]:
         """
         Add a categorical point plot (markers with error bars).
 
@@ -370,14 +384,16 @@
 
         Parameters
         ----------
         name : str, optional
             Name of the layer.
         color : str or sequence of str, optional
             Column name(s) for coloring the lines. Must be categorical.
+        alpha : float, optional
+            Opacity of the layer.
         hatch : str or sequence of str, optional
             Column name(s) for hatches. Must be categorical.
         dodge : str, sequence of str or bool, optional
             Column name(s) for dodging. If True, column name(s) for splitting the data
             will all be used for dodging to avoid overlap.
         capsize : float, default 0.1
             Length of the caps as a fraction of the width of the box.
@@ -389,22 +405,23 @@
         """
         canvas = self._canvas()
         layer = _lt.DFPointPlot(
             self._cat_iter, self._get_value(), name=name, color=color, hatch=hatch,
             dodge=dodge, orient=self._orient, capsize=capsize,
             backend=canvas._get_backend(),
         )  # fmt: skip
-        self._post_add_boxlike(layer, color)
+        self._post_add_boxlike(layer, color, alpha)
         return canvas.add_layer(layer)
 
     def add_barplot(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | None = None,
         hatch: NStr | None = None,
         dodge: NStr | bool = True,
         capsize: float = 0.1,
         extent: float = 0.8,
     ) -> _lt.DFBarPlot[_DF]:
         """
         Add a categorical bar plot (bars with error bars).
@@ -425,14 +442,16 @@
 
         Parameters
         ----------
         name : str, optional
             Name of the layer.
         color : str or sequence of str, optional
             Column name(s) for coloring the lines. Must be categorical.
+        alpha : float, optional
+            Opacity of the layer.
         hatch : str or sequence of str, optional
             Column name(s) for hatches. Must be categorical.
         dodge : str, sequence of str or bool, optional
             Column name(s) for dodging. If True, column name(s) for splitting the data
             will all be used for dodging to avoid overlap.
         capsize : float, default 0.1
             Length of the caps as a fraction of the width of the box.
@@ -446,29 +465,32 @@
         """
         canvas = self._canvas()
         layer = _lt.DFBarPlot(
             self._cat_iter, self._get_value(), name=name, color=color, hatch=hatch,
             dodge=dodge, orient=self._orient, capsize=capsize, extent=extent,
             backend=canvas._get_backend(),
         )  # fmt: skip
-        self._post_add_boxlike(layer, color)
+        self._post_add_boxlike(layer, color, alpha)
         return canvas.add_layer(layer)
 
-    def _post_add_boxlike(self, layer: _BoxLikeMixin, color):
+    def _post_add_boxlike(self, layer: _BoxLikeMixin, color, alpha):
         canvas = self._canvas()
         if color is not None and not layer._color_by.is_const():
             layer.update_color_palette(canvas._color_palette)
         elif color is None:
             layer.update_const(color=canvas._color_palette.next())
+        if alpha is not None:
+            layer.update_const(alpha=alpha)
 
     def add_stripplot(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | str | None = None,
         hatch: NStr | None = None,
         symbol: NStr | None = None,
         size: str | None = None,
         dodge: NStr | bool = False,
         extent: float = 0.5,
         seed: int | None = 0,
     ) -> _lt.DFMarkerGroups[_DF]:
@@ -485,14 +507,16 @@
 
         Parameters
         ----------
         name : str, optional
             Name of the layer.
         color : str or sequence of str, optional
             Column name(s) for coloring the lines. Must be categorical.
+        alpha : float or str, optional
+            Opacity of the markers. If str, it must be a numerical column name.
         hatch : str or sequence of str, optional
             Column name(s) for hatches. Must be categorical.
         symbol : str or sequence of str, optional
             Column name(s) for symbols. Must be categorical.
         size : str, optional
             Column name for marker size. Must be numerical.
         dodge : str, sequence of str or bool, optional
@@ -522,41 +546,40 @@
         yj = _jitter.IdentityJitter(self._get_value()).check(df)
         if not self._orient.is_vertical:
             xj, yj = yj, xj
         layer = _lt.DFMarkerGroups(
             df, xj, yj, name=name, color=color, hatch=hatch, orient=self._orient,
             symbol=symbol, size=size, backend=canvas._get_backend(),
         )  # fmt: skip
-        if color is not None and not layer._color_by.is_const():
-            layer.update_color(layer._color_by.by, palette=canvas._color_palette)
-        elif color is None:
-            layer.update_color(canvas._color_palette.next())
+        layer._init_color_for_canvas(color, alpha, canvas)
         return canvas.add_layer(layer)
 
     def add_markers(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | str | None = None,
         hatch: NStr | None = None,
         symbol: NStr | None = None,
         size: str | None = None,
         dodge: NStr | bool = False,
     ) -> _lt.DFMarkerGroups[_DF]:
         """Alias of `add_stripplot` with no jittering."""
         return self.add_stripplot(
-            color=color, hatch=hatch, symbol=symbol, size=size, dodge=dodge,
-            extent=0, seed=0, name=name,
+            color=color, alpha=alpha, hatch=hatch, symbol=symbol, size=size,
+            dodge=dodge, extent=0, seed=0, name=name,
         )  # fmt: skip
 
     def add_swarmplot(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | str | None = None,
         hatch: NStr | None = None,
         symbol: NStr | None = None,
         size: str | None = None,
         dodge: NStr | bool = False,
         extent: float = 0.8,
         sort: bool = False,
     ) -> _lt.DFMarkerGroups[_DF]:
@@ -573,14 +596,16 @@
 
         Parameters
         ----------
         name : str, optional
             Name of the layer.
         color : str or sequence of str, optional
             Column name(s) for coloring the lines. Must be categorical.
+        alpha : float or str, optional
+            Opacity of the markers. If str, it must be a numerical column name.
         hatch : str or sequence of str, optional
             Column name(s) for hatches. Must be categorical.
         symbol : str or sequence of str, optional
             Column name(s) for symbols. Must be categorical.
         size : str, optional
             Column name for marker size. Must be numerical.
         dodge : str, sequence of str or bool, optional
@@ -614,25 +639,23 @@
         yj = _jitter.IdentityJitter(val).check(df)
         if not self._orient.is_vertical:
             xj, yj = yj, xj
         layer = _lt.DFMarkerGroups(
             df, xj, yj, name=name, color=color, hatch=hatch, orient=self._orient,
             symbol=symbol, size=size, backend=canvas._get_backend(),
         )  # fmt: skip
-        if color is not None and not layer._color_by.is_const():
-            layer.update_color(layer._color_by.by, palette=canvas._color_palette)
-        elif color is None:
-            layer.update_color(canvas._color_palette.next())
+        layer._init_color_for_canvas(color, alpha, canvas)
         return canvas.add_layer(layer)
 
     def add_rugplot(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | str | None = None,
         width: float | None = None,
         style: NStr | None = None,
         dodge: NStr | bool = True,
         extent: float = 0.8,
     ) -> _lt.DFRugGroups[_DF]:
         """
         Add a categorical rug plot.
@@ -647,14 +670,16 @@
 
         Parameters
         ----------
         name : str, optional
             Name of the layer.
         color : str or sequence of str, optional
             Column name(s) for coloring the lines. Must be categorical.
+        alpha : float or str, optional
+            Opacity of the markers. If str, it must be a numerical column name.
         hatch : str or sequence of str, optional
             Column name(s) for hatches. Must be categorical.
         symbol : str or sequence of str, optional
             Column name(s) for symbols. Must be categorical.
         size : str, optional
             Column name for marker size. Must be numerical.
         dodge : str, sequence of str or bool, optional
@@ -680,18 +705,15 @@
         _map = self._cat_iter.prep_position_map(splitby, dodge)
         _extent = self._cat_iter.zoom_factor(dodge) * extent
         jitter = _jitter.CategoricalJitter(splitby, _map)
         layer = _lt.DFRugGroups.from_table(
             df, jitter, self._get_value(), name=name, color=color, orient=self._orient,
             extent=_extent, width=width, style=style, backend=canvas._get_backend(),
         )  # fmt: skip
-        if color is not None and not layer._color_by.is_const():
-            layer.update_color(layer._color_by.by, palette=canvas._color_palette)
-        elif color is None:
-            layer.update_color(canvas._color_palette.next())
+        layer._init_color_for_canvas(color, alpha, canvas)
         return canvas.add_layer(layer)
 
     def add_heatmap_hist(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
@@ -771,14 +793,15 @@
         self._cat_iter = cat_iter
 
     def add_line(
         self,
         *,
         name: str | None = None,
         color: NStr | None = None,
+        alpha: float | None = None,
         width: float | None = None,
         style: NStr | None = None,
         dodge: NStr | bool = False,
     ) -> _lt.DFLines[_DF]:
         """
         Add line that connect the aggregated values.
 
@@ -817,21 +840,24 @@
             df_agg, xj, yj, name=name, color=color, width=width, style=style,
             backend=canvas._get_backend(),
         )  # fmt: skip
         if color is not None and not layer._color_by.is_const():
             layer.update_color(color, palette=canvas._color_palette)
         elif color is None:
             layer.update_color(canvas._color_palette.next())
+        if alpha is not None:
+            layer.update_alpha(alpha)
         return canvas.add_layer(layer)
 
     def add_markers(
         self,
         *,
         name: str | None = None,
         color: NStr | ColorType | None = None,
+        alpha: float | None = None,
         hatch: NStr | Hatch | None = None,
         size: str | float | None = None,
         symbol: NStr | Symbol | None = None,
         dodge: NStr | bool = False,
     ) -> _lt.DFMarkers[_DF]:
         """
         Add markers that represent the aggregated values.
@@ -876,21 +902,24 @@
             df_agg, xj, yj, name=name, color=color, hatch=hatch, size=size,
             symbol=symbol, backend=canvas._get_backend(),
         )  # fmt: skip
         if color is not None and not layer._color_by.is_const():
             layer.update_color(color, palette=canvas._color_palette)
         elif color is None:
             layer.update_color(canvas._color_palette.next())
+        if alpha is not None:
+            layer.update_alpha(alpha)
         return canvas.add_layer(layer)
 
     def add_bars(
         self,
         *,
         name: str | None = None,
         color: NStr | ColorType | None = None,
+        alpha: float | None = None,
         hatch: NStr | Hatch | None = None,
         extent: float = 0.8,
         dodge: NStr | bool = True,
     ) -> _lt.DFBars[_DF]:
         """
         Add bars that represent the aggregated values.
 
@@ -934,14 +963,16 @@
             df_agg, xj, yj, name=name, color=color, hatch=hatch, extent=_extent,
             backend=canvas._get_backend(),
         )  # fmt: skip
         if color is not None and not layer._color_by.is_const():
             layer.update_color(color, palette=canvas._color_palette)
         elif color is None:
             layer.update_color(canvas._color_palette.next())
+        if alpha is not None:
+            layer.update_alpha(alpha)
         return canvas.add_layer(layer)
 
     def _aggregate(
         self,
         df: DataFrameWrapper[_DF],
         by: tuple[str, ...],
         on: str,
```

### Comparing `whitecanvas-0.2.5/whitecanvas/canvas/dataframe/_stacked_cat.py` & `whitecanvas-0.2.6/whitecanvas/canvas/dataframe/_stacked_cat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/__init__.py` & `whitecanvas-0.2.6/whitecanvas/layers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Errorbars,
     Image,
     InfCurve,
     InfLine,
     Line,
     Markers,
     MultiLine,
+    Rects,
     Rug,
     Spans,
     Texts,
 )
 
 __all__ = [
     "Layer",
@@ -35,9 +36,10 @@
     "Spans",
     "Errorbars",
     "Band",
     "Rug",
     "InfLine",
     "InfCurve",
     "Texts",
+    "Rects",
     "Image",
 ]
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_legend.py` & `whitecanvas-0.2.6/whitecanvas/layers/_legend.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_mixin.py` & `whitecanvas-0.2.6/whitecanvas/layers/_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,16 +99,15 @@
         raise NotImplementedError
 
     @abstractproperty
     def alpha(self) -> float | NDArray[np.floating]:
         raise NotImplementedError
 
     @abstractmethod
-    def update(self, color=None, hatch=None, alpha=1.0):
-        ...
+    def update(self, color=None, hatch=None, alpha=1.0): ...
 
 
 class EdgeNamespace(LayerNamespace[PrimitiveLayer[_lp.HasEdges]]):
     _properties = ("color", "style", "width")
     events: EdgeEvents
     _events_class = EdgeEvents
 
@@ -125,16 +124,15 @@
         raise NotImplementedError
 
     @abstractproperty
     def alpha(self) -> float | NDArray[np.floating]:
         raise NotImplementedError
 
     @abstractmethod
-    def update(self, color=None, width=None, style=None, alpha=1.0):
-        ...
+    def update(self, color=None, width=None, style=None, alpha=1.0): ...
 
 
 class SinglePropertyFaceBase(FaceNamespace):
     def update(
         self,
         *,
         color: ColorType | _Void = _void,
@@ -327,14 +325,20 @@
 
     @property
     def alpha(self) -> float:
         return float(self.color[3])
 
     @alpha.setter
     def alpha(self, value: float):
+        if not is_real_number(value):
+            raise ValueError(
+                "Alpha must be a real number for a constant-face layer. If you want to "
+                "set multiple alpha values, use `with_face_multi` method to convert "
+                "the layer to a multi-face layer."
+            )
         if not 0 <= value <= 1:
             raise ValueError(f"Alpha must be between 0 and 1, got {value!r}")
         try:
             self.color = (*self.color[:3], value)
         except IndexError:
             pass  # when the layer is empty
 
@@ -420,27 +424,39 @@
         widths = self._layer._backend._plt_get_edge_width()
         if len(widths) > 0:
             return widths[0]
         return 0.0
 
     @width.setter
     def width(self, value: float):
+        if not is_real_number(value):
+            raise ValueError(
+                "Width must be a real number for a constant-edge layer. If you want to "
+                "set multiple width values, use `with_edge_multi` method to convert "
+                "the layer to a multi-edge layer."
+            )
         if value < 0:
             raise ValueError(f"Edge width must be non-negative, got {value!r}")
         value = float(value)
         self._layer._backend._plt_set_edge_width(value)
         self.events.width.emit(value)
 
     @property
     def alpha(self) -> float:
         """The alpha value of the edge."""
         return float(self.color[3])
 
     @alpha.setter
     def alpha(self, value: float):
+        if not is_real_number(value):
+            raise ValueError(
+                "Alpha must be a real number for a constant-edge layer. If you want to "
+                "set multiple alpha values, use `with_edge_multi` method to convert "
+                "the layer to a multi-edge layer."
+            )
         if not 0 <= value <= 1:
             raise ValueError(f"Alpha must be between 0 and 1, got {value!r}")
         self.color = (*self.color[:3], value)
 
 
 class MultiFace(MultiPropertyFaceBase):
     @property
@@ -538,19 +554,19 @@
     _events_class = FaceEdgeMixinEvents
 
     def __init__(self, face: _NFace, edge: _NEdge):
         self._face_namespace = face
         self._edge_namespace = edge
 
     def _init_events(self):
-        self._face_namespace.events.connect(self.events.face.emit)
-        self._edge_namespace.events.connect(self.events.edge.emit)
+        self._face_namespace.events.connect(self.events.face.emit, max_args=None)
+        self._edge_namespace.events.connect(self.events.edge.emit, max_args=None)
         # _face_namespace may change! _make_sure_hatch_visible should connected to
         # the layer event.
-        self.events.face.connect(self._make_sure_hatch_visible)
+        self.events.face.connect(self._make_sure_hatch_visible, max_args=0)
 
     @property
     def face(self) -> _NFace:
         """The face namespace."""
         return self._face_namespace
 
     @property
@@ -582,18 +598,31 @@
             color = get_theme().foreground_color
         self.edge.update(color=color, style=style, width=width, alpha=alpha)
         return self
 
     def _make_sure_hatch_visible(self):
         pass
 
+    color = property()
+
+    @color.setter
+    def color(self, value):
+        self.face.color = value
+        self.edge.color = value
+
+    alpha = property()
+
+    @alpha.setter
+    def alpha(self, value):
+        self.face.alpha = value
+        self.edge.alpha = value
+
     if TYPE_CHECKING:
 
-        def _as_legend_item(self) -> _legend.LegendItem:
-            ...
+        def _as_legend_item(self) -> _legend.LegendItem: ...
 
 
 class FaceEdgeMixin(AbstractFaceEdgeMixin[MonoFace, MonoEdge]):
     def __init__(self):
         super().__init__(MonoFace(self), MonoEdge(self))
 
     def _make_sure_hatch_visible(self):
@@ -614,15 +643,15 @@
         hatch: Hatch | str = Hatch.SOLID,
         alpha: float = 1,
     ) -> Self:
         """Update the face properties."""
         if not isinstance(self._face_namespace, ConstFace):
             self._face_namespace.events.disconnect()
             self._face_namespace = ConstFace(self)  # type: ignore
-            self._face_namespace.events.connect(self.events.face.emit)
+            self._face_namespace.events.connect(self.events.face.emit, max_args=None)
         self.face.update(color=color, hatch=hatch, alpha=alpha)
         return self
 
     def with_edge(
         self,
         color: ColorType | None = None,
         width: float = 1.0,
@@ -631,28 +660,28 @@
     ) -> Self:
         """Update the edge properties."""
         if color is None:
             color = get_theme().foreground_color
         if not isinstance(self._edge_namespace, ConstEdge):
             self._edge_namespace.events.disconnect()
             self._edge_namespace = ConstEdge(self)  # type: ignore
-            self._edge_namespace.events.connect(self.events.edge.emit)
+            self._edge_namespace.events.connect(self.events.edge.emit, max_args=None)
         self.edge.update(color=color, style=style, width=width, alpha=alpha)
         return self
 
     def with_face_multi(
         self,
         color: ColorType | Sequence[ColorType] | _Void = _void,
         hatch: str | Hatch | Sequence[str | Hatch] | _Void = _void,
         alpha: float = 1,
     ) -> Self:
         if not isinstance(self._face_namespace, MultiFace):
             self._face_namespace.events.disconnect()
             self._face_namespace = MultiFace(self)  # type: ignore
-            self._face_namespace.events.connect(self.events.face.emit)
+            self._face_namespace.events.connect(self.events.face.emit, max_args=None)
         self.face.update(color=color, hatch=hatch, alpha=alpha)
         return self
 
     def with_edge_multi(
         self,
         color: ColorType | Sequence[ColorType] | None = None,
         width: float | Sequence[float] = 1,
@@ -661,15 +690,15 @@
     ) -> Self:
         """Update the edge properties."""
         if color is None:
             color = get_theme().foreground_color
         if not isinstance(self._edge_namespace, MultiEdge):
             self._edge_namespace.events.disconnect()
             self._edge_namespace = MultiEdge(self)  # type: ignore
-            self._edge_namespace.events.connect(self.events.edge.emit)
+            self._edge_namespace.events.connect(self.events.edge.emit, max_args=None)
         self.edge.update(color=color, style=style, width=width, alpha=alpha)
         return self
 
     def _make_sure_hatch_visible(self):
         # TODO: following lines are needed, but it might be slow.
         # if isinstance(self.face, MonoFace):
         #     if self.face.hatch is Hatch.SOLID:
@@ -815,25 +844,22 @@
 
 # just for typing
 _E = TypeVar("_E", bound=Enum)
 
 
 class EnumArray(Generic[_E]):
     @overload
-    def __getitem__(self, key: SupportsIndex) -> _E:
-        ...
+    def __getitem__(self, key: SupportsIndex) -> _E: ...
 
     @overload
     def __getitem__(
         self, key: slice | NDArray[np.integer] | list[SupportsIndex]
-    ) -> EnumArray[_E]:
-        ...
+    ) -> EnumArray[_E]: ...
 
-    def __iter__(self) -> Iterator[_E]:
-        ...
+    def __iter__(self) -> Iterator[_E]: ...
 
 
 class FontEvents(SignalGroup):
     color = Signal(object)
     size = Signal(object)
     family = Signal(str)
 
@@ -978,17 +1004,17 @@
     _events_class = TextMixinEvents
 
     def __init__(self, name: str | None = None):
         self._face_namespace = ConstFace(self)
         self._edge_namespace = ConstEdge(self)
         self._font_namespace = ConstFont(self)
         super().__init__(name=name)
-        self._face_namespace.events.connect(self.events.face.emit)
-        self._edge_namespace.events.connect(self.events.edge.emit)
-        self._font_namespace.events.connect(self.events.font.emit)
+        self._face_namespace.events.connect(self.events.face.emit, max_args=None)
+        self._edge_namespace.events.connect(self.events.edge.emit, max_args=None)
+        self._font_namespace.events.connect(self.events.font.emit, max_args=None)
 
     @property
     def face(self) -> _NFace:
         """Namespace of the text background face."""
         return self._face_namespace
 
     @property
@@ -1008,15 +1034,15 @@
         hatch: Hatch | str = Hatch.SOLID,
         alpha: float = 1,
     ) -> Self:
         """Update the face properties."""
         if not isinstance(self._face_namespace, ConstFace):
             self._face_namespace.events.disconnect()
             self._face_namespace = ConstFace(self)  # type: ignore
-            self._face_namespace.events.connect(self.events.face.emit)
+            self._face_namespace.events.connect(self.events.face.emit, max_args=None)
         self.face.update(color=color, hatch=hatch, alpha=alpha)
         return self
 
     def with_edge(
         self,
         *,
         color: ColorType | None = None,
@@ -1026,29 +1052,29 @@
     ) -> Self:
         """Update the edge properties."""
         if color is None:
             color = get_theme().foreground_color
         if not isinstance(self._edge_namespace, ConstEdge):
             self._edge_namespace.events.disconnect()
             self._edge_namespace = ConstEdge(self)  # type: ignore
-            self._edge_namespace.events.connect(self.events.edge.emit)
+            self._edge_namespace.events.connect(self.events.edge.emit, max_args=None)
         self.edge.update(color=color, style=style, width=width, alpha=alpha)
         return self
 
     def with_face_multi(
         self,
         *,
         color: ColorType | Sequence[ColorType] | _Void = _void,
         hatch: str | Hatch | Sequence[str | Hatch] = Hatch.SOLID,
         alpha: float = 1,
     ) -> Self:
         if not isinstance(self._face_namespace, MultiFace):
             self._face_namespace.events.disconnect()
             self._face_namespace = MultiFace(self)  # type: ignore
-            self._face_namespace.events.connect(self.events.face.emit)
+            self._face_namespace.events.connect(self.events.face.emit, max_args=None)
         self.face.update(color=color, hatch=hatch, alpha=alpha)
         return self
 
     def with_edge_multi(
         self,
         *,
         color: ColorType | Sequence[ColorType] | None = None,
@@ -1058,15 +1084,15 @@
     ) -> Self:
         """Update the edge properties."""
         if color is None:
             color = get_theme().foreground_color
         if not isinstance(self._edge_namespace, MultiEdge):
             self._edge_namespace.events.disconnect()
             self._edge_namespace = MultiEdge(self)  # type: ignore
-            self._edge_namespace.events.connect(self.events.edge.emit)
+            self._edge_namespace.events.connect(self.events.edge.emit, max_args=None)
         self.edge.update(color=color, style=style, width=width, alpha=alpha)
         return self
 
     def with_font(
         self,
         *,
         color: ColorType | None = None,
@@ -1075,15 +1101,15 @@
     ) -> Self:
         """Update the face properties."""
         if color is None:
             color = self.font.color
         if not isinstance(self._font_namespace, ConstFace):
             self._font_namespace.events.disconnect()
             self._font_namespace = ConstFace(self)  # type: ignore
-            self._font_namespace.events.connect(self.events.font.emit)
+            self._font_namespace.events.connect(self.events.font.emit, max_args=None)
         self.font.update(color=color, size=size, family=family)
         return self
 
     def with_font_multi(
         self,
         *,
         color: ColorType | Sequence[ColorType] | None = None,
@@ -1098,10 +1124,10 @@
                 if self.ntexts == 0:
                     color = _void
                 else:
                     color = self.font.color
         if not isinstance(self._font_namespace, MultiFont):
             self._font_namespace.events.disconnect()
             self._font_namespace = MultiFont(self)  # type: ignore
-            self._font_namespace.events.connect(self.events.font.emit)
+            self._font_namespace.events.connect(self.events.font.emit, max_args=None)
         self.font.update(color=color, size=size, family=family)
         return self
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_ndim.py` & `whitecanvas-0.2.6/whitecanvas/layers/_ndim.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,17 @@
         self._base_layer._set_layer_data(data)
         self._base_layer.events.data.emit(data)
 
     def _get_slice(self, index) -> _T:
         return self._base_layer._norm_layer_data(self._data_stack.slice_at(index))
 
     def _connect_canvas(self, canvas: Canvas):
-        canvas.dims.events.indices.connect(self._update_layer_data, unique=True)
+        canvas.dims.events.indices.connect(
+            self._update_layer_data, unique=True, max_args=1
+        )
         return super()._connect_canvas(canvas)
 
     def _disconnect_canvas(self, canvas: Canvas):
         canvas.dims.events.indices.disconnect(self._update_layer_data)
         return super()._disconnect_canvas(canvas)
 
     def _with_axis_names(self, axis_names: list[str]):
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_sizehint.py` & `whitecanvas-0.2.6/whitecanvas/layers/_sizehint.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_text_utils.py` & `whitecanvas-0.2.6/whitecanvas/layers/_text_utils.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/__init__.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from whitecanvas.layers._primitive.band import Band
 from whitecanvas.layers._primitive.bars import Bars
 from whitecanvas.layers._primitive.errorbars import Errorbars
 from whitecanvas.layers._primitive.image import Image
 from whitecanvas.layers._primitive.inf_curve import InfCurve, InfLine
 from whitecanvas.layers._primitive.line import Line, MultiLine
 from whitecanvas.layers._primitive.markers import Markers
+from whitecanvas.layers._primitive.rects import Rects
 from whitecanvas.layers._primitive.rug import Rug
 from whitecanvas.layers._primitive.spans import Spans
 from whitecanvas.layers._primitive.text import Texts
 
 __all__ = [
     "Line",
     "MultiLine",
@@ -18,8 +19,9 @@
     "Spans",
     "Errorbars",
     "Rug",
     "InfLine",
     "InfCurve",
     "Texts",
     "Image",
+    "Rects",
 ]
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/band.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/bars.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/bars.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,44 +354,46 @@
     def with_face(
         self,
         *,
         color: ColorType | _Void = _void,
         hatch: Hatch | str = Hatch.SOLID,
         alpha: float = 1,
     ) -> Bars[ConstFace, _Edge]:
-        return super().with_face(color, hatch, alpha)
+        return super().with_face(color=color, hatch=hatch, alpha=alpha)
 
     def with_face_multi(
         self,
         *,
         color: ColorType | Sequence[ColorType] | _Void = _void,
         hatch: str | Hatch | Sequence[str | Hatch] | _Void = _void,
         alpha: float = 1,
     ) -> Bars[MultiFace, _Edge]:
-        return super().with_face_multi(color, hatch, alpha)
+        return super().with_face_multi(color=color, hatch=hatch, alpha=alpha)
 
     def with_edge(
         self,
         *,
         color: ColorType | None = None,
         width: float = 1,
         style: LineStyle | str = LineStyle.SOLID,
         alpha: float = 1,
     ) -> Bars[_Face, ConstEdge]:
-        return super().with_edge(color, width, style, alpha)
+        return super().with_edge(color=color, width=width, style=style, alpha=alpha)
 
     def with_edge_multi(
         self,
         *,
         color: ColorType | Sequence[ColorType] | None = None,
         width: float | Sequence[float] = 1,
         style: str | LineStyle | list[str | LineStyle] = LineStyle.SOLID,
         alpha: float = 1,
     ) -> Bars[_Face, MultiEdge]:
-        return super().with_edge_multi(color, width, style, alpha)
+        return super().with_edge_multi(
+            color=color, width=width, style=style, alpha=alpha
+        )
 
     def as_edge_only(
         self,
         *,
         width: float = 3.0,
         style: str | LineStyle = LineStyle.SOLID,
     ) -> Self:
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/errorbars.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/errorbars.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/image.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/image.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/inf_curve.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/inf_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import math
 from typing import TYPE_CHECKING, Any, Callable, Generic
 
 import numpy as np
 from typing_extensions import Concatenate, ParamSpec
 
 from whitecanvas.backend import Backend
-from whitecanvas.layers._base import _wrap_deprecation
 from whitecanvas.layers._primitive.line import LineMixin
 from whitecanvas.protocols import LineProtocol
 from whitecanvas.types import ColorType, LineStyle, Rect
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
@@ -55,18 +54,14 @@
 
         self._bounds = bounds
         self._model = model
         self._args = ()
         self._kwargs = {}
         self._linspace_num = 256
 
-        setattr(  # noqa: B010
-            self, "with_params", _wrap_deprecation(self.update_params, "with_params")
-        )
-
     def update_params(self, *args: _P.args, **kwargs: _P.kwargs) -> Self:
         """Set the parameters of the model function."""
         xdata, _ = self._backend._plt_get_data()
         ydata = self._model(xdata, *args, **kwargs)
         self._backend._plt_set_data(xdata, ydata)
         self._args, self._kwargs = args, kwargs
         if not self._params_ready:
@@ -87,15 +82,15 @@
     def with_hover_text(self, text: str) -> Self:
         if not isinstance(text, str):
             raise TypeError(f"Hover text must be str, got {type(text)}.")
         self._backend._plt_set_hover_text([text] * self._linspace_num)
         return self
 
     def _connect_canvas(self, canvas: Canvas):
-        canvas.x.events.lim.connect(self._recalculate_line)
+        canvas.x.events.lim.connect(self._recalculate_line, max_args=1)
         self._recalculate_line(canvas.x.lim)
         super()._connect_canvas(canvas)
 
     def _disconnect_canvas(self, canvas: Canvas):
         canvas.x.events.lim.disconnect(self._recalculate_line)
         super()._disconnect_canvas(canvas)
 
@@ -219,15 +214,15 @@
     def with_hover_text(self, text: str) -> Self:
         if not isinstance(text, str):
             raise TypeError(f"Hover text must be str, got {type(text)}.")
         self._backend._plt_set_hover_text([text] * 2)
         return self
 
     def _connect_canvas(self, canvas: Canvas):
-        canvas.events.lims.connect(self._recalculate_line)
+        canvas.events.lims.connect(self._recalculate_line, max_args=1)
         self._recalculate_line(canvas.lims)
         self._last_rect = canvas.lims
         super()._connect_canvas(canvas)
 
     def _disconnect_canvas(self, canvas: Canvas):
         canvas.events.lims.disconnect(self._recalculate_line)
         super()._disconnect_canvas(canvas)
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/line.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/line.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/markers.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,15 @@
 )
 from whitecanvas.utils.normalize import as_array_1d, normalize_xy, parse_texts
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from whitecanvas.layers import group as _lg
-    from whitecanvas.layers._mixin import (
-        ConstEdge,
-        ConstFace,
-        MultiEdge,
-        MultiFace,
-    )
+    from whitecanvas.layers._mixin import ConstEdge, ConstFace, MultiEdge, MultiFace
 
 _void = _Void()
 _Face = TypeVar("_Face", bound=FaceNamespace)
 _Edge = TypeVar("_Edge", bound=EdgeNamespace)
 _Size = TypeVar("_Size", float, NDArray[np.floating])
 
 
@@ -63,16 +58,15 @@
     Generic[_Face, _Edge, _Size],
 ):
     events: MarkersLayerEvents
     _events_class = MarkersLayerEvents
 
     if TYPE_CHECKING:
 
-        def __new__(cls, *args, **kwargs) -> Markers[ConstFace, ConstEdge, float]:
-            ...
+        def __new__(cls, *args, **kwargs) -> Markers[ConstFace, ConstEdge, float]: ...
 
     def __init__(
         self,
         xdata: ArrayLike1D,
         ydata: ArrayLike1D,
         *,
         name: str | None = None,
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/rug.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/rug.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/spans.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/spans.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,20 +125,20 @@
 
     @property
     def ndata(self) -> int:
         """The number of data points"""
         return self._backend._plt_get_data()[0].size
 
     def _connect_canvas(self, canvas: Canvas):
-        canvas.events.lims.connect(self._recalculate_spans)
+        canvas.events.lims.connect(self._recalculate_spans, max_args=1)
         self._force_update_spans()
         return super()._connect_canvas(canvas)
 
     def _disconnect_canvas(self, canvas: Canvas):
-        canvas.events.lims.connect(self._recalculate_spans)
+        canvas.events.lims.connect(self._recalculate_spans, max_args=1)
         return super()._disconnect_canvas(canvas)
 
     def _recalculate_spans(self, rect: Rect):
         # update the rectangles so that their limits are not visible
         if self.orient.is_vertical:
             _min, _max = rect.bottom, rect.top
         else:
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/_primitive/text.py` & `whitecanvas-0.2.6/whitecanvas/layers/_primitive/text.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/__init__.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/__init__.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/_collections.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/_collections.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/_offsets.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/_offsets.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/band_collection.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/band_collection.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/boxplot.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/boxplot.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/colorbar.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/colorbar.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/graph.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/graph.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/labeled.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/labeled.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,15 @@
         if texts is None:
             texts = Texts(
                 [], [], [], name="texts", backend=layer._backend_name
             ).with_font_multi()
         if colorbar is None:
             colorbar = Colorbar(layer.cmap)
             colorbar.visible = False
-        layer.events.cmap.connect_setattr(colorbar, "cmap")
+        layer.events.cmap.connect_setattr(colorbar, "cmap", maxargs=1)
         super().__init__([layer, texts, colorbar], name=name)
 
     @property
     def image(self) -> Image:
         """The image layer."""
         return self._children[0]
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/line_band.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/line_band.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/line_collection.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/line_collection.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/line_fill.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/line_fill.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/line_markers.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/line_markers.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/marker_collection.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/marker_collection.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/stemplot.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/stemplot.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/group/textinfo.py` & `whitecanvas-0.2.6/whitecanvas/layers/group/textinfo.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/__init__.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/_box_like.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/_box_like.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,15 @@
         return self
 
     def update_const(
         self,
         *,
         color: ColorType | _Void = _void,
         hatch: str | Hatch | _Void = _void,
+        alpha: float | _Void = _void,
     ) -> Self:
         """
         Update the plot features to the constant values.
 
         Parameters
         ----------
         color : color-type, optional
@@ -182,14 +183,29 @@
             color_by = _p.ColorPlan.from_const(Color(color))
             self._get_base().face.color = color_by.generate(cat, self._splitby)
             self._color_by = color_by
         if hatch is not _void:
             hatch_by = _p.HatchPlan.from_const(Hatch(hatch))
             self._get_base().face.hatch = hatch_by.generate(cat, self._splitby)
             self._hatch_by = hatch_by
+        if alpha is not _void:
+            self._get_base().face.alpha = alpha
+            self._get_base().edge.alpha = alpha
+        return self
+
+    def with_face(
+        self,
+        *,
+        color: ColorType | None = None,
+        hatch: str | Hatch | None = None,
+        alpha: float = 1.0,
+    ) -> Self:
+        """Add face to the plot with given settings."""
+        if color is not None:
+            self._get_base().with_face(color=color, hatch=hatch, alpha=alpha)
         return self
 
     def with_edge(
         self,
         *,
         color: ColorType | None = None,
         width: float = 1.0,
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/_dataframe.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,24 +94,22 @@
             segs.append(np.column_stack([xj.map(sub), yj.map(sub)]))
         return DFLines(
             df, segs, labels, name=name, color=color, width=width, style=style,
             backend=backend,
         )  # fmt: skip
 
     @overload
-    def update_color(self, value: ColorType) -> Self:
-        ...
+    def update_color(self, value: ColorType) -> Self: ...
 
     @overload
     def update_color(
         self,
         by: str | Iterable[str],
         palette: ColormapType | None = None,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     def update_color(self, by, /, palette=None):
         """Update the color rule of the layer."""
         cov = _shared.ColumnOrValue(by, self._source)
         if cov.is_column:
             if set(cov.columns) > set(self._splitby):
                 raise ValueError(f"Cannot color by a column other than {self._splitby}")
@@ -136,14 +134,20 @@
             style_by = _p.StylePlan.new(cov.columns, values=styles)
         else:
             style_by = _p.StylePlan.from_const(LineStyle(cov.value))
         self._base_layer.style = style_by.generate(self._categories, self._splitby)
         self._style_by = style_by
         return self
 
+    def update_alpha(self, value: float) -> Self:
+        """Update alpha of the lines."""
+        for line in self._base_layer:
+            line.alpha = value
+        return self
+
     def move(self, dx: float = 0.0, dy: float = 0.0, autoscale: bool = True) -> Self:
         """Add a constant shift to the layer."""
         for layer in self._base_layer:
             old_data = layer.data
             new_data = old_data[0] + dx, old_data[1] + dy
             layer.data = new_data
         if autoscale and (canvas := self._canvas_ref()):
@@ -509,24 +513,22 @@
         super().__init__(base, source)
         self._color_by = _p.ColorPlan.default()
         self._width_by = _p.WidthPlan.default()
         self._style_by = _p.StylePlan.default()
         self._hatch_by = _p.HatchPlan.default()
 
     @overload
-    def update_color(self, value: ColorType) -> Self:
-        ...
+    def update_color(self, value: ColorType) -> Self: ...
 
     @overload
     def update_color(
         self,
         by: str | Iterable[str],
         palette: ColormapType | None = None,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     def update_color(self, by, /, palette=None):
         cov = _shared.ColumnOrValue(by, self._source)
         if cov.is_column:
             if set(cov.columns) > set(self._splitby):
                 raise ValueError(f"Cannot color by a column other than {self._splitby}")
             color_by = _p.ColorPlan.from_palette(cov.columns, palette=palette)
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/_df_compat.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/_df_compat.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/_jitter.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/_jitter.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/_marker_like.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/_marker_like.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,25 +33,26 @@
     _Void,
 )
 from whitecanvas.utils.type_check import is_real_number
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
+    from whitecanvas.canvas import CanvasBase
+
 _DF = TypeVar("_DF")
 _Cols = Union[str, "tuple[str, ...]"]
 _void = _Void()
 
 
 class _MarkerLikeMixin:
     _source: DataFrameWrapper[_DF]
 
     @overload
-    def update_color(self, value: ColorType) -> Self:
-        ...
+    def update_color(self, value: ColorType) -> Self: ...
 
     @overload
     def update_color(
         self, by: str | Iterable[str], palette: ColormapType | None = None,
     ) -> Self:  # fmt: skip
         ...
 
@@ -70,14 +71,36 @@
             if palette is not None:
                 raise TypeError("`palette` can only be used with a column name.")
             color_by = _p.ColorPlan.from_const(Color(cov.value))
         self._apply_color(color_by.map(self._source))
         self._color_by = color_by
         return self
 
+    @overload
+    def update_alpha(self, value: float) -> Self: ...
+
+    @overload
+    def update_alpha(
+        self,
+        by: str | Iterable[str],
+        map_from: tuple[float, float] | None = None,
+        map_to: tuple[float, float] = (0.2, 1.0),
+    ) -> Self: ...
+
+    def update_alpha(self, by, /, map_from=None, map_to=(0.2, 1.0)) -> Self:
+        if isinstance(by, str):
+            alpha_by = _p.AlphaPlan.from_range(by, range=map_to, domain=map_from)
+        else:
+            if map_from is not None:
+                raise TypeError("`map_from` can only be used with a column name.")
+            alpha_by = _p.AlphaPlan.from_const(float(by))
+        self._apply_alpha(alpha_by.map(self._source))
+        self._alpha_by = alpha_by
+        return self
+
     def update_colormap(
         self,
         by: str,
         cmap: ColormapType = "viridis",
         clim: tuple[float, float] | None = None,
     ) -> Self:
         """
@@ -90,16 +113,15 @@
             raise ValueError("Can only colormap by a single column.")
         color_by = _p.ColormapPlan.from_colormap(by, cmap=Colormap(cmap), clim=clim)
         self._apply_color(color_by.map(self._source))
         self._color_by = color_by
         return self
 
     @overload
-    def update_width(self, value: float) -> Self:
-        ...
+    def update_width(self, value: float) -> Self: ...
 
     @overload
     def update_width(
         self, by: str, map_from: tuple[float, float] | None = None,
         map_to: tuple[float, float] = (1.0, 4.0),
     ) -> Self:  # fmt: skip
         ...
@@ -127,45 +149,56 @@
                 raise TypeError("`map_from` can only be used with a column name.")
             width_by = _p.WidthPlan.from_const(float(by))
         self._apply_width(width_by.map(self._source))
         self._width_by = width_by
         return self
 
     @overload
-    def update_style(self, value: ColorType) -> Self:
-        ...
+    def update_style(self, value: ColorType) -> Self: ...
 
     @overload
     def update_style(
         self,
         by: str | Iterable[str],
         palette: ColormapType | None = None,
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     def update_style(self, by, /, palette=None) -> Self:
         cov = _shared.ColumnOrValue(by, self._source)
         if cov.is_column:
             style_by = _p.StylePlan.new(cov.columns, palette)
         else:
             if palette is not None:
                 raise TypeError("`palette` can only be used with a column name.")
             style_by = _p.StylePlan.from_const(LineStyle(cov.value))
         self._apply_style(style_by.map(self._source))
         self._style_by = style_by
         return self
 
+    def _init_color_for_canvas(self, color, alpha, canvas: CanvasBase):
+        if color is not None and not self._color_by.is_const():
+            self.update_color(self._color_by.by, palette=canvas._color_palette)
+        elif color is None:
+            self.update_color(canvas._color_palette.next())
+        if alpha is not None:
+            self.update_alpha(alpha)
+        return self
+
     def _apply_color(self, color):
         """Set color array to the layer."""
         raise NotImplementedError
 
     def _apply_width(self, width):
         """Set width array to the layer."""
         raise NotImplementedError
 
+    def _apply_alpha(self, alpha):
+        """Set alpha array to the layer."""
+        raise NotImplementedError
+
     def _apply_style(self, style):
         """Set style array to the layer."""
         raise NotImplementedError
 
 
 class DFMarkers(
     _shared.DataFrameLayerWrapper[_lg.MarkerCollection, _DF], _MarkerLikeMixin
@@ -213,14 +246,18 @@
 
     def _apply_color(self, color):
         self.base.face.color = color
 
     def _apply_width(self, width):
         self.base.with_edge(color=_void, width=width, style=_void)
 
+    def _apply_alpha(self, alpha):
+        self.base.face.alpha = alpha
+        self.base.edge.alpha = alpha
+
     def _apply_style(self, style):
         self.base.with_edge(color=_void, width=_void, style=style)
 
     def update_edge_color(self, by: str | Iterable[str], palette=None) -> Self:
         cov = _shared.ColumnOrValue(by, self._source)
         if cov.is_column:
             color_by = _p.ColorPlan.from_palette(cov.columns, palette=palette)
@@ -257,16 +294,15 @@
             hatch_by = _p.HatchPlan.from_const(Hatch(cov.value))
         hatches = hatch_by.map(self._source)
         self.base.face.hatch = hatches
         self._hatch_by = hatch_by
         return self
 
     @overload
-    def update_size(self, value: float) -> Self:
-        ...
+    def update_size(self, value: float) -> Self: ...
 
     @overload
     def update_size(
         self, by: str, /, map_from: tuple[float, float] | None = None,
         map_to: tuple[float, float] = (3, 15),
     ) -> Self:  # fmt: skip
         ...
@@ -292,22 +328,20 @@
         else:
             size_by = _p.SizePlan.from_const(float(by))
         self.base.size = size_by.map(self._source)
         self._size_by = size_by
         return self
 
     @overload
-    def update_symbol(self, value: str | Symbol) -> Self:
-        ...
+    def update_symbol(self, value: str | Symbol) -> Self: ...
 
     @overload
     def update_symbol(
         self, by: str | Iterable[str] | None = None, symbols=None
-    ) -> Self:
-        ...
+    ) -> Self: ...
 
     def update_symbol(self, by, /, symbols=None) -> Self:
         cov = _shared.ColumnOrValue(by, self._source)
         if cov.is_column:
             symbol_by = _p.SymbolPlan.new(cov.columns, values=symbols)
         else:
             symbol_by = _p.SymbolPlan.from_const(Symbol(by))
@@ -494,15 +528,15 @@
         self._style_by = _p.StylePlan.default()
         self._splitby = splitby
         self._stackby = stackby
 
         base = _l.Bars(
             x, y, bottom=bottom, name=name, orient=orient, extent=extent,
             backend=backend
-        ).with_face_multi()  # fmt: skip
+        ).with_face_multi().with_edge_multi()  # fmt: skip
         super().__init__(base, source)
         if color is not None:
             self.update_color(color)
         if hatch is not None:
             self.update_hatch(hatch)
         self.with_hover_template(default_template(source.iter_items()))
 
@@ -563,18 +597,22 @@
             extent=extent, orient=orient, backend=backend,
         )  # fmt: skip
 
     def _apply_color(self, color):
         self.base.face.color = color
 
     def _apply_width(self, width):
-        self._base_layer.with_edge(color=_void, width=width, style=_void)
+        self._base_layer.with_edge_multi(color=_void, width=width, style=_void)
+
+    def _apply_alpha(self, alpha):
+        self.base.face.alpha = alpha
+        self.base.edge.alpha = alpha
 
     def _apply_style(self, style):
-        self._base_layer.with_edge(color=_void, width=_void, style=style)
+        self._base_layer.with_edge_multi(color=_void, width=_void, style=style)
 
     def update_hatch(self, by: str | Iterable[str], choices=None) -> Self:
         cov = _shared.ColumnOrValue(by, self._source)
         if cov.is_column:
             if set(cov.columns) > set(self._splitby):
                 raise ValueError(f"Cannot hatch by a column other than {self._splitby}")
             hatch_by = _p.HatchPlan.new(cov.columns, values=choices)
@@ -687,14 +725,17 @@
     def orient(self) -> Orientation:
         """Orientation of the rugs"""
         return self.base.orient
 
     def _apply_color(self, color):
         self.base.color = color
 
+    def _apply_alpha(self, alpha):
+        self.base.alpha = alpha
+
     def _apply_width(self, width):
         self.base.width = width
 
     def _apply_style(self, style):
         self.base.style = style
 
     # def update_scale(self, by: str | float, align: str = "low") -> Self:
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/_plans.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/_plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,14 +399,20 @@
 
 class SizePlan(ScalarMapPlan):
     @classmethod
     def _default_mapper(cls):
         return lambda _: 12.0
 
 
+class AlphaPlan(ScalarMapPlan):
+    @classmethod
+    def _default_mapper(cls):
+        return lambda _: 1.0
+
+
 class ConstMap:
     def __init__(self, value):
         self._value = value
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}<{self._value!r}>"
```

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/_shared.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/_shared.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/layers/tabular/_stackable.py` & `whitecanvas-0.2.6/whitecanvas/layers/tabular/_stackable.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/plot/__init__.py` & `whitecanvas-0.2.6/whitecanvas/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/plot/_canvases.py` & `whitecanvas-0.2.6/whitecanvas/plot/_canvases.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/plot/_methods.py` & `whitecanvas-0.2.6/whitecanvas/plot/_methods.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/protocols/__init__.py` & `whitecanvas-0.2.6/whitecanvas/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/protocols/canvas_protocol.py` & `whitecanvas-0.2.6/whitecanvas/protocols/canvas_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,20 @@
     def _plt_make_legend(
         self,
         items: list[tuple[str, LegendItem]],
         anchor: Location,
     ):
         """Make legend for the given legend items"""
 
+    def _plt_get_mouse_enabled(self) -> bool:
+        """Get mouse interaction enabled state"""
+
+    def _plt_set_mouse_enabled(self, enabled: bool):
+        """Set mouse interaction enabled state"""
+
 
 @runtime_checkable
 class TextLabelProtocol(HasVisibility, Protocol):
     def _plt_get_text(self) -> Any:
         """Get text of label"""
 
     def _plt_set_text(self, text):
```

### Comparing `whitecanvas-0.2.5/whitecanvas/protocols/layer_protocols.py` & `whitecanvas-0.2.6/whitecanvas/protocols/layer_protocols.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/theme/_api.py` & `whitecanvas-0.2.6/whitecanvas/theme/_api.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/theme/_dataclasses.py` & `whitecanvas-0.2.6/whitecanvas/theme/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/types/__init__.py` & `whitecanvas-0.2.6/whitecanvas/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     MouseButton,
     MouseEventType,
     Orientation,
     OrientationLike,
     Origin,
     Symbol,
 )
-from whitecanvas.types._mouse import MouseEvent
+from whitecanvas.types._mouse import MouseEvent, Point
 from whitecanvas.types._tuples import Rect, XYData, XYTextData, XYYData
 
 __all__ = [
     "ColorType",
     "ColormapType",
     "ArrayLike1D",
     "LineStyle",
@@ -40,14 +40,15 @@
     "KdeBandWidthType",
     "Orientation",
     "OrientationLike",
     "Origin",
     "Modifier",
     "MouseButton",
     "MouseEvent",
+    "Point",
     "MouseEventType",
     "Alignment",
     "XYData",
     "XYYData",
     "XYTextData",
     "Rect",
     "_Void",
```

### Comparing `whitecanvas-0.2.5/whitecanvas/types/_alias.py` & `whitecanvas-0.2.6/whitecanvas/types/_alias.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/types/_enums.py` & `whitecanvas-0.2.6/whitecanvas/types/_enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,32 +60,38 @@
             Symbol.PLUS,
             Symbol.VBAR,
             Symbol.HBAR,
         )
 
 
 class Modifier(_StrEnum):
+    """Enum that represents the keyboard modifiers."""
+
     SHIFT = "shift"
     CTRL = "ctrl"
     ALT = "alt"
     META = "meta"
 
 
 class MouseButton(_StrEnum):
+    """Enum that represents the mouse buttons."""
+
     NONE = "none"
     LEFT = "left"
     MIDDLE = "middle"
     RIGHT = "right"
     BACK = "back"
     FORWARD = "forward"
 
 
 class MouseEventType(_StrEnum):
+    """Enum that represents the mouse event type."""
+
     MOVE = "move"
-    CLICK = "click"
+    PRESS = "press"
     RELEASE = "release"
     DOUBLE_CLICK = "double_click"
 
 
 class Alignment(_StrEnum):
     TOP = "top"
     BOTTOM = "bottom"
```

### Comparing `whitecanvas-0.2.5/whitecanvas/types/_mouse.py` & `whitecanvas-0.2.6/whitecanvas/types/_mouse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from typing import NamedTuple
 
 from whitecanvas.types._enums import Modifier, MouseButton, MouseEventType
 
 
+class Point(NamedTuple):
+    x: float
+    y: float
+
+
 @dataclass
 class MouseEvent:
     button: MouseButton
     modifiers: tuple[Modifier, ...]
-    pos: tuple[float, float]
+    pos: Point
     type: MouseEventType
 
+    def __post_init__(self):
+        self.pos = Point(*self.pos)  # normalize
+
     def update(self, other: MouseEvent):
         self.button = other.button
         self.modifiers = other.modifiers
         self.pos = other.pos
         self.type = other.type
 
     def _repr_simple(self):
```

### Comparing `whitecanvas-0.2.5/whitecanvas/types/_tuples.py` & `whitecanvas-0.2.6/whitecanvas/types/_tuples.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,29 +44,41 @@
 class XYTextData(NamedTuple):
     x: NDArray[np.floating]
     y: NDArray[np.floating]
     text: NDArray[np.object_]
 
 
 class Rect(NamedTuple):
-    """Rectangular range."""
+    """Rectangular range in left, right, bottom, top order."""
 
     left: float
     right: float
     bottom: float
     top: float
 
+    def __repr__(self) -> str:
+        return (
+            f"Rect(left={self.left:.6g}, right={self.right:.6g}, "
+            f"bottom={self.bottom:.6g}, top={self.top:.6g})"
+        )
+
     @classmethod
     def with_check(cls, left: float, right: float, bottom: float, top: float):
         if left > right:
             raise ValueError("left must be less than or equal to right")
         if bottom > top:
             raise ValueError("bottom must be less than or equal to top")
         return cls(float(left), float(right), float(bottom), float(top))
 
+    @classmethod
+    def with_sort(cls, left: float, right: float, bottom: float, top: float):
+        left, right = sorted([left, right])
+        bottom, top = sorted([bottom, top])
+        return cls(float(left), float(right), float(bottom), float(top))
+
     @property
     def width(self) -> float:
         """Width of the range."""
         return self.right - self.left
 
     @property
     def height(self) -> float:
```

### Comparing `whitecanvas-0.2.5/whitecanvas/utils/collections.py` & `whitecanvas-0.2.6/whitecanvas/utils/collections.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/utils/hist.py` & `whitecanvas-0.2.6/whitecanvas/utils/hist.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/utils/kde.py` & `whitecanvas-0.2.6/whitecanvas/utils/kde.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/whitecanvas/utils/normalize.py` & `whitecanvas-0.2.6/whitecanvas/utils/normalize.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,33 @@
 
 from typing import Any, Mapping
 
 import numpy as np
 from cmap import Color
 from numpy.typing import ArrayLike, NDArray
 
+from whitecanvas.types import XYData
 from whitecanvas.utils import type_check as _tc
 
 
 def as_array_1d(x: ArrayLike, dtype=None) -> NDArray[np.number]:
+    """Normalize the input as a 1D array."""
     x = np.asarray(x, dtype=dtype)
     if x.ndim != 1:
         raise ValueError(f"Expected 1D array, got {x.ndim}D array")
     if x.dtype.kind not in "iuf":
         raise ValueError(f"Input {x!r} did not return a numeric array")
     return x
 
 
 def normalize_xy(*args) -> tuple[NDArray[np.number], NDArray[np.number]]:
+    """Normalize the input as two 1D array with the same shape."""
     if len(args) == 1:
+        if isinstance(args[0], XYData):
+            return args[0].x, args[0].y
         arr = np.asarray(args[0])
         if arr.dtype.kind not in "iuf":
             raise ValueError(f"Input {args[0]!r} did not return a numeric array")
         if arr.ndim == 1:
             ydata = arr
             xdata = np.arange(ydata.size)
         elif arr.ndim == 2 and arr.shape[1] == 2:
```

### Comparing `whitecanvas-0.2.5/whitecanvas/utils/type_check.py` & `whitecanvas-0.2.6/whitecanvas/utils/type_check.py`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/.gitignore` & `whitecanvas-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/LICENSE` & `whitecanvas-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/README.md` & `whitecanvas-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `whitecanvas-0.2.5/pyproject.toml` & `whitecanvas-0.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "typing_extensions>=4.5.0",
   "numpy>=1.23.2",
-  "psygnal>=0.9.4,<0.10.0",
+  "psygnal>=0.9.4,!=0.10.0",
   "cmap>=0.1.2",
 ]
 
 
 [project.optional-dependencies]
 matplotlib = [
   "matplotlib>=3.4.3,!=3.8.0",
@@ -43,15 +43,15 @@
 
 plotly = [
   "plotly>=5.3.1",
   "kaleido>=0.2.1",
 ]
 
 vispy = [
-  "vispy>=0.14.1",
+  "vispy>=0.14.2",
 ]
 
 bokeh = [
   "bokeh>=3.3.1",
 ]
 
 testing = [
@@ -61,15 +61,15 @@
   "imageio",
   "qtpy>=2.4.1",
   "pyqt5>=5.15.4",
   "ipywidgets>=8.0.0",
   "matplotlib>=3.8.2",
   "pyqtgraph>=0.13.3",
   "plotly>=5.3.1",
-  "vispy>=0.14.1",
+  "vispy>=0.14.2",
   "bokeh>=3.3.1",
   "pandas>=1.3.3",
   "polars>=0.20.10",
 ]
 
 docs = [
   "mkdocs",
@@ -145,15 +145,15 @@
 target-version = ["py37"]
 line-length = 88
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py37"
 line-length = 88
-select = [
+lint.select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
   "F",
@@ -169,42 +169,44 @@
   "S",
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
-ignore = [
+lint.ignore = [
   "A002", "A003", "ARG001", "ARG002",
   # Allow non-abstract empty methods in abstract base classes
   "B027", "B904", "B006",
   "E741",
   "N802",  # Qt function names are not snake_case
   # Ignore checks for possible passwords
   "S101", "S105", "S106", "S107",
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915", "PLW0603",
+  "ISC001",
 ]
-unfixable = [
+lint.unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 exclude = ["tests", "docs", "examples"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["whitecanvas"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 "whitecanvas/theme/_dataclasses.py" = ["RUF"]
 "whitecanvas/backend/**/*" = ["F401"]
+"whitecanvas/backend/pyqtgraph/**/*" = ["N803"]
 
 [tool.coverage.run]
 source_pkgs = ["whitecanvas", "tests"]
 branch = true
 parallel = true
 omit = [
   "whitecanvas/__about__.py",
@@ -218,8 +220,9 @@
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "@overload",
   "@abstractmethod",
   "@deprecated",
+  "raise NotImplementedError",
 ]
```

### Comparing `whitecanvas-0.2.5/PKG-INFO` & `whitecanvas-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: whitecanvas
-Version: 0.2.5
+Version: 0.2.6
 Summary: A type safe and backend independent plotting library for Python.
 Project-URL: Documentation, https://github.com/hanjinliu/whitecanvas#readme
 Project-URL: Issues, https://github.com/hanjinliu/whitecanvas/issues
 Project-URL: Source, https://github.com/hanjinliu/whitecanvas
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
@@ -43,15 +43,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: cmap>=0.1.2
 Requires-Dist: numpy>=1.23.2
-Requires-Dist: psygnal<0.10.0,>=0.9.4
+Requires-Dist: psygnal!=0.10.0,>=0.9.4
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: bokeh
 Requires-Dist: bokeh>=3.3.1; extra == 'bokeh'
 Provides-Extra: docs
 Requires-Dist: imageio>=2.9.0; extra == 'docs'
 Requires-Dist: matplotlib>=3.8.2; extra == 'docs'
 Requires-Dist: mkdocs; extra == 'docs'
@@ -80,17 +80,17 @@
 Requires-Dist: polars>=0.20.10; extra == 'testing'
 Requires-Dist: pyqt5>=5.15.4; extra == 'testing'
 Requires-Dist: pyqtgraph>=0.13.3; extra == 'testing'
 Requires-Dist: pytest; extra == 'testing'
 Requires-Dist: pytest-cov; extra == 'testing'
 Requires-Dist: pytest-qt; extra == 'testing'
 Requires-Dist: qtpy>=2.4.1; extra == 'testing'
-Requires-Dist: vispy>=0.14.1; extra == 'testing'
+Requires-Dist: vispy>=0.14.2; extra == 'testing'
 Provides-Extra: vispy
-Requires-Dist: vispy>=0.14.1; extra == 'vispy'
+Requires-Dist: vispy>=0.14.2; extra == 'vispy'
 Description-Content-Type: text/markdown
 
 # whitecanvas
 
 [![PyPI - Version](https://img.shields.io/pypi/v/whitecanvas.svg)](https://pypi.org/project/whitecanvas)
 [![Python package index download statistics](https://img.shields.io/pypi/dm/whitecanvas.svg)](https://pypistats.org/packages/whitecanvas)
 [![codecov](https://codecov.io/gh/hanjinliu/whitecanvas/graph/badge.svg?token=MYLNFOpEnA)](https://codecov.io/gh/hanjinliu/whitecanvas)
```

