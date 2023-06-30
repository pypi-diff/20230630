# Comparing `tmp/enfugue-0.1.1.tar.gz` & `tmp/enfugue-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enfugue-0.1.1.tar", last modified: Wed Jun 28 02:15:53 2023, max compression
+gzip compressed data, was "enfugue-0.1.2.tar", last modified: Fri Jun 30 00:34:29 2023, max compression
```

## Comparing `enfugue-0.1.1.tar` & `enfugue-0.1.2.tar`

### file list

```diff
@@ -1,256 +1,257 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.859513 enfugue-0.1.1/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      177 2023-06-28 02:15:53.859513 enfugue-0.1.1/PKG-INFO
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.839649 enfugue-0.1.1/enfugue/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1815 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.839649 enfugue-0.1.1/enfugue/api/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      314 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2186 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/config.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/api/controller/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      690 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/controller/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1345 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/controller/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3531 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/controller/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9025 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/controller/invocation.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13671 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/controller/models.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11947 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/controller/system.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8447 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8617 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/invocations.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    19242 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/manager.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12448 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/api/server.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/config/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3002 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/config/cms-context.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       75 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/config/database.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       63 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/config/enfugue.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      118 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/config/logging.yml
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2561 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/config/server.yml
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/database/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      554 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/database/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      130 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/database/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      355 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/database/config.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      814 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/database/invocations.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1199 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/database/models.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/diffusion/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      782 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/constants.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/diffusion/edge/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/edge/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3971 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/edge/detect.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1348 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/edge/hed.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/diffusion/edge/mlsd/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      199 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/edge/mlsd/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9546 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/edge/mlsd/model.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    24714 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/edge/mlsd/util.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10170 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/engine.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    47311 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/manager.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    58197 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/pipeline.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    54711 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/plan.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13690 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/process.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/diffusion/rt/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12412 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/engine.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/diffusion/rt/model/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      465 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/model/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5684 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/model/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3110 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/model/clip.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13244 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/model/controlledunet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7791 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/model/controlnet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3770 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/model/unet.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2580 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/model/vae.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2671 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/optimizer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15776 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/rt/pipeline.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/diffusion/upscale/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3932 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/upscale/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6806 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/upscale/gfpganer.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10440 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/util.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      619 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/diffusion/vision.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      608 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/enfugue.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/interface/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12701 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/interface/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4429 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/interface/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/partner/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/partner/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4752 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/partner/civitai.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1763 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/server.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.839649 enfugue-0.1.1/enfugue/static/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.843622 enfugue-0.1.1/enfugue/static/css/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      773 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/01-reset.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      497 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/02-variables.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      279 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/03-fonts.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12992 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/04-base.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7808 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/05-common.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/06-header.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4241 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/07-main.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18052 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/08-enfugue.min.css
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18392 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/09-enfugue-nodes.min.css
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.839649 enfugue-0.1.1/enfugue/static/css/vendor/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/css/vendor/fa/
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    18620 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/vendor/fa/brands.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    80651 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/vendor/fa/fontawesome.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)      606 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/vendor/fa/regular.min.css
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)      598 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/css/vendor/fa/solid.min.css
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.839649 enfugue-0.1.1/enfugue/static/fonts/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.839649 enfugue-0.1.1/enfugue/static/fonts/vendor/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/fonts/vendor/fa/
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   186112 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   107460 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    62048 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)    25096 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   397728 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf
--rw-r--r--   0 benjamin  (1000) benjamin  (1000)   150472 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/html/
--rw-------   0 benjamin  (1000) benjamin  (1000)      165 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/html/body/
--rw-------   0 benjamin  (1000) benjamin  (1000)      187 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/body-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/html/body/content/
--rw-------   0 benjamin  (1000) benjamin  (1000)      379 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/content/content-admin.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      349 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/content/content-application.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      122 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/content/content-error.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      297 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/content/content-external.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      876 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/content/content-login.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      166 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/content/content-template.html.j2
--rw-------   0 benjamin  (1000) benjamin  (1000)      399 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/external-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/html/body/footer/
--rw-------   0 benjamin  (1000) benjamin  (1000)       55 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/footer/footer-base.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      759 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/footer/footer.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/html/body/header/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       55 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/header/header-base.html.j2
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      140 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/body/header/header.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/html/head/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2162 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/html/head/head-base.html.j2
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/img/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/img/brand/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      852 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/brand/civit-ai-logo.svg
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1293 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/brand/civit-ai.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1521 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/brand/ko-fi.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1486 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/brand/patreon.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9307 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/brand/tensorrt.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    63446 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/cloud-320.png
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/img/favicon/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13112 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/favicon/favicon-128x128.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2235 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/favicon/favicon-16x16.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    38833 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/favicon/favicon-256x256.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2827 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/favicon/favicon-32x32.png
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)   160675 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/favicon/favicon-512x512.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4987 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/favicon/favicon-64x64.png
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1150 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/img/favicon/favicon.ico
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/js/
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/js/application/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12906 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/application/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.851568 enfugue-0.1.1/enfugue/static/js/base/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3038 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/api.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16960 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/builder.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1114 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/csv.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9583 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/helpers.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      915 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/loader.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      350 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/mutex.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      549 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/publisher.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3019 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/session.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2396 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/base/watcher.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/common/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1814 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/common/event-tracker.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4554 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/common/history.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      441 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/common/notify.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      647 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/common/shadowbox.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2469 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/common/tooltip.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/config/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      706 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/config/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/controller/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      845 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/base.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/controller/common/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6200 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/common/announcements.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4531 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/common/downloads.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11935 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/common/invocation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4771 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/common/model-manager.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6527 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/common/model-picker.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/controller/file/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      242 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/file/01-new.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      513 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/file/02-open.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      645 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/file/03-save.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4132 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/file/04-history.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2764 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/file/05-results.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/controller/help/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2637 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/help/01-about.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      338 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/help/02-documentation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      337 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/help/03-discuss.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1298 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/index.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      393 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/menu.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/controller/models/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8688 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/models/01-civitait.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      276 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/models/02-manager.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      259 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/models/03-new.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/controller/sidebar/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3562 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/sidebar/01-canvas.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1671 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/sidebar/02-tweaks.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1323 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/sidebar/03-generation.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11037 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/sidebar/04-upscale.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      900 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/sidebar/05-prompts.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2616 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/sidebar/99-invoke.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/controller/system/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3258 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/system/01-settings.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4587 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/system/02-users.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6733 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/system/03-installation.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/controller/toolbar/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      470 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/toolbar/01-load-image.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/toolbar/02-draw-scribble.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      263 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/controller/toolbar/03-region-prompt.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      670 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/enfugue.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/graphics/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      567 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/graphics/colors.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4622 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/graphics/geometry.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1869 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/graphics/paths.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2942 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/graphics/spline.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/lang/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      203 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/lang/en.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      256 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/lang/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/model/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1009 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/model/enfugue.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5772 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/model/index.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/view/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3767 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/base.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.855540 enfugue-0.1.1/enfugue/static/js/view/forms/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7044 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1456 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/classic.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      502 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/confirm.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.859513 enfugue-0.1.1/enfugue/static/js/view/forms/input/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3301 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      472 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/bool.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5969 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/color.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11312 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/enumerable.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      611 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/file.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      450 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/misc.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2928 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/numeric.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3845 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/parent.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      724 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input/string.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1017 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/forms/input.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9227 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/image.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3631 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/menu.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.859513 enfugue-0.1.1/enfugue/static/js/view/nodes/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12845 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/nodes/base.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3427 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/nodes/decorations.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9870 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/nodes/editor.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    22154 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/nodes/image-editor.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3459 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/nodes/windows.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1512 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/notifications.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4415 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/scribble.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3295 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/status.mjs
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10912 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/static/js/view/table.mjs
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.859513 enfugue-0.1.1/enfugue/util/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      275 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1704 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/downloads.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/gpu.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3975 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/gputil.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5992 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/images.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4280 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/installation.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       76 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/log.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8149 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/security.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1203 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/signature.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1768 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue/util/tokens.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-28 02:15:53.839649 enfugue-0.1.1/enfugue.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      177 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7719 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       50 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      985 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        8 2023-06-28 02:15:53.000000 enfugue-0.1.1/enfugue.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-06-28 02:15:53.859513 enfugue-0.1.1/setup.cfg
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2495 2023-06-28 02:15:53.000000 enfugue-0.1.1/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.955503 enfugue-0.1.2/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      177 2023-06-30 00:34:29.955503 enfugue-0.1.2/PKG-INFO
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3774 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/api/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      314 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2186 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/config.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/api/controller/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      690 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1345 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3638 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/downloads.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9025 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/invocation.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13819 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/models.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    17819 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/controller/system.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8447 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/downloads.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8617 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/invocations.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    19203 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/manager.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13327 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/api/server.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/config/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3002 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/cms-context.yml
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       75 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/database.yml
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      170 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/enfugue.yml
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      119 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/logging.yml
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2312 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/config/server.yml
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/database/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      554 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      130 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      355 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/config.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      814 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/invocations.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1199 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/database/models.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      782 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/constants.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/edge/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3971 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/detect.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1348 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/hed.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/edge/mlsd/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      199 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/mlsd/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9546 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/mlsd/model.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    24714 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/edge/mlsd/util.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10752 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/engine.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    48134 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/manager.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    66164 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/pipeline.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    54605 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/plan.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    14172 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/process.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/rt/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12412 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/engine.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/rt/model/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      465 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5684 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3110 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/clip.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13244 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/controlledunet.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7791 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/controlnet.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3770 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/unet.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2580 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/model/vae.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2671 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/optimizer.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    15776 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/rt/pipeline.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/diffusion/upscale/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3932 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/upscale/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6806 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/upscale/gfpganer.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10440 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/util.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      619 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/diffusion/vision.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      608 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/enfugue.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/interface/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12980 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/interface/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4429 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/interface/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/partner/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/partner/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4752 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/partner/civitai.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1925 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/server.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue/static/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/static/css/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      773 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/01-reset.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      497 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/02-variables.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      279 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/03-fonts.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12992 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/04-base.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7808 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/05-common.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/06-header.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4241 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/07-main.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18052 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/08-enfugue.min.css
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    18689 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/09-enfugue-nodes.min.css
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.935504 enfugue-0.1.2/enfugue/static/css/vendor/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.943504 enfugue-0.1.2/enfugue/static/css/vendor/fa/
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)    18620 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/vendor/fa/brands.min.css
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)    80651 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/vendor/fa/fontawesome.min.css
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)      606 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/vendor/fa/regular.min.css
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)      598 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/css/vendor/fa/solid.min.css
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.935504 enfugue-0.1.2/enfugue/static/fonts/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.935504 enfugue-0.1.2/enfugue/static/fonts/vendor/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)   186112 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)   107460 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)    62048 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)    25096 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)   397728 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf
+-rw-r--r--   0 benjamin  (1000) benjamin  (1000)   150472 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      165 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/base.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/body/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      187 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/body-base.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/body/content/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      379 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-admin.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      349 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-application.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      122 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-error.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      297 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-external.html.j2
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      876 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-login.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      166 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/content/content-template.html.j2
+-rw-------   0 benjamin  (1000) benjamin  (1000)      399 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/external-base.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/body/footer/
+-rw-------   0 benjamin  (1000) benjamin  (1000)       55 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/footer/footer-base.html.j2
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      759 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/footer/footer.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/body/header/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       55 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/header/header-base.html.j2
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      140 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/body/header/header.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/html/head/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2162 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/html/head/head-base.html.j2
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/img/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/img/brand/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      852 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/civit-ai-logo.svg
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1293 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/civit-ai.png
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1521 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/ko-fi.png
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)     1486 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/patreon.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9307 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/brand/tensorrt.png
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    63446 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/cloud-320.png
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/img/favicon/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    13112 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-128x128.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2235 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-16x16.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    38833 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-256x256.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2827 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-32x32.png
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)   160675 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-512x512.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4987 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon-64x64.png
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1150 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/img/favicon/favicon.ico
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/application/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12929 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/application/index.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/base/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3038 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/api.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16960 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/builder.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1114 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/csv.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9583 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/helpers.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      915 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/loader.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      350 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/mutex.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      549 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/publisher.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3019 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/session.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2396 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/base/watcher.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/common/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1814 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/event-tracker.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4554 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/history.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      441 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/notify.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      647 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/shadowbox.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2469 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/common/tooltip.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/config/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      706 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/config/index.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.947503 enfugue-0.1.2/enfugue/static/js/controller/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      845 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/base.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/common/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7149 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/announcements.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4531 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/downloads.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11935 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/invocation.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4771 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/model-manager.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6969 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/common/model-picker.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/file/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      242 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/01-new.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      513 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/02-open.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      645 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/03-save.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4132 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/04-history.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2764 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/file/05-results.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/help/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2637 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/help/01-about.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      338 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/help/02-documentation.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      337 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/help/03-discuss.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1298 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/index.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      393 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/menu.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/models/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8688 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/models/01-civitait.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      276 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/models/02-manager.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      259 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/models/03-new.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/sidebar/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3562 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/01-canvas.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1671 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/02-tweaks.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1323 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/03-generation.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11037 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/04-upscale.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      900 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/05-prompts.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2616 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/sidebar/99-invoke.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/system/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3258 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/system/01-settings.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4587 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/system/02-users.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7985 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/system/03-installation.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2601 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/system/04-logs.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/controller/toolbar/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      470 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/toolbar/01-load-image.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      317 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/toolbar/02-draw-scribble.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      263 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/controller/toolbar/03-region-prompt.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      670 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/enfugue.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/graphics/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      567 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/graphics/colors.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4622 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/graphics/geometry.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1869 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/graphics/paths.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2942 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/graphics/spline.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/lang/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      203 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/lang/en.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      256 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/lang/index.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/model/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1009 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/model/enfugue.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5772 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/model/index.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/view/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3767 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/base.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.951503 enfugue-0.1.2/enfugue/static/js/view/forms/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7044 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/base.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1456 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/classic.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      502 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/confirm.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.955503 enfugue-0.1.2/enfugue/static/js/view/forms/input/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3301 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/base.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      472 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/bool.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5969 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/color.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    11312 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/enumerable.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      611 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/file.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      450 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/misc.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2928 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/numeric.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3845 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/parent.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      724 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input/string.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1017 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/forms/input.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9227 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/image.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3631 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/menu.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.955503 enfugue-0.1.2/enfugue/static/js/view/nodes/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    12845 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/base.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3427 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/decorations.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     9870 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/editor.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    22154 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/image-editor.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3459 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/nodes/windows.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1512 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/notifications.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4415 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/scribble.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3295 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/status.mjs
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10912 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/static/js/view/table.mjs
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.955503 enfugue-0.1.2/enfugue/util/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      275 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1802 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/downloads.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      989 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/gpu.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     3975 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/gputil.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5992 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/images.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     4280 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/installation.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       76 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/log.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     8149 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/security.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1203 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/signature.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1768 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue/util/tokens.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-30 00:34:29.939504 enfugue-0.1.2/enfugue.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      177 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7767 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       50 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1008 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        8 2023-06-30 00:34:29.000000 enfugue-0.1.2/enfugue.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-06-30 00:34:29.955503 enfugue-0.1.2/setup.cfg
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2533 2023-06-30 00:34:29.000000 enfugue-0.1.2/setup.py
```

### Comparing `enfugue-0.1.1/enfugue/api/config.py` & `enfugue-0.1.2/enfugue/api/config.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/api/controller/__init__.py` & `enfugue-0.1.2/enfugue/api/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/api/controller/base.py` & `enfugue-0.1.2/enfugue/api/controller/base.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/api/controller/downloads.py` & `enfugue-0.1.2/enfugue/api/controller/downloads.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,25 @@
     @handlers.format()
     @handlers.secured("Download", "create")
     def start_download(self, request: Request, response: Response) -> Dict[str, Any]:
         """
         Starts a download.
         """
         try:
-            target_dir = os.path.join(self.engine_root, str(request.parsed["type"]))
+            download_type = str(request.parsed["type"])
+            target_dir = self.configuration.get(
+                f"enfugue.engine.{download_type}", os.path.join(self.engine_root, download_type)
+            )
             target_file = os.path.join(target_dir, request.parsed["filename"])
 
             if os.path.exists(target_file) and not request.parsed.get("overwrite", False):
                 raise StateConflictError(f"File exists: {request.parsed['filename']}")
-            
+
             check_make_directory(target_dir)
-            
+
             return self.manager.download(
                 request.token.user.id, request.parsed["url"], target_file
             ).format()
         except KeyError as ex:
             raise BadRequestError(f"Missing required argument {ex}")
 
     @handlers.path("^/api/download$")
```

### Comparing `enfugue-0.1.1/enfugue/api/controller/invocation.py` & `enfugue-0.1.2/enfugue/api/controller/invocation.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/api/controller/models.py` & `enfugue-0.1.2/enfugue/api/controller/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,63 +27,67 @@
     @handlers.format()
     @handlers.secured()
     def get_checkpoints(self, request: Request, response: Response) -> List[str]:
         """
         Gets installed checkpoints.
         """
         checkpoints = []
-        checkpoints_dir = os.path.join(self.engine_root, "checkpoint")
+        checkpoints_dir = self.configuration.get(
+            "enfugue.engine.checkpoint", os.path.join(self.engine_root, "checkpoint")
+        )
         if os.path.exists(checkpoints_dir):
             checkpoints = os.listdir(checkpoints_dir)
         return checkpoints
 
     @handlers.path("^/api/lora$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured()
     def get_lora(self, request: Request, response: Response) -> List[str]:
         """
         Gets installed lora.
         """
         lora = []
-        lora_dir = os.path.join(self.engine_root, "lora")
+        lora_dir = self.configuration.get(
+            "enfugue.engine.lora", os.path.join(self.engine_root, "lora")
+        )
         if os.path.exists(lora_dir):
             lora = os.listdir(lora_dir)
         return lora
 
     @handlers.path("^/api/inversions$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured()
     def get_inversions(self, request: Request, response: Response) -> List[str]:
         """
         Gets installed textual inversions.
         """
         inversions = []
-        inversions_dir = os.path.join(self.engine_root, "inversion")
+        inversions_dir = self.configuration.get(
+            "enfugue.engine.inversion", os.path.join(self.engine_root, "inversion")
+        )
         if os.path.exists(inversions_dir):
             inversions = os.listdir(inversions_dir)
         return inversions
 
     @handlers.path("^/api/tensorrt$")
     @handlers.methods("GET")
     @handlers.format()
     @handlers.secured("DiffusionModel", "read")
     def get_tensorrt_engines(self, request: Request, response: Response) -> List[Dict[str, Any]]:
         """
         Finds engines in the model directory and determines their metadata and status.
         """
         engines = []
-        for engine in glob.glob(f"{self.engine_root}/**/engine.plan", recursive=True):
+        for engine in glob.glob(f"{self.engine_root}/tensorrt/**/engine.plan", recursive=True):
             engine_dir = os.path.abspath(os.path.dirname(engine))
             engine_type = os.path.basename(os.path.dirname(engine_dir))
             engine_key = os.path.basename(os.path.dirname(engine))
-            engine_model = os.path.basename(
-                os.path.dirname(os.path.dirname(os.path.dirname(engine_dir)))
-            )
+            engine_model = os.path.basename(os.path.dirname(os.path.dirname(engine_dir)))
             engine_model_name = engine_model
             engine_metadata_path = os.path.join(engine_dir, "metadata.json")
             engine_used = False
             engine_used_by = []
             engine_lora = []
             engine_inversion = []
             engine_metadata = {}
@@ -168,17 +172,15 @@
         model_name: str,
         engine_type: str,
         engine_key: str,
     ) -> None:
         """
         Removes an individual tensorrt engine.
         """
-        engine_dir = os.path.join(
-            self.engine_root, "models", model_name, "tensorrt", engine_type, engine_key
-        )
+        engine_dir = os.path.join(self.engine_root, "tensorrt", model_name, engine_type, engine_key)
         if not os.path.exists(engine_dir):
             raise NotFoundError(
                 f"Couldn't find {engine_type} TensorRT engine for {model_name} with key {engine_key}"
             )
         shutil.rmtree(engine_dir)
 
     @handlers.path("^/api/models/(?P<model_name>[^\/]+)/tensorrt$")
```

### Comparing `enfugue-0.1.1/enfugue/api/downloads.py` & `enfugue-0.1.2/enfugue/api/downloads.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/api/invocations.py` & `enfugue-0.1.2/enfugue/api/invocations.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/api/manager.py` & `enfugue-0.1.2/enfugue/api/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,28 +145,32 @@
         Gets the location for image intermediate outputs.
         """
         directory = os.path.join(self.engine_root_dir, "intermediates")
         check_make_directory(directory)
         return directory
 
     @property
-    def engine_models_dir(self) -> str:
+    def engine_tensorrt_dir(self) -> str:
         """
-        Gets the location for models.
+        Gets the location for tensorrt engines.
         """
-        directory = os.path.join(self.engine_root_dir, "models")
+        directory = self.configuration.get(
+            "enfugue.engine.tensorrt", os.path.join(self.engine_root_dir, "tensorrt")
+        )
         check_make_directory(directory)
         return directory
 
     @property
     def engine_checkpoint_dir(self) -> str:
         """
         Returns the engine checkpoint location.
         """
-        path = os.path.join(self.engine_root_dir, "checkpoint")
+        path = self.configuration.get(
+            "enfugue.engine.checkpoint", os.path.join(self.engine_root_dir, "checkpoint")
+        )
         check_make_directory(path)
         return path
 
     @property
     def default_model_ckpt(self) -> str:
         """
         Returns the location where the default model should be.
@@ -450,53 +454,51 @@
             logger.info(f"Reclaimed {human_size(reclaimed_bytes)} from intermediates")
 
     def clean_models(self) -> None:
         """
         Cleans up models, engines, etc.
         """
         reclaimed_bytes = 0
-        for model_name in os.listdir(self.engine_models_dir):
-            model_path = os.path.join(self.engine_models_dir, model_name)
-            model_tensorrt_dir = os.path.join(model_path, "tensorrt")
-            if os.path.exists(model_tensorrt_dir):
-                for stage in ["clip", "unet", "vae"]:
-                    model_tensorrt_stage_dir = os.path.join(model_tensorrt_dir, stage)
-                    if os.path.exists(model_tensorrt_stage_dir):
-                        for stage_key in os.listdir(model_tensorrt_stage_dir):
-                            stage_dir = os.path.join(model_tensorrt_stage_dir, stage_key)
-                            stage_files = os.listdir(stage_dir)
-                            to_remove = []
-
-                            for file_name in stage_files:
-                                file_path = os.path.join(stage_dir, file_name)
-                                if file_name == "model.opt.onnx":
-                                    if "engine.plan" in stage_files:
-                                        to_remove.append(file_path)
-                                elif file_name == "model.onnx":
-                                    if "model.opt.onnx" in stage_files:
-                                        to_remove.append(file_path)
-                                elif file_name == "timing_cache":
-                                    file_mod_time = datetime.datetime.fromtimestamp(
-                                        os.path.getmtime(file_path)
-                                    )
-                                    file_age = (
-                                        datetime.datetime.now() - file_mod_time
-                                    ).total_seconds()
-                                    if (
-                                        file_age > self.max_timing_cache_age
-                                        or "engine.plan" in stage_files
-                                    ):
-                                        to_remove.append(file_path)
-                                elif file_name != "engine.plan" and file_name != "metadata.json":
+        for model_name in os.listdir(self.engine_tensorrt_dir):
+            model_path = os.path.join(self.engine_tensorrt_dir, model_name)
+            for stage in ["clip", "unet", "vae", "controlledunet", "controlnet"]:
+                model_tensorrt_stage_dir = os.path.join(model_path, stage)
+                if os.path.exists(model_tensorrt_stage_dir):
+                    for stage_key in os.listdir(model_tensorrt_stage_dir):
+                        stage_dir = os.path.join(model_tensorrt_stage_dir, stage_key)
+                        if not os.path.isdir(stage_dir):
+                            continue
+                        stage_files = os.listdir(stage_dir)
+                        to_remove = []
+
+                        for file_name in stage_files:
+                            file_path = os.path.join(stage_dir, file_name)
+                            if file_name == "model.opt.onnx":
+                                if "engine.plan" in stage_files:
+                                    to_remove.append(file_path)
+                            elif file_name == "model.onnx":
+                                if "model.opt.onnx" in stage_files:
+                                    to_remove.append(file_path)
+                            elif file_name == "timing_cache":
+                                file_mod_time = datetime.datetime.fromtimestamp(
+                                    os.path.getmtime(file_path)
+                                )
+                                file_age = (datetime.datetime.now() - file_mod_time).total_seconds()
+                                if (
+                                    file_age > self.max_timing_cache_age
+                                    or "engine.plan" in stage_files
+                                ):
                                     to_remove.append(file_path)
+                            elif file_name != "engine.plan" and file_name != "metadata.json":
+                                to_remove.append(file_path)
 
-                            for file_path in to_remove:
-                                logger.info(f"Removing unneeded engine file {file_path}")
-                                reclaimed_bytes += os.path.getsize(file_path)
-                                os.remove(file_path)
+                        for file_path in to_remove:
+                            logger.info(f"Removing unneeded engine file {file_path}")
+                            reclaimed_bytes += os.path.getsize(file_path)
+                            os.remove(file_path)
         if reclaimed_bytes > 0:
             logger.info(f"Reclaimed {human_size(reclaimed_bytes)} from models")
 
     def do_periodic_tasks(self) -> None:
         """
         Looks at the queues and starts actions if necessary.
         """
```

### Comparing `enfugue-0.1.1/enfugue/api/server.py` & `enfugue-0.1.2/enfugue/api/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,22 +169,42 @@
             self.database.query(self.orm.DiffusionModel)
             .filter(self.orm.DiffusionModel.name == model_name)
             .one_or_none()
         )
         if not diffusion_model:
             raise NotFoundError(f"Unknown diffusion model {model_name}")
 
-        model = os.path.join(self.manager.engine_root_dir, "checkpoint", diffusion_model.model)
+        model = os.path.join(
+            self.configuration.get(
+                "enfugue.engine.checkpoint",
+                os.path.join(self.manager.engine_root_dir, "checkpoint"),
+            ),
+            diffusion_model.model,
+        )
         size = diffusion_model.size
         lora = [
-            (os.path.join(self.manager.engine_root_dir, "lora", lora.model), float(lora.weight))
+            (
+                os.path.join(
+                    self.configuration.get(
+                        "enfugue.engine.lora", os.path.join(self.manager.engine_root_dir, "lora")
+                    ),
+                    lora.model,
+                ),
+                float(lora.weight),
+            )
             for lora in diffusion_model.lora
         ]
         inversion = [
-            os.path.join(self.manager.engine_root_dir, "inversion", inversion.model)
+            os.path.join(
+                self.configuration.get(
+                    "enfugue.engine.inversion",
+                    os.path.join(self.manager.engine_root_dir, "inversion"),
+                ),
+                inversion.model,
+            )
             for inversion in diffusion_model.inversion
         ]
         model_prompt = diffusion_model.prompt
         model_negative_prompt = diffusion_model.negative_prompt
 
         plan_kwargs: Dict[str, Any] = {
             "model": model,
@@ -269,32 +289,41 @@
         """
         announcements = []
 
         snooze_time = self.user_config.get("enfugue.snooze", None)
         snooze_duration = float("inf")
         if snooze_time is not None:
             snooze_duration = (datetime.datetime.now() - snooze_time).total_seconds()
+
         is_snoozed = snooze_duration < (60 * 60 * 24)
+
         if not is_snoozed:
             is_initialized = self.user_config.get("enfugue.initialized", False)
             if not is_initialized:
-                announcements.append({"type": "initialize"})
+                directories = {}
+                for dirname in ["cache", "checkpoint", "lora", "inversion", "other", "tensorrt"]:
+                    directories[dirname] = self.configuration.get(
+                        f"enfugue.engine.{dirname}", os.path.join(self.engine_root, dirname)
+                    )
+
+                announcements.append({"type": "initialize", "directories": directories})
 
             pending_downloads = self.manager.pending_default_downloads
             for url, dest in pending_downloads:
                 model = os.path.basename(url)
                 announcements.append(
                     {
                         "type": "download",
                         "url": url,
                         "size": requests.head(url, allow_redirects=True).headers["Content-Length"],
                         "model": model,
                         "destination": dest,
                     }
                 )
+
             pending_versions = get_pending_versions()
             for version in pending_versions:
                 announcements.append(
                     {
                         "type": "update",
                         "version": version["version"],
                         "release": version["release"].strftime("%Y-%m-%d"),
```

### Comparing `enfugue-0.1.1/enfugue/config/cms-context.yml` & `enfugue-0.1.2/enfugue/config/cms-context.yml`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/config/server.yml` & `enfugue-0.1.2/enfugue/config/server.yml`

 * *Files 16% similar despite different names*

```diff
@@ -60,27 +60,20 @@
                 - admin
     server:
         secure: true
         host: 0.0.0.0
         port: 45554
         domain: app.enfugue.ai
         driver: cherrypy
-        origin:
-            allow_missing: true
-            allowlist:
-                - 127.0.0.1
-                - app.enfugue.ai
-                - localhost
         allowlist:
             - 127.0.0.0/24
             - 192.168.0.0/16
         classes:
             - enfugue.server.EnfugueServer
             - pibble.api.middleware.webservice.screening.ScreeningWebServiceAPIMiddleware
-            - pibble.api.middleware.webservice.origin.CrossOriginWebServiceAPIMiddleware
         template:
             recurse: true
         cms:
             name: Enfugue
             path:
                 root: https://app.enfugue.ai:45554/
                 static: https://app.enfugue.ai:45554/static/
```

### Comparing `enfugue-0.1.1/enfugue/database/__init__.py` & `enfugue-0.1.2/enfugue/database/__init__.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/database/invocations.py` & `enfugue-0.1.2/enfugue/database/invocations.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/database/models.py` & `enfugue-0.1.2/enfugue/database/models.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/constants.py` & `enfugue-0.1.2/enfugue/diffusion/constants.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/edge/detect.py` & `enfugue-0.1.2/enfugue/diffusion/edge/detect.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/edge/hed.py` & `enfugue-0.1.2/enfugue/diffusion/edge/hed.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/edge/mlsd/model.py` & `enfugue-0.1.2/enfugue/diffusion/edge/mlsd/model.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/edge/mlsd/util.py` & `enfugue-0.1.2/enfugue/diffusion/edge/mlsd/util.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/engine.py` & `enfugue-0.1.2/enfugue/diffusion/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -297,7 +297,27 @@
         return id
 
     def __call__(self, timeout: Optional[Union[int, float]] = None, **kwargs: Any) -> Any:
         """
         Issues a single invocation request using kwarg syntax.
         """
         return self.wait(self.dispatch("invoke", kwargs), timeout)
+
+    @staticmethod
+    def debug() -> DiffusionEngine:
+        """
+        Gets a DiffusionEngine instance with debug logging enabled.
+        """
+        return DiffusionEngine(
+            APIConfiguration(
+                enfugue={
+                    "engine": {
+                        "logging": {
+                            "level": "DEBUG",
+                            "handler": "stream",
+                            "stream": "stdout",
+                            "colored": True,
+                        }
+                    }
+                }
+            )
+        )
```

### Comparing `enfugue-0.1.1/enfugue/diffusion/manager.py` & `enfugue-0.1.2/enfugue/diffusion/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,32 +3,20 @@
 import os
 import time
 import torch
 import random
 import datetime
 import threading
 
-from typing import (
-    Type,
-    Union,
-    Any,
-    Optional,
-    List,
-    Tuple,
-    Dict,
-    Literal,
-    Callable,
-    TYPE_CHECKING,
-    cast,
-)
+from typing import Type, Union, Any, Optional, List, Tuple, Dict, Literal, Callable, TYPE_CHECKING
 from hashlib import md5
 
 from pibble.api.configuration import APIConfiguration
 from pibble.api.exceptions import ConfigurationError
-from pibble.util.files import load_json, dump_json
+from pibble.util.files import dump_json
 
 from enfugue.util import logger, check_download, check_make_directory
 from enfugue.diffusion.constants import (
     DEFAULT_MODEL,
     DEFAULT_INPAINTING_MODEL,
     CONTROLNET_CANNY,
     CONTROLNET_MLSD,
@@ -265,91 +253,99 @@
         self._chunking_blur = new_chunking_blur
 
     @property
     def engine_root(self) -> str:
         """
         Gets the root of the engine.
         """
-        root = self.configuration.get("enfugue.engine.root", "~/.cache/enfugue")
-        if root.startswith("~"):
-            root = os.path.expanduser(root)
-        root = os.path.realpath(root)
-        check_make_directory(root)
-        return root
+        path = self.configuration.get("enfugue.engine.root", "~/.cache/enfugue")
+        if path.startswith("~"):
+            path = os.path.expanduser(path)
+        path = os.path.realpath(path)
+        check_make_directory(path)
+        return path
 
     @property
-    def diffusers_cache_dir(self) -> str:
+    def engine_cache_dir(self) -> str:
         """
         Gets the cache for diffusers-downloaded configuration files, base models, etc.
         """
-        path = os.path.join(self.engine_root, "cache")
+        path = self.configuration.get("enfugue.engine.cache", "~/.cache/enfugue/cache")
+        if path.startswith("~"):
+            path = os.path.expanduser(path)
+        path = os.path.realpath(path)
         check_make_directory(path)
         return path
 
     @property
     def engine_checkpoints_dir(self) -> str:
         """
         Gets where checkpoints are downloaded in.
         """
-        path = os.path.join(self.engine_root, "checkpoint")
+        path = self.configuration.get("enfugue.engine.checkpoint", "~/.cache/enfugue/checkpoint")
+        if path.startswith("~"):
+            path = os.path.expanduser(path)
+        path = os.path.realpath(path)
         check_make_directory(path)
         return path
 
     @property
     def engine_other_dir(self) -> str:
         """
         Gets where any other weights are download in
         """
-        path = os.path.join(self.engine_root, "other")
+        path = self.configuration.get("enfugue.engine.other", "~/.cache/enfugue/other")
+        if path.startswith("~"):
+            path = os.path.expanduser(path)
+        path = os.path.realpath(path)
         check_make_directory(path)
         return path
 
     @property
     def engine_lora_dir(self) -> str:
         """
         Gets where lora are downloaded in.
         """
-        path = os.path.join(self.engine_root, "lora")
-        check_make_directory(path)
-        return path
-
-    @property
-    def engine_inversions_dir(self) -> str:
-        """
-        Gets where inversions are downloaded in.
-        """
-        path = os.path.join(self.engine_root, "inversions")
+        path = self.configuration.get("enfugue.engine.lora", "~/.cache/enfugue/lora")
+        if path.startswith("~"):
+            path = os.path.expanduser(path)
+        path = os.path.realpath(path)
         check_make_directory(path)
         return path
 
     @property
-    def engine_models_dir(self) -> str:
+    def engine_inversion_dir(self) -> str:
         """
-        Gets where models are pushed to after converting to diffusers.
+        Gets where inversion are downloaded to.
         """
-        path = os.path.join(self.engine_root, "models")
+        path = self.configuration.get("enfugue.engine.inversion", "~/.cache/enfugue/inversion")
+        if path.startswith("~"):
+            path = os.path.expanduser(path)
+        path = os.path.realpath(path)
         check_make_directory(path)
         return path
 
     @property
-    def model_dir(self) -> str:
+    def engine_tensorrt_dir(self) -> str:
         """
-        Gets where the current model should be stored.
+        Gets where TensorRT engines are downloaded to.
         """
-        model = self.model
-        path = os.path.join(self.engine_models_dir, self.model)
+        path = self.configuration.get("enfugue.engine.tensorrt", "~/.cache/enfugue/tensorrt")
+        if path.startswith("~"):
+            path = os.path.expanduser(path)
+        path = os.path.realpath(path)
         check_make_directory(path)
         return path
 
     @property
     def model_tensorrt_dir(self) -> str:
         """
         Gets where tensorrt engines will be built per model.
         """
-        path = os.path.join(self.model_dir, "tensorrt")
+        path = os.path.join(self.engine_tensorrt_dir, self.model_name)
         check_make_directory(path)
         return path
 
     @staticmethod
     def get_tensorrt_clip_key(
         size: int, lora: List[Tuple[str, float]], inversion: List[str], **kwargs: Any
     ) -> str:
@@ -594,15 +590,15 @@
         return self._tensorrt_enabled
 
     @tensorrt_is_enabled.setter
     def tensorrt_is_enabled(self, new_enabled: bool) -> None:
         """
         Disables or enables TensorRT.
         """
-        if new_enabled != self.tensorrt_is_enabled:
+        if new_enabled != self.tensorrt_is_enabled and self.tensorrt_is_ready:
             del self.pipeline
         self._tensorrt_enabled = new_enabled
 
     @property
     def tensorrt_is_ready(self) -> bool:
         """
         Checks to determine if Tensor RT is ready based on the existence of engines.
@@ -680,32 +676,39 @@
     @property
     def model(self) -> str:
         """
         Gets the configured model.
         """
         if not hasattr(self, "_model"):
             self._model = self.configuration.get("enfugue.model", DEFAULT_MODEL)
-            if self._model.endswith(".ckpt") or self._model.endswith(".safetensors"):
-                self._model = self.check_convert_checkpoint(self._model)
+            if self._model.startswith("http"):
+                self._model = self.check_download_checkpoint(self._model)
         return self._model
 
     @model.setter
     def model(self, new_model: Optional[str]) -> None:
         """
         Sets a new model. Destroys the pipeline.
         """
         if new_model is None:
             new_model = self.configuration.get("enfugue.model", DEFAULT_MODEL)
-        if new_model.endswith(".ckpt") or new_model.endswith(".safetensors"):
-            new_model = self.check_convert_checkpoint(new_model)
+        if new_model.startswith("http"):
+            new_model = self.check_download_checkpoint(new_model)
         if self.model != new_model:
             del self.pipeline
         self._model = new_model
 
     @property
+    def model_name(self) -> str:
+        """
+        Gets just the basename of the model
+        """
+        return os.path.splitext(os.path.basename(self.model))[0]
+
+    @property
     def dtype(self) -> torch.dtype:
         if not hasattr(self, "_torch_dtype"):
             if self.device == "cpu":
                 logger.debug("Inferencing on CPU, using BFloat")
                 self._torch_dtype = torch.float
             else:
                 configuration_dtype = self.configuration.get("enfugue.dtype", "float16")
@@ -785,22 +788,22 @@
         Gets the basenames of any LoRA present.
         """
         return [(os.path.splitext(os.path.basename(lora))[0], weight) for lora, weight in self.lora]
 
     @property
     def inversion(self) -> List[str]:
         """
-        Get textual inversions added to the text encoder.
+        Get textual inversion added to the text encoder.
         """
         return getattr(self, "_inversion", [])
 
     @inversion.setter
     def inversion(self, new_inversion: Optional[Union[str, List[str]]]) -> None:
         """
-        Sets new textual inversions. Destroys the pipeline.
+        Sets new textual inversion. Destroys the pipeline.
         """
         if new_inversion is None:
             if hasattr(self, "_inversion") and len(self._inversion) > 0:
                 del self.pipeline
             self._inversion: List[str] = []
             return
 
@@ -829,62 +832,32 @@
             return ckpt_path
         elif os.path.exists(safetensor_path):
             return safetensor_path
         else:
             raise IOError(f"Unknown model {self.model}")
 
     @property
-    def vae_config(self) -> Dict:
-        """
-        Reads the VAE config.json file.
-        """
-        path = os.path.join(self.model_dir, "vae", "config.json")
-        if not os.path.exists(path):
-            raise OSError(f"Couldn't find VAE config file at {path}")
-        return cast(Dict, load_json(path))
-
-    @property
-    def unet_config(self) -> Dict:
-        """
-        Reads the unet config.json file.
-        """
-        path = os.path.join(self.model_dir, "unet", "config.json")
-        if not os.path.exists(path):
-            raise OSError(f"Couldn't find unet config file at {path}")
-        return cast(Dict, load_json(path))
-
-    @property
-    def clip_config(self) -> Dict:
-        """
-        Reads the clip config.json file.
-        """
-        path = os.path.join(self.model_dir, "text_encoder", "config.json")
-        if not os.path.exists(path):
-            raise OSError(f"Couldn't find clip config file at {path}")
-        return cast(Dict, load_json(path))
-
-    @property
     def inpainting(self) -> bool:
         """
         Returns true if the model is an inpainting model.
         """
-        return self.unet_config["in_channels"] == 9
+        return "inpaint" in self.model
 
     @inpainting.setter
     def inpainting(self, new_inpainting: bool) -> None:
         """
         Sets whether or not we are inpainting.
 
         We trade efficiency for ease-of-use here; we just keep a model named `-inpainting`
         for any model.
         """
         if self.inpainting != new_inpainting:
             del self.pipeline
-            current_checkpoint_path = self.model_ckpt_path
 
+            current_checkpoint_path = self.model
             default_checkpoint_name, _ = os.path.splitext(os.path.basename(DEFAULT_MODEL))
             default_inpainting_name, _ = os.path.splitext(
                 os.path.basename(DEFAULT_INPAINTING_MODEL)
             )
             checkpoint_name, ext = os.path.splitext(os.path.basename(current_checkpoint_path))
 
             if default_checkpoint_name == checkpoint_name and new_inpainting:
@@ -916,51 +889,94 @@
                     "Switching to {0}inpainting checkpoint at {1}".format(
                         "" if new_inpainting else "non-", target_checkpoint_path
                     )
                 )
                 self.model = target_checkpoint_path
 
     @property
+    def engine_cache_exists(self) -> bool:
+        """
+        Gets whether or not the diffusers cache exists.
+        """
+        return os.path.exists(os.path.join(self.model_tensorrt_dir, "model_index.json"))
+
+    def check_create_tensorrt_engine_cache(self) -> None:
+        """
+        Converts a .ckpt file to the directory structure from diffusers
+            This ensures TRT compatibility
+        """
+        if not self.engine_cache_exists:
+            from diffusers.pipelines.stable_diffusion.convert_from_ckpt import (
+                download_from_original_stable_diffusion_ckpt,
+            )
+
+            self.start_keepalive()
+            _, ext = os.path.splitext(self.model)
+            pipe = download_from_original_stable_diffusion_ckpt(
+                checkpoint_path=self.model,
+                scheduler_type="ddim",
+                from_safetensors=ext == ".safetensors",
+                num_in_channels=9 if "inpaint" in self.model else 4,
+            ).to(torch_dtype=self.dtype)
+            pipe.save_pretrained(self.model_tensorrt_dir)
+            del pipe
+            torch.cuda.empty_cache()
+            self.stop_keepalive()
+
+    @property
     def pipeline(self) -> EnfugueStableDiffusionPipeline:
         """
         Instantiates the pipeline.
         """
         if not hasattr(self, "_pipeline"):
             kwargs = {
-                "cache_dir": self.diffusers_cache_dir,
+                "cache_dir": self.engine_cache_dir,
                 "engine_size": self.size,
                 "chunking_size": self.chunking_size,
                 "requires_safety_checker": self.safe,
+                "controlnet": self.controlnet,
                 "torch_dtype": self.dtype,
             }
 
-            if not self.safe:
-                kwargs["safety_checker"] = None
-
             if self.use_tensorrt:
                 if "unet" in self.TENSORRT_STAGES:
                     if self.controlnet is None and not self.TENSORRT_ALWAYS_USE_CONTROLLED_UNET:
                         kwargs["unet_engine_dir"] = self.model_tensorrt_unet_dir
                     else:
                         kwargs[
                             "controlled_unet_engine_dir"
                         ] = self.model_tensorrt_controlled_unet_dir
                 if "controlnet" in self.TENSORRT_STAGES and self.controlnet is not None:
                     kwargs["controlnet_engine_dir"] = self.model_tensorrt_controlnet_dir
                 if "vae" in self.TENSORRT_STAGES:
                     kwargs["vae_engine_dir"] = self.model_tensorrt_vae_dir
                 if "clip" in self.TENSORRT_STAGES:
                     kwargs["clip_engine_dir"] = self.model_tensorrt_clip_dir
-
-            logger.debug(
-                f"Initializing pipeline model {self.model} in directory {self.model_dir} with arguments {kwargs}"
-            )
-            kwargs["controlnet"] = self.controlnet
-
-            pipeline = self.pipeline_class.from_pretrained(self.model_dir, **kwargs)
+                if not self.safe:
+                    kwargs["safety_checker"] = None
+                self.check_create_tensorrt_engine_cache()
+                logger.debug(
+                    f"Initializing pipeline from diffusers cache directory at {self.model_tensorrt_dir}. Arguments are {kwargs}"
+                )
+                pipeline = self.pipeline_class.from_pretrained(self.model_tensorrt_dir, **kwargs)
+            elif self.engine_cache_exists:
+                if not self.safe:
+                    kwargs["safety_checker"] = None
+                logger.debug(
+                    f"Initializing pipeline from diffusers cache directory at {self.model_tensorrt_dir}. Arguments are {kwargs}"
+                )
+                pipeline = self.pipeline_class.from_pretrained(self.model_tensorrt_dir, **kwargs)
+            else:
+                kwargs["load_safety_checker"] = self.safe
+                logger.debug(
+                    f"Initializing pipeline from checkpoint at {self.model}. Arguments are {kwargs}"
+                )
+                pipeline = self.pipeline_class.from_ckpt(
+                    self.model, num_in_channels=9 if self.inpainting else 4, **kwargs
+                )
             if not self.tensorrt_is_ready:
                 for lora, weight in self.lora:
                     logger.debug(f"Adding LoRA {lora} to pipeline")
                     pipeline.load_lora_weights(lora, multiplier=weight)
                 for inversion in self.inversion:
                     logger.debug(f"Adding textual inversion {inversion} to pipeline")
                     pipeline.load_textual_inversion(inversion)
@@ -1031,19 +1047,28 @@
         """
         Loads a controlnet
         """
         if controlnet is None:
             return None
         from diffusers.models import ControlNetModel
 
+        expected_controlnet_location = os.path.join(
+            self.engine_cache_dir, controlnet.replace("/", "--")
+        )
+
+        if not os.path.exists(expected_controlnet_location):
+            logger.info(
+                f"Controlnet {controlnet} does not exist in cache directory {self.engine_cache_dir}, it will be downloaded."
+            )
+
         self.start_keepalive()
         result = ControlNetModel.from_pretrained(
             controlnet,
             torch_dtype=torch.half,
-            cache_dir=self.diffusers_cache_dir,
+            cache_dir=self.engine_cache_dir,
         )
         self.stop_keepalive()
         return result
 
     @property
     def controlnet(self) -> Optional[ControlNetModel]:
         """
@@ -1108,51 +1133,26 @@
         output_file = os.path.basename(remote_url)
         output_path = os.path.join(self.engine_checkpoints_dir, output_file)
         self.start_keepalive()
         check_download(remote_url, output_path)
         self.stop_keepalive()
         return output_path
 
-    def check_convert_checkpoint(self, checkpoint_path: str) -> str:
-        """
-        Converts a .ckpt file to the directory structure from diffusers
-        """
-        checkpoint_file = os.path.basename(checkpoint_path)
-        model_name, ext = os.path.splitext(checkpoint_file)
-        model_dir = os.path.join(self.engine_models_dir, model_name)
-
-        if not os.path.exists(model_dir):
-            if checkpoint_path.startswith("http"):
-                checkpoint_path = self.check_download_checkpoint(checkpoint_path)
-
-            from diffusers.pipelines.stable_diffusion.convert_from_ckpt import (
-                download_from_original_stable_diffusion_ckpt,
-            )
-
-            self.start_keepalive()
-            pipe = download_from_original_stable_diffusion_ckpt(
-                checkpoint_path=checkpoint_path,
-                scheduler_type="ddim",
-                from_safetensors=ext == ".safetensors",
-                num_in_channels=9 if "inpaint" in checkpoint_path else 4,
-            ).to(torch_dtype=self.dtype)
-            pipe.save_pretrained(model_dir)
-            self.stop_keepalive()
-        return model_name
-
     def __call__(self, **kwargs: Any) -> Any:
         """
         Passes an invocation down to the pipeline, doing whatever it needs to do to initialize it.
         Will switch between inpainting and non-inpainting models
         """
         logger.debug(f"Calling pipeline with arguments {kwargs}")
+
         if kwargs.get("mask", None) is not None:
             self.inpainting = True
         else:
             self.inpainting = False
+
         called_width = kwargs.get("width", self.size)
         called_height = kwargs.get("height", self.size)
         chunk_size = kwargs.get("chunking_size", self.chunking_size)
         if called_width < self.size:
             self.tensorrt_is_enabled = False
             logger.info(
                 f"Width ({called_width}) less than configured width ({self.size}), disabling TensorRT"
@@ -1221,16 +1221,16 @@
         else:
             model = os.path.basename(model)
 
         if model.endswith("-inpainting"):
             # Look for the base model instead, we'll look for inpainting separately
             model, _, _ = model.rpartition("-")
 
-        model_dir = os.path.join(engine_root, "models", model)
-        inpaint_model_dir = os.path.join(engine_root, "models", f"{model}-inpainting")
+        model_dir = os.path.join(engine_root, "tensorrt", model)
+        inpaint_model_dir = os.path.join(engine_root, "tensorrt", f"{model}-inpainting")
 
         if size is None:
             size = DiffusionPipelineManager.DEFAULT_SIZE
 
         if inversion is None:
             inversion = []
         elif not isinstance(inversion, list):
@@ -1264,41 +1264,39 @@
             "controlnet" not in DiffusionPipelineManager.TENSORRT_STAGES
         )
 
         if not clip_ready:
             clip_key = DiffusionPipelineManager.get_tensorrt_clip_key(
                 size, lora=lora_key, inversion=inversion_key
             )
-            clip_plan = os.path.join(model_dir, "tensorrt", "clip", clip_key, "engine.plan")
+            clip_plan = os.path.join(model_dir, "clip", clip_key, "engine.plan")
             clip_ready = os.path.exists(clip_plan)
 
         if not vae_ready:
             vae_key = DiffusionPipelineManager.get_tensorrt_vae_key(
                 size, lora=lora_key, inversion=inversion_key
             )
-            vae_plan = os.path.join(model_dir, "tensorrt", "vae", vae_key, "engine.plan")
+            vae_plan = os.path.join(model_dir, "vae", vae_key, "engine.plan")
             vae_ready = os.path.exists(vae_plan)
 
         if not unet_ready:
             unet_key = DiffusionPipelineManager.get_tensorrt_unet_key(
                 size, lora=lora_key, inversion=inversion_key
             )
-            unet_plan = os.path.join(model_dir, "tensorrt", "unet", unet_key, "engine.plan")
+            unet_plan = os.path.join(model_dir, "unet", unet_key, "engine.plan")
             unet_ready = os.path.exists(unet_plan)
 
-            inpaint_unet_plan = os.path.join(
-                inpaint_model_dir, "tensorrt", "unet", unet_key, "engine.plan"
-            )
+            inpaint_unet_plan = os.path.join(inpaint_model_dir, "unet", unet_key, "engine.plan")
             inpaint_unet_ready = os.path.exists(inpaint_unet_plan)
 
             controlled_unet_key = DiffusionPipelineManager.get_tensorrt_controlled_unet_key(
                 size, lora=lora_key, inversion=inversion_key
             )
             controlled_unet_plan = os.path.join(
-                model_dir, "tensorrt", "controlledunet", controlled_unet_key, "engine.plan"
+                model_dir, "controlledunet", controlled_unet_key, "engine.plan"
             )
             controlled_unet_ready = os.path.exists(controlled_unet_plan)
 
         if not controlnet_ready:
             if controlnet is None:
                 controlnet_ready = True
             else:
@@ -1306,15 +1304,15 @@
                 if not isinstance(controlnet, list):
                     controlnet = [controlnet]
                 for controlnet_name in controlnet:
                     controlnet_key = DiffusionPipelineManager.get_tensorrt_controlnet_key(
                         size, controlnet=controlnet_name
                     )
                     controlnet_plan = os.path.join(
-                        model_dir, "tensorrt", "controlnet", controlnet_key, "engine.plan"
+                        model_dir, "controlnet", controlnet_key, "engine.plan"
                     )
                     controlnet_ready[controlnet_name] = os.path.exists(controlnet_plan)
 
         ready = clip_ready and vae_ready
         if controlnet is not None or DiffusionPipelineManager.TENSORRT_ALWAYS_USE_CONTROLLED_UNET:
             ready = ready and controlled_unet_ready
             if isinstance(controlnet_ready, dict):
```

### Comparing `enfugue-0.1.1/enfugue/diffusion/pipeline.py` & `enfugue-0.1.2/enfugue/diffusion/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import (
     Any,
     List,
     Callable,
     Dict,
     List,
     Optional,
@@ -21,32 +23,47 @@
 import datetime
 import numpy as np
 
 from contextlib import contextmanager
 from collections import defaultdict
 
 from transformers import (
+    AutoFeatureExtractor,
     CLIPImageProcessor,
     CLIPTextModel,
     CLIPTokenizer,
 )
-from diffusers.schedulers import KarrasDiffusionSchedulers, DDIMScheduler
-
+from diffusers.schedulers import (
+    KarrasDiffusionSchedulers,
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    HeunDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
 from diffusers.models import AutoencoderKL, UNet2DConditionModel, ControlNetModel
-
 from diffusers.pipelines.stable_diffusion import (
     StableDiffusionPipeline,
     StableDiffusionPipelineOutput,
     StableDiffusionSafetyChecker,
 )
+from diffusers.pipelines.stable_diffusion.convert_from_ckpt import (
+    create_unet_diffusers_config,
+    create_vae_diffusers_config,
+    convert_ldm_unet_checkpoint,
+    convert_ldm_vae_checkpoint,
+    convert_ldm_clip_checkpoint,
+)
 
 from diffusers.utils import randn_tensor, PIL_INTERPOLATION
 from diffusers.image_processor import VaeImageProcessor
 
-from enfugue.util import logger
+from enfugue.util import logger, check_download_to_dir
 
 # This is ~64k×64k. Absurd, but I don't judge
 PIL.Image.MAX_IMAGE_PIXELS = 2**32
 
 
 class EnfugueStableDiffusionPipeline(StableDiffusionPipeline):
     """
@@ -99,14 +116,186 @@
 
         # Add an image processor for later
         self.image_processor = VaeImageProcessor(vae_scale_factor=self.vae_scale_factor)
 
         # Register controlnet, it can be None
         self.register_modules(controlnet=controlnet)
 
+    @classmethod
+    def from_ckpt(
+        cls,
+        checkpoint_path: str,
+        cache_dir: str,
+        prediction_type: Optional[str] = None,
+        image_size: int = 512,
+        scheduler_type: Literal[
+            "pndm", "lms", "heun", "euler", "euler-ancestral", "dpm", "ddim"
+        ] = "ddim",
+        load_safety_checker: bool = True,
+        torch_dtype: Optional[torch.dtype] = None,
+        upcast_attention: Optional[bool] = None,
+        extract_ema: Optional[bool] = None,
+        num_in_channels: Optional[int] = None,
+        **kwargs: Any,
+    ) -> EnfugueStableDiffusionPipeline:
+        """
+        Loads a checkpoint into this pipeline.
+        Diffusers' `from_pretrained` lets us pass arbitrary kwargs in, but `from_ckpt` does not.
+        That's why we override it for this method - most of this is copied from
+        https://github.com/huggingface/diffusers/blob/49949f321d9b034440b52e54937fd2df3027bf0a/src/diffusers/pipelines/stable_diffusion/convert_from_ckpt.py
+        """
+        device = "cuda" if torch.cuda.is_available() else "cpu"
+        if checkpoint_path.endswith("safetensors"):
+            from safetensors import safe_open
+
+            checkpoint = {}
+            with safe_open(checkpoint_path, framework="pt", device="cpu") as f:
+                for key in f.keys():
+                    checkpoint[key] = f.get_tensor(key)
+        else:
+            checkpoint = torch.load(checkpoint_path, map_location=device)
+
+        # Sometimes models don't have the global_step item
+        if "global_step" in checkpoint:
+            global_step = checkpoint["global_step"]
+        else:
+            global_step = None
+
+        # NOTE: this while loop isn't great but this controlnet checkpoint has one additional
+        # "state_dict" key https://huggingface.co/thibaud/controlnet-canny-sd21
+        while "state_dict" in checkpoint:
+            checkpoint = checkpoint["state_dict"]
+
+        key_name = "model.diffusion_model.input_blocks.2.1.transformer_blocks.0.attn2.to_k.weight"
+
+        # model_type = "v1"
+        config_url = "https://raw.githubusercontent.com/CompVis/stable-diffusion/main/configs/stable-diffusion/v1-inference.yaml"
+
+        if key_name in checkpoint and checkpoint[key_name].shape[-1] == 1024:
+            # model_type = "v2"
+            config_url = "https://raw.githubusercontent.com/Stability-AI/stablediffusion/main/configs/stable-diffusion/v2-inference-v.yaml"
+
+            if global_step == 110000:
+                # v2.1 needs to upcast attention
+                upcast_attention = True
+
+        original_config_file = check_download_to_dir(config_url, cache_dir, check_size=False)
+
+        from omegaconf import OmegaConf
+
+        original_config = OmegaConf.load(original_config_file)
+
+        if num_in_channels is not None:
+            original_config["model"]["params"]["unet_config"]["params"]["in_channels"] = num_in_channels  # type: ignore
+
+        if (
+            "parameterization" in original_config["model"]["params"]  # type: ignore
+            and original_config["model"]["params"]["parameterization"] == "v"  # type: ignore
+        ):
+            if prediction_type is None:
+                # NOTE: For stable diffusion 2 base it is recommended to pass `prediction_type=="epsilon"`
+                # as it relies on a brittle global step parameter here
+                prediction_type = "epsilon" if global_step == 875000 else "v_prediction"
+            if image_size is None:
+                # NOTE: For stable diffusion 2 base one has to pass `image_size==512`
+                # as it relies on a brittle global step parameter here
+                image_size = 512 if global_step == 875000 else 768  # type: ignore[unreachable]
+        else:
+            if prediction_type is None:
+                prediction_type = "epsilon"
+            if image_size is None:
+                image_size = 512  # type: ignore[unreachable]
+
+        num_train_timesteps = original_config.model.params.timesteps
+        beta_start = original_config.model.params.linear_start
+        beta_end = original_config.model.params.linear_end
+
+        scheduler = DDIMScheduler(
+            beta_end=beta_end,
+            beta_schedule="scaled_linear",
+            beta_start=beta_start,
+            num_train_timesteps=num_train_timesteps,
+            steps_offset=1,
+            clip_sample=False,
+            set_alpha_to_one=False,
+            prediction_type=prediction_type,
+        )
+
+        # make sure scheduler works correctly with DDIM
+        scheduler.register_to_config(clip_sample=False)
+
+        if scheduler_type == "pndm":
+            config = dict(scheduler.config)
+            config["skip_prk_steps"] = True
+            scheduler = PNDMScheduler.from_config(config)
+        elif scheduler_type == "lms":
+            scheduler = LMSDiscreteScheduler.from_config(scheduler.config)
+        elif scheduler_type == "heun":
+            scheduler = HeunDiscreteScheduler.from_config(scheduler.config)
+        elif scheduler_type == "euler":
+            scheduler = EulerDiscreteScheduler.from_config(scheduler.config)
+        elif scheduler_type == "euler-ancestral":
+            scheduler = EulerAncestralDiscreteScheduler.from_config(scheduler.config)
+        elif scheduler_type == "dpm":
+            scheduler = DPMSolverMultistepScheduler.from_config(scheduler.config)
+        elif scheduler_type == "ddim":
+            scheduler = scheduler
+        else:
+            raise ValueError(f"Scheduler of type {scheduler_type} doesn't exist!")
+
+        unet_config = create_unet_diffusers_config(original_config, image_size=image_size)
+        unet_config["upcast_attention"] = upcast_attention
+        unet = UNet2DConditionModel(**unet_config)
+
+        converted_unet_checkpoint = convert_ldm_unet_checkpoint(
+            checkpoint, unet_config, path=checkpoint_path, extract_ema=extract_ema
+        )
+
+        unet.load_state_dict(converted_unet_checkpoint)
+
+        # Convert the VAE model.
+        vae_config = create_vae_diffusers_config(original_config, image_size=image_size)
+        converted_vae_checkpoint = convert_ldm_vae_checkpoint(checkpoint, vae_config)
+
+        vae = AutoencoderKL(**vae_config)
+        vae.load_state_dict(converted_vae_checkpoint)
+
+        # Convert the text model.
+        model_type = original_config.model.params.cond_stage_config.target.split(".")[-1]
+        if model_type != "FrozenCLIPEmbedder":
+            raise ValueError("Enfugue currently only supports Stable Diffusion 1.5")
+
+        text_model = convert_ldm_clip_checkpoint(checkpoint)
+        tokenizer = CLIPTokenizer.from_pretrained("openai/clip-vit-large-patch14")
+
+        if load_safety_checker:
+            safety_checker = StableDiffusionSafetyChecker.from_pretrained(
+                "CompVis/stable-diffusion-safety-checker"
+            )
+            feature_extractor = AutoFeatureExtractor.from_pretrained(
+                "CompVis/stable-diffusion-safety-checker"
+            )
+        else:
+            safety_checker = None
+            feature_extractor = None
+
+        pipe = cls(
+            vae=vae,
+            text_encoder=text_model,
+            tokenizer=tokenizer,
+            unet=unet,
+            scheduler=scheduler,
+            safety_checker=safety_checker,
+            feature_extractor=feature_extractor,
+            **kwargs,
+        )
+        if torch_dtype is not None:
+            return pipe.to(torch_dtype=torch_dtype)
+        return pipe
+
     @contextmanager
     def get_runtime_context(
         self, batch_size: int, device: Union[str, torch.device]
     ) -> Iterator[None]:
         """
         Used by other implementations (tensorrt), but not base.
         """
```

### Comparing `enfugue-0.1.1/enfugue/diffusion/plan.py` & `enfugue-0.1.2/enfugue/diffusion/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,20 +300,18 @@
                     invocation_kwargs[key] = self.scale_image(invocation_kwargs[key], image_scale)
 
         result = pipeline(**invocation_kwargs)
 
         if self.remove_background:
             for i, image in enumerate(result["images"]):
                 result["images"][i] = remove_background(image)
-                logger.critical(result["images"][i])
 
         if image_scale > 1:
             for i, image in enumerate(result["images"]):
                 result["images"][i] = self.scale_image(image, 1 / image_scale)
-                logger.critical(result["images"][i])
 
         self.result = result
         return result
 
     @staticmethod
     def scale_image(image: PIL.Image.Image, scale: Union[int, float]) -> PIL.Image.Image:
         """
```

### Comparing `enfugue-0.1.1/enfugue/diffusion/process.py` & `enfugue-0.1.2/enfugue/diffusion/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """
     This process allows for easy two-way communication with a waiting
     Stable Diffusion Pipeline. Torch is only initiated after the process
     has began.
     """
 
     POLLING_DELAY_MS = 500
-    IDLE_SEC = 30
+    IDLE_SEC = 15
 
     def __init__(
         self,
         instructions: Queue,
         results: Queue,
         intermediates: Queue,
         configuration: Optional[APIConfiguration] = None,
@@ -269,16 +269,19 @@
     def run(self) -> None:
         """
         This is the function that the process will run.
         First instantiate the diffusion pipeline, then communicate as needed.
         """
         from pibble.util.helpers import OutputCatcher
         from pibble.util.log import ConfigurationLoggingContext
-        with OutputCatcher():
-            with ConfigurationLoggingContext(self.configuration):
+
+        catcher = OutputCatcher()
+
+        with ConfigurationLoggingContext(self.configuration, prefix="enfugue.engine.logging."):
+            with catcher:
                 last_data = datetime.datetime.now()
                 idle_seconds = 0.0
 
                 while True:
                     try:
                         payload = self.instructions.get(timeout=self.POLLING_DELAY_MS / 1000)
                     except KeyboardInterrupt:
@@ -305,29 +308,35 @@
                         logger.error(f"Unexpected non-dictionary argument {instruction}")
                         continue
 
                     instruction_id = instruction["id"]
                     instruction_action = instruction["action"]
                     instruction_payload = instruction.get("payload", None)
 
-                    logger.debug(f"Received instruction {instruction_id}, action {instruction_action}")
+                    logger.debug(
+                        f"Received instruction {instruction_id}, action {instruction_action}"
+                    )
                     if instruction_action == "ping":
                         logger.debug("Responding with 'pong'")
-                        self.results.put(Serializer.serialize({"id": instruction_id, "result": "pong"}))
+                        self.results.put(
+                            Serializer.serialize({"id": instruction_id, "result": "pong"})
+                        )
                     elif instruction_action in ["exit", "stop"]:
                         logger.debug("Exiting process")
                         self.pipemanager.unload_pipeline()
                         self.pipemanager.unload_upscaler()
                         return
                     elif instruction_action in ["invoke", "plan"]:
                         response = {"id": instruction_id, "payload": instruction_payload}
                         try:
                             if instruction_action == "plan":
                                 intermediate_dir = instruction_payload.get("intermediate_dir", None)
-                                intermediate_steps = instruction_payload.get("intermediate_steps", None)
+                                intermediate_steps = instruction_payload.get(
+                                    "intermediate_steps", None
+                                )
                                 plan = self.get_diffusion_plan(instruction_payload)
                                 response["result"] = self.execute_diffusion_plan(
                                     instruction_id,
                                     plan,
                                     intermediate_dir=intermediate_dir,
                                     intermediate_steps=intermediate_steps,
                                 )
@@ -350,8 +359,14 @@
                             Serializer.serialize(
                                 {
                                     "id": instruction_id,
                                     "error": f"Unknown action '{instruction_action}'",
                                 }
                             )
                         )
+                    out, err = catcher.output()
+                    if out:
+                        logger.debug(f"stdout: {out}")
+                    if err:
+                        logger.error(f"stderr: {err}")
+                    catcher.clean()
                     last_data = datetime.datetime.now()
```

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/engine.py` & `enfugue-0.1.2/enfugue/diffusion/rt/engine.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/model/base.py` & `enfugue-0.1.2/enfugue/diffusion/rt/model/base.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/model/clip.py` & `enfugue-0.1.2/enfugue/diffusion/rt/model/clip.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/model/controlledunet.py` & `enfugue-0.1.2/enfugue/diffusion/rt/model/controlledunet.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/model/controlnet.py` & `enfugue-0.1.2/enfugue/diffusion/rt/model/controlnet.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/model/unet.py` & `enfugue-0.1.2/enfugue/diffusion/rt/model/unet.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/model/vae.py` & `enfugue-0.1.2/enfugue/diffusion/rt/model/vae.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/optimizer.py` & `enfugue-0.1.2/enfugue/diffusion/rt/optimizer.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/rt/pipeline.py` & `enfugue-0.1.2/enfugue/diffusion/rt/pipeline.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/upscale/__init__.py` & `enfugue-0.1.2/enfugue/diffusion/upscale/__init__.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/upscale/gfpganer.py` & `enfugue-0.1.2/enfugue/diffusion/upscale/gfpganer.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/util.py` & `enfugue-0.1.2/enfugue/diffusion/util.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/diffusion/vision.py` & `enfugue-0.1.2/enfugue/diffusion/vision.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/enfugue.py` & `enfugue-0.1.2/enfugue/enfugue.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/interface/__init__.py` & `enfugue-0.1.2/enfugue/interface/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,17 @@
         ORMMiddlewareBase,
     )  # Bypass token checking and ORM instantiation
     @handlers.reverse("static", "/static/{path}")
     @handlers.methods("GET")
     @handlers.path("/static/(?P<path>\S+)")
     @handlers.cache()
     @handlers.download()
-    def static(self, request: Request, response: Response, path: str) -> Union[str, io.BytesIO]:
+    def static(
+        self, request: Request, response: Response, path: str
+    ) -> Union[str, io.BytesIO, io.BufferedReader]:
         directories = self.configuration.get("server.static.directories", [])
         if path.endswith("/index.autogenerated.mjs"):
             # Create autogenerated file index for JS directories.
             for root in directories:
                 dir_path = os.path.dirname(os.path.join(root, path))
                 if os.path.exists(dir_path) and os.path.isdir(dir_path):
                     js_files = [
@@ -262,27 +264,32 @@
                         )
                         response.content_type = "application/javascript"
                         return io.BytesIO(index.encode("utf-8"))
             raise NotFoundError(f"No javascript files found at path {path[:-23]}")
         for root in directories:
             root_path = os.path.join(root, path)
             if os.path.exists(root_path) and os.path.isfile(root_path):
-                return root_path
+                if root_path.endswith(".mjs"):
+                    # Force content-type
+                    response.content_type = "application/javascript"
+                    return open(root_path, "rb")
+                else:
+                    # Let pibble infer by filename
+                    return root_path
         logger.debug(f"Couldn't find path {path}, tried {directories}")
         raise NotFoundError(f"No file at {path}")
 
     @handlers.errors(401)
     def handle_authentication_error(self, request: Request, response: Response) -> None:
         """
         Determine what to do when authentication errors occur, then do it.
         """
         if self.configuration.get("enfugue.noauth", False):
             # Bypass login
             self.bypass_login(request, response)
-            logger.critical(":BYOP")
             self.handle_request(request, response)  # type: ignore
         else:
             self.redirect(response, "/login", 302)
 
     @handlers.cache(86400)
     @handlers.template("content-login.html.j2")
     @handlers.methods("GET")
```

### Comparing `enfugue-0.1.1/enfugue/interface/helpers.py` & `enfugue-0.1.2/enfugue/interface/helpers.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/partner/civitai.py` & `enfugue-0.1.2/enfugue/partner/civitai.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/server.py` & `enfugue-0.1.2/enfugue/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,30 +14,32 @@
     This class tries to get signing details at configuration time.
     """
 
     def configure(self, server=Dict[str, Any], **kwargs: Any) -> None:
         """
         At configuration, get cached or remote resources.
         """
-        try:
-            key, cert, chain = get_signature()
-            directory = tempfile.mkdtemp()
-            keyfile = os.path.join(directory, "key.pem")
-            certfile = os.path.join(directory, "cert.pem")
-            chainfile = os.path.join(directory, "chain.pem")
-            open(keyfile, "w").write(key)
-            open(certfile, "w").write(cert)
-            open(chainfile, "w").write(chain)
-            server["secure"] = True
-            server["cert"] = certfile
-            server["key"] = keyfile
-            server["chain"] = chainfile
-        except Exception as ex:
-            logger.error(f"Couldn't get signatures, disabling SSL. {ex}")
-            server["secure"] = False
+        secure = server.get("secure", True)
+        domain = server.get("domain", True)
+        if secure and domain == "app.enfugue.ai":
+            try:
+                key, cert, chain = get_signature()
+                directory = tempfile.mkdtemp()
+                keyfile = os.path.join(directory, "key.pem")
+                certfile = os.path.join(directory, "cert.pem")
+                chainfile = os.path.join(directory, "chain.pem")
+                open(keyfile, "w").write(key)
+                open(certfile, "w").write(cert)
+                open(chainfile, "w").write(chain)
+                server["cert"] = certfile
+                server["key"] = keyfile
+                server["chain"] = chainfile
+            except Exception as ex:
+                logger.error(f"Couldn't get signatures, disabling SSL. {ex}")
+                server["secure"] = False
         super(EnfugueSecureServer, self).configure(server=server, **kwargs)
 
     def on_destroy(self) -> None:
         """
         On destroy, clear tempfiles.
         """
         if hasattr(self, "_keyfile"):
```

### Comparing `enfugue-0.1.1/enfugue/static/css/01-reset.min.css` & `enfugue-0.1.2/enfugue/static/css/01-reset.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/04-base.min.css` & `enfugue-0.1.2/enfugue/static/css/04-base.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/05-common.min.css` & `enfugue-0.1.2/enfugue/static/css/05-common.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/06-header.min.css` & `enfugue-0.1.2/enfugue/static/css/06-header.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/07-main.min.css` & `enfugue-0.1.2/enfugue/static/css/07-main.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/08-enfugue.min.css` & `enfugue-0.1.2/enfugue/static/css/08-enfugue.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/09-enfugue-nodes.min.css` & `enfugue-0.1.2/enfugue/static/css/09-enfugue-nodes.min.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-enfugue-node-editor,enfugue-nodes{display:block;flex-grow:1;height:100%;overflow:hidden;position:relative;width:100%}enfugue-node-editor{display:block}enfugue-nodes{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center}enfugue-nodes.oversize-x{justify-content:flex-start;overflow-x:auto}enfugue-node-canvas{left:0;position:absolute;top:0;transform-origin:top left}enfugue-node-editor enfugue-node-canvas{background:linear-gradient(to right,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to right,var(--darker-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--darker-color) 0,transparent 1px) 0 0;background-color:var(--darkest-color);background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px}enfugue-node-editor enfugue-node-canvas>canvas{pointer-events:none}enfugue-nodes enfugue-node-canvas{position:relative}enfugue-nodes enfugue-node-canvas>canvas{display:none}enfugue-node-editor.windows>enfugue-node-canvas{background:none}enfugue-node-editor-position,enfugue-node-editor-zoom{bottom:5px;color:var(--light-color);font-weight:700;position:absolute;text-transform:uppercase;z-index:3}enfugue-node-editor-position{left:5px}enfugue-node-editor-position-reset,enfugue-node-editor-zoom-reset{background-color:hsla(0,0%,100%,.05);border:1px solid #000;border-radius:2px;cursor:pointer;font-size:12px;padding:2px 4px;transition:background-color .25s ease-in-out}enfugue-node-editor-position-reset:hover,enfugue-node-editor-zoom-reset:hover{background-color:hsla(0,0%,100%,.1)}enfugue-node-editor-position-reset{margin-left:5px}enfugue-node-editor-zoom-reset{margin-right:5px}enfugue-node-editor-zoom{right:5px}enfugue-node-editor-zoom-readout:after{content:"×"}enfugue-node-editor-zoom-in,enfugue-node-editor-zoom-out{cursor:pointer;margin-right:5px}enfugue-node{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch;padding:10px;pointer-events:all;position:absolute;transition:transform .25s ease-out;z-index:1}enfugue-node.minimized{pointer-events:none;transition:all .25s ease-in}enfugue-node.focused{z-index:2}enfugue-node-container{align-items:stretch;background-color:var(--darkest-color);border:1px solid #000;border-radius:4px;display:block;flex-flow:column nowrap;justify-content:stretch;overflow:hidden;width:100%}enfugue-node.input-output>enfugue-node-container{background-color:#153131;color:var(--lightest-color)}enfugue-node-header,enfugue-windows-toolbar-item{align-items:center;background-color:var(--darker-color);color:var(--lightest-color);display:flex;flex-flow:row nowrap;flex-grow:0;font-size:14px;justify-content:stretch;overflow:hidden;padding:0 5px;transition:background-color .2s ease-in-out,height .2s ease-in-out;z-index:10}enfugue-node.flipped enfugue-node-header{bottom:0}enfugue-windows-toolbar-item{cursor:pointer;height:30px}enfugue-node-header:hover,enfugue-windows-toolbar-item:hover{background-color:var(--dark-color)}enfugue-node-name,enfugue-windows-toolbar-item-name{flex-grow:1;font-family:var(--monospace-font),monospace;margin-right:5px}enfugue-node-button,enfugue-windows-toolbar-item-button{cursor:pointer;flex-grow:0;margin:0 3px;transition:color .25s ease-in-out;z-index:10}enfugue-node-button:hover,enfugue-windows-toolbar-item-button:hover{color:var(--theme-color-primary)}enfugue-windows-toolbar{background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:0;display:flex;flex-flow:row wrap;gap:1px;left:0;min-height:30px;pointer-events:all;position:absolute;right:0}enfugue-node-contents{display:block;flex-grow:1;overflow:auto;position:relative;width:100%}enfugue-node-contents h1,enfugue-node-contents h2,enfugue-node-contents h3{margin:1rem 0 0 1rem}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header{background-color:rgba(0,0,0,.4);background-image:linear-gradient(180deg,rgba(0,0,0,.7),transparent);position:absolute;width:100%}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-container{background:transparent;border-radius:0;border-width:0;position:relative}enfugue-node-editor.image-editor enfugue-node:hover enfugue-node-container{background:hsla(0,0%,100%,.02)}enfugue-node-editor.image-editor enfugue-node-contents{overflow:hidden}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view{display:block;height:100%;position:relative;width:100%;z-index:-1}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view .background{background-position:0 0;background-repeat:no-repeat;background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-actual .background{background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-stretch .background{background-size:100% 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-contain .background{background-size:contain}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-cover .background{background-size:cover}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-left .background{background-position:0 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-center .background{background-position:top}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-right .background{background-position:100% 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-left .background{background-position:0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-center .background{background-position:50%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-right .background{background-position:100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-left .background{background-position:0 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-center .background{background-position:bottom}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-right .background{background-position:100% 100%}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.top-right{transform:rotate(90deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-right{transform:rotate(180deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-left{transform:rotate(270deg)}enfugue-node-editor.image-editor enfugue-node-canvas .current-invocation-image-view{left:0;position:absolute;top:0}enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas enfugue-background-image-view{image-rendering:auto}enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas enfugue-background-image-view{image-rendering:pixelated}enfugue-node-editor.image-editor enfugue-node-canvas{background:none;border:1px solid var(--dark-color);box-sizing:content-box}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-image-editor-grid{background-color:transparent;background:linear-gradient(90deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(90deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0;background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px;height:100%;left:0;opacity:1;pointer-events:none;position:absolute;top:0;transition:.1s ease-in-out;width:100%;z-index:2}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-image-editor-grid{opacity:0}enfugue-node-editor.image-editor.has-image enfugue-node-canvas:hover enfugue-image-editor-grid{opacity:1}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-node{display:none}enfugue-node-editor.image-editor enfugue-invocation-loading{border:1px solid var(--dark-color);border-radius:10px;bottom:5px;display:block;height:20px;left:175px;line-height:18px;position:absolute;right:175px;transition:all .25s ease-in-out;z-index:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser{align-items:center;bottom:30px;display:flex;flex-flow:row nowrap;gap:5px;justify-content:center;left:175px;position:absolute;right:175px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample{align-items:center;border:1px solid var(--dark-color);border-radius:2px;cursor:pointer;display:flex;flex-flow:row nowrap;height:100px;justify-content:center;opacity:.7;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:hover{opacity:.9}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:active{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample.no-sample{color:var(--dark-color);font-size:100px;width:100px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample img{max-height:100px}enfugue-node-editor.image-editor enfugue-invocation-stop{background-color:var(--theme-color-primary);border-radius:80px;color:#fff;cursor:not-allowed;display:block;filter:grayscale(100%);font-size:11px;height:40px;line-height:40px;opacity:0;pointer-events:none;position:absolute;right:5px;text-align:center;text-transform:uppercase;top:5px;transition:all .25s ease-in-out;width:40px}enfugue-node-editor.image-editor enfugue-invocation-stop.ready{cursor:pointer;filter:grayscale(50%);opacity:1;pointer-events:all}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:hover{filter:grayscale(25%)}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:active{filter:grayscale(0)}enfugue-node-editor.image-editor enfugue-invocation-loading{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;overflow:hidden}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-loaded{display:block;height:100%;opacity:0;position:absolute;transition:all .1s linear;z-index:-1}enfugue-node-editor.image-editor enfugue-invocation-loading.loading enfugue-invocation-loaded{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{bottom:0;color:#fff;display:block;font-size:10px;text-shadow:1px 1px 1px #000;top:0}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration{margin-left:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations{margin-left:5px;margin-right:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{margin-right:5px}enfugue-node-editor.image-editor enfugue-node form{font-size:11px;height:0;opacity:0;overflow-y:auto;padding-bottom:1em;position:absolute;top:0;transition:all .25s ease-in-out;width:100%}enfugue-node-editor.image-editor enfugue-node.image-editor-prompt-node-view form{background-color:var(--dark-color)!important;height:100%!important;opacity:1!important;top:0!important}enfugue-node-editor.image-editor enfugue-node.image-editor-image-node-view enfugue-scribble-view{opacity:.5}enfugue-node-editor.image-editor enfugue-node.flipped form{bottom:0;top:auto}enfugue-node-editor.image-editor enfugue-node form input,enfugue-node-editor.image-editor enfugue-node form label,enfugue-node-editor.image-editor enfugue-node form select{color:#fff;font-size:11px}enfugue-node-editor.image-editor enfugue-node form legend{display:none}enfugue-node-editor.image-editor enfugue-node form .field-container{flex-basis:30%}enfugue-node-editor.image-editor enfugue-node form .field-container.checkbox-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-anchor-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-fit-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.text-input-view{flex-basis:40%}enfugue-node-editor.image-editor enfugue-node:hover form{background-color:rgba(0,0,0,.4);height:calc(100% - 30px);opacity:1;top:30px}enfugue-node-editor.image-editor enfugue-node.flipped:hover form{bottom:30px;top:auto}enfugue-node-editor.image-editor enfugue-node:hover form:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar{background-color:transparent;background-image:linear-gradient(90deg,transparent,rgba(0,0,0,.4));border:none;bottom:0;left:auto;right:0;top:0}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item{background:none;border:none;opacity:.5;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:active,enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:hover{border:none;opacity:1}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:after{display:none}.field-container.checkpoint-input-view,.field-container.multi-inversion-input-view,.field-container.multi-lora-input-view,.field-container.upscale-diffusion-guidance-scale-input-view,.field-container.upscale-diffusion-negative-prompt-input-view,.field-container.upscale-diffusion-prompt-input-view,.field-container.upscale-diffusion-steps-input-view,.field-container.upscale-methods-input-view,fieldset.field-set-prompts .field-container{flex-basis:100%}fieldset.field-set-prompts .field-container{margin-bottom:1em}.field-container.multi-lora-input-view legend{display:none}.field-container.multi-lora-input-view form .field-container{flex-basis:100%}enfugue-model-table{display:flex;flex-flow:column nowrap;justify-content:space-between}enfugue-model-table-paging{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;padding:5px 1em 0}enfugue-model-table-paging>span{color:var(--theme-color-tertiary);font-size:12px}enfugue-model-table-paging ul{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table-paging ul li{align-items:center;background-color:var(--theme-color-tertiary);border-radius:3px;color:#fff;cursor:pointer;display:flex;flex-flow:row nowrap;height:25px;justify-content:center;line-height:25px;position:relative;text-align:center;transition:background-color .25s ease-in-out;width:25px}enfugue-model-table-paging ul li.selected{background-color:var(--theme-color-secondary)}enfugue-model-table-paging ul li span{font-family:var(--monospace-font),monospace}enfugue-model-table ul.include-first li:first-child{margin-right:30px}enfugue-model-table ul.include-first li:first-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;left:calc(100% + 11px);position:absolute}enfugue-model-table ul.include-last li:last-child{margin-left:30px}enfugue-model-table ul.include-last li:last-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;position:absolute;right:calc(100% + 11px)}enfugue-model-table-paging ul li:before{background-color:#fff;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}enfugue-model-table-paging ul li:hover:before{opacity:.1}enfugue-invocation-outputs{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table.invocation-history tr td:first-child,enfugue-model-table.invocation-history tr td:nth-child(2),enfugue-model-table.invocation-history tr th:first-child,enfugue-model-table.invocation-history tr th:nth-child(2){width:15%}enfugue-model-table.invocation-history tr td:nth-child(3),enfugue-model-table.invocation-history tr th:nth-child(3){width:25%}enfugue-model-table.invocation-history tr td:nth-child(4),enfugue-model-table.invocation-history tr th:nth-child(4){width:35%}div.about-view>p,div.announcements-view>.view>p{line-height:1.1em;margin:1rem 0 0 1rem}div.announcements-view>.view>h3{color:var(--theme-color-tertiary);margin:1rem 0 0 1rem;text-align:left}div.about-view .donate-links{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;padding:.5em 1em}div.about-view .donate-links a{border-radius:5px;border-style:solid;border-width:2px;color:#fff;display:block;flex-basis:100%;font-weight:900;padding:1em;text-decoration:none;transition:all .25s ease-in-out}div.about-view .donate-links a:before{background-position:50%;background-repeat:no-repeat;background-size:contain;content:"\A";display:inline-block;height:25px;margin-right:10px;vertical-align:middle;width:25px}div.about-view .donate-links a.patreon{background-color:#ee614a;border-color:#ee614a}div.about-view .donate-links a.ko-fi{background-color:#29abe0;border-color:#29abe0}div.about-view .donate-links a.patreon:before{background-image:url(../img/brand/patreon.png)}div.about-view .donate-links a.ko-fi:before{background-image:url(../img/brand/ko-fi.png)}div.about-view .donate-links a:hover{background-color:transparent}div.about-view .donate-links a.patreon:hover{color:#ee614a}div.about-view .donate-links a.ko-fi:hover{color:#29abe0}div.history-view>input{float:right;margin:1em 1em 0 0}table.history-table-view tr td:first-child,table.history-table-view tr th:first-child{width:150px}input.new-model-input-view,input.new-user-input-view,input.upload-file-input-view{float:right;margin-right:1em}input.upload-file-input-view{margin-top:1em}input.download-input-view{margin:1em;width:calc(100% - 2em)}enfugue-invocation-outputs enfugue-invocation-output{cursor:pointer}enfugue-invocation-outputs enfugue-invocation-output img{max-height:50px}
+enfugue-node-editor,enfugue-nodes{display:block;flex-grow:1;height:100%;overflow:hidden;position:relative;width:100%}enfugue-node-editor{display:block}enfugue-nodes{align-items:center;display:flex;flex-flow:row nowrap;justify-content:center}enfugue-nodes.oversize-x{justify-content:flex-start;overflow-x:auto}enfugue-node-canvas{left:0;position:absolute;top:0;transform-origin:top left}enfugue-node-editor enfugue-node-canvas{background:linear-gradient(to right,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to right,var(--darker-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--dark-color) 0,transparent 1px) 0 0,linear-gradient(to bottom,var(--darker-color) 0,transparent 1px) 0 0;background-color:var(--darkest-color);background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px}enfugue-node-editor enfugue-node-canvas>canvas{pointer-events:none}enfugue-nodes enfugue-node-canvas{position:relative}enfugue-nodes enfugue-node-canvas>canvas{display:none}enfugue-node-editor.windows>enfugue-node-canvas{background:none}enfugue-node-editor-position,enfugue-node-editor-zoom{bottom:5px;color:var(--light-color);font-weight:700;position:absolute;text-transform:uppercase;z-index:3}enfugue-node-editor-position{left:5px}enfugue-node-editor-position-reset,enfugue-node-editor-zoom-reset{background-color:hsla(0,0%,100%,.05);border:1px solid #000;border-radius:2px;cursor:pointer;font-size:12px;padding:2px 4px;transition:background-color .25s ease-in-out}enfugue-node-editor-position-reset:hover,enfugue-node-editor-zoom-reset:hover{background-color:hsla(0,0%,100%,.1)}enfugue-node-editor-position-reset{margin-left:5px}enfugue-node-editor-zoom-reset{margin-right:5px}enfugue-node-editor-zoom{right:5px}enfugue-node-editor-zoom-readout:after{content:"×"}enfugue-node-editor-zoom-in,enfugue-node-editor-zoom-out{cursor:pointer;margin-right:5px}enfugue-node{align-items:stretch;display:flex;flex-flow:row nowrap;justify-content:stretch;padding:10px;pointer-events:all;position:absolute;transition:transform .25s ease-out;z-index:1}enfugue-node.minimized{pointer-events:none;transition:all .25s ease-in}enfugue-node.focused{z-index:2}enfugue-node-container{align-items:stretch;background-color:var(--darkest-color);border:1px solid #000;border-radius:4px;display:block;flex-flow:column nowrap;justify-content:stretch;overflow:hidden;width:100%}enfugue-node.input-output>enfugue-node-container{background-color:#153131;color:var(--lightest-color)}enfugue-node-header,enfugue-windows-toolbar-item{align-items:center;background-color:var(--darker-color);color:var(--lightest-color);display:flex;flex-flow:row nowrap;flex-grow:0;font-size:14px;justify-content:stretch;overflow:hidden;padding:0 5px;transition:background-color .2s ease-in-out,height .2s ease-in-out;z-index:10}enfugue-node.flipped enfugue-node-header{bottom:0}enfugue-windows-toolbar-item{cursor:pointer;height:30px}enfugue-node-header:hover,enfugue-windows-toolbar-item:hover{background-color:var(--dark-color)}enfugue-node-name,enfugue-windows-toolbar-item-name{flex-grow:1;font-family:var(--monospace-font),monospace;margin-right:5px}enfugue-node-button,enfugue-windows-toolbar-item-button{cursor:pointer;flex-grow:0;margin:0 3px;transition:color .25s ease-in-out;z-index:10}enfugue-node-button:hover,enfugue-windows-toolbar-item-button:hover{color:var(--theme-color-primary)}enfugue-windows-toolbar{background-color:var(--dark-color);border-bottom:1px solid rgba(0,0,0,.2);border-top:1px solid hsla(0,0%,100%,.1);bottom:0;display:flex;flex-flow:row wrap;gap:1px;left:0;min-height:30px;pointer-events:all;position:absolute;right:0}enfugue-node-contents{display:block;flex-grow:1;overflow:auto;position:relative;width:100%}enfugue-node-contents h1,enfugue-node-contents h2,enfugue-node-contents h3{margin:1rem 0 0 1rem}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header{background-color:rgba(0,0,0,.4);background-image:linear-gradient(180deg,rgba(0,0,0,.7),transparent);position:absolute;width:100%}enfugue-node-editor.image-editor enfugue-node.hide-header enfugue-node-header:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-container{background:transparent;border-radius:0;border-width:0;position:relative}enfugue-node-editor.image-editor enfugue-node:hover enfugue-node-container{background:hsla(0,0%,100%,.02)}enfugue-node-editor.image-editor enfugue-node-contents{overflow:hidden}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view{display:block;height:100%;position:relative;width:100%;z-index:-1}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view .background{background-position:0 0;background-repeat:no-repeat;background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-actual .background{background-size:auto}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-stretch .background{background-size:100% 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-contain .background{background-size:contain}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.fit-cover .background{background-size:cover}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-left .background{background-position:0 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-center .background{background-position:top}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-top-right .background{background-position:100% 0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-left .background{background-position:0}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-center .background{background-position:50%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-center-right .background{background-position:100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-left .background{background-position:0 100%}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-center .background{background-position:bottom}enfugue-node-editor.image-editor enfugue-node-contents enfugue-background-image-view.anchor-bottom-right .background{background-position:100% 100%}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.top-right{transform:rotate(90deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-right{transform:rotate(180deg)}enfugue-node-editor.image-editor enfugue-node-header enfugue-node-button.bottom-left{transform:rotate(270deg)}enfugue-node-editor.image-editor enfugue-node-canvas .current-invocation-image-view{left:0;position:absolute;top:0}enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-out enfugue-node-canvas enfugue-background-image-view{image-rendering:auto}enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas .current-invocation-image-view,enfugue-node-editor.image-editor.zoom-in enfugue-node-canvas enfugue-background-image-view{image-rendering:pixelated}enfugue-node-editor.image-editor enfugue-node-canvas{background:none;border:1px solid var(--dark-color);box-sizing:content-box}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-image-editor-grid{background-color:transparent;background:linear-gradient(90deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(90deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.1) 0,hsla(0,0%,100%,.1) 1px,transparent 0) 0 0,linear-gradient(180deg,hsla(0,0%,100%,.02) 0,hsla(0,0%,100%,.02) 1px,transparent 0) 0 0;background-position:-.5px -.5px;background-size:64px 64px,8px 8px,64px 64px,8px 8px;height:100%;left:0;opacity:1;pointer-events:none;position:absolute;top:0;transition:.1s ease-in-out;width:100%;z-index:2}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-image-editor-grid{opacity:0}enfugue-node-editor.image-editor.has-image enfugue-node-canvas:hover enfugue-image-editor-grid{opacity:1}enfugue-node-editor.image-editor.has-image enfugue-node-canvas enfugue-node{display:none}enfugue-node-editor.image-editor enfugue-invocation-loading{border:1px solid var(--dark-color);border-radius:10px;bottom:5px;display:block;height:20px;left:175px;line-height:18px;position:absolute;right:175px;transition:all .25s ease-in-out;z-index:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser{align-items:center;bottom:30px;display:flex;flex-flow:row nowrap;gap:5px;justify-content:center;left:175px;position:absolute;right:175px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample{align-items:center;border:1px solid var(--dark-color);border-radius:2px;cursor:pointer;display:flex;flex-flow:row nowrap;height:100px;justify-content:center;opacity:.7;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:hover{opacity:.9}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample:active{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample.no-sample{color:var(--dark-color);font-size:100px;width:100px}enfugue-node-editor.image-editor enfugue-invocation-sample-chooser enfugue-invocation-sample img{max-height:100px}enfugue-node-editor.image-editor enfugue-invocation-stop{background-color:var(--theme-color-primary);border-radius:80px;color:#fff;cursor:not-allowed;display:block;filter:grayscale(100%);font-size:11px;height:40px;line-height:40px;opacity:0;pointer-events:none;position:absolute;right:5px;text-align:center;text-transform:uppercase;top:5px;transition:all .25s ease-in-out;width:40px}enfugue-node-editor.image-editor enfugue-invocation-stop.ready{cursor:pointer;filter:grayscale(50%);opacity:1;pointer-events:all}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:hover{filter:grayscale(25%)}enfugue-node-editor.image-editor enfugue-invocation-stop.ready:active{filter:grayscale(0)}enfugue-node-editor.image-editor enfugue-invocation-loading{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;overflow:hidden}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-loaded{display:block;height:100%;opacity:0;position:absolute;transition:all .1s linear;z-index:-1}enfugue-node-editor.image-editor enfugue-invocation-loading.loading enfugue-invocation-loaded{opacity:1}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations,enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{bottom:0;color:#fff;display:block;font-size:10px;text-shadow:1px 1px 1px #000;top:0}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-duration{margin-left:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-iterations{margin-left:5px;margin-right:5px}enfugue-node-editor.image-editor enfugue-invocation-loading enfugue-invocation-remaining{margin-right:5px}enfugue-node-editor.image-editor enfugue-node form{font-size:11px;height:0;opacity:0;overflow-y:auto;padding-bottom:1em;position:absolute;top:0;transition:all .25s ease-in-out;width:100%}enfugue-node-editor.image-editor enfugue-node.image-editor-prompt-node-view form{background-color:var(--dark-color)!important;height:100%!important;opacity:1!important;top:0!important}enfugue-node-editor.image-editor enfugue-node.image-editor-image-node-view enfugue-scribble-view{opacity:.5}enfugue-node-editor.image-editor enfugue-node.flipped form{bottom:0;top:auto}enfugue-node-editor.image-editor enfugue-node form input,enfugue-node-editor.image-editor enfugue-node form label,enfugue-node-editor.image-editor enfugue-node form select{color:#fff;font-size:11px}enfugue-node-editor.image-editor enfugue-node form legend{display:none}enfugue-node-editor.image-editor enfugue-node form .field-container{flex-basis:30%}enfugue-node-editor.image-editor enfugue-node form .field-container.checkbox-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-anchor-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.image-editor-image-fit-input-view,enfugue-node-editor.image-editor enfugue-node form .field-container.text-input-view{flex-basis:40%}enfugue-node-editor.image-editor enfugue-node:hover form{background-color:rgba(0,0,0,.4);height:calc(100% - 30px);opacity:1;top:30px}enfugue-node-editor.image-editor enfugue-node.flipped:hover form{bottom:30px;top:auto}enfugue-node-editor.image-editor enfugue-node:hover form:hover{background-color:rgba(0,0,0,.6)}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar{background-color:transparent;background-image:linear-gradient(90deg,transparent,rgba(0,0,0,.4));border:none;bottom:0;left:auto;right:0;top:0}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item{background:none;border:none;opacity:.5;transition:all .25s ease-in-out}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:active,enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:hover{border:none;opacity:1}enfugue-node-editor.image-editor enfugue-node-canvas enfugue-toolbar-item:after{display:none}.field-container.checkpoint-input-view,.field-container.multi-inversion-input-view,.field-container.multi-lora-input-view,.field-container.upscale-diffusion-guidance-scale-input-view,.field-container.upscale-diffusion-negative-prompt-input-view,.field-container.upscale-diffusion-prompt-input-view,.field-container.upscale-diffusion-steps-input-view,.field-container.upscale-methods-input-view,fieldset.field-set-directories .field-container,fieldset.field-set-prompts .field-container{flex-basis:100%}fieldset.field-set-prompts .field-container{margin-bottom:1em}.field-container.multi-lora-input-view legend{display:none}.field-container.multi-lora-input-view form .field-container{flex-basis:100%}enfugue-model-table{display:flex;flex-flow:column nowrap;justify-content:space-between}enfugue-model-table-paging{align-items:center;display:flex;flex-flow:row nowrap;justify-content:space-between;padding:5px 1em 0}enfugue-model-table-paging>span{color:var(--theme-color-tertiary);font-size:12px}enfugue-model-table-paging ul{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table-paging ul li{align-items:center;background-color:var(--theme-color-tertiary);border-radius:3px;color:#fff;cursor:pointer;display:flex;flex-flow:row nowrap;height:25px;justify-content:center;line-height:25px;position:relative;text-align:center;transition:background-color .25s ease-in-out;width:25px}enfugue-model-table-paging ul li.selected{background-color:var(--theme-color-secondary)}enfugue-model-table-paging ul li span{font-family:var(--monospace-font),monospace}enfugue-model-table ul.include-first li:first-child{margin-right:30px}enfugue-model-table ul.include-first li:first-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;left:calc(100% + 11px);position:absolute}enfugue-model-table ul.include-last li:last-child{margin-left:30px}enfugue-model-table ul.include-last li:last-child:after{color:var(--theme-color-tertiary);content:"…";font-size:16px;position:absolute;right:calc(100% + 11px)}enfugue-model-table-paging ul li:before{background-color:#fff;bottom:0;content:"\A";left:0;opacity:0;pointer-events:none;position:absolute;right:0;top:0;transition:opacity .25s ease-in-out}enfugue-model-table-paging ul li:hover:before{opacity:.1}enfugue-invocation-outputs{display:flex;flex-flow:row nowrap;gap:5px}enfugue-model-table.invocation-history tr td:first-child,enfugue-model-table.invocation-history tr td:nth-child(2),enfugue-model-table.invocation-history tr th:first-child,enfugue-model-table.invocation-history tr th:nth-child(2){width:15%}enfugue-model-table.invocation-history tr td:nth-child(3),enfugue-model-table.invocation-history tr th:nth-child(3){width:25%}enfugue-model-table.invocation-history tr td:nth-child(4),enfugue-model-table.invocation-history tr th:nth-child(4){width:35%}div.about-view>p,div.announcements-view>.view>p{line-height:1.1em;margin:1rem 0 0 1rem}div.announcements-view>.view>h3{color:var(--theme-color-tertiary);margin:1rem 0 0 1rem;text-align:left}div.about-view .donate-links{align-items:stretch;display:flex;flex-flow:row nowrap;gap:1em;justify-content:stretch;margin-top:1em;padding:.5em 1em}div.about-view .donate-links a{border-radius:5px;border-style:solid;border-width:2px;color:#fff;display:block;flex-basis:100%;font-weight:900;padding:1em;text-decoration:none;transition:all .25s ease-in-out}div.about-view .donate-links a:before{background-position:50%;background-repeat:no-repeat;background-size:contain;content:"\A";display:inline-block;height:25px;margin-right:10px;vertical-align:middle;width:25px}div.about-view .donate-links a.patreon{background-color:#ee614a;border-color:#ee614a}div.about-view .donate-links a.ko-fi{background-color:#29abe0;border-color:#29abe0}div.about-view .donate-links a.patreon:before{background-image:url(../img/brand/patreon.png)}div.about-view .donate-links a.ko-fi:before{background-image:url(../img/brand/ko-fi.png)}div.about-view .donate-links a:hover{background-color:transparent}div.about-view .donate-links a.patreon:hover{color:#ee614a}div.about-view .donate-links a.ko-fi:hover{color:#29abe0}div.history-view>input{float:right;margin:1em 1em 0 0}table.history-table-view tr td:first-child,table.history-table-view tr th:first-child,table.log-table-view tr td:first-child,table.log-table-view tr th:first-child{width:150px}table.log-table-view tr td:nth-child(2),table.log-table-view tr td:nth-child(3),table.log-table-view tr th:nth-child(2),table.log-table-view tr th:nth-child(3){width:80px}input.new-model-input-view,input.new-user-input-view,input.upload-file-input-view{float:right;margin-right:1em}input.upload-file-input-view{margin-top:1em}input.download-input-view{margin:1em;width:calc(100% - 2em)}enfugue-invocation-outputs enfugue-invocation-output{cursor:pointer}enfugue-invocation-outputs enfugue-invocation-output img{max-height:50px}
```

### Comparing `enfugue-0.1.1/enfugue/static/css/vendor/fa/brands.min.css` & `enfugue-0.1.2/enfugue/static/css/vendor/fa/brands.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/vendor/fa/fontawesome.min.css` & `enfugue-0.1.2/enfugue/static/css/vendor/fa/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/vendor/fa/regular.min.css` & `enfugue-0.1.2/enfugue/static/css/vendor/fa/regular.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/css/vendor/fa/solid.min.css` & `enfugue-0.1.2/enfugue/static/css/vendor/fa/solid.min.css`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf` & `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2` & `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf` & `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2` & `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf` & `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2` & `enfugue-0.1.2/enfugue/static/fonts/vendor/fa/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/html/body/content/content-login.html.j2` & `enfugue-0.1.2/enfugue/static/html/body/content/content-login.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/html/body/footer/footer.html.j2` & `enfugue-0.1.2/enfugue/static/html/body/footer/footer.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/html/head/head-base.html.j2` & `enfugue-0.1.2/enfugue/static/html/head/head-base.html.j2`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/brand/civit-ai-logo.svg` & `enfugue-0.1.2/enfugue/static/img/brand/civit-ai-logo.svg`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/brand/civit-ai.png` & `enfugue-0.1.2/enfugue/static/img/brand/civit-ai.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/brand/ko-fi.png` & `enfugue-0.1.2/enfugue/static/img/brand/ko-fi.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/brand/patreon.png` & `enfugue-0.1.2/enfugue/static/img/brand/patreon.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/brand/tensorrt.png` & `enfugue-0.1.2/enfugue/static/img/brand/tensorrt.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/cloud-320.png` & `enfugue-0.1.2/enfugue/static/img/cloud-320.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/favicon/favicon-128x128.png` & `enfugue-0.1.2/enfugue/static/img/favicon/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/favicon/favicon-16x16.png` & `enfugue-0.1.2/enfugue/static/img/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/favicon/favicon-256x256.png` & `enfugue-0.1.2/enfugue/static/img/favicon/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/favicon/favicon-32x32.png` & `enfugue-0.1.2/enfugue/static/img/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/favicon/favicon-512x512.png` & `enfugue-0.1.2/enfugue/static/img/favicon/favicon-512x512.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/favicon/favicon-64x64.png` & `enfugue-0.1.2/enfugue/static/img/favicon/favicon-64x64.png`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/img/favicon/favicon.ico` & `enfugue-0.1.2/enfugue/static/img/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/application/index.mjs` & `enfugue-0.1.2/enfugue/static/js/application/index.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,getQueryParameters,getDataParameters,waitFor,createEvent}from"../base/helpers.mjs";import{Publisher}from"../base/publisher.mjs";import{TooltipHelper}from"../common/tooltip.mjs";import{MenuView,SidebarView,ToolbarView}from"../view/menu.mjs";import{StatusView}from"../view/status.mjs";import{NotificationCenterView}from"../view/notifications.mjs";import{WindowsView}from"../view/nodes/windows.mjs";import{ImageEditorView,ImageEditorNodeView,ImageEditorImageNodeView}from"../view/nodes/image-editor.mjs";import{ImageView}from"../view/image.mjs";import{Model}from"../model/enfugue.mjs";import{ConfirmFormView,YesNoFormView}from"../view/forms/confirm.mjs";import{View}from"../view/base.mjs";import{FormView}from"../view/forms/base.mjs";import{StringInputView}from"../view/forms/input.mjs";import{InvocationController}from"../controller/common/invocation.mjs";import{ModelPickerController}from"../controller/common/model-picker.mjs";import{ModelManagerController}from"../controller/common/model-manager.mjs";import{DownloadsController}from"../controller/common/downloads.mjs";import{AnnouncementsController}from"../controller/common/announcements.mjs";import{HistoryDatabase}from"../common/history.mjs";import{SimpleNotification}from"../common/notify.mjs";class FileNameFormView extends FormView{static fieldSets={"File Name":{filename:{class:StringInputView,config:{required:!0,placeholder:"Please enter a filename."}}}}}class LogoutButtonView extends View{static tagName="i";static className="fa-solid fa-right-from-bracket logout";async logout(){window.location="/logout"}async build(){let t=await super.build();return t.on("click",(()=>this.logout())),t.data("tooltip","Logout"),t}}class Application{static menuCategories={file:"File"};static adminMenuCategories={models:"Models",system:"System"};static filenameFormInputWidth=400;static filenameFormInputHeight=250;static logoShadowRGB=[0,0,0];static logoShadowOpacity=.5;static logoShadowSteps=10;static logoShadowOffset=2;static logoShadowSpread=0;static confirmViewWidth=500;static confirmViewHeight=200;constructor(t){this.config=t,this.publisher=new Publisher}async initialize(){this.tooltips=new TooltipHelper,this.container=document.querySelector(this.config.view.applicationContainer),isEmpty(this.container)?console.error(`Couldn't find application configuration using selector ${this.config.view.applicationContainer}, abandoning initialization.`):(this.model=new Model(this.config),this.menu=new MenuView(this.config),this.sidebar=new SidebarView(this.config),this.toolbar=new ToolbarView(this.config),this.windows=new WindowsView(this.config),this.notifications=new NotificationCenterView(this.config),this.history=new HistoryDatabase(this.config.history.size,this.config.debug),this.images=new ImageEditorView(this),this.container.appendChild(await this.menu.render()),this.container.appendChild(await this.sidebar.render()),this.container.appendChild(await this.toolbar.render()),this.container.appendChild(await this.images.render()),this.container.appendChild(await this.windows.render()),this.container.appendChild(await this.notifications.render()),await this.startAnimations(),await this.registerModelControllers(),await this.registerDownloadsControllers(),await this.registerInvocationControllers(),await this.registerMenuControllers(),await this.registerSidebarControllers(),await this.registerToolbarControllers(),await this.startAutosave(),await this.startKeepalive(),await this.startAnnouncements(),await this.registerLogout(),window.onpopstate=t=>this.popState(t),document.addEventListener("paste",(t=>this.onPaste(t))),document.addEventListener("keypress",(t=>this.onKeyPress(t))))}async startAnnouncements(){this.announcements=new AnnouncementsController(this),await this.announcements.initialize()}async startAnimations(){let t=document.querySelector("header h1");isEmpty(t)?console.warn("Can't find header logo, not binding animations."):window.addEventListener("mousemove",(e=>{let[i,o]=[e.clientX/window.innerWidth,e.clientY/window.innerHeight],s=[];for(let t=0;t<this.constructor.logoShadowSteps;t++){let[e,n]=[i*(t+1)*this.constructor.logoShadowOffset,o*(t+1)*this.constructor.logoShadowOffset],a=this.constructor.logoShadowOpacity-t/this.constructor.logoShadowSteps*this.constructor.logoShadowOpacity,r=`rgba(${this.constructor.logoShadowRGB.concat(a.toFixed(2)).join(",")})`;s.push(`${e}px ${n}px ${this.constructor.logoShadowSpread}px ${r}`)}t.style.textShadow=s.join(",")}))}async registerModelControllers(){this.modelManager=new ModelManagerController(this),await this.modelManager.initialize(),this.modelPicker=new ModelPickerController(this),await this.modelPicker.initialize()}async registerDownloadsControllers(){this.downloads=new DownloadsController(this),await this.downloads.initialize()}async registerInvocationControllers(){this.engine=new InvocationController(this),await this.engine.initialize()}getMenuCategories(){let t={...this.constructor.menuCategories};return isEmpty(window.enfugue)||!0!==window.enfugue.admin||(t={...t,...this.constructor.adminMenuCategories}),t.help="Help",t}async registerMenuControllers(){let t=this.getMenuCategories();this.menuControllers={};for(let e in t){let i=t[e];this.menuControllers[e]=[];try{let t=await import(`../controller/${e}/index.autogenerated.mjs`),o=await this.menu.addCategory(i);for(let i of t.Index)try{let t=(await import(`../controller/${e}/${i}`)).MenuController;if(isEmpty(t))throw"Module does not provide a 'MenuController' export.";if(!t.isDisabled()){let i=await o.addItem(t.menuName,t.menuIcon),s=new t(this);await s.initialize(),i.onClick((()=>s.onClick())),this.menuControllers[e].push(s)}}catch(t){console.warn("Couldn't import",e,"menu controller",i,t)}}catch(t){console.warn("Couldn't register controllers for menu",e,t)}}}async registerSidebarControllers(){let t=await import("../controller/sidebar/index.autogenerated.mjs");this.sidebarControllers=[];for(let e of t.Index){let t=(await import(`../controller/sidebar/${e}`)).SidebarController;if(isEmpty(t))throw"Module does not provide a 'SidebarController' export.";let i=new t(this);await i.initialize(),this.sidebarControllers.push(i)}}async registerToolbarControllers(){let t=await import("../controller/toolbar/index.autogenerated.mjs");this.toolbarControllers=[];for(let e of t.Index){let t=(await import(`../controller/toolbar/${e}`)).ToolbarController;if(isEmpty(t))throw"Module does not provide a 'ToolbarController' export.";let i=await this.toolbar.addItem(t.menuName,t.menuIcon),o=new t(this);await o.initialize(),i.onClick((()=>o.onClick())),this.toolbarControllers.push(o)}}async startKeepalive(){const t=this.config.model.status.interval||15e3,e=t=>{"ready"===t?this.publish("engineReady"):"busy"===t?this.publish("engineBusy"):"idle"===t?this.publish("engineIdle"):console.warn("Unknown status",t)};let i=document.querySelector("header");if(isEmpty(i))return void console.warn("No header found on page, not appending status view.");let o=await this.model.get(),s=new StatusView(this.config,o),n=await s.getNode();s.onStatusClicked((async()=>{await this.confirm("Stop engine and terminate any active invocations?")&&(await this.model.post("/invocation/stop"),this.notifications.push("info","Stopped","Engine successfully terminated."))})),e(o.status),i.appendChild(n.render()),setInterval((async()=>{try{let t=await this.model.get();o.status!==t.status&&e(t.status),s.updateStatus(t),o=t}catch{s.updateStatus("error")}}),t);let a=await this.model.get("/invocation"),r=null;for(let t of a)if("processing"===t.status){r=t;break}isEmpty(r)||(isEmpty(r)||isEmpty(r.metadata.tensorrt_build)?(this.notifications.push("info","Active Invocation Found","You have an image currently being generated, beginning monitoring process."),this.engine.canvasInvocation(r.uuid)):this.notifications.push("info","TensorRT Build in Progress",`You have a TensorRT engine build in progress for ${r.metadata.tensorrt_build.model}. You'll receive a notification in this window when it is complete. The engine will remain unavailable until that time.`)),setInterval((async()=>{try{let t,e=await this.model.get("/invocation");for(let i of e)"processing"===i.status&&(null!==r&&r.id===i.id||(t=i)),isEmpty(r)||i.id!==r.id||i.status===r.status||("completed"===i.status?this.publish("invocationComplete",i):this.publish("invocationError",i),r=null);isEmpty(t)||(this.publish("invocationBegin",t),r=t)}catch(t){console.error(t)}}),t)}async registerLogout(){if(!isEmpty(window.enfugue.user)&&"noauth"!==window.enfugue.user){let t=new LogoutButtonView(this.config);document.querySelector("header").appendChild((await t.getNode()).render())}}async startAutosave(){try{let t=await this.history.getCurrentState();isEmpty(t)||(this.setState(t),this.notifications.push("info","Session Restored","Your last autosaved session was successfully loaded."));const e=this.config.model.autosave.interval||3e4;setInterval((()=>this.autosave()),e)}catch(t){console.error(t),this.notifications.push("warning","History Disabled","Couldn't open IndexedDB, history and autosave are disabled.")}}async autosave(t=!0){try{await this.history.setCurrentState(this.getState()),t&&SimpleNotification.notify("Session autosaved!",2e3)}catch(t){console.error("Couldn't autosave",t)}}subscribe(t,e){this.publisher.subscribe(t,e)}unsubscribe(t,e){this.publisher.unsubscribe(t,e)}async publish(t,e=null){this.publisher.publish(t,e)}spawnConfirmForm(t,e,i,o=!0,s=!1){return new Promise((async(n,a)=>{let r,l=!1,h=new t(this.config,i);h.onSubmit((()=>{l=!0,n(!0),o&&r.remove()})),h.onCancel((()=>{l=!0,n(!1),r.remove()})),r=await this.windows.spawnWindow(e,h,this.constructor.confirmViewWidth,this.constructor.confirmViewHeight),r.onClose((()=>{!l&&s?a():n(!1),l=!0}))}))}confirm(t,e=!0){return this.spawnConfirmForm(ConfirmFormView,"Confirm",t,e)}yesNo(t,e=!0){return this.spawnConfirmForm(YesNoFormView,"Yes or No",t,e,!0)}async saveAs(t,e,i,o){let s=new Blob([e],i);return this.saveBlobAs(t,s,o)}async saveBlobAs(t,e,i){i.startsWith(".")||(i=`.${i}`);let o=window.URL.createObjectURL(e),s=new FileNameFormView(this.config),n=await this.windows.spawnWindow(t,s,this.constructor.filenameFormInputWidth,this.constructor.filenameFormInputHeight);s.onCancel((()=>n.close())),s.onSubmit((t=>{let e=t.filename;e.endsWith(i)&&(e=e.substring(0,e.length-i.length));let s=document.createElement("a");s.setAttribute("download",`${e}${i}`),s.href=o,document.body.appendChild(s),window.requestAnimationFrame((()=>{s.dispatchEvent(createEvent("click")),document.body.removeChild(s),n.remove()}))})),n.onClose((()=>window.URL.revokeObjectURL(o)))}async onPaste(t){let e=(t.clipboardData||t.originalEvent.clipboardData).items;for(let t of e)if("file"===t.kind){let e=t.getAsFile(),i=new FileReader;i.onload=t=>this.images.addImageNode(t.target.result,"Pasted Image"),i.readAsDataURL(e)}else t.getAsString((t=>this.onTextPaste(t)))}async onImagePaste(t){let e=new ImageView(this.config,t);await e.waitForLoad(),this.images.addNode(ImageEditorImageNodeView,"Pasted Image",e,0,0,e.width,e.height)}async onTextPaste(t){t.startsWith("<html>")||console.warn("Text paste",t)}getStatefulControllers(){let t=[this.modelPicker].concat(this.toolbarControllers).concat(this.sidebarControllers);for(let e in this.menuControllers)t=t.concat(this.menuControllers[e]);return t}getState(){let t={images:this.images.getState()},e=this.getStatefulControllers();for(let i of e)t={...t,...i.getState()};return t}shouldSaveState(){let t=this.getState();return!(isEmpty(t.prompts)||isEmpty(t.prompts.prompt)&&isEmpty(t.prompts.negativePrompt))||!isEmpty(t.images)}async setState(t,e=!1){!0===e&&this.shouldSaveState()&&(await this.autosave(!1),await this.history.flush(t));let i=this.getStatefulControllers();for(let e of i)await e.setState(t);isEmpty(t.canvas)||(isEmpty(t.canvas.width)||(this.images.width=t.canvas.width),isEmpty(t.canvas.height)||(this.images.height=t.canvas.height)),void 0!==t.images&&null!==t.images&&(this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.setState(t.images))}async resetState(t=!0){let e={images:[]},i=this.getStatefulControllers();for(let t of i)e={...e,...t.getDefaultState()};await this.setState(e,t)}async initializeStateFromImage(t,e=!0){try{let i={},o=await this.yesNo("Would you like to keep settings?<br /><br />This will maintain things like prompts and other global settings the same while only changing the dimensions to match the image."),s=this.getStatefulControllers();for(let t of s)i=o?{...i,...t.getState()}:{...i,...t.getDefaultState()};isEmpty(i.canvas)&&(i.canvas={}),i.canvas.width=t.width,i.canvas.height=t.height,i.images=[ImageEditorView.getNodeDataForImage(t)],this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.width=t.width,this.images.height=t.height,await this.setState(i,e)}catch(t){}}onKeyPress(t){}async popState(t){}}export{Application};
+import{isEmpty,getQueryParameters,getDataParameters,waitFor,createEvent}from"../base/helpers.mjs";import{Publisher}from"../base/publisher.mjs";import{TooltipHelper}from"../common/tooltip.mjs";import{MenuView,SidebarView,ToolbarView}from"../view/menu.mjs";import{StatusView}from"../view/status.mjs";import{NotificationCenterView}from"../view/notifications.mjs";import{WindowsView}from"../view/nodes/windows.mjs";import{ImageEditorView,ImageEditorNodeView,ImageEditorImageNodeView}from"../view/nodes/image-editor.mjs";import{ImageView}from"../view/image.mjs";import{Model}from"../model/enfugue.mjs";import{ConfirmFormView,YesNoFormView}from"../view/forms/confirm.mjs";import{View}from"../view/base.mjs";import{FormView}from"../view/forms/base.mjs";import{StringInputView}from"../view/forms/input.mjs";import{InvocationController}from"../controller/common/invocation.mjs";import{ModelPickerController}from"../controller/common/model-picker.mjs";import{ModelManagerController}from"../controller/common/model-manager.mjs";import{DownloadsController}from"../controller/common/downloads.mjs";import{AnnouncementsController}from"../controller/common/announcements.mjs";import{HistoryDatabase}from"../common/history.mjs";import{SimpleNotification}from"../common/notify.mjs";class FileNameFormView extends FormView{static fieldSets={"File Name":{filename:{class:StringInputView,config:{required:!0,placeholder:"Please enter a filename."}}}}}class LogoutButtonView extends View{static tagName="i";static className="fa-solid fa-right-from-bracket logout";async logout(){window.location="/logout"}async build(){let t=await super.build();return t.on("click",(()=>this.logout())),t.data("tooltip","Logout"),t}}class Application{static menuCategories={file:"File"};static adminMenuCategories={models:"Models",system:"System"};static filenameFormInputWidth=400;static filenameFormInputHeight=250;static logoShadowRGB=[0,0,0];static logoShadowOpacity=.5;static logoShadowSteps=10;static logoShadowOffset=2;static logoShadowSpread=0;static confirmViewWidth=500;static confirmViewHeight=200;constructor(t){this.config=t,this.publisher=new Publisher}async initialize(){this.tooltips=new TooltipHelper,this.container=document.querySelector(this.config.view.applicationContainer),isEmpty(this.container)?console.error(`Couldn't find application configuration using selector ${this.config.view.applicationContainer}, abandoning initialization.`):(this.model=new Model(this.config),console.log(this.model),this.menu=new MenuView(this.config),this.sidebar=new SidebarView(this.config),this.toolbar=new ToolbarView(this.config),this.windows=new WindowsView(this.config),this.notifications=new NotificationCenterView(this.config),this.history=new HistoryDatabase(this.config.history.size,this.config.debug),this.images=new ImageEditorView(this),this.container.appendChild(await this.menu.render()),this.container.appendChild(await this.sidebar.render()),this.container.appendChild(await this.toolbar.render()),this.container.appendChild(await this.images.render()),this.container.appendChild(await this.windows.render()),this.container.appendChild(await this.notifications.render()),await this.startAnimations(),await this.registerModelControllers(),await this.registerDownloadsControllers(),await this.registerInvocationControllers(),await this.registerMenuControllers(),await this.registerSidebarControllers(),await this.registerToolbarControllers(),await this.startAutosave(),await this.startKeepalive(),await this.startAnnouncements(),await this.registerLogout(),window.onpopstate=t=>this.popState(t),document.addEventListener("paste",(t=>this.onPaste(t))),document.addEventListener("keypress",(t=>this.onKeyPress(t))))}async startAnnouncements(){this.announcements=new AnnouncementsController(this),await this.announcements.initialize()}async startAnimations(){let t=document.querySelector("header h1");isEmpty(t)?console.warn("Can't find header logo, not binding animations."):window.addEventListener("mousemove",(e=>{let[i,o]=[e.clientX/window.innerWidth,e.clientY/window.innerHeight],s=[];for(let t=0;t<this.constructor.logoShadowSteps;t++){let[e,n]=[i*(t+1)*this.constructor.logoShadowOffset,o*(t+1)*this.constructor.logoShadowOffset],a=this.constructor.logoShadowOpacity-t/this.constructor.logoShadowSteps*this.constructor.logoShadowOpacity,r=`rgba(${this.constructor.logoShadowRGB.concat(a.toFixed(2)).join(",")})`;s.push(`${e}px ${n}px ${this.constructor.logoShadowSpread}px ${r}`)}t.style.textShadow=s.join(",")}))}async registerModelControllers(){this.modelManager=new ModelManagerController(this),await this.modelManager.initialize(),this.modelPicker=new ModelPickerController(this),await this.modelPicker.initialize()}async registerDownloadsControllers(){this.downloads=new DownloadsController(this),await this.downloads.initialize()}async registerInvocationControllers(){this.engine=new InvocationController(this),await this.engine.initialize()}getMenuCategories(){let t={...this.constructor.menuCategories};return isEmpty(window.enfugue)||!0!==window.enfugue.admin||(t={...t,...this.constructor.adminMenuCategories}),t.help="Help",t}async registerMenuControllers(){let t=this.getMenuCategories();this.menuControllers={};for(let e in t){let i=t[e];this.menuControllers[e]=[];try{let t=await import(`../controller/${e}/index.autogenerated.mjs`),o=await this.menu.addCategory(i);for(let i of t.Index)try{let t=(await import(`../controller/${e}/${i}`)).MenuController;if(isEmpty(t))throw"Module does not provide a 'MenuController' export.";if(!t.isDisabled()){let i=await o.addItem(t.menuName,t.menuIcon),s=new t(this);await s.initialize(),i.onClick((()=>s.onClick())),this.menuControllers[e].push(s)}}catch(t){console.warn("Couldn't import",e,"menu controller",i,t)}}catch(t){console.warn("Couldn't register controllers for menu",e,t)}}}async registerSidebarControllers(){let t=await import("../controller/sidebar/index.autogenerated.mjs");this.sidebarControllers=[];for(let e of t.Index){let t=(await import(`../controller/sidebar/${e}`)).SidebarController;if(isEmpty(t))throw"Module does not provide a 'SidebarController' export.";let i=new t(this);await i.initialize(),this.sidebarControllers.push(i)}}async registerToolbarControllers(){let t=await import("../controller/toolbar/index.autogenerated.mjs");this.toolbarControllers=[];for(let e of t.Index){let t=(await import(`../controller/toolbar/${e}`)).ToolbarController;if(isEmpty(t))throw"Module does not provide a 'ToolbarController' export.";let i=await this.toolbar.addItem(t.menuName,t.menuIcon),o=new t(this);await o.initialize(),i.onClick((()=>o.onClick())),this.toolbarControllers.push(o)}}async startKeepalive(){const t=this.config.model.status.interval||1e4,e=t=>{"ready"===t?this.publish("engineReady"):"busy"===t?this.publish("engineBusy"):"idle"===t?this.publish("engineIdle"):console.warn("Unknown status",t)};let i=document.querySelector("header");if(isEmpty(i))return void console.warn("No header found on page, not appending status view.");let o=await this.model.get(),s=new StatusView(this.config,o),n=await s.getNode();s.onStatusClicked((async()=>{await this.confirm("Stop engine and terminate any active invocations?")&&(await this.model.post("/invocation/stop"),this.notifications.push("info","Stopped","Engine successfully terminated."))})),e(o.status),i.appendChild(n.render()),setInterval((async()=>{try{let t=await this.model.get();o.status!==t.status&&e(t.status),s.updateStatus(t),o=t}catch{s.updateStatus("error")}}),t);let a=await this.model.get("/invocation"),r=null;for(let t of a)if("processing"===t.status){r=t;break}isEmpty(r)||(isEmpty(r)||isEmpty(r.metadata.tensorrt_build)?(this.notifications.push("info","Active Invocation Found","You have an image currently being generated, beginning monitoring process."),this.engine.canvasInvocation(r.uuid)):this.notifications.push("info","TensorRT Build in Progress",`You have a TensorRT engine build in progress for ${r.metadata.tensorrt_build.model}. You'll receive a notification in this window when it is complete. The engine will remain unavailable until that time.`)),setInterval((async()=>{try{let t,e=await this.model.get("/invocation");for(let i of e)"processing"===i.status&&(null!==r&&r.id===i.id||(t=i)),isEmpty(r)||i.id!==r.id||i.status===r.status||("completed"===i.status?this.publish("invocationComplete",i):this.publish("invocationError",i),r=null);isEmpty(t)||(this.publish("invocationBegin",t),r=t)}catch(t){console.error(t)}}),t)}async registerLogout(){if(!isEmpty(window.enfugue.user)&&"noauth"!==window.enfugue.user){let t=new LogoutButtonView(this.config);document.querySelector("header").appendChild((await t.getNode()).render())}}async startAutosave(){try{let t=await this.history.getCurrentState();isEmpty(t)||(this.setState(t),this.notifications.push("info","Session Restored","Your last autosaved session was successfully loaded."));const e=this.config.model.autosave.interval||3e4;setInterval((()=>this.autosave()),e)}catch(t){console.error(t),this.notifications.push("warning","History Disabled","Couldn't open IndexedDB, history and autosave are disabled.")}}async autosave(t=!0){try{await this.history.setCurrentState(this.getState()),t&&SimpleNotification.notify("Session autosaved!",2e3)}catch(t){console.error("Couldn't autosave",t)}}subscribe(t,e){this.publisher.subscribe(t,e)}unsubscribe(t,e){this.publisher.unsubscribe(t,e)}async publish(t,e=null){this.publisher.publish(t,e)}spawnConfirmForm(t,e,i,o=!0,s=!1){return new Promise((async(n,a)=>{let r,l=!1,h=new t(this.config,i);h.onSubmit((()=>{l=!0,n(!0),o&&r.remove()})),h.onCancel((()=>{l=!0,n(!1),r.remove()})),r=await this.windows.spawnWindow(e,h,this.constructor.confirmViewWidth,this.constructor.confirmViewHeight),r.onClose((()=>{!l&&s?a():n(!1),l=!0}))}))}confirm(t,e=!0){return this.spawnConfirmForm(ConfirmFormView,"Confirm",t,e)}yesNo(t,e=!0){return this.spawnConfirmForm(YesNoFormView,"Yes or No",t,e,!0)}async saveAs(t,e,i,o){let s=new Blob([e],i);return this.saveBlobAs(t,s,o)}async saveBlobAs(t,e,i){i.startsWith(".")||(i=`.${i}`);let o=window.URL.createObjectURL(e),s=new FileNameFormView(this.config),n=await this.windows.spawnWindow(t,s,this.constructor.filenameFormInputWidth,this.constructor.filenameFormInputHeight);s.onCancel((()=>n.close())),s.onSubmit((t=>{let e=t.filename;e.endsWith(i)&&(e=e.substring(0,e.length-i.length));let s=document.createElement("a");s.setAttribute("download",`${e}${i}`),s.href=o,document.body.appendChild(s),window.requestAnimationFrame((()=>{s.dispatchEvent(createEvent("click")),document.body.removeChild(s),n.remove()}))})),n.onClose((()=>window.URL.revokeObjectURL(o)))}async onPaste(t){let e=(t.clipboardData||t.originalEvent.clipboardData).items;for(let t of e)if("file"===t.kind){let e=t.getAsFile(),i=new FileReader;i.onload=t=>this.images.addImageNode(t.target.result,"Pasted Image"),i.readAsDataURL(e)}else t.getAsString((t=>this.onTextPaste(t)))}async onImagePaste(t){let e=new ImageView(this.config,t);await e.waitForLoad(),this.images.addNode(ImageEditorImageNodeView,"Pasted Image",e,0,0,e.width,e.height)}async onTextPaste(t){t.startsWith("<html>")||console.warn("Text paste",t)}getStatefulControllers(){let t=[this.modelPicker].concat(this.toolbarControllers).concat(this.sidebarControllers);for(let e in this.menuControllers)t=t.concat(this.menuControllers[e]);return t}getState(){let t={images:this.images.getState()},e=this.getStatefulControllers();for(let i of e)t={...t,...i.getState()};return t}shouldSaveState(){let t=this.getState();return!(isEmpty(t.prompts)||isEmpty(t.prompts.prompt)&&isEmpty(t.prompts.negativePrompt))||!isEmpty(t.images)}async setState(t,e=!1){!0===e&&this.shouldSaveState()&&(await this.autosave(!1),await this.history.flush(t));let i=this.getStatefulControllers();for(let e of i)await e.setState(t);isEmpty(t.canvas)||(isEmpty(t.canvas.width)||(this.images.width=t.canvas.width),isEmpty(t.canvas.height)||(this.images.height=t.canvas.height)),void 0!==t.images&&null!==t.images&&(this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.setState(t.images))}async resetState(t=!0){let e={images:[]},i=this.getStatefulControllers();for(let t of i)e={...e,...t.getDefaultState()};await this.setState(e,t)}async initializeStateFromImage(t,e=!0){try{let i={},o=await this.yesNo("Would you like to keep settings?<br /><br />This will maintain things like prompts and other global settings the same while only changing the dimensions to match the image."),s=this.getStatefulControllers();for(let t of s)i=o?{...i,...t.getState()}:{...i,...t.getDefaultState()};isEmpty(i.canvas)&&(i.canvas={}),i.canvas.width=t.width,i.canvas.height=t.height,i.images=[ImageEditorView.getNodeDataForImage(t)],this.engine.hideSampleChooser(),this.images.hideCurrentInvocation(),this.images.width=t.width,this.images.height=t.height,await this.setState(i,e)}catch(t){}}onKeyPress(t){}async popState(t){}}export{Application};
```

### Comparing `enfugue-0.1.1/enfugue/static/js/base/api.mjs` & `enfugue-0.1.2/enfugue/static/js/base/api.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/base/builder.mjs` & `enfugue-0.1.2/enfugue/static/js/base/builder.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/base/csv.mjs` & `enfugue-0.1.2/enfugue/static/js/base/csv.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/base/helpers.mjs` & `enfugue-0.1.2/enfugue/static/js/base/helpers.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/base/loader.mjs` & `enfugue-0.1.2/enfugue/static/js/base/loader.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/base/publisher.mjs` & `enfugue-0.1.2/enfugue/static/js/base/publisher.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/base/session.mjs` & `enfugue-0.1.2/enfugue/static/js/base/session.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/base/watcher.mjs` & `enfugue-0.1.2/enfugue/static/js/base/watcher.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/common/event-tracker.mjs` & `enfugue-0.1.2/enfugue/static/js/common/event-tracker.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/common/history.mjs` & `enfugue-0.1.2/enfugue/static/js/common/history.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/common/shadowbox.mjs` & `enfugue-0.1.2/enfugue/static/js/common/shadowbox.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/common/tooltip.mjs` & `enfugue-0.1.2/enfugue/static/js/common/tooltip.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/config/index.mjs` & `enfugue-0.1.2/enfugue/static/js/config/index.mjs`

 * *Files 17% similar despite different names*

```diff
@@ -1 +1 @@
-let Configuration={debug:!0,controller:{module:"index"},view:{applicationContainer:"enfugue-application",language:"en"},url:{root:"http://dev.enfugue.local/",api:"http://dev.enfugue.local/api/",baseTitle:"Enfugue",titleSeparator:" | "},history:{size:100},model:{cache:0,cookie:{name:"enfugue_token"},status:{interval:1e4},autosave:{interval:3e4},queue:{interval:5e3},downloads:{interval:5e3},invocation:{width:512,height:512,chunkingSize:64,chunkingBlur:64,guidanceScale:7.5,inferenceSteps:50,interval:1e3,upscaleDiffusionSteps:80,upscaleDiffusionGuidanceScale:10,upscaleDiffusionStrength:.15,upscaleDiffusionChunkingSize:64,upscaleDiffusionChunkingBlur:64,errors:{consecutive:2}}}};export{Configuration};
+let Configuration={debug:!1,controller:{module:"index"},view:{applicationContainer:"enfugue-application",language:"en"},url:{root:"http://dev.enfugue.local/",api:"http://dev.enfugue.local/api/",baseTitle:"Enfugue",titleSeparator:" | "},history:{size:100},model:{cache:0,cookie:{name:"enfugue_token"},status:{interval:1e4},autosave:{interval:3e4},queue:{interval:5e3},downloads:{interval:5e3},invocation:{width:512,height:512,chunkingSize:64,chunkingBlur:64,guidanceScale:7.5,inferenceSteps:50,interval:1e3,upscaleDiffusionSteps:80,upscaleDiffusionGuidanceScale:10,upscaleDiffusionStrength:.15,upscaleDiffusionChunkingSize:64,upscaleDiffusionChunkingBlur:64,errors:{consecutive:2}}}};export{Configuration};
```

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/base.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/common/announcements.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/common/announcements.mjs`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-import{isEmpty,waitFor,humanSize,humanDuration}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";import{View,ParentView}from"../../view/base.mjs";import{TableView}from"../../view/table.mjs";import{ButtonInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class AcknowledgeButtonInputView extends ButtonInputView{static className="download-input-view";static defaultValue="I Acknowledge"}class InitializationAnnouncementView extends View{async build(){let e=await super.build();return e.append(E.h2().content("Welcome to Enfugue")),e.append(E.p().content("Thank you for downloading Enfugue! I hope you enjoy it. Please read the following brief disclaimers before you begin.")),e.append(E.h3().content("Your Privacy")),e.append(E.p().content("Enfugue does not track usage in any way. Your images, prompts, configurations, and all other details only exist on your computer and are never sent elsewhere over a network or otherwise, unless specifically required by the user.")),e.append(E.p().content(E.span().content("Some resources, such as public model data, is provided by "),E.a().content("Hugging Face").href("https://huggingface.co/").target("_blank"),E.span().content(" and by using this application Enfugue will reach out to their servers to download resources as needed. By doing so, you agree to their "),E.a().content("Privacy Policy").href("https://huggingface.co/privacy").target("_blank"),E.span().content("."))),e.append(E.p().content("Additional resources may be downloaded from other providers at your request. Please review the privacy policy and terms of service of the resource providers stated when these resources are requested.")),e.append(E.h3().content("Terms of Service")),e.append(E.p().content("Enfugue makes no guarantees of this software's functionality, and by continuing you release Enfugue, Benjamin Paine, GitHub, Hugging Face, Stability AI, Runway, CivitAI, and all other parties whose software contributions are employed within Enfugue from any liability of any kind arising from use of the software, including but not limited to wear and tear on your hardware and expenses incurred by consuming bandwidth.")),e.append(E.p().content("Furthermore, you hold all the above parties blameless from any and all liability, damage, loss, and expense (including without limitation reasonable attorney’s fees and court costs) arising from claims against parties that Enfugue, or your use of the same as permitted by this Agreement, infringe the intellectual property rights of a third party.")),e.append(E.p().class("strong").content("Enfugue is and always will be free and open-source software.")),e.append(E.p().content("To support further development, please consider financially supporting it if you are able. Simply click 'About' under 'Help' above to see ways you can help keep Enfugue improving.")),e}}class DownloadAnnouncementHeaderView extends View{async build(){let e=await super.build();return e.content(E.h2().content("Downloads"),E.p().content("The following downloads are required by Enfugue to function. They are the base Stable Diffusion models, from which more tuned models are made. These models are used when you are not using any other models, as well as when calculating derived models."),E.p().content("Click 'Download Now' to being downloading them. If you do not download them now, they will be downloaded the first time they are needed.")),e}}class DownloadTableView extends TableView{static canSort=!1;static columns={model:"Model",size:"Size"};static columnFormatters={size:e=>humanSize(e)}}class UpdateAnnouncementHeaderView extends View{static releasesLink="https://github.com/painebenjamin/app.enfugue.ai/releases/";async build(){let e=await super.build();return e.content(E.h2().content("Updates"),E.p().content("An updated version of Enfugue is available. See below for details regarding new features and fixes."),E.p().content(E.span().content("If you are managing your own installation, simply executing "),E.createElement("code").content("pip install enfugue --update"),E.span().content(" will fetch the latest details. If you are using an easy installation, you will need to download the updated package. See below for any additional steps required.")),E.p().class("center").content(E.a().class("button").href(this.constructor.releasesLink).target("_blank").content("Download Now"))),e}}class UpdateAnnouncementView extends View{constructor(e,n){super(e),this.update=n}async build(){let e=await super.build();return e.content(E.h3().content(`Version ${this.update.version}`),E.p().addClass("note").content(`Released ${this.update.release}`),E.p().content(this.update.description)),e}}class AnnouncementsController extends Controller{static announcementsWindowWidth=800;static announcementsWindowHeight=1e3;async checkShowAnnouncements(){let e=await this.model.get("/announcements");if(!isEmpty(e)){let n=e.filter((e=>"initialize"===e.type)).length>0,t=e.filter((e=>"download"===e.type)),a=e.filter((e=>"update"===e.type)),o=new ParentView(this.config);if(await o.addClass("announcements-view"),n&&await o.addChild(InitializationAnnouncementView),!isEmpty(t)){await o.addChild(DownloadAnnouncementHeaderView);let e=await o.addChild(DownloadTableView,t);e.addButton("Download","fa-solid fa-download",(async n=>{let t=(await e.getNode()).find("tbody").findAll("tr");for(let e of t)e.find("td").getText()==n.model&&e.find("button").disabled(!0).addClass("disabled");this.download("checkpoint",n.url,n.model)}))}if(!isEmpty(a)){await o.addChild(UpdateAnnouncementHeaderView);for(let e of a)await o.addChild(UpdateAnnouncementView,e)}if(!o.isEmpty()){let e=await o.addChild(AcknowledgeButtonInputView),t=await this.spawnWindow("Announcements",o,this.constructor.announcementsWindowWidth,this.constructor.announcementsWindowHeight);if(e.onChange((()=>{t.remove()})),t.onClose((async()=>{await this.model.post("/announcements/snooze")})),n){let e=(await t.getNode()).findAll("enfugue-node-button");for(let n of e)n.hide()}}}}async initialize(){this.checkShowAnnouncements(),setInterval((()=>this.checkShowAnnouncements()),864e5)}}export{AnnouncementsController};
+import{isEmpty,waitFor,humanSize,humanDuration,titleCase}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{Controller}from"../base.mjs";import{View,ParentView}from"../../view/base.mjs";import{TableView}from"../../view/table.mjs";import{FormView}from"../../view/forms/base.mjs";import{ButtonInputView,StringInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class AcknowledgeButtonInputView extends ButtonInputView{static className="download-input-view";static defaultValue="I Acknowledge"}class InitializationAnnouncementView extends View{constructor(e,t){super(e),this.directories=t,this.formView=new FormView(e);for(let e in this.directories)this.formView.addInput("Directories",StringInputView,e,titleCase(e),{required:!0,value:this.directories[e]})}async build(){let e=await super.build();return e.append(E.h2().content("Welcome to Enfugue")),e.append(E.p().content("Thank you for downloading Enfugue! I hope you enjoy it. Please read the following brief disclaimers before you begin.")),e.append(E.h3().content("Your Privacy")),e.append(E.p().content("Enfugue does not track usage in any way. Your images, prompts, configurations, and all other details only exist on your computer and are never sent elsewhere over a network or otherwise, unless specifically required by the user.")),e.append(E.p().content(E.span().content("Some resources, such as public model data, is provided by "),E.a().content("Hugging Face").href("https://huggingface.co/").target("_blank"),E.span().content(" and by using this application Enfugue will reach out to their servers to download resources as needed. By doing so, you agree to their "),E.a().content("Privacy Policy").href("https://huggingface.co/privacy").target("_blank"),E.span().content("."))),e.append(E.p().content("Additional resources may be downloaded from other providers at your request. Please review the privacy policy and terms of service of the resource providers stated when these resources are requested.")),e.append(E.h3().content("Terms of Service")),e.append(E.p().content("Enfugue makes no guarantees of this software's functionality, and by continuing you release Enfugue, Benjamin Paine, GitHub, Hugging Face, Stability AI, Runway, CivitAI, and all other parties whose software contributions are employed within Enfugue from any liability of any kind arising from use of the software, including but not limited to wear and tear on your hardware and expenses incurred by consuming bandwidth.")),e.append(E.p().content("Furthermore, you hold all the above parties blameless from any and all liability, damage, loss, and expense (including without limitation reasonable attorney’s fees and court costs) arising from claims against parties that Enfugue, or your use of the same as permitted by this Agreement, infringe the intellectual property rights of a third party.")),e.append(E.p().class("strong").content("Enfugue is and always will be free and open-source software.")),e.append(E.p().content("To support further development, please consider financially supporting it if you are able. Simply click 'About' under 'Help' above to see ways you can help keep Enfugue improving.")),e.append(E.h2().content("Directories")),e.append(E.p().content("Use these fields to specify the directories to use for your installation. These do not need to be solely used by Enfugue, and Enfugue will never delete anything from these directories unless you specifically request.")),e.append(await this.formView.getNode()),e}}class DownloadAnnouncementHeaderView extends View{async build(){let e=await super.build();return e.content(E.h2().content("Downloads"),E.p().content("The following downloads are required by Enfugue to function. They are the base Stable Diffusion models, from which more tuned models are made. These models are used when you are not using any other models, as well as when calculating derived models."),E.p().content("Click 'Download Now' to being downloading them. If you do not download them now, they will be downloaded the first time they are needed.")),e}}class DownloadTableView extends TableView{static canSort=!1;static columns={model:"Model",size:"Size"};static columnFormatters={size:e=>humanSize(e)}}class UpdateAnnouncementHeaderView extends View{static releasesLink="https://github.com/painebenjamin/app.enfugue.ai/releases/";async build(){let e=await super.build();return e.content(E.h2().content("Updates"),E.p().content("An updated version of Enfugue is available. See below for details regarding new features and fixes."),E.p().content(E.span().content("If you are managing your own installation, simply executing "),E.createElement("code").content("pip install enfugue --update"),E.span().content(" will fetch the latest details. If you are using an easy installation, you will need to download the updated package. See below for any additional steps required.")),E.p().class("center").content(E.a().class("button").href(this.constructor.releasesLink).target("_blank").content("Download Now"))),e}}class UpdateAnnouncementView extends View{constructor(e,t){super(e),this.update=t}async build(){let e=await super.build();return e.content(E.h3().content(`Version ${this.update.version}`),E.p().addClass("note").content(`Released ${this.update.release}`),E.p().content(this.update.description)),e}}class AnnouncementsController extends Controller{static announcementsWindowWidth=800;static announcementsWindowHeight=1e3;async checkShowAnnouncements(){let e=await this.model.get("/announcements");if(!isEmpty(e)){let t,n=e.filter((e=>"initialize"===e.type)),o=e.filter((e=>"download"===e.type)),i=e.filter((e=>"update"===e.type)),a=new ParentView(this.config);if(await a.addClass("announcements-view"),!isEmpty(n)){let e=(await a.addChild(InitializationAnnouncementView,n[0].directories)).formView;e.onChange((()=>{t.disable(),e.setError("You must submit directory changes before continuing.")})),e.onSubmit((async n=>{await this.model.post("installation",null,null,{directories:n}),this.notify("info","Success","Directories successfully set."),e.clearError(),e.enable(),t.enable()}))}if(!isEmpty(o)){await a.addChild(DownloadAnnouncementHeaderView);let e=await a.addChild(DownloadTableView,o);e.addButton("Download","fa-solid fa-download",(async t=>{let n=(await e.getNode()).find("tbody").findAll("tr");for(let e of n)e.find("td").getText()==t.model&&e.find("button").disabled(!0).addClass("disabled");this.download("checkpoint",t.url,t.model)}))}if(!isEmpty(i)){await a.addChild(UpdateAnnouncementHeaderView);for(let e of i)await a.addChild(UpdateAnnouncementView,e)}if(!a.isEmpty()){t=await a.addChild(AcknowledgeButtonInputView);let e=await this.spawnWindow("Announcements",a,this.constructor.announcementsWindowWidth,this.constructor.announcementsWindowHeight);if(t.onChange((()=>{e.remove()})),e.onClose((async()=>{await this.model.post("/announcements/snooze")})),!isEmpty(n)){let t=(await e.getNode()).findAll("enfugue-node-button");for(let e of t)e.hide()}}}}async initialize(){this.checkShowAnnouncements(),setInterval((()=>this.checkShowAnnouncements()),864e5)}}export{AnnouncementsController};
```

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/common/downloads.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/common/downloads.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/common/invocation.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/common/invocation.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/common/model-manager.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/common/model-manager.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/common/model-picker.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/common/model-picker.mjs`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-import{Controller}from"../base.mjs";import{TableView}from"../../view/table.mjs";import{View}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{SearchListInputView}from"../../view/forms/input.mjs";import{isEmpty,waitFor}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";const E=new ElementBuilder;class ModelPickerInputView extends SearchListInputView{static placeholder="Start typing to search models…"}class ModelTensorRTTableView extends TableView{constructor(e,t,i){super(e,t),this.buildEngine=i}static canSort=!1;static columnFormatters={Build:function(e,t){if(!0===e)return E.span().content("Ready");{let i=E.button().content("Build").on("click",(async()=>{try{i.disabled(!0).addClass("loading-bar loading"),await this.buildEngine(t),i.removeClass("loading-bar").removeClass("loading").content("Ready")}catch(e){i.removeClass("loading-bar loading").disabled(!1)}}));return"building"===e&&i.disabled(!0).addClass("loading-bar loading"),i}}}}class ModelTensorRTStatusView extends View{static tagNam="enfugue-tensorrt-status-view";static supportedNetworks={unet:"UNet",controlled_unet:"Controlled UNet",inpaint_unet:"Inpainting UNet"};static tensorRTDescription=["TensorRT is a technology created by Nvidia that transforms an AI model into one that takes advantage of hardware acceleration available on Nvidia GPUs.","As there are numerous varying architectures used by Nvidia that support this technology, these engines must be compiled by an architecture compatible with your actual hardware, rather than distributed by AI model providers.","The compilation time for each model varies, but generally takes between 15 and 30 minutes each. You can expect between 50% and 100% faster inference speeds during the engine's respective step(s).","The compiled engine is only useable for a model with the same checkpoint, LoRA, Textual Inversion and engine size. If you change any of those details about this model, it will require recompilation. You can safely change model prompts as desired without requiring a new engine."];static networkDescriptions={unet:"The network used when creating images with a prompt or base image.",controlled_unet:"The network used when creating images with a control image.",inpaint_unet:"The network used when inpainting or outpainting."};constructor(e,t,i){super(e),this.status=t,this.buildEngine=i}get tableData(){return Object.getOwnPropertyNames(this.constructor.supportedNetworks).map((e=>({"Network Name":this.constructor.supportedNetworks[e],Description:this.constructor.networkDescriptions[e],Build:this.status.building===e?"building":this.status[`${e}_ready`]})))}getNameFromLabel(e){for(let t in this.constructor.supportedNetworks)if(this.constructor.supportedNetworks[t]===e)return t;throw`Unknown network ${e}`}async build(){let e=await super.build(),t=new ModelTensorRTTableView(this.config,this.tableData,(e=>this.buildEngine(this.getNameFromLabel(e["Network Name"]))));for(let t of this.constructor.tensorRTDescription)e.append(E.p().class("margin").content(t));return e.append(await t.getNode())}}class ModelPickerFormView extends FormView{static className="model-picker";static autoSubmit=!0;static fieldSets={Model:{model:{class:ModelPickerInputView}}};static tensorRTLogo="/static/img/brand/tensorrt.png";setTensorRTStatus(e,t){let i=this.node.find("#tensorrt");if(e.supported){let s=ModelTensorRTStatusView.supportedNetworks,n=Object.getOwnPropertyNames(s),o=n.length,a=n.reduce(((t,i)=>(t[i]=e[`${i}_ready`],t)),{}),r=Object.values(a).filter((e=>e)).length;isEmpty(i)?(i=E.div().id("tensorrt").append(E.img().src(this.constructor.tensorRTLogo),E.span().class("fraction").content(E.span().content(`${r}`),E.span().content(`${o}`))).on("click",(()=>t())),this.node.append(i)):i.off("click").on("click",(()=>t())).find("span.fraction").content(E.span().content(`${r}`),E.span().content(`${o}`)),e.ready?i.addClass("ready").data("tooltip","TensorRT is <strong>ready</strong>"):i.removeClass("ready").data("tooltip","TensorRT is <strong>not ready</strong>")}else isEmpty(i)||this.node.remove(i)}}class ModelPickerController extends Controller{static tensorRTStatusWindowWidth=500;static tensorRTStatusWindowHeight=750;getState(){return{model:this.formView.values}}getDefaultState(){return{model:null}}setState(e){isEmpty(e.model)||this.formView.setValues(e.model).then((()=>this.formView.submit()))}async buildEngine(e,t){await this.model.post(`/models/${e}/tensorrt/${t}`),this.notify("info","Build Started","The engine will be busy throughout this TensorRT build. You will see a notification when it is complete, and the status indicator in the top bar will show ready or idle."),await waitFor((()=>(console.log("Built engines are",this.builtEngines),!isEmpty(this.builtEngines[e])&&-1!==this.builtEngines[e].indexOf(t))),{interval:5e3})}async showBuildTensorRT(e){let t=await e.getTensorRTStatus(),i=await this.getCurrentEngineBuildProcess();isEmpty(i)||i.metadata.tensorrt_build.model!==e.name||(t.building=i.metadata.tensorrt_build.network);let s=new ModelTensorRTStatusView(this.config,t,(t=>this.buildEngine(e.name,t)));return await this.spawnWindow(`${e.name} TensorRT Status`,s,this.constructor.tensorRTStatusWindowWidth,this.constructor.tensorRTStatusWindowHeight)}async getCurrentEngineBuildProcess(){let e=await this.model.get("/invocation");for(let t of e)if(void 0!==t.metadata&&void 0!==t.metadata.tensorrt_build&&-1!==["queued","processing"].indexOf(t.status))return t;return null}async initialize(){this.builtEngines={},ModelPickerInputView.defaultOptions=async()=>(await this.model.DiffusionModel.queryAll()).map((e=>e.name)),this.formView=new ModelPickerFormView(this.config),this.formView.onSubmit((async e=>{try{let t=await this.model.DiffusionModel.query({name:e.model}),i=await t.getTensorRTStatus();this.publish("modelPickerChange",t),this.engine.model=e.model,this.formView.setTensorRTStatus(i,(()=>this.showBuildTensorRT(t)))}catch(e){this.formView.setValues({model:null})}})),this.application.container.appendChild(await this.formView.render()),this.subscribe("invocationComplete",(e=>{if(!isEmpty(e.metadata)&&!isEmpty(e.metadata.tensorrt_build)){let t=e.metadata.tensorrt_build.network,i=ModelTensorRTStatusView.supportedNetworks[t],s=e.metadata.tensorrt_build.model;this.notify("info","TensorRT Engine Build Complete",`Successfully built ${s} ${i} TensorRT Engine.`),isEmpty(this.builtEngines[s])&&(this.builtEngines[s]=[]),this.builtEngines[s].push(t)}}))}}export{ModelPickerController};
+import{Controller}from"../base.mjs";import{TableView}from"../../view/table.mjs";import{View}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{SearchListInputView}from"../../view/forms/input.mjs";import{isEmpty,waitFor}from"../../base/helpers.mjs";import{ElementBuilder}from"../../base/builder.mjs";const E=new ElementBuilder;class ModelPickerInputView extends SearchListInputView{static placeholder="Start typing to search models…"}class ModelTensorRTTableView extends TableView{constructor(t,e,i){super(t,e),this.buildEngine=i}static canSort=!1;static columnFormatters={Build:function(t,e){if(!0===t)return E.span().content("Ready");{let i=E.button().content("Build").on("click",(async()=>{try{i.disabled(!0).addClass("loading-bar loading"),await this.buildEngine(e),i.removeClass("loading-bar").removeClass("loading").content("Ready")}catch(t){i.removeClass("loading-bar loading").disabled(!1)}}));return"building"===t&&i.disabled(!0).addClass("loading-bar loading"),i}}}}class ModelTensorRTStatusView extends View{static tagNam="enfugue-tensorrt-status-view";static supportedNetworks={unet:"UNet",controlled_unet:"Controlled UNet",inpaint_unet:"Inpainting UNet"};static tensorRTDescription=["TensorRT is a technology created by Nvidia that transforms an AI model into one that takes advantage of hardware acceleration available on Nvidia GPUs.","As there are numerous varying architectures used by Nvidia that support this technology, these engines must be compiled by an architecture compatible with your actual hardware, rather than distributed by AI model providers.","The compilation time for each model varies, but generally takes between 15 and 30 minutes each. You can expect between 50% and 100% faster inference speeds during the engine's respective step(s).","The compiled engine is only useable for a model with the same checkpoint, LoRA, Textual Inversion and engine size. If you change any of those details about this model, it will require recompilation. You can safely change model prompts as desired without requiring a new engine."];static networkDescriptions={unet:"The network used when creating images with a prompt or base image.",controlled_unet:"The network used when creating images with a control image.",inpaint_unet:"The network used when inpainting or outpainting."};constructor(t,e,i){super(t),this.status=e,this.buildEngine=i}get tableData(){return Object.getOwnPropertyNames(this.constructor.supportedNetworks).map((t=>({"Network Name":this.constructor.supportedNetworks[t],Description:this.constructor.networkDescriptions[t],Build:this.status.building===t?"building":this.status[`${t}_ready`]})))}getNameFromLabel(t){for(let e in this.constructor.supportedNetworks)if(this.constructor.supportedNetworks[e]===t)return e;throw`Unknown network ${t}`}async build(){let t=await super.build(),e=new ModelTensorRTTableView(this.config,this.tableData,(t=>this.buildEngine(this.getNameFromLabel(t["Network Name"]))));for(let e of this.constructor.tensorRTDescription)t.append(E.p().class("margin").content(e));return t.append(await e.getNode())}}class ModelPickerFormView extends FormView{static className="model-picker";static autoSubmit=!0;static fieldSets={Model:{model:{class:ModelPickerInputView}}};static tensorRTLogo="/static/img/brand/tensorrt.png";setTensorRTStatus(t,e){let i=this.node.find("#tensorrt");if(t.supported){let s=ModelTensorRTStatusView.supportedNetworks,n=Object.getOwnPropertyNames(s),o=n.length,a=n.reduce(((e,i)=>(e[i]=t[`${i}_ready`],e)),{}),r=Object.values(a).filter((t=>t)).length;isEmpty(i)?(i=E.div().id("tensorrt").append(E.img().src(this.constructor.tensorRTLogo),E.span().class("fraction").content(E.span().content(`${r}`),E.span().content(`${o}`))).on("click",(()=>e())),this.node.append(i)):i.off("click").on("click",(()=>e())).find("span.fraction").content(E.span().content(`${r}`),E.span().content(`${o}`)),t.ready?i.addClass("ready").data("tooltip","TensorRT is <strong>ready</strong>"):i.removeClass("ready").data("tooltip","TensorRT is <strong>not ready</strong>")}else isEmpty(i)||this.node.remove(i)}}class ModelPickerController extends Controller{static tensorRTStatusWindowWidth=500;static tensorRTStatusWindowHeight=750;getState(){return{model:this.formView.values}}getDefaultState(){return{model:null}}setState(t){isEmpty(t.model)||this.formView.setValues(t.model).then((()=>this.formView.submit()))}async buildEngine(t,e){await this.model.post(`/models/${t}/tensorrt/${e}`),this.notify("info","Build Started","The engine will be busy throughout this TensorRT build. You will see a notification when it is complete, and the status indicator in the top bar will show ready or idle."),await waitFor((()=>(console.log("Built engines are",this.builtEngines),!isEmpty(this.builtEngines[t])&&-1!==this.builtEngines[t].indexOf(e))),{interval:5e3})}async showBuildTensorRT(t){let e=await t.getTensorRTStatus(),i=await this.getCurrentEngineBuildProcess();isEmpty(i)||i.metadata.tensorrt_build.model!==t.name||(e.building=i.metadata.tensorrt_build.network);let s=new ModelTensorRTStatusView(this.config,e,(e=>this.buildEngine(t.name,e)));return await this.spawnWindow(`${t.name} TensorRT Status`,s,this.constructor.tensorRTStatusWindowWidth,this.constructor.tensorRTStatusWindowHeight)}async getCurrentEngineBuildProcess(){let t=await this.model.get("/invocation");for(let e of t)if(void 0!==e.metadata&&void 0!==e.metadata.tensorrt_build&&-1!==["queued","processing"].indexOf(e.status))return e;return null}async initialize(){this.builtEngines={},ModelPickerInputView.defaultOptions=async()=>(await this.model.DiffusionModel.queryAll()).map((t=>t.name)),this.formView=new ModelPickerFormView(this.config),this.formView.onSubmit((async t=>{try{let e=await this.model.DiffusionModel.query({name:t.model}),i=await e.getTensorRTStatus();this.publish("modelPickerChange",e),this.engine.model=t.model,this.formView.setTensorRTStatus(i,(()=>this.showBuildTensorRT(e)))}catch(t){this.formView.setValues({model:null})}})),this.application.container.appendChild(await this.formView.render()),this.subscribe("invocationError",(t=>{if(console.error(t),!isEmpty(t.metadata)&&!isEmpty(t.metadata.tensorrt_build)){let e=t.metadata.tensorrt_build.network,i=ModelTensorRTStatusView.supportedNetworks[e],s=t.metadata.tensorrt_build.model;this.notify("info","TensorRT Engine Build Failed",`${s} ${i} TensorRT Engine failed to build. Please try again.`),isEmpty(this.builtEngines[s])&&(this.builtEngines[s]=[]),this.builtEngines[s].push(e)}})),this.subscribe("invocationComplete",(t=>{if(!isEmpty(t.metadata)&&!isEmpty(t.metadata.tensorrt_build)){let e=t.metadata.tensorrt_build.network,i=ModelTensorRTStatusView.supportedNetworks[e],s=t.metadata.tensorrt_build.model;this.notify("info","TensorRT Engine Build Complete",`Successfully built ${s} ${i} TensorRT Engine.`),isEmpty(this.builtEngines[s])&&(this.builtEngines[s]=[]),this.builtEngines[s].push(e)}}))}}export{ModelPickerController};
```

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/file/02-open.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/file/02-open.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/file/03-save.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/file/03-save.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/file/04-history.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/file/04-history.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/file/05-results.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/file/05-results.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/help/01-about.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/help/01-about.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/index.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/index.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/models/01-civitait.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/models/01-civitait.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/sidebar/01-canvas.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/sidebar/01-canvas.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/sidebar/02-tweaks.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/sidebar/02-tweaks.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/sidebar/03-generation.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/sidebar/03-generation.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/sidebar/04-upscale.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/sidebar/04-upscale.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/sidebar/05-prompts.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/sidebar/05-prompts.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/sidebar/99-invoke.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/sidebar/99-invoke.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/system/01-settings.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/system/01-settings.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/system/02-users.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/system/02-users.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/controller/system/03-installation.mjs` & `enfugue-0.1.2/enfugue/static/js/controller/system/03-installation.mjs`

 * *Files 15% similar despite different names*

```diff
@@ -1 +1 @@
-import{MenuController}from"../menu.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,humanSize}from"../../base/helpers.mjs";import{View,ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView}from"../../view/table.mjs";import{FileInputView,ButtonInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class UploadFileFormView extends FormView{static showCancel=!0;static fieldSets={File:{file:{class:FileInputView,config:{required:!0}}}}}class UploadFileButtonInputView extends ButtonInputView{static className="upload-file-input-view";static defaultValue="Upload File"}class InstallationDirectorySummaryTableView extends TableView{static columns={directory:"Directory",items:"Items",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class InstallationDirectoryTableView extends TableView{static columns={name:"Name",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class TensorRTEngineTableView extends TableView{static columns={model:"Model",type:"Type",size:"Size",lora:"LoRA",inversion:"Inversions",bytes:"File Size",used_by:"Used By"};static columnFormatters={type:(t,e)=>{let i="";return e.model.endsWith("-inpainting")&&(i="Inpainting "),`${i}${{unet:"UNet",controlledunet:"Controlled UNet",clip:"CLIP",vae:"VAE",controlnet:"ControlNet"}[t]}`},size:t=>`${t}px`,bytes:t=>humanSize(t),lora:t=>isEmpty(t)?"None":t.map((t=>t.join(":"))).join("<br />"),inversion:t=>isEmpty(t)?"None":t.map((t=>t.model)).join("<br />"),used_by:t=>isEmpty(t)?"None":t.length<=2?t.join("<br />"):t.slice(0,2).join("<br />")+`<br />…and ${t.length-2} more`}}class TensorRTEngineSummaryTableView extends TableView{static columns={total:"Total Engines",used:"Currently Used",bytes:"Total File Size"};static columnFormatters={total:t=>isEmpty(t)?"None":t,used:t=>isEmpty(t)?"None":t,bytes:t=>isEmpty(t)?"0 Bytes":humanSize(t)}}class InstallationSummaryView extends View{constructor(t){super(t.config),this.controller=t,this.summaryTable=new InstallationDirectorySummaryTableView(this.config),this.summaryTable.addButton("Manage","fa-solid fa-list-check",(t=>{this.controller.showDirectoryManager(t.directory)})),this.engineTable=new TensorRTEngineSummaryTableView(this.config),this.engineTable.addButton("Manage","fa-solid fa-list-check",(()=>{this.controller.showTensorRTManager()}))}async update(){let t=await this.controller.model.get("/installation"),e=await this.controller.model.get("/tensorrt");await this.summaryTable.setData(Object.getOwnPropertyNames(t).map((e=>({directory:e,items:t[e].items,bytes:t[e].bytes}))),!1),await this.engineTable.setData([e.reduce(((t,e)=>(void 0===t.total&&(t.total=0),void 0===t.used&&(t.used=0),void 0===t.bytes&&(t.bytes=0),t.total+=1,t.used+=e.used,t.bytes+=e.bytes,t)),{})],!1)}async build(){let t=await super.build();return await this.update(),t.content(E.h2().content("Weights and Configuration"),await this.summaryTable.getNode(),E.h2().content("TensorRT Engines"),await this.engineTable.getNode())}}class InstallationController extends MenuController{static menuName="Installation";static menuIcon="fa-solid fa-folder-tree";static summaryWindowWidth=400;static summaryWindowHeight=600;static managerWindowWidth=600;static managerWindowHeight=800;static uploadWindowWidth=400;static uploadWindowHeight=250;static uploadableDirectories=["lora","checkpoint","inversion"];async initialize(){await super.initialize(),this.directoryWindows={}}async showSummaryWindow(){isEmpty(this.summaryWindow)?(this.summaryWindow=await this.spawnWindow("Installation Summary",await this.getSummaryView(),this.constructor.summaryWindowWidth,this.constructor.summaryWindowHeight),this.summaryWindow.onClose((()=>{this.summaryWindow=null}))):this.summaryWindow.focus()}async getSummaryView(){return isEmpty(this.summaryView)?this.summaryView=new InstallationSummaryView(this):this.summaryView.update(),this.summaryView}async showTensorRTManager(){let t=await this.model.get("/tensorrt");if(isEmpty(this.tensorRTManagerWindow)){let e=new TensorRTEngineTableView(this.config,t);e.addButton("Delete","fa-solid fa-trash",(async t=>{let i=`/tensorrt/${t.model}/${t.type}/${t.key}`;try{await this.model.delete(i),this.notify("info","Success","TensorRT engine deleted."),e.setData(await this.model.get("/tensorrt"),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}})),this.tensorRTManagerWindow=await this.spawnWindow("TensorRT Engines",e,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.tensorRTManagerWindow.onClose((()=>{this.tensorRTManagerWindow=null}))}else this.tensorRTManagerWindow.content.setData(t,!1),this.tensorRTManagerWindow.focus()}async showUploadFile(t){let e=new UploadFileFormView(this.config),i=await this.spawnWindow(`Upload File to '${t}'`,e,this.constructor.uploadWindowWidth,this.constructor.uploadWindowHeight);e.onSubmit((async s=>{await this.model.multiPart(`/installation/${t}`,null,null,{file:s.file},(async t=>{(await e.getInputView("file")).setProgress(t.loaded/t.total)})),this.notify("info","Uploaded",`File successfully uploaded to '${t}'`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),i.remove()})),e.onCancel((()=>{i.remove()}))}async showDirectoryManager(t){let e=await this.model.get(`/installation/${t}`);if(isEmpty(this.directoryWindows[t])){let i=new InstallationDirectoryTableView(this.config,e);i.addButton("Delete","fa-solid fa-trash",(async e=>{let s=`/installation/${t}/${e.name}`;try{await this.model.delete(s),this.notify("info","Success",`Successfully deleted <strong>${t}/${e.name}</strong>`),i.setData(await this.model.get(`/installation/${t}`),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}}));let s=new ParentView(this.config);if(s.addChild(i),-1!==this.constructor.uploadableDirectories.indexOf(t)){let e=new UploadFileButtonInputView(this.config);e.onChange((()=>{this.showUploadFile(t)})),s.addChild(e)}this.directoryWindows[t]=await this.spawnWindow(`Manage Directory '${t}'`,s,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.directoryWindows[t].onClose((()=>{this.directoryWindows[t]=null}))}else this.directoryWindows[t].content.getChild(0).setData(e),this.directoryWindows[t].focus()}async onClick(){this.showSummaryWindow()}}export{InstallationController as MenuController};
+import{MenuController}from"../menu.mjs";import{ElementBuilder}from"../../base/builder.mjs";import{isEmpty,humanSize}from"../../base/helpers.mjs";import{View,ParentView}from"../../view/base.mjs";import{FormView}from"../../view/forms/base.mjs";import{TableView}from"../../view/table.mjs";import{FileInputView,ButtonInputView,StringInputView}from"../../view/forms/input.mjs";const E=new ElementBuilder;class ChangeDirectoryForm extends FormView{static showCancel=!0;static fieldSets={Directory:{directory:{class:StringInputView,config:{required:!0,placeholder:"C:\\Users\\MyUser\\..."}}}}}class UploadFileFormView extends FormView{static showCancel=!0;static fieldSets={File:{file:{class:FileInputView,config:{required:!0}}}}}class UploadFileButtonInputView extends ButtonInputView{static className="upload-file-input-view";static defaultValue="Upload File"}class InstallationDirectorySummaryTableView extends TableView{static columns={directory:"Directory",location:"Location",items:"Items",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class InstallationDirectoryTableView extends TableView{static columns={name:"Name",bytes:"Total File Size"};static columnFormatters={bytes:t=>humanSize(t)}}class TensorRTEngineTableView extends TableView{static columns={model:"Model",type:"Type",size:"Size",lora:"LoRA",inversion:"Inversions",bytes:"File Size",used_by:"Used By"};static columnFormatters={type:(t,e)=>{let i="";return e.model.endsWith("-inpainting")&&(i="Inpainting "),`${i}${{unet:"UNet",controlledunet:"Controlled UNet",clip:"CLIP",vae:"VAE",controlnet:"ControlNet"}[t]}`},size:t=>`${t}px`,bytes:t=>humanSize(t),lora:t=>isEmpty(t)?"None":t.map((t=>t.join(":"))).join("<br />"),inversion:t=>isEmpty(t)?"None":t.map((t=>t.model)).join("<br />"),used_by:t=>isEmpty(t)?"None":t.length<=2?t.join("<br />"):t.slice(0,2).join("<br />")+`<br />…and ${t.length-2} more`}}class TensorRTEngineSummaryTableView extends TableView{static columns={total:"Total Engines",used:"Currently Used",bytes:"Total File Size"};static columnFormatters={total:t=>isEmpty(t)?"None":`${t}`,used:t=>isEmpty(t)?"None":`${t}`,bytes:t=>isEmpty(t)?"0 Bytes":humanSize(t)}}class InstallationSummaryView extends View{constructor(t){super(t.config),this.controller=t,this.summaryTable=new InstallationDirectorySummaryTableView(this.config),this.summaryTable.addButton("Manage","fa-solid fa-list-check",(t=>{this.controller.showDirectoryManager(t.directory)})),this.summaryTable.addButton("Change Directory","fa-solid fa-edit",(t=>{this.controller.showChangeDirectory(t.directory)})),this.engineTable=new TensorRTEngineSummaryTableView(this.config),this.engineTable.addButton("Manage","fa-solid fa-list-check",(()=>{this.controller.showTensorRTManager()}))}async update(){let t=await this.controller.model.get("/installation"),e=await this.controller.model.get("/tensorrt");await this.summaryTable.setData(Object.getOwnPropertyNames(t).map((e=>(console.log(e),{directory:e,location:t[e].path,items:t[e].items,bytes:t[e].bytes}))),!1),await this.engineTable.setData([e.reduce(((t,e)=>(void 0===t.total&&(t.total=0),void 0===t.used&&(t.used=0),void 0===t.bytes&&(t.bytes=0),t.total+=1,t.used+=e.used,t.bytes+=e.bytes,t)),{})],!1)}async build(){let t=await super.build();return await this.update(),t.content(E.h2().content("Weights and Configuration"),await this.summaryTable.getNode(),E.h2().content("TensorRT Engines"),await this.engineTable.getNode())}}class InstallationController extends MenuController{static menuName="Installation";static menuIcon="fa-solid fa-folder-tree";static summaryWindowWidth=600;static summaryWindowHeight=600;static managerWindowWidth=600;static managerWindowHeight=800;static uploadWindowWidth=400;static uploadWindowHeight=250;static changeDirectoryWindowWidth=400;static changeDirectoryWindowHeight=200;static uploadableDirectories=["lora","checkpoint","inversion"];async initialize(){await super.initialize(),this.directoryWindows={}}async showSummaryWindow(){isEmpty(this.summaryWindow)?(this.summaryWindow=await this.spawnWindow("Installation Summary",await this.getSummaryView(),this.constructor.summaryWindowWidth,this.constructor.summaryWindowHeight),this.summaryWindow.onClose((()=>{this.summaryWindow=null}))):this.summaryWindow.focus()}async getSummaryView(){return isEmpty(this.summaryView)?this.summaryView=new InstallationSummaryView(this):this.summaryView.update(),this.summaryView}async showTensorRTManager(){let t=await this.model.get("/tensorrt");if(isEmpty(this.tensorRTManagerWindow)){let e=new TensorRTEngineTableView(this.config,t);e.addButton("Delete","fa-solid fa-trash",(async t=>{let i=`/tensorrt/${t.model}/${t.type}/${t.key}`;try{await this.model.delete(i),this.notify("info","Success","TensorRT engine deleted."),e.setData(await this.model.get("/tensorrt"),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}})),this.tensorRTManagerWindow=await this.spawnWindow("TensorRT Engines",e,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.tensorRTManagerWindow.onClose((()=>{this.tensorRTManagerWindow=null}))}else this.tensorRTManagerWindow.content.setData(t,!1),this.tensorRTManagerWindow.focus()}async showUploadFile(t){let e=new UploadFileFormView(this.config),i=await this.spawnWindow(`Upload File to '${t}'`,e,this.constructor.uploadWindowWidth,this.constructor.uploadWindowHeight);e.onSubmit((async s=>{await this.model.multiPart(`/installation/${t}`,null,null,{file:s.file},(async t=>{(await e.getInputView("file")).setProgress(t.loaded/t.total)})),this.notify("info","Uploaded",`File successfully uploaded to '${t}'`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),i.remove()})),e.onCancel((()=>{i.remove()}))}async showChangeDirectory(t){let e=new ChangeDirectoryForm(this.config),i=await this.spawnWindow(`Change Filesystem Location for ${t}`,e,this.constructor.changeDirectoryWindowWidth,this.constructor.changeDirectoryWindowHeight);e.onSubmit((async s=>{try{await this.model.post(`/installation/${t}/move`,null,null,{directory:s.directory}),this.notify("info","Changed",`Filesystem Location successfully changed for ${t}`),isEmpty(this.summaryView)||this.summaryView.update(),isEmpty(this.directoryWindows[t])||this.directoryWindows[t].content.getChild(0).setData(await this.model.get(`/installation/${t}`),!1),i.remove()}catch(t){let i=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(i=t.title):i=t.detail,this.notify("error","Couldn't Change",i),e.enable()}})),e.onCancel((()=>{i.remove()}))}async showDirectoryManager(t){let e=await this.model.get(`/installation/${t}`);if(isEmpty(this.directoryWindows[t])){let i=new InstallationDirectoryTableView(this.config,e);i.addButton("Delete","fa-solid fa-trash",(async e=>{let s=`/installation/${t}/${e.name}`;try{await this.model.delete(s),this.notify("info","Success",`Successfully deleted <strong>${t}/${e.name}</strong>`),i.setData(await this.model.get(`/installation/${t}`),!1),isEmpty(this.summaryView)||this.summaryView.update()}catch(t){let e=`${t}`;isEmpty(t.detail)?isEmpty(t.title)||(e=t.title):e=t.detail,this.notify("error","Couldn't Delete",e)}}));let s=new ParentView(this.config);if(s.addChild(i),-1!==this.constructor.uploadableDirectories.indexOf(t)){let e=new UploadFileButtonInputView(this.config);e.onChange((()=>{this.showUploadFile(t)})),s.addChild(e)}this.directoryWindows[t]=await this.spawnWindow(`Manage Directory '${t}'`,s,this.constructor.managerWindowWidth,this.constructor.managerWindowHeight),this.directoryWindows[t].onClose((()=>{this.directoryWindows[t]=null}))}else this.directoryWindows[t].content.getChild(0).setData(e),this.directoryWindows[t].focus()}async onClick(){this.showSummaryWindow()}}export{InstallationController as MenuController};
```

### Comparing `enfugue-0.1.1/enfugue/static/js/enfugue.mjs` & `enfugue-0.1.2/enfugue/static/js/enfugue.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/graphics/colors.mjs` & `enfugue-0.1.2/enfugue/static/js/graphics/colors.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/graphics/geometry.mjs` & `enfugue-0.1.2/enfugue/static/js/graphics/geometry.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/graphics/paths.mjs` & `enfugue-0.1.2/enfugue/static/js/graphics/paths.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/graphics/spline.mjs` & `enfugue-0.1.2/enfugue/static/js/graphics/spline.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/model/enfugue.mjs` & `enfugue-0.1.2/enfugue/static/js/model/enfugue.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/model/index.mjs` & `enfugue-0.1.2/enfugue/static/js/model/index.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/base.mjs` & `enfugue-0.1.2/enfugue/static/js/view/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/base.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/classic.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/classic.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/input/base.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/input/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/input/color.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/input/color.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/input/enumerable.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/input/enumerable.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/input/file.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/input/file.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/input/numeric.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/input/numeric.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/input/parent.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/input/parent.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/input/string.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/input/string.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/forms/input.mjs` & `enfugue-0.1.2/enfugue/static/js/view/forms/input.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/image.mjs` & `enfugue-0.1.2/enfugue/static/js/view/image.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/menu.mjs` & `enfugue-0.1.2/enfugue/static/js/view/menu.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/nodes/base.mjs` & `enfugue-0.1.2/enfugue/static/js/view/nodes/base.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/nodes/decorations.mjs` & `enfugue-0.1.2/enfugue/static/js/view/nodes/decorations.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/nodes/editor.mjs` & `enfugue-0.1.2/enfugue/static/js/view/nodes/editor.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/nodes/image-editor.mjs` & `enfugue-0.1.2/enfugue/static/js/view/nodes/image-editor.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/nodes/windows.mjs` & `enfugue-0.1.2/enfugue/static/js/view/nodes/windows.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/notifications.mjs` & `enfugue-0.1.2/enfugue/static/js/view/notifications.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/scribble.mjs` & `enfugue-0.1.2/enfugue/static/js/view/scribble.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/status.mjs` & `enfugue-0.1.2/enfugue/static/js/view/status.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/static/js/view/table.mjs` & `enfugue-0.1.2/enfugue/static/js/view/table.mjs`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/util/downloads.py` & `enfugue-0.1.2/enfugue/util/downloads.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,42 +2,46 @@
 import requests
 
 from enfugue.util.log import logger
 
 __all__ = ["check_download", "check_download_to_dir"]
 
 
-def check_download(remote_url: str, local_path: str, chunk_size: int = 8192) -> None:
+def check_download(
+    remote_url: str, local_path: str, chunk_size: int = 8192, check_size: bool = True
+) -> None:
     """
     Checks if a file exists.
     If it does, checks the size and matches against the remote URL.
     If it doesn't, or the size doesn't match, download it.
     """
-    if os.path.exists(local_path):
+    if os.path.exists(local_path) and check_size:
         expected_length = requests.head(remote_url, allow_redirects=True).headers.get(
             "Content-Length", None
         )
         actual_length = os.path.getsize(local_path)
         if expected_length and actual_length != int(expected_length):
-            logger.debug(
+            logger.info(
                 f"File at {local_path} looks like an interrupted download, or the remote resource has changed. Removing."
             )
             os.remove(local_path)
 
     if not os.path.exists(local_path):
-        logger.debug(f"Downloading file from {remote_url}. Will write to {local_path}")
+        logger.info(f"Downloading file from {remote_url}. Will write to {local_path}")
         response = requests.get(remote_url, allow_redirects=True, stream=True)
         with open(local_path, "wb") as fh:
             for chunk in response.iter_content(chunk_size=chunk_size):
                 fh.write(chunk)
 
 
-def check_download_to_dir(remote_url: str, local_dir: str, chunk_size: int = 8192) -> str:
+def check_download_to_dir(
+    remote_url: str, local_dir: str, chunk_size: int = 8192, check_size: bool = True
+) -> str:
     """
     Checks if a file exists in a directory based on a remote path.
     If it does, checks the size and matches against the remote URL.
     If it doesn't, or the size doesn't match, download it.
     """
     file_name = os.path.basename(remote_url)
     local_path = os.path.join(local_dir, file_name)
-    check_download(remote_url, local_path, chunk_size=chunk_size)
+    check_download(remote_url, local_path, chunk_size=chunk_size, check_size=check_size)
     return local_path
```

### Comparing `enfugue-0.1.1/enfugue/util/gpu.py` & `enfugue-0.1.2/enfugue/util/gpu.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/util/gputil.py` & `enfugue-0.1.2/enfugue/util/gputil.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/util/images.py` & `enfugue-0.1.2/enfugue/util/images.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/util/installation.py` & `enfugue-0.1.2/enfugue/util/installation.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/util/security.py` & `enfugue-0.1.2/enfugue/util/security.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/util/signature.py` & `enfugue-0.1.2/enfugue/util/signature.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue/util/tokens.py` & `enfugue-0.1.2/enfugue/util/tokens.py`

 * *Files identical despite different names*

### Comparing `enfugue-0.1.1/enfugue.egg-info/SOURCES.txt` & `enfugue-0.1.2/enfugue.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,15 @@
 enfugue/static/js/controller/sidebar/03-generation.mjs
 enfugue/static/js/controller/sidebar/04-upscale.mjs
 enfugue/static/js/controller/sidebar/05-prompts.mjs
 enfugue/static/js/controller/sidebar/99-invoke.mjs
 enfugue/static/js/controller/system/01-settings.mjs
 enfugue/static/js/controller/system/02-users.mjs
 enfugue/static/js/controller/system/03-installation.mjs
+enfugue/static/js/controller/system/04-logs.mjs
 enfugue/static/js/controller/toolbar/01-load-image.mjs
 enfugue/static/js/controller/toolbar/02-draw-scribble.mjs
 enfugue/static/js/controller/toolbar/03-region-prompt.mjs
 enfugue/static/js/graphics/colors.mjs
 enfugue/static/js/graphics/geometry.mjs
 enfugue/static/js/graphics/paths.mjs
 enfugue/static/js/graphics/spline.mjs
```

### Comparing `enfugue-0.1.1/enfugue.egg-info/requires.txt` & `enfugue-0.1.2/enfugue.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 test-tube<0.8,>=0.7.5
 streamlit<0.74,>=0.73
 einops<0.4,>=0.3
 torch-fidelity<0.4,>=0.3
 transformers<5.0,>=4.28
 torchmetrics==0.11.4
 kornia<0.7,>=0.6
-polygraphy<0.48,>=0.47
 accelerate<0.19,>=0.18
 tqdm>=4.27
 safetensors<0.4,>=0.3
 realesrgan<0.4,>=0.3
 gfpgan<1.4,>=1.3.8
 backgroundremover<0.3,>=0.2.3
 beautifulsoup4<5,>=4.12
@@ -36,14 +35,16 @@
 
 [build]
 types-protobuf<5.0,>=4.23.0.1
 types-requests<3.0,>=2.30
 types-setuptools<68.0,>=67.7
 types-urllib3<2.0,>=1.26.25
 types-tabulate<0.10,>=0.9
+types-pyyaml<7.0,>=6.0
 importchecker<3.0,>=2.0
 
 [tensorrt]
+polygraphy<0.48,>=0.47
 onnx==1.12
 onnxruntime-gpu==1.12.1
 onnx-graphsurgeon==0.3.26
 tensorrt<8.7,>=8.6
```

### Comparing `enfugue-0.1.1/setup.py` & `enfugue-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "enfugue"
 version_major = "0"
 version_minor = "1"
-version_patch = "1"
+version_patch = "2"
 
 install_requires = [
     "cheroot>=9.0.0",
     "nvidia-pyindex>=1.0.9",
     "pibble[cherrypy]>=0.5",
     "torch>=1.13.1,<2.0",
     "numpy>=1.24.0",
@@ -25,15 +25,14 @@
     "test-tube>=0.7.5,<0.8",
     "streamlit>=0.73,<0.74",
     "einops>=0.3,<0.4",
     "torch-fidelity>=0.3,<0.4",
     "transformers>=4.28,<5.0",
     "torchmetrics==0.11.4",
     "kornia>=0.6,<0.7",
-    "polygraphy>=0.47,<0.48",
     "accelerate>=0.18,<0.19",
     "tqdm>=4.27",
     "safetensors>=0.3,<0.4",
     "realesrgan>=0.3,<0.4",
     "gfpgan>=1.3.8,<1.4",
     "backgroundremover>=0.2.3,<0.3",
     "beautifulsoup4>=4.12,<5",
@@ -42,25 +41,27 @@
     "taming-transformers",
     "clip",
     "latent-diffusion",
 ]
 
 extras_require = {
     "tensorrt": [
+        "polygraphy>=0.47,<0.48",
         "onnx==1.12",
         "onnxruntime-gpu==1.12.1",
         "onnx-graphsurgeon==0.3.26",
         "tensorrt>=8.6,<8.7",
     ],
     "build": [
         "types-protobuf>=4.23.0.1,<5.0",
         "types-requests>=2.30,<3.0",
         "types-setuptools>=67.7,<68.0",
         "types-urllib3>=1.26.25,<2.0",
         "types-tabulate>=0.9,<0.10",
+        "types-pyyaml>=6.0,<7.0",
         "importchecker>=2.0,<3.0",
     ],
 }
 
 packaged_files = []
 
 here = os.path.dirname(os.path.abspath(__file__))
```

