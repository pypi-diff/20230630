# Comparing `tmp/coldtype-0.9.8.tar.gz` & `tmp/coldtype-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coldtype-0.9.8.tar", last modified: Thu Aug 25 16:59:12 2022, max compression
+gzip compressed data, was "coldtype-0.9.9.tar", last modified: Mon Aug 29 21:30:54 2022, max compression
```

## Comparing `coldtype-0.9.8.tar` & `coldtype-0.9.9.tar`

### file list

```diff
@@ -1,185 +1,188 @@
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.432635 coldtype-0.9.8/
--rw-r--r--   0 robstenson   (501) staff       (20)    11397 2021-10-30 00:05:47.000000 coldtype-0.9.8/LICENSE
--rw-r--r--   0 robstenson   (501) staff       (20)      730 2022-08-25 16:59:12.432473 coldtype-0.9.8/PKG-INFO
--rw-r--r--   0 robstenson   (501) staff       (20)     2849 2021-10-30 00:05:47.000000 coldtype-0.9.8/README.md
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.392157 coldtype-0.9.8/coldtype/
--rw-r--r--   0 robstenson   (501) staff       (20)     2189 2022-08-25 16:57:43.000000 coldtype-0.9.8/coldtype/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4221 2022-01-24 18:05:54.000000 coldtype-0.9.8/coldtype/axidraw.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4734 2022-02-01 18:13:46.000000 coldtype-0.9.8/coldtype/beziers.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.395627 coldtype-0.9.8/coldtype/blender/
--rw-r--r--   0 robstenson   (501) staff       (20)    11548 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/blender/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)    31750 2022-07-22 17:26:15.000000 coldtype-0.9.8/coldtype/blender/fluent.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1971 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/blender/livepreview.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3388 2022-02-21 18:10:34.000000 coldtype-0.9.8/coldtype/blender/panel3d.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2660 2021-12-10 17:19:05.000000 coldtype-0.9.8/coldtype/blender/render.py
--rw-r--r--   0 robstenson   (501) staff       (20)    13372 2021-12-07 18:09:55.000000 coldtype-0.9.8/coldtype/blender/timedtext.py
--rw-r--r--   0 robstenson   (501) staff       (20)      776 2022-02-21 17:22:38.000000 coldtype-0.9.8/coldtype/blender/util.py
--rw-r--r--   0 robstenson   (501) staff       (20)    12958 2022-08-08 16:01:40.000000 coldtype-0.9.8/coldtype/blender/watch.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.395939 coldtype-0.9.8/coldtype/capture/
--rw-r--r--   0 robstenson   (501) staff       (20)      503 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/capture/__init__.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.396352 coldtype-0.9.8/coldtype/color/
--rw-r--r--   0 robstenson   (501) staff       (20)     9736 2022-01-25 21:24:30.000000 coldtype-0.9.8/coldtype/color/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     5751 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/color/html.py
--rw-r--r--   0 robstenson   (501) staff       (20)      351 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/css.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4470 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/drawbot.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.387092 coldtype-0.9.8/coldtype/fontgoggles/
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.397701 coldtype-0.9.8/coldtype/fontgoggles/compile/
--rw-r--r--   0 robstenson   (501) staff       (20)        0 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/compile/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1324 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/compile/compilerPool.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2417 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/compile/dsCompiler.py
--rw-r--r--   0 robstenson   (501) staff       (20)      167 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/compile/ttxCompiler.py
--rw-r--r--   0 robstenson   (501) staff       (20)     8173 2022-08-06 00:33:56.000000 coldtype-0.9.8/coldtype/fontgoggles/compile/ufoCompiler.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1120 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/compile/workServer.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.398744 coldtype-0.9.8/coldtype/fontgoggles/font/
--rw-r--r--   0 robstenson   (501) staff       (20)     6278 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/font/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     7339 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/font/baseFont.py
--rw-r--r--   0 robstenson   (501) staff       (20)    21628 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/font/dsFont.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1075 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/font/glyphDrawing.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3336 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/font/otfFont.py
--rw-r--r--   0 robstenson   (501) staff       (20)    18528 2022-07-29 17:56:20.000000 coldtype-0.9.8/coldtype/fontgoggles/font/ufoFont.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.400696 coldtype-0.9.8/coldtype/fontgoggles/misc/
--rw-r--r--   0 robstenson   (501) staff       (20)        0 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/misc/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2781 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/misc/ftFont.py
--rw-r--r--   0 robstenson   (501) staff       (20)     8270 2022-03-25 18:52:02.000000 coldtype-0.9.8/coldtype/fontgoggles/misc/hbShape.py
--rw-r--r--   0 robstenson   (501) staff       (20)    53377 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/misc/opentypeTags.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4334 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/misc/properties.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2924 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/misc/rectTree.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3855 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/misc/segmenting.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2748 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fontgoggles/misc/textInfo.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.401627 coldtype-0.9.8/coldtype/fx/
--rw-r--r--   0 robstenson   (501) staff       (20)      205 2021-11-11 19:52:09.000000 coldtype-0.9.8/coldtype/fx/chainable.py
--rw-r--r--   0 robstenson   (501) staff       (20)      448 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fx/motion.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2743 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/fx/shapes.py
--rw-r--r--   0 robstenson   (501) staff       (20)    10207 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/fx/skia.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2768 2021-11-01 15:54:34.000000 coldtype-0.9.8/coldtype/fx/warping.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2555 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/fx/xray.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.403698 coldtype-0.9.8/coldtype/geometry/
--rw-r--r--   0 robstenson   (501) staff       (20)      654 2021-11-12 22:46:47.000000 coldtype-0.9.8/coldtype/geometry/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)      812 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/geometry/atom.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1925 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/geometry/curve.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1623 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/geometry/edge.py
--rw-r--r--   0 robstenson   (501) staff       (20)       29 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/geometry/geometrical.py
--rw-r--r--   0 robstenson   (501) staff       (20)     5483 2022-02-03 17:40:28.000000 coldtype-0.9.8/coldtype/geometry/line.py
--rw-r--r--   0 robstenson   (501) staff       (20)     5016 2021-11-05 16:46:39.000000 coldtype-0.9.8/coldtype/geometry/point.py
--rw-r--r--   0 robstenson   (501) staff       (20)     5577 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/geometry/primitives.py
--rw-r--r--   0 robstenson   (501) staff       (20)    23411 2022-08-25 16:27:21.000000 coldtype-0.9.8/coldtype/geometry/rect.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.403868 coldtype-0.9.8/coldtype/grid/
--rw-r--r--   0 robstenson   (501) staff       (20)     7616 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/grid/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1794 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/helpers.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.404712 coldtype-0.9.8/coldtype/img/
--rw-r--r--   0 robstenson   (501) staff       (20)     2038 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/img/blendmode.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3804 2022-08-25 16:30:30.000000 coldtype-0.9.8/coldtype/img/datimage.py
--rw-r--r--   0 robstenson   (501) staff       (20)      664 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/img/skiaimage.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.404997 coldtype-0.9.8/coldtype/interpolation/
--rw-r--r--   0 robstenson   (501) staff       (20)      442 2022-01-27 23:35:50.000000 coldtype-0.9.8/coldtype/interpolation/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)      271 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/interpolation.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.405301 coldtype-0.9.8/coldtype/midi/
--rw-r--r--   0 robstenson   (501) staff       (20)     1518 2022-02-02 18:43:53.000000 coldtype-0.9.8/coldtype/midi/controllers.py
--rw-r--r--   0 robstenson   (501) staff       (20)    12039 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/notebook.py
--rw-r--r--   0 robstenson   (501) staff       (20)      752 2022-05-04 20:28:36.000000 coldtype-0.9.8/coldtype/osutil.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.408996 coldtype-0.9.8/coldtype/pens/
--rw-r--r--   0 robstenson   (501) staff       (20)     2450 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/pens/axidrawpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)    16742 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/pens/blenderpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)       63 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/pens/datpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1720 2022-01-14 16:32:17.000000 coldtype-0.9.8/coldtype/pens/drawablepen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4043 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/pens/drawbotpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3823 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/pens/jsonpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3878 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/pens/misc.py
--rw-r--r--   0 robstenson   (501) staff       (20)    23172 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/pens/outlinepen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1805 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/pens/rendererdrawbotpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2962 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/pens/reportlabpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1704 2022-03-01 17:12:02.000000 coldtype-0.9.8/coldtype/pens/skiapathpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)    11651 2022-04-30 18:30:56.000000 coldtype-0.9.8/coldtype/pens/skiapen.py
--rw-r--r--   0 robstenson   (501) staff       (20)    11794 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/pens/svgpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     6194 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/pens/translationpen.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.409538 coldtype-0.9.8/coldtype/physics/
--rw-r--r--   0 robstenson   (501) staff       (20)      855 2022-02-10 21:25:49.000000 coldtype-0.9.8/coldtype/physics/pymunk.py
--rw-r--r--   0 robstenson   (501) staff       (20)      228 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/random.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.410795 coldtype-0.9.8/coldtype/renderable/
--rw-r--r--   0 robstenson   (501) staff       (20)      287 2021-12-06 19:20:07.000000 coldtype-0.9.8/coldtype/renderable/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)    13799 2022-08-07 01:16:51.000000 coldtype-0.9.8/coldtype/renderable/animation.py
--rw-r--r--   0 robstenson   (501) staff       (20)     5276 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/renderable/font.py
--rw-r--r--   0 robstenson   (501) staff       (20)    16364 2022-08-06 16:36:57.000000 coldtype-0.9.8/coldtype/renderable/renderable.py
--rw-r--r--   0 robstenson   (501) staff       (20)      230 2022-03-15 22:57:34.000000 coldtype-0.9.8/coldtype/renderable/tools.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1576 2021-12-13 01:26:57.000000 coldtype-0.9.8/coldtype/renderable/ui.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.414352 coldtype-0.9.8/coldtype/renderer/
--rw-r--r--   0 robstenson   (501) staff       (20)    63217 2022-08-07 18:00:35.000000 coldtype-0.9.8/coldtype/renderer/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     9305 2022-03-15 21:44:04.000000 coldtype-0.9.8/coldtype/renderer/config.py
--rw-r--r--   0 robstenson   (501) staff       (20)    20175 2022-03-09 02:12:48.000000 coldtype-0.9.8/coldtype/renderer/keyboard.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1392 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/renderer/picklejar.py
--rw-r--r--   0 robstenson   (501) staff       (20)    21314 2022-07-14 15:58:36.000000 coldtype-0.9.8/coldtype/renderer/reader.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4461 2022-01-31 17:25:39.000000 coldtype-0.9.8/coldtype/renderer/state.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1497 2022-05-04 20:28:19.000000 coldtype-0.9.8/coldtype/renderer/utils.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.416725 coldtype-0.9.8/coldtype/renderer/winman/
--rw-r--r--   0 robstenson   (501) staff       (20)     8249 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/renderer/winman/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2811 2021-12-18 02:56:40.000000 coldtype-0.9.8/coldtype/renderer/winman/audio.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1708 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/renderer/winman/blender.py
--rw-r--r--   0 robstenson   (501) staff       (20)    16441 2022-08-10 15:38:18.000000 coldtype-0.9.8/coldtype/renderer/winman/glfwskia.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4446 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/renderer/winman/midi.py
--rw-r--r--   0 robstenson   (501) staff       (20)      341 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/renderer/winman/passthrough.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.418315 coldtype-0.9.8/coldtype/runon/
--rw-r--r--   0 robstenson   (501) staff       (20)       38 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/runon/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     9290 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/runon/_path.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4035 2022-01-14 03:16:22.000000 coldtype-0.9.8/coldtype/runon/arrangement.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.420374 coldtype-0.9.8/coldtype/runon/mixins/
--rw-r--r--   0 robstenson   (501) staff       (20)    13400 2022-02-04 23:04:23.000000 coldtype-0.9.8/coldtype/runon/mixins/DrawingMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)     8481 2022-02-01 17:38:31.000000 coldtype-0.9.8/coldtype/runon/mixins/FXMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3250 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/runon/mixins/GeometryMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1910 2022-03-01 17:23:46.000000 coldtype-0.9.8/coldtype/runon/mixins/GlyphMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)    13643 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/runon/mixins/LayoutMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1742 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/runon/mixins/PathopsMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)     6084 2022-04-21 17:22:43.000000 coldtype-0.9.8/coldtype/runon/mixins/SegmentingMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1434 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/runon/mixins/SerializationMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3989 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/runon/mixins/StylingMixin.py
--rw-r--r--   0 robstenson   (501) staff       (20)    63865 2022-07-21 17:09:37.000000 coldtype-0.9.8/coldtype/runon/path.py
--rw-r--r--   0 robstenson   (501) staff       (20)    25902 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/runon/runon.py
--rw-r--r--   0 robstenson   (501) staff       (20)      732 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/test.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.422020 coldtype-0.9.8/coldtype/text/
--rw-r--r--   0 robstenson   (501) staff       (20)      301 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/text/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)    11746 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/text/composer.py
--rw-r--r--   0 robstenson   (501) staff       (20)    40841 2022-08-06 16:57:24.000000 coldtype-0.9.8/coldtype/text/reader.py
--rw-r--r--   0 robstenson   (501) staff       (20)     9205 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/text/richtext.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2188 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/text/shaper.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.424677 coldtype-0.9.8/coldtype/time/
--rw-r--r--   0 robstenson   (501) staff       (20)     1424 2022-02-03 02:08:03.000000 coldtype-0.9.8/coldtype/time/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1624 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/time/audio.py
--rw-r--r--   0 robstenson   (501) staff       (20)     6257 2021-12-06 19:20:07.000000 coldtype-0.9.8/coldtype/time/clip.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4450 2022-01-14 03:12:46.000000 coldtype-0.9.8/coldtype/time/easing.py
--rw-r--r--   0 robstenson   (501) staff       (20)    11905 2022-03-04 01:57:53.000000 coldtype-0.9.8/coldtype/time/midi.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.425655 coldtype-0.9.8/coldtype/time/nle/
--rw-r--r--   0 robstenson   (501) staff       (20)     5010 2022-05-01 17:31:35.000000 coldtype-0.9.8/coldtype/time/nle/ableton.py
--rw-r--r--   0 robstenson   (501) staff       (20)     8574 2022-01-28 02:44:50.000000 coldtype-0.9.8/coldtype/time/nle/ascii.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2626 2021-11-29 21:10:37.000000 coldtype-0.9.8/coldtype/time/nle/premiere.py
--rw-r--r--   0 robstenson   (501) staff       (20)    24050 2022-01-17 23:25:34.000000 coldtype-0.9.8/coldtype/time/sequence.py
--rw-r--r--   0 robstenson   (501) staff       (20)    10990 2022-03-04 21:36:40.000000 coldtype-0.9.8/coldtype/time/timeable.py
--rw-r--r--   0 robstenson   (501) staff       (20)     7238 2022-03-04 01:31:40.000000 coldtype-0.9.8/coldtype/time/timeline.py
--rw-r--r--   0 robstenson   (501) staff       (20)     3282 2022-08-06 16:40:50.000000 coldtype-0.9.8/coldtype/time/viewer.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1451 2022-07-08 17:12:14.000000 coldtype-0.9.8/coldtype/tool.py
--rw-r--r--   0 robstenson   (501) staff       (20)       61 2021-10-30 00:05:47.000000 coldtype-0.9.8/coldtype/warping.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.393066 coldtype-0.9.8/coldtype.egg-info/
--rw-r--r--   0 robstenson   (501) staff       (20)      730 2022-08-25 16:59:12.000000 coldtype-0.9.8/coldtype.egg-info/PKG-INFO
--rw-r--r--   0 robstenson   (501) staff       (20)     4408 2022-08-25 16:59:12.000000 coldtype-0.9.8/coldtype.egg-info/SOURCES.txt
--rw-r--r--   0 robstenson   (501) staff       (20)        1 2022-08-25 16:59:12.000000 coldtype-0.9.8/coldtype.egg-info/dependency_links.txt
--rw-r--r--   0 robstenson   (501) staff       (20)       53 2022-08-25 16:59:12.000000 coldtype-0.9.8/coldtype.egg-info/entry_points.txt
--rw-r--r--   0 robstenson   (501) staff       (20)      355 2022-08-25 16:59:12.000000 coldtype-0.9.8/coldtype.egg-info/requires.txt
--rw-r--r--   0 robstenson   (501) staff       (20)        9 2022-08-25 16:59:12.000000 coldtype-0.9.8/coldtype.egg-info/top_level.txt
--rw-r--r--   0 robstenson   (501) staff       (20)       38 2022-08-25 16:59:12.432687 coldtype-0.9.8/setup.cfg
--rw-r--r--   0 robstenson   (501) staff       (20)     3015 2022-08-25 16:57:43.000000 coldtype-0.9.8/setup.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-25 16:59:12.432089 coldtype-0.9.8/test/
--rw-r--r--   0 robstenson   (501) staff       (20)     1727 2022-01-14 03:16:22.000000 coldtype-0.9.8/test/test_arrangement.py
--rw-r--r--   0 robstenson   (501) staff       (20)      439 2021-10-30 00:05:47.000000 coldtype-0.9.8/test/test_color.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2359 2022-08-06 16:53:52.000000 coldtype-0.9.8/test/test_drawbot_pens.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1264 2021-11-05 19:16:45.000000 coldtype-0.9.8/test/test_fx_xray.py
--rw-r--r--   0 robstenson   (501) staff       (20)      895 2022-02-19 18:23:26.000000 coldtype-0.9.8/test/test_geometry.py
--rw-r--r--   0 robstenson   (501) staff       (20)     7449 2022-08-06 16:54:02.000000 coldtype-0.9.8/test/test_glyphwise.py
--rw-r--r--   0 robstenson   (501) staff       (20)     5935 2022-08-06 17:00:20.000000 coldtype-0.9.8/test/test_i18n.py
--rw-r--r--   0 robstenson   (501) staff       (20)     5548 2022-01-14 03:12:46.000000 coldtype-0.9.8/test/test_p.py
--rw-r--r--   0 robstenson   (501) staff       (20)    13906 2022-01-14 03:12:46.000000 coldtype-0.9.8/test/test_pens.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1835 2022-01-14 03:12:46.000000 coldtype-0.9.8/test/test_pens_rendered.py
--rw-r--r--   0 robstenson   (501) staff       (20)     2426 2022-05-04 20:28:22.000000 coldtype-0.9.8/test/test_reader.py
--rw-r--r--   0 robstenson   (501) staff       (20)      957 2022-01-14 03:12:46.000000 coldtype-0.9.8/test/test_reportlabpen.py
--rw-r--r--   0 robstenson   (501) staff       (20)     1760 2022-08-06 16:54:43.000000 coldtype-0.9.8/test/test_richtext.py
--rw-r--r--   0 robstenson   (501) staff       (20)    12601 2022-03-08 16:22:19.000000 coldtype-0.9.8/test/test_runon.py
--rw-r--r--   0 robstenson   (501) staff       (20)     5553 2021-10-30 00:05:47.000000 coldtype-0.9.8/test/test_syntax_mods.py
--rw-r--r--   0 robstenson   (501) staff       (20)     7020 2022-08-06 16:55:11.000000 coldtype-0.9.8/test/test_text.py
--rw-r--r--   0 robstenson   (501) staff       (20)     4965 2022-08-06 17:03:31.000000 coldtype-0.9.8/test/test_time.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.046480 coldtype-0.9.9/
+-rw-r--r--   0 robstenson   (501) staff       (20)    11397 2021-10-30 00:05:47.000000 coldtype-0.9.9/LICENSE
+-rw-r--r--   0 robstenson   (501) staff       (20)      730 2022-08-29 21:30:54.045861 coldtype-0.9.9/PKG-INFO
+-rw-r--r--   0 robstenson   (501) staff       (20)     2849 2021-10-30 00:05:47.000000 coldtype-0.9.9/README.md
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.987405 coldtype-0.9.9/coldtype/
+-rw-r--r--   0 robstenson   (501) staff       (20)     2189 2022-08-29 21:07:16.000000 coldtype-0.9.9/coldtype/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4221 2022-01-24 18:05:54.000000 coldtype-0.9.9/coldtype/axidraw.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4734 2022-02-01 18:13:46.000000 coldtype-0.9.9/coldtype/beziers.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.992485 coldtype-0.9.9/coldtype/blender/
+-rw-r--r--   0 robstenson   (501) staff       (20)    11548 2022-07-08 17:12:14.000000 coldtype-0.9.9/coldtype/blender/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    31750 2022-07-22 17:26:15.000000 coldtype-0.9.9/coldtype/blender/fluent.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1971 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/blender/livepreview.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3388 2022-02-21 18:10:34.000000 coldtype-0.9.9/coldtype/blender/panel3d.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2660 2021-12-10 17:19:05.000000 coldtype-0.9.9/coldtype/blender/render.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    13372 2021-12-07 18:09:55.000000 coldtype-0.9.9/coldtype/blender/timedtext.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      776 2022-02-21 17:22:38.000000 coldtype-0.9.9/coldtype/blender/util.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    12958 2022-08-08 16:01:40.000000 coldtype-0.9.9/coldtype/blender/watch.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.992765 coldtype-0.9.9/coldtype/capture/
+-rw-r--r--   0 robstenson   (501) staff       (20)      503 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/capture/__init__.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.993687 coldtype-0.9.9/coldtype/color/
+-rw-r--r--   0 robstenson   (501) staff       (20)     9736 2022-01-25 21:24:30.000000 coldtype-0.9.9/coldtype/color/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     5751 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/color/html.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      351 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/css.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4470 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/drawbot.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.980702 coldtype-0.9.9/coldtype/fontgoggles/
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.995040 coldtype-0.9.9/coldtype/fontgoggles/compile/
+-rw-r--r--   0 robstenson   (501) staff       (20)        0 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/compile/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1324 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/compile/compilerPool.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2417 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/compile/dsCompiler.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      167 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/compile/ttxCompiler.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     8173 2022-08-06 00:33:56.000000 coldtype-0.9.9/coldtype/fontgoggles/compile/ufoCompiler.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1120 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/compile/workServer.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.996053 coldtype-0.9.9/coldtype/fontgoggles/font/
+-rw-r--r--   0 robstenson   (501) staff       (20)     6278 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/font/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     7339 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/font/baseFont.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    21628 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/font/dsFont.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1075 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/font/glyphDrawing.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3336 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/font/otfFont.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    18528 2022-07-29 17:56:20.000000 coldtype-0.9.9/coldtype/fontgoggles/font/ufoFont.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.997859 coldtype-0.9.9/coldtype/fontgoggles/misc/
+-rw-r--r--   0 robstenson   (501) staff       (20)        0 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/misc/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2781 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/misc/ftFont.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     8270 2022-03-25 18:52:02.000000 coldtype-0.9.9/coldtype/fontgoggles/misc/hbShape.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    53377 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/misc/opentypeTags.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4334 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/misc/properties.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2924 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/misc/rectTree.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3855 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/misc/segmenting.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2748 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fontgoggles/misc/textInfo.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.999219 coldtype-0.9.9/coldtype/fx/
+-rw-r--r--   0 robstenson   (501) staff       (20)      205 2021-11-11 19:52:09.000000 coldtype-0.9.9/coldtype/fx/chainable.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      448 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fx/motion.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2743 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/fx/shapes.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    10207 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/fx/skia.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2768 2021-11-01 15:54:34.000000 coldtype-0.9.9/coldtype/fx/warping.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2555 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/fx/xray.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.002941 coldtype-0.9.9/coldtype/geometry/
+-rw-r--r--   0 robstenson   (501) staff       (20)      654 2021-11-12 22:46:47.000000 coldtype-0.9.9/coldtype/geometry/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      812 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/geometry/atom.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1925 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/geometry/curve.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1623 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/geometry/edge.py
+-rw-r--r--   0 robstenson   (501) staff       (20)       29 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/geometry/geometrical.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     5483 2022-02-03 17:40:28.000000 coldtype-0.9.9/coldtype/geometry/line.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     5016 2021-11-05 16:46:39.000000 coldtype-0.9.9/coldtype/geometry/point.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     5577 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/geometry/primitives.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    23411 2022-08-25 16:27:21.000000 coldtype-0.9.9/coldtype/geometry/rect.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.005096 coldtype-0.9.9/coldtype/grid/
+-rw-r--r--   0 robstenson   (501) staff       (20)     7616 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/grid/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1794 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/helpers.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.008195 coldtype-0.9.9/coldtype/img/
+-rw-r--r--   0 robstenson   (501) staff       (20)     2038 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/img/blendmode.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3804 2022-08-25 16:30:30.000000 coldtype-0.9.9/coldtype/img/datimage.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      664 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/img/skiaimage.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.010198 coldtype-0.9.9/coldtype/interpolation/
+-rw-r--r--   0 robstenson   (501) staff       (20)      442 2022-01-27 23:35:50.000000 coldtype-0.9.9/coldtype/interpolation/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      271 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/interpolation.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.010507 coldtype-0.9.9/coldtype/midi/
+-rw-r--r--   0 robstenson   (501) staff       (20)     1518 2022-02-02 18:43:53.000000 coldtype-0.9.9/coldtype/midi/controllers.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    12039 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/notebook.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      752 2022-05-04 20:28:36.000000 coldtype-0.9.9/coldtype/osutil.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.015797 coldtype-0.9.9/coldtype/pens/
+-rw-r--r--   0 robstenson   (501) staff       (20)     2450 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/pens/axidrawpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    16742 2022-07-08 17:12:14.000000 coldtype-0.9.9/coldtype/pens/blenderpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)       63 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/pens/datpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1720 2022-01-14 16:32:17.000000 coldtype-0.9.9/coldtype/pens/drawablepen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4043 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/pens/drawbotpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3823 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/pens/jsonpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3878 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/pens/misc.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    23172 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/pens/outlinepen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1805 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/pens/rendererdrawbotpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2962 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/pens/reportlabpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1704 2022-03-01 17:12:02.000000 coldtype-0.9.9/coldtype/pens/skiapathpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    12794 2022-08-29 21:06:28.000000 coldtype-0.9.9/coldtype/pens/skiapen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    11794 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/pens/svgpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     6194 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/pens/translationpen.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.016183 coldtype-0.9.9/coldtype/physics/
+-rw-r--r--   0 robstenson   (501) staff       (20)      855 2022-02-10 21:25:49.000000 coldtype-0.9.9/coldtype/physics/pymunk.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      228 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/random.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.017623 coldtype-0.9.9/coldtype/renderable/
+-rw-r--r--   0 robstenson   (501) staff       (20)      287 2021-12-06 19:20:07.000000 coldtype-0.9.9/coldtype/renderable/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    13799 2022-08-07 01:16:51.000000 coldtype-0.9.9/coldtype/renderable/animation.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     5276 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/renderable/font.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    16364 2022-08-06 16:36:57.000000 coldtype-0.9.9/coldtype/renderable/renderable.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      230 2022-03-15 22:57:34.000000 coldtype-0.9.9/coldtype/renderable/tools.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1576 2021-12-13 01:26:57.000000 coldtype-0.9.9/coldtype/renderable/ui.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.021688 coldtype-0.9.9/coldtype/renderer/
+-rw-r--r--   0 robstenson   (501) staff       (20)    63217 2022-08-07 18:00:35.000000 coldtype-0.9.9/coldtype/renderer/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     9305 2022-03-15 21:44:04.000000 coldtype-0.9.9/coldtype/renderer/config.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    20175 2022-03-09 02:12:48.000000 coldtype-0.9.9/coldtype/renderer/keyboard.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1392 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/renderer/picklejar.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    21314 2022-07-14 15:58:36.000000 coldtype-0.9.9/coldtype/renderer/reader.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4461 2022-01-31 17:25:39.000000 coldtype-0.9.9/coldtype/renderer/state.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1497 2022-05-04 20:28:19.000000 coldtype-0.9.9/coldtype/renderer/utils.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.023980 coldtype-0.9.9/coldtype/renderer/winman/
+-rw-r--r--   0 robstenson   (501) staff       (20)     8249 2022-07-08 17:12:14.000000 coldtype-0.9.9/coldtype/renderer/winman/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2811 2021-12-18 02:56:40.000000 coldtype-0.9.9/coldtype/renderer/winman/audio.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1708 2022-07-08 17:12:14.000000 coldtype-0.9.9/coldtype/renderer/winman/blender.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    16441 2022-08-10 15:38:18.000000 coldtype-0.9.9/coldtype/renderer/winman/glfwskia.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4446 2022-07-08 17:12:14.000000 coldtype-0.9.9/coldtype/renderer/winman/midi.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      341 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/renderer/winman/passthrough.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.025466 coldtype-0.9.9/coldtype/runon/
+-rw-r--r--   0 robstenson   (501) staff       (20)       38 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/runon/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     9290 2022-07-08 17:12:14.000000 coldtype-0.9.9/coldtype/runon/_path.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4035 2022-01-14 03:16:22.000000 coldtype-0.9.9/coldtype/runon/arrangement.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.027394 coldtype-0.9.9/coldtype/runon/mixins/
+-rw-r--r--   0 robstenson   (501) staff       (20)    13669 2022-08-29 21:06:28.000000 coldtype-0.9.9/coldtype/runon/mixins/DrawingMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     8481 2022-02-01 17:38:31.000000 coldtype-0.9.9/coldtype/runon/mixins/FXMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3250 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/runon/mixins/GeometryMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1910 2022-03-01 17:23:46.000000 coldtype-0.9.9/coldtype/runon/mixins/GlyphMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    14011 2022-08-29 21:06:28.000000 coldtype-0.9.9/coldtype/runon/mixins/LayoutMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1742 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/runon/mixins/PathopsMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     6084 2022-04-21 17:22:43.000000 coldtype-0.9.9/coldtype/runon/mixins/SegmentingMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1434 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/runon/mixins/SerializationMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3997 2022-08-29 21:06:28.000000 coldtype-0.9.9/coldtype/runon/mixins/StylingMixin.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    64519 2022-08-29 21:06:28.000000 coldtype-0.9.9/coldtype/runon/path.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    25902 2022-08-29 17:09:02.000000 coldtype-0.9.9/coldtype/runon/runon.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      732 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/test.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.028978 coldtype-0.9.9/coldtype/text/
+-rw-r--r--   0 robstenson   (501) staff       (20)      301 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/text/__init__.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.031370 coldtype-0.9.9/coldtype/text/colr/
+-rw-r--r--   0 robstenson   (501) staff       (20)     3508 2022-08-29 21:06:28.000000 coldtype-0.9.9/coldtype/text/colr/brsurface.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2248 2022-08-29 21:06:28.000000 coldtype-0.9.9/coldtype/text/colr/skia.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    11746 2022-07-08 17:12:14.000000 coldtype-0.9.9/coldtype/text/composer.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    42961 2022-08-29 21:29:13.000000 coldtype-0.9.9/coldtype/text/reader.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     9205 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/text/richtext.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2188 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/text/shaper.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.034556 coldtype-0.9.9/coldtype/time/
+-rw-r--r--   0 robstenson   (501) staff       (20)     1424 2022-02-03 02:08:03.000000 coldtype-0.9.9/coldtype/time/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1624 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/time/audio.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     6257 2021-12-06 19:20:07.000000 coldtype-0.9.9/coldtype/time/clip.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4450 2022-01-14 03:12:46.000000 coldtype-0.9.9/coldtype/time/easing.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    11905 2022-03-04 01:57:53.000000 coldtype-0.9.9/coldtype/time/midi.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.035354 coldtype-0.9.9/coldtype/time/nle/
+-rw-r--r--   0 robstenson   (501) staff       (20)     5010 2022-05-01 17:31:35.000000 coldtype-0.9.9/coldtype/time/nle/ableton.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     8574 2022-01-28 02:44:50.000000 coldtype-0.9.9/coldtype/time/nle/ascii.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2626 2021-11-29 21:10:37.000000 coldtype-0.9.9/coldtype/time/nle/premiere.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    24050 2022-01-17 23:25:34.000000 coldtype-0.9.9/coldtype/time/sequence.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    10990 2022-03-04 21:36:40.000000 coldtype-0.9.9/coldtype/time/timeable.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     7238 2022-03-04 01:31:40.000000 coldtype-0.9.9/coldtype/time/timeline.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     3282 2022-08-06 16:40:50.000000 coldtype-0.9.9/coldtype/time/viewer.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1451 2022-07-08 17:12:14.000000 coldtype-0.9.9/coldtype/tool.py
+-rw-r--r--   0 robstenson   (501) staff       (20)       61 2021-10-30 00:05:47.000000 coldtype-0.9.9/coldtype/warping.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:53.989325 coldtype-0.9.9/coldtype.egg-info/
+-rw-r--r--   0 robstenson   (501) staff       (20)      730 2022-08-29 21:30:53.000000 coldtype-0.9.9/coldtype.egg-info/PKG-INFO
+-rw-r--r--   0 robstenson   (501) staff       (20)     4467 2022-08-29 21:30:53.000000 coldtype-0.9.9/coldtype.egg-info/SOURCES.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)        1 2022-08-29 21:30:53.000000 coldtype-0.9.9/coldtype.egg-info/dependency_links.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)       53 2022-08-29 21:30:53.000000 coldtype-0.9.9/coldtype.egg-info/entry_points.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)      376 2022-08-29 21:30:53.000000 coldtype-0.9.9/coldtype.egg-info/requires.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)        9 2022-08-29 21:30:53.000000 coldtype-0.9.9/coldtype.egg-info/top_level.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)       38 2022-08-29 21:30:54.046537 coldtype-0.9.9/setup.cfg
+-rw-r--r--   0 robstenson   (501) staff       (20)     3078 2022-08-29 21:09:48.000000 coldtype-0.9.9/setup.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2022-08-29 21:30:54.045250 coldtype-0.9.9/test/
+-rw-r--r--   0 robstenson   (501) staff       (20)     1727 2022-01-14 03:16:22.000000 coldtype-0.9.9/test/test_arrangement.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      439 2021-10-30 00:05:47.000000 coldtype-0.9.9/test/test_color.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2359 2022-08-06 16:53:52.000000 coldtype-0.9.9/test/test_drawbot_pens.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1264 2021-11-05 19:16:45.000000 coldtype-0.9.9/test/test_fx_xray.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      895 2022-02-19 18:23:26.000000 coldtype-0.9.9/test/test_geometry.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     7449 2022-08-06 16:54:02.000000 coldtype-0.9.9/test/test_glyphwise.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     5935 2022-08-06 17:00:20.000000 coldtype-0.9.9/test/test_i18n.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     5548 2022-01-14 03:12:46.000000 coldtype-0.9.9/test/test_p.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    13906 2022-01-14 03:12:46.000000 coldtype-0.9.9/test/test_pens.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1835 2022-01-14 03:12:46.000000 coldtype-0.9.9/test/test_pens_rendered.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     2426 2022-05-04 20:28:22.000000 coldtype-0.9.9/test/test_reader.py
+-rw-r--r--   0 robstenson   (501) staff       (20)      957 2022-01-14 03:12:46.000000 coldtype-0.9.9/test/test_reportlabpen.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     1760 2022-08-06 16:54:43.000000 coldtype-0.9.9/test/test_richtext.py
+-rw-r--r--   0 robstenson   (501) staff       (20)    12601 2022-03-08 16:22:19.000000 coldtype-0.9.9/test/test_runon.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     5553 2021-10-30 00:05:47.000000 coldtype-0.9.9/test/test_syntax_mods.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     7020 2022-08-06 16:55:11.000000 coldtype-0.9.9/test/test_text.py
+-rw-r--r--   0 robstenson   (501) staff       (20)     4965 2022-08-06 17:03:31.000000 coldtype-0.9.9/test/test_time.py
```

### Comparing `coldtype-0.9.8/LICENSE` & `coldtype-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/PKG-INFO` & `coldtype-0.9.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coldtype
-Version: 0.9.8
+Version: 0.9.9
 Summary: Functions for manual vectorized typesetting
 Home-page: https://github.com/goodhertz/coldtype
 Author: Rob Stenson / Goodhertz
 Author-email: rob@goodhertz.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `coldtype-0.9.8/README.md` & `coldtype-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/__init__.py` & `coldtype-0.9.9/coldtype/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from coldtype.time.easing import ez
 from coldtype.time.nle.ascii import AsciiTimeline
 from coldtype.time.midi import MidiTimeline
 from coldtype.img.blendmode import BlendMode
 from coldtype.grid import Grid
 
 name = "coldtype"
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 __FILE__ = None # will be redefined contextually
 __BLENDER__ = None # will be redefined contextually
 
 __sibling__ = lambda x: x # will be redefined contextually
 __inputs__ = [] # will be redefined contextually
 __memory__ = [] # will be redefined contextually
```

### Comparing `coldtype-0.9.8/coldtype/axidraw.py` & `coldtype-0.9.9/coldtype/axidraw.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/beziers.py` & `coldtype-0.9.9/coldtype/beziers.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/blender/__init__.py` & `coldtype-0.9.9/coldtype/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/blender/fluent.py` & `coldtype-0.9.9/coldtype/blender/fluent.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/blender/livepreview.py` & `coldtype-0.9.9/coldtype/blender/livepreview.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/blender/panel3d.py` & `coldtype-0.9.9/coldtype/blender/panel3d.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/blender/render.py` & `coldtype-0.9.9/coldtype/blender/render.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/blender/timedtext.py` & `coldtype-0.9.9/coldtype/blender/timedtext.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/blender/util.py` & `coldtype-0.9.9/coldtype/blender/util.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/blender/watch.py` & `coldtype-0.9.9/coldtype/blender/watch.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/color/__init__.py` & `coldtype-0.9.9/coldtype/color/__init__.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/color/html.py` & `coldtype-0.9.9/coldtype/color/html.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/drawbot.py` & `coldtype-0.9.9/coldtype/drawbot.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/compile/compilerPool.py` & `coldtype-0.9.9/coldtype/fontgoggles/compile/compilerPool.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/compile/dsCompiler.py` & `coldtype-0.9.9/coldtype/fontgoggles/compile/dsCompiler.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/compile/ufoCompiler.py` & `coldtype-0.9.9/coldtype/fontgoggles/compile/ufoCompiler.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/compile/workServer.py` & `coldtype-0.9.9/coldtype/fontgoggles/compile/workServer.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/font/__init__.py` & `coldtype-0.9.9/coldtype/fontgoggles/font/__init__.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/font/baseFont.py` & `coldtype-0.9.9/coldtype/fontgoggles/font/baseFont.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/font/dsFont.py` & `coldtype-0.9.9/coldtype/fontgoggles/font/dsFont.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/font/glyphDrawing.py` & `coldtype-0.9.9/coldtype/fontgoggles/font/glyphDrawing.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/font/otfFont.py` & `coldtype-0.9.9/coldtype/fontgoggles/font/otfFont.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/font/ufoFont.py` & `coldtype-0.9.9/coldtype/fontgoggles/font/ufoFont.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/misc/ftFont.py` & `coldtype-0.9.9/coldtype/fontgoggles/misc/ftFont.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/misc/hbShape.py` & `coldtype-0.9.9/coldtype/fontgoggles/misc/hbShape.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/misc/opentypeTags.py` & `coldtype-0.9.9/coldtype/fontgoggles/misc/opentypeTags.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/misc/properties.py` & `coldtype-0.9.9/coldtype/fontgoggles/misc/properties.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/misc/rectTree.py` & `coldtype-0.9.9/coldtype/fontgoggles/misc/rectTree.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/misc/segmenting.py` & `coldtype-0.9.9/coldtype/fontgoggles/misc/segmenting.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fontgoggles/misc/textInfo.py` & `coldtype-0.9.9/coldtype/fontgoggles/misc/textInfo.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fx/shapes.py` & `coldtype-0.9.9/coldtype/fx/shapes.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fx/skia.py` & `coldtype-0.9.9/coldtype/fx/skia.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fx/warping.py` & `coldtype-0.9.9/coldtype/fx/warping.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/fx/xray.py` & `coldtype-0.9.9/coldtype/fx/xray.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/geometry/__init__.py` & `coldtype-0.9.9/coldtype/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/geometry/atom.py` & `coldtype-0.9.9/coldtype/geometry/atom.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/geometry/curve.py` & `coldtype-0.9.9/coldtype/geometry/curve.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/geometry/edge.py` & `coldtype-0.9.9/coldtype/geometry/edge.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/geometry/line.py` & `coldtype-0.9.9/coldtype/geometry/line.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/geometry/point.py` & `coldtype-0.9.9/coldtype/geometry/point.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/geometry/primitives.py` & `coldtype-0.9.9/coldtype/geometry/primitives.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/geometry/rect.py` & `coldtype-0.9.9/coldtype/geometry/rect.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/grid/__init__.py` & `coldtype-0.9.9/coldtype/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/helpers.py` & `coldtype-0.9.9/coldtype/helpers.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/img/blendmode.py` & `coldtype-0.9.9/coldtype/img/blendmode.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/img/datimage.py` & `coldtype-0.9.9/coldtype/img/datimage.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/img/skiaimage.py` & `coldtype-0.9.9/coldtype/img/skiaimage.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/midi/controllers.py` & `coldtype-0.9.9/coldtype/midi/controllers.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/notebook.py` & `coldtype-0.9.9/coldtype/notebook.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/osutil.py` & `coldtype-0.9.9/coldtype/osutil.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/axidrawpen.py` & `coldtype-0.9.9/coldtype/pens/axidrawpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/blenderpen.py` & `coldtype-0.9.9/coldtype/pens/blenderpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/drawablepen.py` & `coldtype-0.9.9/coldtype/pens/drawablepen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/drawbotpen.py` & `coldtype-0.9.9/coldtype/pens/drawbotpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/jsonpen.py` & `coldtype-0.9.9/coldtype/pens/jsonpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/misc.py` & `coldtype-0.9.9/coldtype/pens/misc.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/outlinepen.py` & `coldtype-0.9.9/coldtype/pens/outlinepen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/rendererdrawbotpen.py` & `coldtype-0.9.9/coldtype/pens/rendererdrawbotpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/reportlabpen.py` & `coldtype-0.9.9/coldtype/pens/reportlabpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/skiapathpen.py` & `coldtype-0.9.9/coldtype/pens/skiapathpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/skiapen.py` & `coldtype-0.9.9/coldtype/pens/skiapen.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 from coldtype.pens.skiapathpen import SkiaPathPen
 from coldtype.runon.path import P
 from coldtype.img.datimage import DATImage
 from coldtype.geometry import Rect, Point
 from coldtype.text.reader import Style
 from coldtype.color import Color
 
+try:
+    from coldtype.text.colr.skia import SkiaShaders
+except ImportError:
+    pass
+
 
 class SkiaPen(DrawablePenMixin, SkiaPathPen):
     def __init__(self, dat, rect, canvas, scale, style=None, alpha=1):
         super().__init__(dat, rect.h)
         self.scale = scale
         self.canvas = canvas
         self.rect = rect
@@ -50,20 +55,49 @@
                 pass
             elif method == "stroke" and args[0].get("weight") == 0:
                 pass
             elif method == "dash":
                 pass
             else:
                 canvas.save()
-                did_draw = self.applyDATAttribute(attrs, attr)
+                
+                if method == "COLR":
+                    did_draw = False
+                    self.colr(args[0], dat)
+                else:
+                    did_draw = self.applyDATAttribute(attrs, attr)
+
                 self.paint.setAlphaf(self.paint.getAlphaf()*self.alpha)
                 if not did_draw:
                     canvas.drawPath(self.path, self.paint)
                 canvas.restore()
-    
+
+    def colr(self, data, pen:P):
+        method, args = data
+        shader_fn = getattr(SkiaShaders, method)
+        if shader_fn:
+            ss = pen.data("substructure").copy()
+            ss.invertYAxis(self.rect.h)
+            sval = ss._val.value
+            
+            if method == "drawPathLinearGradient":
+                args["pt1"] = sval[0][1][0]
+                args["pt2"] = sval[1][1][0]
+            elif method == "drawPathSweepGradient":
+                args["center"] = sval[0][1][0]
+            elif method == "drawPathRadialGradient":
+                args["startCenter"] = sval[0][1][0]
+                args["endCenter"] = sval[1][1][0]
+
+            shader = shader_fn(*args.values())
+            self.paint.setStyle(skia.Paint.kFill_Style)
+            self.paint.setShader(shader)
+        else:
+            raise Exception("No matching SkiaShaders function for " + method)
+
     def fill(self, color):
         self.paint.setStyle(skia.Paint.kFill_Style)
         if color:
             if isinstance(color, Gradient):
                 self.gradient(color)
             elif isinstance(color, Color):
                 self.paint.setColor(color.skia())
```

### Comparing `coldtype-0.9.8/coldtype/pens/svgpen.py` & `coldtype-0.9.9/coldtype/pens/svgpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/pens/translationpen.py` & `coldtype-0.9.9/coldtype/pens/translationpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/physics/pymunk.py` & `coldtype-0.9.9/coldtype/physics/pymunk.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderable/animation.py` & `coldtype-0.9.9/coldtype/renderable/animation.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderable/font.py` & `coldtype-0.9.9/coldtype/renderable/font.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderable/renderable.py` & `coldtype-0.9.9/coldtype/renderable/renderable.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderable/ui.py` & `coldtype-0.9.9/coldtype/renderable/ui.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/__init__.py` & `coldtype-0.9.9/coldtype/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/config.py` & `coldtype-0.9.9/coldtype/renderer/config.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/keyboard.py` & `coldtype-0.9.9/coldtype/renderer/keyboard.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/picklejar.py` & `coldtype-0.9.9/coldtype/renderer/picklejar.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/reader.py` & `coldtype-0.9.9/coldtype/renderer/reader.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/state.py` & `coldtype-0.9.9/coldtype/renderer/state.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/utils.py` & `coldtype-0.9.9/coldtype/renderer/utils.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/winman/__init__.py` & `coldtype-0.9.9/coldtype/renderer/winman/__init__.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/winman/audio.py` & `coldtype-0.9.9/coldtype/renderer/winman/audio.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/winman/blender.py` & `coldtype-0.9.9/coldtype/renderer/winman/blender.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/winman/glfwskia.py` & `coldtype-0.9.9/coldtype/renderer/winman/glfwskia.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/renderer/winman/midi.py` & `coldtype-0.9.9/coldtype/renderer/winman/midi.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/_path.py` & `coldtype-0.9.9/coldtype/runon/_path.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/arrangement.py` & `coldtype-0.9.9/coldtype/runon/arrangement.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/DrawingMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/DrawingMixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -450,8 +450,17 @@
         self._val = RecordingPen()
 
         self._val.moveTo(self._els[0].v.value[0][-1][-1])
         for el in self._els:
             self._val.value.extend(el.v.value[1:])
         
         self._els = []
-        return self
+        return self
+    
+    def substructure(self):
+        indicators = type(self)()
+        def append(p):
+            substructure = p.data("substructure")
+            if substructure:
+                indicators.append(substructure)
+        self.mapv(append)
+        return indicators
```

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/FXMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/FXMixin.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/GeometryMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/GeometryMixin.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/GlyphMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/GlyphMixin.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/LayoutMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/LayoutMixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,20 +222,31 @@
         f = self._data.get("frame")
         if transformFrame and f:
             self.data(frame=f.transform(transform))
         
         for p in self._els:
             p.transform(transform, transformFrame=transformFrame)
         
+        substructure = self._data.get("substructure")
+        if substructure:
+            substructure.transform(transform, transformFrame=transformFrame)
+        
         img = self.img()
         if img:
             img["rect"] = img["rect"].transform(transform)
         
         return self
     
+    def invertYAxis(self, height):
+        rp = RecordingPen()
+        tp = TransformPen(rp, (1, 0, 0, -1, 0, height))
+        self.replay(tp)
+        self._val.value = rp.value
+        return self
+    
     def nonlinear_transform(self, fn):
         for el in self._els:
             el.nonlinear_transform(fn)
         
         if self.val_present():
             for idx, (move, pts) in enumerate(self._val.value):
                 if len(pts) > 0:
```

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/PathopsMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/PathopsMixin.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/SegmentingMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/SegmentingMixin.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/SerializationMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/SerializationMixin.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/runon/mixins/StylingMixin.py` & `coldtype-0.9.9/coldtype/runon/mixins/StylingMixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             sf = True
             del st["strokeFirst"]
         
 
         if "fill" not in st:
             st["fill"] = rgb(1, 0, 0.5)
         
-        rest = ["blendmode", "image", "skp"]
+        rest = ["blendmode", "image", "skp", "COLR"]
         if sf:
             order = ["shadow", "stroke", "fill", *rest]
         else:
             order = ["shadow", "fill", "stroke", *rest]
         
         sort = {k:v for k,v in sorted(st.items(), key=lambda kv: order.index(kv[0]))}
         return sort
```

### Comparing `coldtype-0.9.8/coldtype/runon/path.py` & `coldtype-0.9.9/coldtype/runon/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -865,14 +865,23 @@
 
         self._val.moveTo(self._els[0].v.value[0][-1][-1])
         for el in self._els:
             self._val.value.extend(el.v.value[1:])
         
         self._els = []
         return self
+    
+    def substructure(self):
+        indicators = type(self)()
+        def append(p):
+            substructure = p.data("substructure")
+            if substructure:
+                indicators.append(substructure)
+        self.mapv(append)
+        return indicators
 
     def bounds(self):
         """Calculate the exact bounds of this shape, using a BoundPen"""
         b = Rect(0, 0, 0, 0)
         
         if self.val_present():
             try:
@@ -1096,21 +1105,34 @@
         f = self._data.get("frame")
         if transformFrame and f:
             self.data(frame=f.transform(transform))
         
         for p in self._els:
             p.transform(transform, transformFrame=transformFrame)
         
+        substructure = self._data.get("substructure")
+        if substructure:
+            substructure.transform(transform, transformFrame=transformFrame)
+        
         img = self.img()
         if img:
             img["rect"] = img["rect"].transform(transform)
         
         return self
     
 
+    def invertYAxis(self, height) -> "P":
+
+        rp = RecordingPen()
+        tp = TransformPen(rp, (1, 0, 0, -1, 0, height))
+        self.replay(tp)
+        self._val.value = rp.value
+        return self
+    
+
     def nonlinear_transform(self, fn) -> "P":
 
         for el in self._els:
             el.nonlinear_transform(fn)
         
         if self.val_present():
             for idx, (move, pts) in enumerate(self._val.value):
@@ -1364,15 +1386,15 @@
             sf = True
             del st["strokeFirst"]
         
 
         if "fill" not in st:
             st["fill"] = rgb(1, 0, 0.5)
         
-        rest = ["blendmode", "image", "skp"]
+        rest = ["blendmode", "image", "skp", "COLR"]
         if sf:
             order = ["shadow", "stroke", "fill", *rest]
         else:
             order = ["shadow", "fill", "stroke", *rest]
         
         sort = {k:v for k,v in sorted(st.items(), key=lambda kv: order.index(kv[0]))}
         return sort
```

### Comparing `coldtype-0.9.8/coldtype/runon/runon.py` & `coldtype-0.9.9/coldtype/runon/runon.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/test.py` & `coldtype-0.9.9/coldtype/test.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/text/composer.py` & `coldtype-0.9.9/coldtype/text/composer.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/text/reader.py` & `coldtype-0.9.9/coldtype/text/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 from coldtype.runon.path import P
 from coldtype.geometry import Rect
 
 from coldtype.osutil import on_linux, on_mac, on_windows
 
 from typing import Union
 
-try:
-    from skia import Matrix
-    from coldtype.pens.skiapathpen import SkiaPathPen
-except ImportError:
-    Matrix = None
-    SkiaPathPen = None
-
 from coldtype.fontgoggles.font import getOpener
 from coldtype.fontgoggles.font.baseFont import BaseFont
 from coldtype.fontgoggles.font.otfFont import OTFFont
 from coldtype.fontgoggles.misc.textInfo import TextInfo
 
+try:
+    from blackrenderer.font import BlackRendererFont
+    #from blackrenderer.backends.pathCollector import PathCollectorSurface, PathCollectorRecordingPen
+    from coldtype.text.colr.brsurface import BRPathCollectorSurface, BRPathCollectorRecordingPen
+except ImportError:
+    BlackRendererFont = None
+    pass
+
 
 class FittableMixin():
     def textContent(self):
         print("textContent() not overwritten")
 
     def fit(self, width):
         """Use various methods (tracking, `wdth` axis, etc. — properties specified in the `Style` object) to fit a piece of text horizontally to a given `width` (warning: not very fast)"""
@@ -129,29 +130,39 @@
         numFonts, opener, getSortInfo = getOpener(self.path)
         self.font:BaseFont = opener(self.path, number)
         self.font.cocoa = False
         self.cacheable = cacheable
         self._loaded = False
         self.load()
 
+        self._colr = self.font.ttFont.get("COLR")
+        self._colrv1 = self._colr is not None and self._colr.version == 1 and BlackRendererFont is not None
+
+        if self._colrv1:
+            self._brFont = BlackRendererFont(self.path, fontNumber=number)
+        else:
+            self._brFont = None
+
+        self._variations = self.font.ttFont.get("fvar")
+
         if tmp and delete_tmp:
             os.unlink(tmp.name)
     
     def load(self):
         if self._loaded:
             return self
         else:
             self.font.load(None)
             self._loaded = True
             return self
     
     def variations(self):
         axes = {}
-        if "fvar" in self.font.ttFont:
-            fvar = self.font.ttFont['fvar']
+        if self._variations:
+            fvar = self._variations
             for axis in fvar.axes:
                 axes[axis.axisTag] = (axis.__dict__)
         return axes
     
     @staticmethod
     def Cacheable(path, suffix=None, delete_tmp=False):
         if path not in FontCache:
@@ -330,29 +341,27 @@
             increments=dict(),
             varyFontSize=False,
             preventHwid=False,
             fitHeight=None,
             meta=dict(),
             no_shapes=False,
             show_frames=False,
-            _skiaback=False,
             load_font=True, # should we attempt to load the font?
             tag=None, # way to differentiate in __eq__
             _stst=False,
             **kwargs):
 
         self.input = locals()
         self.input["self"] = None
 
         if load_font:
             self.font = Font.Normalize(font)
         else:
             self.font = font
 
-        self._skiaback = _skiaback
         self.meta = meta
 
         self.fallback = fallback
         self.narrower = narrower
         self.layer = layer
         self.reverse = kwargs.get("r", reverse)
         self.removeOverlap = kwargs.get("ro", removeOverlap)
@@ -884,58 +893,14 @@
             self.features["hwid"] = True
             self.tracking = self.style.tracking # reset to widest
             self.resetGlyphRun()
             #self.glyphs = self.hb.glyphs(self.variations, self.features)
             adjusted = True
         self.resetGlyphRun()
         return adjusted
-
-    def _skia_scalePenToStyle(self, glyph, in_pen, idx):
-        s = self.scale()
-        tx, ty = 0, 0
-        try:
-            bs = self.style.baselineShift[idx]
-        except:
-            bs = self.style.baselineShift
-        
-        if callable(bs):
-            ty = bs(idx)
-        else:
-            try:
-                ty = bs[idx]
-            except:
-                try:
-                    ty = bs
-                except:
-                    pass
-        tx = glyph.frame.x#/self.scale()
-        ty = ty + glyph.frame.y#/self.scale()
-        out_pen = P()
-        skia_pen = SkiaPathPen(in_pen)
-        skia_pen.path.transform(Matrix.Scale(s, s))
-        skia_pen.path.transform(Matrix.Translate(tx, ty))
-        
-        # TODO how to parallel this?
-        #if self.style.mods and glyph.name in self.style.mods:
-        #    w, mod = self.style.mods[glyph.name]
-        #    mod(-1, ip)
-
-        out_pen = skia_pen.to_drawing()
-
-        if self.style.rotate:
-            out_pen.rotate(self.style.rotate)
-        
-        # # TODO this shouldn't be necessary
-        # if True:
-        #     valid_values = []
-        #     for (move, pts) in out_pen.value:
-        #         if move != "addComponent":
-        #             valid_values.append((move, pts))
-        #     out_pen.value = valid_values
-        return out_pen
     
     def scalePenToStyle(self, glyph, in_pen, idx):
         s = self.scale()
         t = Transform()
         try:
             bs = self.style.baselineShift[idx]
         except:
@@ -981,22 +946,93 @@
         #attrs = dict(fill=self.style.fill)
         #if self.style.stroke:
         #    attrs["stroke"] = dict(color=self.style.stroke, weight=self.style.strokeWidth)
         dp = P().f(self.style.fill)
         if self.style.stroke:
             dp.s(self.style.stroke).sw(self.style.strokeWidth)
         return dp
+    
+    def buildLayeredGlyph(self, output, layer, frame):
+        layerGlyph = P().record(layer)
+        output.append(layerGlyph)
+
+        if layer.method == "drawPathSolid":
+            layerGlyph.f(layer.data["color"])
+        else:
+            gradientGlyph = P()
+            if layer.method == "drawPathLinearGradient":
+                (gradientGlyph
+                    .line([layer.data["pt1"], layer.data["pt2"]])
+                    .fssw(-1, 0, 2).translate(frame.x, 0))
+            elif layer.method == "drawPathSweepGradient":
+                gradientGlyph.moveTo(layer.data["center"])
+            elif layer.method == "drawPathRadialGradient":
+                gradientGlyph.line([layer.data["startCenter"], layer.data["endCenter"]])
+            else:
+                print(">", layer.method)
+                gradientGlyph.rect(frame)
+            
+            (layerGlyph
+                .f(-1)
+                .attr(COLR=[layer.method, layer.data])
+                .data(substructure=gradientGlyph))
+    
+    def addBRGlyphDrawings(self, glyphs):
+        ax = 0
+        surface = BRPathCollectorSurface()
+
+        self.style.font._brFont.setLocation(self.variations)
+
+        with surface.canvas((0, 0, 1000, 1000)) as canvas:
+            for glyph in glyphs:
+                frame = Rect(
+                    ax + glyph.dx,
+                    glyph.dy,
+                    glyph.ax,
+                    self.style._asc) # how does ay play in?
+                
+                output = P().data(glyphName=glyph.name, frame=frame)
+
+                with canvas.savedState():
+                    canvas.translate(glyph.dx, glyph.dy)
+
+                    self.style.font._brFont.drawGlyph(glyph.name, canvas)
+
+                    layers = canvas.paths
+
+                    if isinstance(layers, BRPathCollectorRecordingPen):
+                        if layers.method == "drawPathSolid": # trad font
+                            output.record(layers).f(layers.data["color"])
+                            layers = None
+                        else:
+                            layers = [layers]
+                    
+                    if layers:
+                        for layer in layers:
+                            self.buildLayeredGlyph(output, layer, frame)
+                    
+                    canvas.paths = []
+
+                #canvas.translate(glyph.ax, glyph.ay)
+
+                glyph.glyphDrawing = output
+                #ax += glyph.ax
 
     def pens(self) -> P:
         """
         Vectorize text into a ``P``, such that each glyph (or ligature) is represented by a single `P` (or a ``P`` in the case of a color font, which will then nest a `P` for each layer of that color glyph)
         """
 
         self.resetGlyphRun()
-        if not self.style.no_shapes:
+
+        colrv1 = self.style.font._colrv1
+        if colrv1:
+            self.addBRGlyphDrawings(self.glyphs)
+
+        elif not self.style.no_shapes:
             self.style.font.font.addGlyphDrawings(self.glyphs, colorLayers=True)
         
         pens = P()
         for idx, g in enumerate(self.glyphs):
 
             # TODO this is sketchy but seems to correct
             # some line-spacing issues with arabic?
@@ -1012,19 +1048,16 @@
                 dp_atom.data(
                     frame=norm_frame,
                     glyphName=g.name
                 )
                 # dp_atom.typographic = True
                 # dp_atom.addFrame(norm_frame)
                 # dp_atom.glyphName = g.name
-            elif len(g.glyphDrawing.layers) == 1:
-                if self.style._skiaback:
-                    dp_atom.v.value = self._skia_scalePenToStyle(g, g.glyphDrawing.layers[0][0], idx).v.value
-                else:
-                    dp_atom.v.value = self.scalePenToStyle(g, g.glyphDrawing.layers[0][0], idx).v.value
+            elif not colrv1 and len(g.glyphDrawing.layers) == 1:
+                dp_atom.v.value = self.scalePenToStyle(g, g.glyphDrawing.layers[0][0], idx).v.value
                 
                 if "d" in self.style.metrics:
                     dp_atom.translate(0, self.style.descender*self.scale())
                 
                 dp_atom.data(
                     frame=norm_frame,
                     glyphName=g.name
@@ -1037,14 +1070,28 @@
                     else:
                         dp_atom.record(P().rect(g.frame).outline(1 if self.style.show_frames is True else self.style.show_frames))
                         #dp_atom.rect(g.frame)
                 if self.style.q2c:
                     dp_atom.q2c()
                 if self.style.removeOverlap:
                     dp_atom.removeOverlap()
+            elif colrv1:
+                dp_atom = g.glyphDrawing
+                dp_atom.layered = True
+
+                for idx, layer in enumerate(dp_atom):
+                    layer.v.value = self.scalePenToStyle(g, layer, idx).v.value
+
+                    ss = layer.data("substructure")
+                    ss.v.value = self.scalePenToStyle(g, ss, idx).v.value
+                
+                dp_atom.data(
+                   frame=norm_frame,
+                   glyphName=g.name
+                )
             else:
                 dp_atom = P()
                 dp_atom.layered = True
                 for lidx, layer in enumerate(g.glyphDrawing.layers):
                     dp_layer = self._emptyPenWithAttrs()
                     #dp_layer.value = layer[0].value
                     dp_layer.v.value = self.scalePenToStyle(g, layer[0], idx).v.value
@@ -1066,14 +1113,17 @@
                 # dp_atom.glyphName = g.name
             
             #dp_atom._parent = pens
             if self.style.meta:
                 dp_atom.data(**self.style.meta)
             
             pens.append(dp_atom)
+        
+        #if colrv1:
+        #    pens.scale(self.style.fontSize/1000, point=(0,0))
 
         if self.style.reverse:
             pens.reversePens()
         
         pens.data(**self.style.data)
 
         ro = pens
```

### Comparing `coldtype-0.9.8/coldtype/text/richtext.py` & `coldtype-0.9.9/coldtype/text/richtext.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/text/shaper.py` & `coldtype-0.9.9/coldtype/text/shaper.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/__init__.py` & `coldtype-0.9.9/coldtype/time/__init__.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/audio.py` & `coldtype-0.9.9/coldtype/time/audio.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/clip.py` & `coldtype-0.9.9/coldtype/time/clip.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/easing.py` & `coldtype-0.9.9/coldtype/time/easing.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/midi.py` & `coldtype-0.9.9/coldtype/time/midi.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/nle/ableton.py` & `coldtype-0.9.9/coldtype/time/nle/ableton.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/nle/ascii.py` & `coldtype-0.9.9/coldtype/time/nle/ascii.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/nle/premiere.py` & `coldtype-0.9.9/coldtype/time/nle/premiere.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/sequence.py` & `coldtype-0.9.9/coldtype/time/sequence.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/timeable.py` & `coldtype-0.9.9/coldtype/time/timeable.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/timeline.py` & `coldtype-0.9.9/coldtype/time/timeline.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/time/viewer.py` & `coldtype-0.9.9/coldtype/time/viewer.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype/tool.py` & `coldtype-0.9.9/coldtype/tool.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/coldtype.egg-info/PKG-INFO` & `coldtype-0.9.9/coldtype.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coldtype
-Version: 0.9.8
+Version: 0.9.9
 Summary: Functions for manual vectorized typesetting
 Home-page: https://github.com/goodhertz/coldtype
 Author: Rob Stenson / Goodhertz
 Author-email: rob@goodhertz.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `coldtype-0.9.8/coldtype.egg-info/SOURCES.txt` & `coldtype-0.9.9/coldtype.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,16 @@
 coldtype/runon/mixins/SerializationMixin.py
 coldtype/runon/mixins/StylingMixin.py
 coldtype/text/__init__.py
 coldtype/text/composer.py
 coldtype/text/reader.py
 coldtype/text/richtext.py
 coldtype/text/shaper.py
+coldtype/text/colr/brsurface.py
+coldtype/text/colr/skia.py
 coldtype/time/__init__.py
 coldtype/time/audio.py
 coldtype/time/clip.py
 coldtype/time/easing.py
 coldtype/time/midi.py
 coldtype/time/sequence.py
 coldtype/time/timeable.py
```

### Comparing `coldtype-0.9.8/setup.py` & `coldtype-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ### Programmatic display typography
 
 More info available at: [coldtype.goodhertz.com](https://coldtype.goodhertz.com)
 """
 
 setuptools.setup(
     name="coldtype",
-    version="0.9.8",
+    version="0.9.9",
     author="Rob Stenson / Goodhertz",
     author_email="rob@goodhertz.com",
     description="Functions for manual vectorized typesetting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/goodhertz/coldtype",
     #package_dir={"": "coldtype"},
@@ -31,14 +31,15 @@
         "coldtype.runon",
         "coldtype.physics",
         "coldtype.capture",
         "coldtype.blender",
         "coldtype.geometry",
         "coldtype.time.nle",
         "coldtype.renderer",
+        "coldtype.text.colr",
         "coldtype.renderable",
         "coldtype.fontgoggles",
         "coldtype.interpolation",
         "coldtype.runon.mixins",
         "coldtype.renderer.winman",
         "coldtype.fontgoggles.font",
         "coldtype.fontgoggles.misc",
@@ -102,20 +103,21 @@
         "audio": [
             "pyaudio",
             "soundfile",
         ]
     },
     install_requires=[
         "fonttools[ufo]",
+        "blackrenderer>=0.5.3",
         "fontPens",
         "easing-functions",
         "mido",
         "defcon",
         "freetype-py",
         "uharfbuzz>=0.14.0",
-        "python-bidi"
+        "python-bidi",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `coldtype-0.9.8/test/test_arrangement.py` & `coldtype-0.9.9/test/test_arrangement.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_drawbot_pens.py` & `coldtype-0.9.9/test/test_drawbot_pens.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_fx_xray.py` & `coldtype-0.9.9/test/test_fx_xray.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_geometry.py` & `coldtype-0.9.9/test/test_geometry.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_glyphwise.py` & `coldtype-0.9.9/test/test_glyphwise.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_i18n.py` & `coldtype-0.9.9/test/test_i18n.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_p.py` & `coldtype-0.9.9/test/test_p.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_pens.py` & `coldtype-0.9.9/test/test_pens.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_pens_rendered.py` & `coldtype-0.9.9/test/test_pens_rendered.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_reader.py` & `coldtype-0.9.9/test/test_reader.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_reportlabpen.py` & `coldtype-0.9.9/test/test_reportlabpen.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_richtext.py` & `coldtype-0.9.9/test/test_richtext.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_runon.py` & `coldtype-0.9.9/test/test_runon.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_syntax_mods.py` & `coldtype-0.9.9/test/test_syntax_mods.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_text.py` & `coldtype-0.9.9/test/test_text.py`

 * *Files identical despite different names*

### Comparing `coldtype-0.9.8/test/test_time.py` & `coldtype-0.9.9/test/test_time.py`

 * *Files identical despite different names*

