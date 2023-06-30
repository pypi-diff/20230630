# Comparing `tmp/malariagen_data-7.8.0.tar.gz` & `tmp/malariagen_data-7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malariagen_data-7.8.0.tar", max compression
+gzip compressed data, was "malariagen_data-7.9.0.tar", max compression
```

## Comparing `malariagen_data-7.8.0.tar` & `malariagen_data-7.9.0.tar`

### file list

```diff
@@ -1,23 +1,39 @@
--rw-r--r--   0        0        0     1067 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/LICENSE
--rw-r--r--   0        0        0      987 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/__init__.py
--rw-r--r--   0        0        0    10005 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/af1.py
--rw-r--r--   0        0        0    92409 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/ag3.py
--rw-r--r--   0        0        0     9451 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/amin1.py
--rw-r--r--   0        0        0        0 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/__init__.py
--rw-r--r--   0        0        0    21458 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/base.py
--rw-r--r--   0        0        0    15659 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/genome_features.py
--rw-r--r--   0        0        0     3204 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/genome_sequence.py
--rw-r--r--   0        0        0    27811 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/sample_metadata.py
--rw-r--r--   0        0        0    45071 2023-05-19 18:50:50.651732 malariagen_data-7.8.0/malariagen_data/anoph/snp_data.py
--rw-r--r--   0        0        0   219720 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/anopheles.py
--rw-r--r--   0        0        0    10514 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/mjn.py
--rw-r--r--   0        0        0     1253 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/pf7.py
--rw-r--r--   0        0        0     4442 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/pf7_config.json
--rw-r--r--   0        0        0    11756 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/plasmodium.py
--rw-r--r--   0        0        0    14253 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/plotly_dendrogram.py
--rw-r--r--   0        0        0     1253 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/pv4.py
--rw-r--r--   0        0        0     2060 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/pv4_config.json
--rw-r--r--   0        0        0    26186 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/util.py
--rw-r--r--   0        0        0    17981 2023-05-19 18:50:50.655732 malariagen_data-7.8.0/malariagen_data/veff.py
--rw-r--r--   0        0        0     2028 2023-05-19 18:54:41.669683 malariagen_data-7.8.0/pyproject.toml
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 malariagen_data-7.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/LICENSE
+-rw-r--r--   0        0        0      987 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/__init__.py
+-rw-r--r--   0        0        0     9661 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/af1.py
+-rw-r--r--   0        0        0    92036 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/ag3.py
+-rw-r--r--   0        0        0     9451 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/amin1.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/__init__.py
+-rw-r--r--   0        0        0    15170 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/base.py
+-rw-r--r--   0        0        0     5640 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/base_params.py
+-rw-r--r--   0        0        0      732 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/dash_params.py
+-rw-r--r--   0        0        0     1883 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/frq_params.py
+-rw-r--r--   0        0        0      533 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/fst_params.py
+-rw-r--r--   0        0        0     1096 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/g123_params.py
+-rw-r--r--   0        0        0    13604 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/genome_features.py
+-rw-r--r--   0        0        0     3217 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/genome_sequence.py
+-rw-r--r--   0        0        0     1890 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/gplt_params.py
+-rw-r--r--   0        0        0      738 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/h12_params.py
+-rw-r--r--   0        0        0    10319 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/hap_data.py
+-rw-r--r--   0        0        0      288 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/hap_params.py
+-rw-r--r--   0        0        0     1130 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/hapclust_params.py
+-rw-r--r--   0        0        0     1172 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/hapnet_params.py
+-rw-r--r--   0        0        0     1782 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/het_params.py
+-rw-r--r--   0        0        0     2758 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/ihs_params.py
+-rw-r--r--   0        0        0     1597 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/map_params.py
+-rw-r--r--   0        0        0     1428 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/pca_params.py
+-rw-r--r--   0        0        0     3179 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/plotly_params.py
+-rw-r--r--   0        0        0    25961 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/sample_metadata.py
+-rw-r--r--   0        0        0    45091 2023-05-26 15:53:16.431671 malariagen_data-7.9.0/malariagen_data/anoph/snp_data.py
+-rw-r--r--   0        0        0   192986 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/anopheles.py
+-rw-r--r--   0        0        0    10514 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/mjn.py
+-rw-r--r--   0        0        0     1253 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/pf7.py
+-rw-r--r--   0        0        0     4442 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/pf7_config.json
+-rw-r--r--   0        0        0    11756 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/plasmodium.py
+-rw-r--r--   0        0        0    14253 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/plotly_dendrogram.py
+-rw-r--r--   0        0        0     1253 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/pv4.py
+-rw-r--r--   0        0        0     2060 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/pv4_config.json
+-rw-r--r--   0        0        0    26373 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/util.py
+-rw-r--r--   0        0        0    17981 2023-05-26 15:53:16.435671 malariagen_data-7.9.0/malariagen_data/veff.py
+-rw-r--r--   0        0        0     2028 2023-05-26 15:56:15.782385 malariagen_data-7.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 malariagen_data-7.9.0/PKG-INFO
```

### Comparing `malariagen_data-7.8.0/LICENSE` & `malariagen_data-7.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/__init__.py` & `malariagen_data-7.9.0/malariagen_data/__init__.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/af1.py` & `malariagen_data-7.9.0/malariagen_data/af1.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 from .anopheles import AnophelesDataResource
 
 MAJOR_VERSION_NUMBER = 1
 MAJOR_VERSION_PATH = "v1.0"
 CONFIG_PATH = "v1.0-config.json"
 GCS_URL = "gs://vo_afun_release/"
-SITE_ANNOTATIONS_ZARR_PATH = "reference/genome/idAnoFuneDA-416_04/Anopheles-funestus-DA-416_04_1_SEQANNOTATION.zarr"
 PCA_RESULTS_CACHE_NAME = "af1_pca_v1"
-SNP_ALLELE_COUNTS_CACHE_NAME = "af1_snp_allele_counts_v2"
 FST_GWSS_CACHE_NAME = "af1_fst_gwss_v1"
 H12_CALIBRATION_CACHE_NAME = "af1_h12_calibration_v1"
 H12_GWSS_CACHE_NAME = "af1_h12_gwss_v1"
 G123_GWSS_CACHE_NAME = "af1_g123_gwss_v1"
 G123_CALIBRATION_CACHE_NAME = "af1_g123_calibration_v1"
 H1X_GWSS_CACHE_NAME = "af1_h1x_gwss_v1"
 IHS_GWSS_CACHE_NAME = "af1_ihs_gwss_v1"
@@ -68,26 +66,22 @@
     Set up caching of some longer-running computations on the local file system,
     in a directory named "results_cache":
 
         >>> af1 = malariagen_data.Af1(results_cache="results_cache")
 
     """
 
-    _site_annotations_zarr_path = SITE_ANNOTATIONS_ZARR_PATH
     _pca_results_cache_name = PCA_RESULTS_CACHE_NAME
-    _snp_allele_counts_results_cache_name = SNP_ALLELE_COUNTS_CACHE_NAME
     _fst_gwss_results_cache_name = FST_GWSS_CACHE_NAME
     _h12_calibration_cache_name = H12_CALIBRATION_CACHE_NAME
     _h12_gwss_cache_name = H12_GWSS_CACHE_NAME
     _g123_gwss_cache_name = G123_GWSS_CACHE_NAME
     _g123_calibration_cache_name = G123_CALIBRATION_CACHE_NAME
     _h1x_gwss_cache_name = H1X_GWSS_CACHE_NAME
     _ihs_gwss_cache_name = IHS_GWSS_CACHE_NAME
-    phasing_analysis_ids = ("funestus",)
-    _default_phasing_analysis = "funestus"
 
     def __init__(
         self,
         url=GCS_URL,
         bokeh_output_notebook=True,
         results_cache=None,
         log=sys.stdout,
@@ -103,14 +97,15 @@
             url=url,
             config_path=CONFIG_PATH,
             cohorts_analysis=cohorts_analysis,
             aim_analysis=None,
             aim_metadata_dtype=None,
             site_filters_analysis=site_filters_analysis,
             default_site_mask="funestus",
+            default_phasing_analysis="funestus",
             bokeh_output_notebook=bokeh_output_notebook,
             results_cache=results_cache,
             log=log,
             debug=debug,
             show_progress=show_progress,
             check_location=check_location,
             pre=pre,
```

### Comparing `malariagen_data-7.8.0/malariagen_data/ag3.py` & `malariagen_data-7.9.0/malariagen_data/ag3.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
 import zarr
 
 import malariagen_data  # used for .__version__
 
-from .anoph.base import base_params
+from .anoph import base_params
 from .anopheles import AnophelesDataResource, gplt_params
 from .util import (
     DIM_SAMPLE,
     DIM_VARIANT,
     Region,
     da_from_zarr,
     init_zarr_store,
@@ -31,20 +31,16 @@
 # silence dask performance warnings
 dask.config.set(**{"array.slicing.split_large_chunks": False})  # type: ignore
 
 MAJOR_VERSION_NUMBER = 3
 MAJOR_VERSION_PATH = "v3"
 CONFIG_PATH = "v3-config.json"
 GCS_URL = "gs://vo_agam_release/"
-SITE_ANNOTATIONS_ZARR_PATH = (
-    "reference/genome/agamp4/Anopheles-gambiae-PEST_SEQANNOTATION_AgamP4.12.zarr"
-)
 DEFAULT_MAX_COVERAGE_VARIANCE = 0.2
 PCA_RESULTS_CACHE_NAME = "ag3_pca_v1"
-SNP_ALLELE_COUNTS_CACHE_NAME = "ag3_snp_allele_counts_v2"
 FST_GWSS_CACHE_NAME = "ag3_fst_gwss_v1"
 H12_CALIBRATION_CACHE_NAME = "ag3_h12_calibration_v1"
 H12_GWSS_CACHE_NAME = "ag3_h12_gwss_v1"
 G123_CALIBRATION_CACHE_NAME = "ag3_g123_calibration_v1"
 G123_GWSS_CACHE_NAME = "ag3_g123_gwss_v1"
 H1X_GWSS_CACHE_NAME = "ag3_h1x_gwss_v1"
 IHS_GWSS_CACHE_NAME = "ag3_ihs_gwss_v1"
@@ -103,26 +99,22 @@
     in a directory named "results_cache":
 
         >>> ag3 = malariagen_data.Ag3(results_cache="results_cache")
 
     """
 
     virtual_contigs = "2RL", "3RL"
-    _site_annotations_zarr_path = SITE_ANNOTATIONS_ZARR_PATH
     _pca_results_cache_name = PCA_RESULTS_CACHE_NAME
-    _snp_allele_counts_results_cache_name = SNP_ALLELE_COUNTS_CACHE_NAME
     _fst_gwss_results_cache_name = FST_GWSS_CACHE_NAME
     _h12_calibration_cache_name = H12_CALIBRATION_CACHE_NAME
     _h12_gwss_cache_name = H12_GWSS_CACHE_NAME
     _g123_gwss_cache_name = G123_GWSS_CACHE_NAME
     _g123_calibration_cache_name = G123_CALIBRATION_CACHE_NAME
     _h1x_gwss_cache_name = H1X_GWSS_CACHE_NAME
     _ihs_gwss_cache_name = IHS_GWSS_CACHE_NAME
-    phasing_analysis_ids = ("gamb_colu_arab", "gamb_colu", "arab")
-    _default_phasing_analysis = "gamb_colu_arab"
 
     def __init__(
         self,
         url=GCS_URL,
         bokeh_output_notebook=True,
         results_cache=None,
         log=sys.stdout,
@@ -146,14 +138,15 @@
                 "aim_species_fraction_colu_no2l": "float64",
                 "aim_species_gambcolu_arabiensis": object,
                 "aim_species_gambiae_coluzzii": object,
                 "aim_species": object,
             },
             site_filters_analysis=site_filters_analysis,
             default_site_mask="gamb_colu_arab",
+            default_phasing_analysis="gamb_colu_arab",
             bokeh_output_notebook=bokeh_output_notebook,
             results_cache=results_cache,
             log=log,
             debug=debug,
             show_progress=show_progress,
             check_location=check_location,
             pre=pre,
```

### Comparing `malariagen_data-7.8.0/malariagen_data/amin1.py` & `malariagen_data-7.9.0/malariagen_data/amin1.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/anoph/genome_features.py` & `malariagen_data-7.9.0/malariagen_data/anoph/genome_features.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,29 @@
-from typing import Dict, Literal, Optional, Tuple, Union
+from typing import Dict, Optional, Tuple
 
 import bokeh.models
 import bokeh.plotting
 import numpy as np
 import pandas as pd
 from numpydoc_decorator import doc
 from pandas.io.common import infer_compression
-from typing_extensions import Annotated, TypeAlias
 
 from ..util import (
     Region,
     check_types,
     parse_multi_region,
     parse_single_region,
     read_gff3,
     unpack_gff3_attributes,
 )
-from .base import DEFAULT, base_params
+from . import base_params, gplt_params
+from .base_params import DEFAULT
 from .genome_sequence import AnophelesGenomeSequenceData
 
 
-class gplt_params:
-    """Parameters for genome plotting functions. N.B., genome plots are always
-    plotted with bokeh."""
-
-    sizing_mode: TypeAlias = Annotated[
-        Literal[
-            "fixed",
-            "stretch_width",
-            "stretch_height",
-            "stretch_both",
-            "scale_width",
-            "scale_height",
-            "scale_both",
-        ],
-        """
-        Bokeh plot sizing mode, see also
-        https://docs.bokeh.org/en/latest/docs/user_guide/basic/layouts.html#sizing-modes
-        """,
-    ]
-    sizing_mode_default: sizing_mode = "stretch_width"
-    width: TypeAlias = Annotated[
-        Optional[int],  # always can be None
-        "Plot width in pixels (px).",
-    ]
-    width_default: width = None
-    height: TypeAlias = Annotated[
-        int,
-        "Plot height in pixels (px).",
-    ]
-    track_height: TypeAlias = Annotated[
-        int,
-        "Main track height in pixels (px).",
-    ]
-    genes_height: TypeAlias = Annotated[
-        int,
-        "Genes track height in pixels (px).",
-    ]
-    genes_height_default: genes_height = 120
-    show: TypeAlias = Annotated[
-        bool,
-        "If true, show the plot. If False, do not show the plot, but return the figure.",
-    ]
-    toolbar_location: TypeAlias = Annotated[
-        Literal["above", "below", "left", "right"],
-        "Location of bokeh toolbar.",
-    ]
-    toolbar_location_default: toolbar_location = "above"
-    x_range: TypeAlias = Annotated[
-        bokeh.models.Range,
-        "X axis range (for linking to other tracks).",
-    ]
-    title: TypeAlias = Annotated[
-        Union[str, bool],
-        "Plot title. If True, a title may be automatically generated.",
-    ]
-    figure: TypeAlias = Annotated[
-        # Use quite a broad type here to accommodate both single-panel figures
-        # created via bokeh.plotting and multi-panel figures created via
-        # bokeh.layouts.
-        Optional[bokeh.model.Model],
-        "A bokeh figure (only returned if show=False).",
-    ]
-
-
 class AnophelesGenomeFeaturesData(AnophelesGenomeSequenceData):
     def __init__(
         self,
         *,
         gff_gene_type: str,
         gff_default_attributes: Tuple[str, ...],
         **kwargs,
```

### Comparing `malariagen_data-7.8.0/malariagen_data/anoph/genome_sequence.py` & `malariagen_data-7.9.0/malariagen_data/anoph/genome_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from ..util import (
     Region,
     check_types,
     da_from_zarr,
     init_zarr_store,
     parse_single_region,
 )
-from .base import AnophelesBase, base_params
+from . import base_params
+from .base import AnophelesBase
 
 
 class AnophelesGenomeSequenceData(AnophelesBase):
     def __init__(self, **kwargs):
         # N.B., this class is designed to work cooperatively, and
         # so it's important that any remaining parameters are passed
         # to the superclass constructor.
```

### Comparing `malariagen_data-7.8.0/malariagen_data/anoph/sample_metadata.py` & `malariagen_data-7.9.0/malariagen_data/anoph/sample_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,18 @@
 import io
 from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
 
 import ipyleaflet
 import numpy as np
 import pandas as pd
-import xyzservices
 from numpydoc_decorator import doc
-from typing_extensions import Annotated, TypeAlias
 
 from ..util import check_types
-from .base import AnophelesBase, base_params
-
-
-class map_params:
-    center: TypeAlias = Annotated[
-        Tuple[int, int],
-        "Location to center the map.",
-    ]
-    center_default: center = (-2, 20)
-    zoom: TypeAlias = Annotated[int, "Initial zoom level."]
-    zoom_default: zoom = 3
-    basemap: TypeAlias = Annotated[
-        Union[str, Dict, ipyleaflet.TileLayer, xyzservices.lib.TileProvider],
-        """
-        Basemap from ipyleaflet or other TileLayer provider. Strings are abbreviations mapped to corresponding
-        basemaps, e.g. "mapnik" (case-insensitive) maps to TileProvider ipyleaflet.basemaps.OpenStreetMap.Mapnik.
-        """,
-    ]
-    basemap_default: basemap = "mapnik"
-    height: TypeAlias = Annotated[
-        Union[int, str], "Height of the map in pixels (px) or other units."
-    ]
-    height_default: height = 500
-    width: TypeAlias = Annotated[
-        Union[int, str], "Width of the map in pixels (px) or other units."
-    ]
-    width_default: width = "100%"
-
-
-def _get_basemap_abbrevs():
-    """Get the dict of basemap abbreviations.
-
-    Returns
-    -------
-    basemap_abbrevs : dict
-        A dictionary where each key is a basemap abbreviation string, e.g. "mapnik",
-        and each value is a corresponding TileProvider, e.g. `ipyleaflet.basemaps.OpenStreetMap.Mapnik`.
-    """
-    import ipyleaflet
-
-    basemap_abbrevs = {
-        "mapnik": ipyleaflet.basemaps.OpenStreetMap.Mapnik,
-        "natgeoworldmap": ipyleaflet.basemaps.Esri.NatGeoWorldMap,
-        "opentopomap": ipyleaflet.basemaps.OpenTopoMap,
-        "positron": ipyleaflet.basemaps.CartoDB.Positron,
-        "satellite": ipyleaflet.basemaps.Gaode.Satellite,
-        "terrain": ipyleaflet.basemaps.Stamen.Terrain,
-        "watercolor": ipyleaflet.basemaps.Stamen.Watercolor,
-        "worldimagery": ipyleaflet.basemaps.Esri.WorldImagery,
-        "worldstreetmap": ipyleaflet.basemaps.Esri.WorldStreetMap,
-        "worldtopomap": ipyleaflet.basemaps.Esri.WorldTopoMap,
-    }
-    return basemap_abbrevs
+from . import base_params, map_params
+from .base import AnophelesBase
 
 
 class AnophelesSampleMetadata(AnophelesBase):
     def __init__(
         self,
         cohorts_analysis: Optional[str] = None,
         aim_analysis: Optional[str] = None,
@@ -505,18 +452,22 @@
             df_samples = self._cache_sample_metadata[cache_key]
 
         except KeyError:
             # Build a dataframe from all available metadata.
             df_samples = self.general_metadata(sample_sets=prepped_sample_sets)
             if self._aim_analysis:
                 df_aim = self.aim_metadata(sample_sets=prepped_sample_sets)
-                df_samples = df_samples.merge(df_aim, on="sample_id", sort=False)
+                df_samples = df_samples.merge(
+                    df_aim, on="sample_id", sort=False, how="left"
+                )
             if self._cohorts_analysis:
                 df_cohorts = self.cohorts_metadata(sample_sets=prepped_sample_sets)
-                df_samples = df_samples.merge(df_cohorts, on="sample_id", sort=False)
+                df_samples = df_samples.merge(
+                    df_cohorts, on="sample_id", sort=False, how="left"
+                )
 
             # Store sample metadata in the cache.
             self._cache_sample_metadata[cache_key] = df_samples
 
         # Add extra metadata.
         for on, data in self._extra_metadata:
             df_samples = df_samples.merge(data, how="left", on=on)
@@ -640,24 +591,26 @@
             }
         )
         df_pivot = df_pivot.merge(
             df_location_aggs, on=location_composite_key, validate="one_to_one"
         )
 
         # Handle basemap.
-        basemap_providers_dict = _get_basemap_abbrevs()
+        basemap_abbrevs = map_params.basemap_abbrevs
 
         # Determine basemap_provider via basemap
         if isinstance(basemap, str):
             # Interpret string
             # Support case-insensitive basemap abbreviations
             basemap_str = basemap.lower()
-            if basemap_str not in basemap_providers_dict:
-                raise ValueError("Basemap abbreviation not recognised:", basemap_str)
-            basemap_provider = basemap_providers_dict[basemap_str]
+            if basemap_str not in basemap_abbrevs:
+                raise ValueError(
+                    f"Basemap abbreviation not recognised: {basemap_str!r}; try one of {list(basemap_abbrevs.keys())}"
+                )
+            basemap_provider = basemap_abbrevs[basemap_str]
         elif basemap is None:
             # Default.
             basemap_provider = ipyleaflet.basemaps.Esri.WorldImagery
         else:
             # Expect dict or TileProvider or TileLayer.
             basemap_provider = basemap
```

### Comparing `malariagen_data-7.8.0/malariagen_data/anoph/snp_data.py` & `malariagen_data-7.9.0/malariagen_data/anoph/snp_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     init_zarr_store,
     locate_region,
     parse_multi_region,
     parse_single_region,
     simple_xarray_concat,
     true_runs,
 )
-from .base import DEFAULT, base_params
+from . import base_params
+from .base_params import DEFAULT
 from .genome_features import AnophelesGenomeFeaturesData, gplt_params
 from .genome_sequence import AnophelesGenomeSequenceData
 from .sample_metadata import AnophelesSampleMetadata
 
 
 class AnophelesSnpData(
     AnophelesSampleMetadata, AnophelesGenomeFeaturesData, AnophelesGenomeSequenceData
```

### Comparing `malariagen_data-7.8.0/malariagen_data/anopheles.py` & `malariagen_data-7.9.0/malariagen_data/anopheles.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,582 +13,56 @@
 import igv_notebook
 import numba
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 import xarray as xr
-import zarr
 from numpydoc_decorator import doc
-from typing_extensions import Annotated, Literal, TypeAlias
 
 from . import veff
-from .anoph.base import DEFAULT, AnophelesBase, base_params
-from .anoph.genome_features import AnophelesGenomeFeaturesData, gplt_params
+from .anoph import (
+    base_params,
+    dash_params,
+    frq_params,
+    fst_params,
+    g123_params,
+    gplt_params,
+    h12_params,
+    hapclust_params,
+    hapnet_params,
+    het_params,
+    ihs_params,
+    map_params,
+    pca_params,
+    plotly_params,
+)
+from .anoph.base import AnophelesBase
+from .anoph.base_params import DEFAULT
+from .anoph.genome_features import AnophelesGenomeFeaturesData
 from .anoph.genome_sequence import AnophelesGenomeSequenceData
-from .anoph.sample_metadata import AnophelesSampleMetadata, map_params
+from .anoph.hap_data import AnophelesHapData, hap_params
+from .anoph.sample_metadata import AnophelesSampleMetadata
 from .anoph.snp_data import AnophelesSnpData
 from .mjn import median_joining_network, mjn_graph
 from .util import (
-    DIM_ALLELE,
-    DIM_PLOIDY,
-    DIM_SAMPLE,
-    DIM_VARIANT,
     CacheMiss,
     Region,
     check_types,
-    da_from_zarr,
-    init_zarr_store,
     jackknife_ci,
     jitter,
     locate_region,
-    parse_multi_region,
     parse_single_region,
     plotly_discrete_legend,
-    simple_xarray_concat,
 )
 
 AA_CHANGE_QUERY = (
     "effect in ['NON_SYNONYMOUS_CODING', 'START_LOST', 'STOP_LOST', 'STOP_GAINED']"
 )
 
-
-class hap_params:
-    """Parameter definitions for haplotype functions."""
-
-    analysis: TypeAlias = Annotated[
-        str,
-        """
-        Which haplotype phasing analysis to use. See the
-        `phasing_analysis_ids` property for available values.
-        """,
-    ]
-
-
-class h12_params:
-    """Parameter definitions for H12 analysis functions."""
-
-    window_sizes: TypeAlias = Annotated[
-        Tuple[int, ...],
-        """
-        The sizes of windows (number of SNPs) used to calculate statistics within.
-        """,
-    ]
-    window_sizes_default: window_sizes = (100, 200, 500, 1000, 2000, 5000, 10000, 20000)
-    window_size: TypeAlias = Annotated[
-        int,
-        """
-        The size of windows (number of SNPs) used to calculate statistics within.
-        """,
-    ]
-    cohort_size_default: Optional[base_params.cohort_size] = None
-    min_cohort_size_default: base_params.min_cohort_size = 15
-    max_cohort_size_default: base_params.max_cohort_size = 50
-
-
-class g123_params:
-    """Parameter definitions for G123 analysis functions."""
-
-    sites: TypeAlias = Annotated[
-        str,
-        """
-        Which sites to use: 'all' includes all sites that pass
-        site filters; 'segregating' includes only segregating sites for
-        the given cohort; or a phasing analysis identifier can be
-        provided to use sites from the haplotype data, which is an
-        approximation to finding segregating sites in the entire Ag3.0
-        (gambiae complex) or Af1.0 (funestus) cohort.
-        """,
-    ]
-    window_sizes: TypeAlias = Annotated[
-        Tuple[int, ...],
-        """
-        The sizes of windows (number of sites) used to calculate statistics within.
-        """,
-    ]
-    window_sizes_default: window_sizes = (100, 200, 500, 1000, 2000, 5000, 10000, 20000)
-    window_size: TypeAlias = Annotated[
-        int,
-        """
-        The size of windows (number of sites) used to calculate statistics within.
-        """,
-    ]
-    min_cohort_size_default: base_params.min_cohort_size = 20
-    max_cohort_size_default: base_params.max_cohort_size = 50
-
-
-class fst_params:
-    """Parameter definitions for Fst functions."""
-
-    # N.B., window size can mean different things for different functions
-    window_size: TypeAlias = Annotated[
-        int,
-        "The size of windows (number of sites) used to calculate statistics within.",
-    ]
-    cohort_size_default: Optional[base_params.cohort_size] = None
-    min_cohort_size_default: base_params.min_cohort_size = 15
-    max_cohort_size_default: base_params.max_cohort_size = 50
-
-
-class frq_params:
-    """Parameter definitions for functions computing and plotting allele frequencies."""
-
-    drop_invariant: TypeAlias = Annotated[
-        bool,
-        """
-        If True, drop variants not observed in the selected samples.
-        """,
-    ]
-    effects: TypeAlias = Annotated[bool, "If True, add SNP effect annotations."]
-    area_by: TypeAlias = Annotated[
-        str,
-        """
-        Column name in the sample metadata to use to group samples spatially. E.g.,
-        use "admin1_iso" or "admin1_name" to group by level 1 administrative
-        divisions, or use "admin2_name" to group by level 2 administrative
-        divisions.
-        """,
-    ]
-    period_by: TypeAlias = Annotated[
-        Literal["year", "quarter", "month"],
-        "Length of time to group samples temporally.",
-    ]
-    variant_query: TypeAlias = Annotated[
-        str,
-        "A pandas query to be evaluated against variants.",
-    ]
-    nobs_mode: TypeAlias = Annotated[
-        Literal["called", "fixed"],
-        """
-        Method for calculating the denominator when computing frequencies. If
-        "called" then use the number of called alleles, i.e., number of samples
-        with non-missing genotype calls multiplied by 2. If "fixed" then use the
-        number of samples multiplied by 2.
-        """,
-    ]
-    nobs_mode_default: nobs_mode = "called"
-    ci_method: TypeAlias = Annotated[
-        Literal["normal", "agresti_coull", "beta", "wilson", "binom_test"],
-        """
-        Method to use for computing confidence intervals, passed through to
-        `statsmodels.stats.proportion.proportion_confint`.
-        """,
-    ]
-    ci_method_default: ci_method = "wilson"
-    ds_frequencies_advanced: TypeAlias = Annotated[
-        xr.Dataset,
-        """
-        A dataset of variant frequencies, such as returned by
-        `snp_allele_frequencies_advanced()`,
-        `aa_allele_frequencies_advanced()` or
-        `gene_cnv_frequencies_advanced()`.
-        """,
-    ]
-
-
-class het_params:
-    """Parameters for functions related to heterozygosity and runs of homozygosity."""
-
-    single_sample: TypeAlias = Annotated[
-        Union[str, int],
-        "Sample identifier or index within sample set.",
-    ]
-    sample: TypeAlias = Annotated[
-        Union[single_sample, List[single_sample], Tuple[single_sample, ...]],
-        "Sample identifier or index within sample set. Multiple values can also be provided as a list or tuple.",
-    ]
-    window_size: TypeAlias = Annotated[
-        int,
-        "Number of sites per window.",
-    ]
-    window_size_default: window_size = 20_000
-    phet_roh: TypeAlias = Annotated[
-        float,
-        "Probability of observing a heterozygote in a ROH.",
-    ]
-    phet_roh_default: phet_roh = 0.001
-    phet_nonroh: TypeAlias = Annotated[
-        Tuple[float, ...],
-        "One or more probabilities of observing a heterozygote outside a ROH.",
-    ]
-    phet_nonroh_default: phet_nonroh = (0.003, 0.01)
-    transition: TypeAlias = Annotated[
-        float,
-        """
-        Probability of moving between states. A larger window size may call
-        for a larger transitional probability.
-        """,
-    ]
-    transition_default: transition = 0.001
-    y_max: TypeAlias = Annotated[
-        float,
-        "Y axis limit.",
-    ]
-    y_max_default: y_max = 0.03
-    circle_kwargs: TypeAlias = Annotated[
-        Mapping,
-        "Passed through to bokeh circle() function.",
-    ]
-    df_roh: TypeAlias = Annotated[
-        pd.DataFrame,
-        """
-        A DataFrame where each row provides data about a single run of
-        homozygosity.
-        """,
-    ]
-    heterozygosity_height: TypeAlias = Annotated[
-        int,
-        "Height in pixels (px) of heterozygosity track.",
-    ]
-    roh_height: TypeAlias = Annotated[
-        int,
-        "Height in pixels (px) of runs of homozygosity track.",
-    ]
-
-
-class pca_params:
-    """Parameters for PCA functions."""
-
-    n_snps: TypeAlias = Annotated[
-        int,
-        """
-        The desired number of SNPs to use when running the analysis.
-        SNPs will be evenly thinned to approximately this number.
-        """,
-    ]
-    thin_offset: TypeAlias = Annotated[
-        int,
-        """
-        Starting index for SNP thinning. Change this to repeat the analysis
-        using a different set of SNPs.
-        """,
-    ]
-    thin_offset_default: thin_offset = 0
-    min_minor_ac: TypeAlias = Annotated[
-        int,
-        """
-        The minimum minor allele count. SNPs with a minor allele count
-        below this value will be excluded prior to thinning.
-        """,
-    ]
-    min_minor_ac_default: min_minor_ac = 2
-    max_missing_an: TypeAlias = Annotated[
-        int,
-        """
-        The maximum number of missing allele calls to accept. SNPs with
-        more than this value will be excluded prior to thinning. Set to 0
-        (default) to require no missing calls.
-        """,
-    ]
-    max_missing_an_default = 0
-    n_components: TypeAlias = Annotated[
-        int,
-        "Number of components to return.",
-    ]
-    n_components_default: n_components = 20
-    df_pca: TypeAlias = Annotated[
-        pd.DataFrame,
-        """
-        A dataframe of sample metadata, with columns "PC1", "PC2", "PC3",
-        etc., added.
-        """,
-    ]
-    evr: TypeAlias = Annotated[
-        np.ndarray,
-        "An array of explained variance ratios, one per component.",
-    ]
-
-
-class plotly_params:
-    """Parameters for any plotting functions using plotly."""
-
-    # N.B., most of these parameters are always able to take None
-    # and so we set as Optional here, rather than having to repeat
-    # that for each function doc.
-
-    x_label: TypeAlias = Annotated[
-        Optional[str],
-        "X axis label.",
-    ]
-    y_label: TypeAlias = Annotated[
-        Optional[str],
-        "Y axis label.",
-    ]
-    width: TypeAlias = Annotated[
-        Optional[int],
-        "Plot width in pixels (px).",
-    ]
-    height: TypeAlias = Annotated[
-        Optional[int],
-        "Plot height in pixels (px).",
-    ]
-    aspect: TypeAlias = Annotated[
-        Optional[Literal["equal", "auto"]],
-        "Aspect ratio, see also https://plotly.com/python-api-reference/generated/plotly.express.imshow",
-    ]
-    title: TypeAlias = Annotated[
-        Optional[Union[str, bool]],
-        """
-        If True, attempt to use metadata from input dataset as a plot title.
-        Otherwise, use supplied value as a title.
-        """,
-    ]
-    text_auto: TypeAlias = Annotated[
-        Union[bool, str],
-        """
-        If True or a string, single-channel img values will be displayed as text. A
-        string like '.2f' will be interpreted as a texttemplate numeric formatting
-        directive.
-        """,
-    ]
-    color_continuous_scale: TypeAlias = Annotated[
-        Optional[Union[str, List[str]]],
-        """
-        Colormap used to map scalar data to colors (for a 2D image). This
-        parameter is not used for RGB or RGBA images. If a string is provided,
-        it should be the name of a known color scale, and if a list is provided,
-        it should be a list of CSS-compatible colors.
-        """,
-    ]
-    colorbar: TypeAlias = Annotated[
-        bool,
-        "If False, do not display a color bar.",
-    ]
-    x: TypeAlias = Annotated[
-        str,
-        "Name of variable to plot on the X axis.",
-    ]
-    y: TypeAlias = Annotated[
-        str,
-        "Name of variable to plot on the Y axis.",
-    ]
-    z: TypeAlias = Annotated[
-        str,
-        "Name of variable to plot on the Z axis.",
-    ]
-    color: TypeAlias = Annotated[
-        Optional[str],
-        "Name of variable to use to color the markers.",
-    ]
-    symbol: TypeAlias = Annotated[
-        Optional[str],
-        "Name of the variable to use to choose marker symbols.",
-    ]
-    jitter_frac: TypeAlias = Annotated[
-        Optional[float],
-        "Randomly jitter points by this fraction of their range.",
-    ]
-    marker_size: TypeAlias = Annotated[
-        int,
-        "Marker size.",
-    ]
-    template: TypeAlias = Annotated[
-        Optional[
-            Literal[
-                "ggplot2",
-                "seaborn",
-                "simple_white",
-                "plotly",
-                "plotly_white",
-                "plotly_dark",
-                "presentation",
-                "xgridoff",
-                "ygridoff",
-                "gridon",
-                "none",
-            ]
-        ],
-        "The figure template name (must be a key in plotly.io.templates).",
-    ]
-    show: TypeAlias = Annotated[
-        bool,
-        "If true, show the plot. If False, do not show the plot, but return the figure.",
-    ]
-    renderer: TypeAlias = Annotated[Optional[str], "The name of the renderer to use."]
-    figure: TypeAlias = Annotated[
-        Optional[go.Figure], "A plotly figure (only returned if show=False)."
-    ]
-
-
-class ihs_params:
-    window_size: TypeAlias = Annotated[
-        int,
-        """
-        The size of window in number of SNPs used to summarise iHS over.
-        If None, per-variant iHS values are returned.
-        """,
-    ]
-    window_size_default: window_size = 200
-    min_cohort_size_default: base_params.min_cohort_size = 15
-    max_cohort_size_default: base_params.max_cohort_size = 50
-    percentiles: TypeAlias = Annotated[
-        Union[int, Tuple[int, ...]],
-        """
-        If window size is specified, this returns the iHS percentiles
-        for each window.
-        """,
-    ]
-    percentiles_default: percentiles = (50, 75, 100)
-    standardize: TypeAlias = Annotated[
-        bool, "If True, standardize iHS values by alternate allele counts."
-    ]
-    standardization_bins: TypeAlias = Annotated[
-        Tuple[float, ...],
-        "If provided, use these allele count bins to standardize iHS values.",
-    ]
-    standardization_n_bins: TypeAlias = Annotated[
-        int,
-        """
-        Number of allele count bins to use for standardization.
-        Overrides standardization_bins.
-        """,
-    ]
-    standardization_n_bins_default: standardization_n_bins = 20
-    standardization_diagnostics: TypeAlias = Annotated[
-        bool, "If True, plot some diagnostics about the standardization."
-    ]
-    filter_min_maf: TypeAlias = Annotated[
-        float,
-        """
-        Minimum minor allele frequency to use for filtering prior to passing
-        haplotypes to allel.ihs function
-        """,
-    ]
-    filter_min_maf_default: filter_min_maf = 0.05
-    compute_min_maf: TypeAlias = Annotated[
-        float,
-        """
-        Do not compute integrated haplotype homozygosity for variants with
-        minor allele frequency below this threshold.
-        """,
-    ]
-    compute_min_maf_default: compute_min_maf = 0.05
-    min_ehh: TypeAlias = Annotated[
-        float,
-        """
-        Minimum EHH beyond which to truncate integrated haplotype homozygosity
-        calculation.
-        """,
-    ]
-    min_ehh_default: min_ehh = 0.05
-    max_gap: TypeAlias = Annotated[
-        int,
-        """
-        Do not report scores if EHH spans a gap larger than this number of
-        base pairs.
-        """,
-    ]
-    max_gap_default: max_gap = 200_000
-    gap_scale: TypeAlias = Annotated[
-        int, "Rescale distance between variants if gap is larger than this value."
-    ]
-    gap_scale_default: gap_scale = 20_000
-    include_edges: TypeAlias = Annotated[
-        bool,
-        """
-        If True, report scores even if EHH does not decay below min_ehh at the
-        end of the chromosome.
-        """,
-    ]
-    use_threads: TypeAlias = Annotated[
-        bool, "If True, use multiple threads to compute iHS."
-    ]
-    palette: TypeAlias = Annotated[
-        str, "Name of bokeh palette to use for plotting multiple percentiles."
-    ]
-    palette_default: palette = "Blues"
-
-
-class hapclust_params:
-    linkage_method: TypeAlias = Annotated[
-        Literal[
-            "single", "complete", "average", "weighted", "centroid", "median", "ward"
-        ],
-        """
-        The linkage algorithm to use. See the Linkage Methods section of the
-        scipy.cluster.hierarchy.linkage docs for full descriptions.
-        """,
-    ]
-    linkage_method_default: linkage_method = "single"
-    count_sort: TypeAlias = Annotated[
-        bool,
-        """
-        For each node n, the order (visually, from left-to-right) n's two descendant
-        links are plotted is determined by this parameter. If True, the child with
-        the minimum number of original objects in its cluster is plotted first. Note
-        distance_sort and count_sort cannot both be True.
-        """,
-    ]
-    distance_sort: TypeAlias = Annotated[
-        bool,
-        """
-        For each node n, the order (visually, from left-to-right) n's two descendant
-        links are plotted is determined by this parameter. If True, The child with the
-        minimum distance between its direct descendants is plotted first.
-        """,
-    ]
-
-
-class hapnet_params:
-    max_dist: TypeAlias = Annotated[
-        int,
-        "Join network components up to a maximum distance of 2 SNP differences.",
-    ]
-    max_dist_default: max_dist = 2
-    color: TypeAlias = Annotated[
-        str,
-        """
-        Identifies a column in the sample metadata which determines the colour
-        of pie chart segments within nodes.
-        """,
-    ]
-    color_discrete_sequence: TypeAlias = Annotated[
-        List, "Provide a list of colours to use."
-    ]
-    color_discrete_map: TypeAlias = Annotated[
-        Mapping, "Provide an explicit mapping from values to colours."
-    ]
-    category_order: TypeAlias = Annotated[
-        List,
-        "Control the order in which values appear in the legend.",
-    ]
-    node_size_factor: TypeAlias = Annotated[
-        int,
-        "Control the sizing of nodes.",
-    ]
-    node_size_factor_default: node_size_factor = 50
-    layout: TypeAlias = Annotated[
-        str,
-        "Name of the network layout to use to position nodes.",
-    ]
-    layout_default: layout = "cose"
-    layout_params: TypeAlias = Annotated[
-        Mapping,
-        "Additional parameters to the layout algorithm.",
-    ]
-
-
-class dash_params:
-    height: TypeAlias = Annotated[int, "Height of the Dash app in pixels (px)."]
-    width: TypeAlias = Annotated[Union[int, str], "Width of the Dash app."]
-    server_mode: TypeAlias = Annotated[
-        Literal["inline", "external", "jupyterlab"],
-        """
-        Controls how the Jupyter Dash app will be launched. See
-        https://medium.com/plotly/introducing-jupyterdash-811f1f57c02e for
-        more information.
-        """,
-    ]
-    server_mode_default: server_mode = "inline"
-    server_port: TypeAlias = Annotated[
-        int,
-        "Manually override the port on which the Dash app will run.",
-    ]
-
-
 # N.B., we are in the process of breaking up the AnophelesDataResource
 # class into multiple parent classes like AnophelesGenomeSequenceData
 # and AnophelesBase. This is work in progress, and further PRs are
 # expected to factor out functions defined here in to separate classes.
 # For more information, see:
 #
 # https://github.com/malariagen/malariagen-data-python/issues/366
@@ -603,14 +77,15 @@
 # https://en.wikipedia.org/wiki/C3_linearization
 # https://rhettinger.wordpress.com/2011/05/26/super-considered-super/
 
 
 # work around pycharm failing to recognise that doc() is callable
 # noinspection PyCallingNonCallable
 class AnophelesDataResource(
+    AnophelesHapData,
     AnophelesSnpData,
     AnophelesSampleMetadata,
     AnophelesGenomeFeaturesData,
     AnophelesGenomeSequenceData,
     AnophelesBase,
 ):
     """Anopheles data resources."""
@@ -620,14 +95,15 @@
         url,
         config_path,
         cohorts_analysis: Optional[str],
         aim_analysis: Optional[str],
         aim_metadata_dtype: Optional[Mapping[str, Any]],
         site_filters_analysis: Optional[str],
         default_site_mask: Optional[str],
+        default_phasing_analysis: Optional[str],
         bokeh_output_notebook: bool,
         results_cache: Optional[str],
         log,
         debug,
         show_progress,
         check_location,
         pre,
@@ -654,37 +130,29 @@
             gff_gene_type=gff_gene_type,
             gff_default_attributes=gff_default_attributes,
             cohorts_analysis=cohorts_analysis,
             aim_analysis=aim_analysis,
             aim_metadata_dtype=aim_metadata_dtype,
             site_filters_analysis=site_filters_analysis,
             default_site_mask=default_site_mask,
+            default_phasing_analysis=default_phasing_analysis,
             results_cache=results_cache,
         )
 
         # set up caches
         # TODO review type annotations here, maybe can tighten
         self._cache_annotator = None
-        self._cache_site_annotations = None
-        self._cache_locate_site_class: Dict = dict()
-        self._cache_haplotypes: Dict = dict()
-        self._cache_haplotype_sites: Dict = dict()
 
     @property
     @abstractmethod
     def _pca_results_cache_name(self):
         raise NotImplementedError("Must override _pca_results_cache_name")
 
     @property
     @abstractmethod
-    def _snp_allele_counts_results_cache_name(self):
-        raise NotImplementedError("Must override _snp_allele_counts_results_cache_name")
-
-    @property
-    @abstractmethod
     def _fst_gwss_results_cache_name(self):
         raise NotImplementedError("Must override _fst_gwss_results_cache_name")
 
     @property
     @abstractmethod
     def _h12_calibration_cache_name(self):
         raise NotImplementedError("Must override _h12_calibration_cache_name")
@@ -710,58 +178,28 @@
         raise NotImplementedError("Must override _h1x_gwss_cache_name")
 
     @property
     @abstractmethod
     def _ihs_gwss_cache_name(self):
         raise NotImplementedError("Must override _ihs_gwss_cache_name")
 
-    @property
-    @abstractmethod
-    def _site_annotations_zarr_path(self):
-        raise NotImplementedError("Must override _site_annotations_zarr_path")
-
     @abstractmethod
     def _transcript_to_gene_name(self, transcript):
         # children may have different manual overrides.
         raise NotImplementedError("Must override _transcript_to_gene_name")
 
     @abstractmethod
     def _view_alignments_add_site_filters_tracks(
         self, *, contig, visibility_window, tracks
     ):
         # default implementation, do nothing
         raise NotImplementedError(
             "Must override _view_alignments_add_site_filters_tracks"
         )
 
-    @property
-    @abstractmethod
-    def phasing_analysis_ids(self):
-        """Identifiers for the different phasing analyses that are available.
-        These are values than can be used for the `analysis` parameter in any
-        method making using of haplotype data.
-
-        """
-        # Not all children have the same phasing analysis IDs.
-        raise NotImplementedError("Must override _phasing_analysis_ids")
-
-    @property
-    @abstractmethod
-    def _default_phasing_analysis(self):
-        raise NotImplementedError("Must override _default_phasing_analysis")
-
-    def _prep_phasing_analysis_param(self, *, analysis):
-        if analysis == DEFAULT:
-            analysis = self._default_phasing_analysis
-        if analysis not in self.phasing_analysis_ids:
-            raise ValueError(
-                f"Invalid phasing analysis, must be one of f{self.phasing_analysis_ids}."
-            )
-        return analysis
-
     @check_types
     @doc(
         summary="""
             Group samples by taxon, area (space) and period (time), then compute
             SNP allele frequencies.
         """,
         returns="""
@@ -3926,236 +3364,14 @@
             bokeh.plotting.show(fig)
             return None
         else:
             return fig
 
     @check_types
     @doc(
-        summary="Open haplotypes zarr.",
-        returns="Zarr hierarchy.",
-    )
-    def open_haplotypes(
-        self,
-        sample_set: base_params.sample_set,
-        analysis: hap_params.analysis = DEFAULT,
-    ) -> Optional[zarr.hierarchy.Group]:
-        analysis = self._prep_phasing_analysis_param(analysis=analysis)
-        try:
-            return self._cache_haplotypes[(sample_set, analysis)]
-        except KeyError:
-            release = self.lookup_release(sample_set=sample_set)
-            release_path = self._release_to_path(release)
-            path = f"{self._base_path}/{release_path}/snp_haplotypes/{sample_set}/{analysis}/zarr"
-            store = init_zarr_store(fs=self._fs, path=path)
-            # Some sample sets have no data for a given analysis, handle this.
-            try:
-                root = zarr.open_consolidated(store=store)
-            except FileNotFoundError:
-                root = None
-            self._cache_haplotypes[(sample_set, analysis)] = root
-        return root
-
-    @check_types
-    @doc(
-        summary="Open haplotype sites zarr.",
-        returns="Zarr hierarchy.",
-    )
-    def open_haplotype_sites(
-        self, analysis: hap_params.analysis = DEFAULT
-    ) -> zarr.hierarchy.Group:
-        analysis = self._prep_phasing_analysis_param(analysis=analysis)
-        try:
-            return self._cache_haplotype_sites[analysis]
-        except KeyError:
-            path = f"{self._base_path}/{self._major_version_path}/snp_haplotypes/sites/{analysis}/zarr"
-            store = init_zarr_store(fs=self._fs, path=path)
-            root = zarr.open_consolidated(store=store)
-            self._cache_haplotype_sites[analysis] = root
-        return root
-
-    def _haplotype_sites_for_contig(
-        self, *, contig, analysis, field, inline_array, chunks
-    ):
-        sites = self.open_haplotype_sites(analysis=analysis)
-        arr = sites[f"{contig}/variants/{field}"]
-        arr = da_from_zarr(arr, inline_array=inline_array, chunks=chunks)
-        return arr
-
-    def _haplotypes_for_contig(
-        self, *, contig, sample_set, analysis, inline_array, chunks
-    ):
-        debug = self._log.debug
-
-        debug("open zarr")
-        root = self.open_haplotypes(sample_set=sample_set, analysis=analysis)
-        sites = self.open_haplotype_sites(analysis=analysis)
-
-        debug("variant_position")
-        pos = sites[f"{contig}/variants/POS"]
-
-        # some sample sets have no data for a given analysis, handle this
-        # TODO consider returning a dataset with 0 length samples dimension instead, would
-        # probably simplify a lot of other logic
-        if root is None:
-            return None
-
-        coords = dict()
-        data_vars = dict()
-
-        coords["variant_position"] = (
-            [DIM_VARIANT],
-            da_from_zarr(pos, inline_array=inline_array, chunks=chunks),
-        )
-
-        debug("variant_contig")
-        contig_index = self.contigs.index(contig)
-        coords["variant_contig"] = (
-            [DIM_VARIANT],
-            da.full_like(pos, fill_value=contig_index, dtype="u1"),
-        )
-
-        debug("variant_allele")
-        ref = da_from_zarr(
-            sites[f"{contig}/variants/REF"], inline_array=inline_array, chunks=chunks
-        )
-        alt = da_from_zarr(
-            sites[f"{contig}/variants/ALT"], inline_array=inline_array, chunks=chunks
-        )
-        variant_allele = da.hstack([ref[:, None], alt[:, None]])
-        data_vars["variant_allele"] = [DIM_VARIANT, DIM_ALLELE], variant_allele
-
-        debug("call_genotype")
-        data_vars["call_genotype"] = (
-            [DIM_VARIANT, DIM_SAMPLE, DIM_PLOIDY],
-            da_from_zarr(
-                root[f"{contig}/calldata/GT"], inline_array=inline_array, chunks=chunks
-            ),
-        )
-
-        debug("sample arrays")
-        coords["sample_id"] = (
-            [DIM_SAMPLE],
-            da_from_zarr(root["samples"], inline_array=inline_array, chunks=chunks),
-        )
-
-        debug("set up attributes")
-        attrs = {"contigs": self.contigs}
-
-        debug("create a dataset")
-        ds = xr.Dataset(data_vars=data_vars, coords=coords, attrs=attrs)
-
-        return ds
-
-    @check_types
-    @doc(
-        summary="Access haplotype data.",
-        returns="A dataset of haplotypes and associated data.",
-    )
-    def haplotypes(
-        self,
-        region: base_params.region,
-        analysis: hap_params.analysis = DEFAULT,
-        sample_sets: Optional[base_params.sample_sets] = None,
-        sample_query: Optional[base_params.sample_query] = None,
-        inline_array: base_params.inline_array = base_params.inline_array_default,
-        chunks: base_params.chunks = base_params.chunks_default,
-        cohort_size: Optional[base_params.cohort_size] = None,
-        min_cohort_size: Optional[base_params.min_cohort_size] = None,
-        max_cohort_size: Optional[base_params.max_cohort_size] = None,
-        random_seed: base_params.random_seed = 42,
-    ) -> Optional[xr.Dataset]:
-        debug = self._log.debug
-
-        debug("normalise parameters")
-        sample_sets = self._prep_sample_sets_param(sample_sets=sample_sets)
-        regions: List[Region] = parse_multi_region(self, region)
-        del region
-        analysis = self._prep_phasing_analysis_param(analysis=analysis)
-
-        debug("build dataset")
-        lx = []
-        for r in regions:
-            ly = []
-
-            for s in sample_sets:
-                y = self._haplotypes_for_contig(
-                    contig=r.contig,
-                    sample_set=s,
-                    analysis=analysis,
-                    inline_array=inline_array,
-                    chunks=chunks,
-                )
-                if y is not None:
-                    ly.append(y)
-
-            if len(ly) == 0:
-                debug("early out, no data for given sample sets and analysis")
-                return None
-
-            debug("concatenate data from multiple sample sets")
-            x = simple_xarray_concat(ly, dim=DIM_SAMPLE)
-
-            debug("handle region")
-            if r.start or r.end:
-                pos = x["variant_position"].values
-                loc_region = locate_region(r, pos)
-                x = x.isel(variants=loc_region)
-
-            lx.append(x)
-
-        debug("concatenate data from multiple regions")
-        ds = simple_xarray_concat(lx, dim=DIM_VARIANT)
-
-        debug("handle sample query")
-        if sample_query is not None:
-            debug("load sample metadata")
-            df_samples = self.sample_metadata(sample_sets=sample_sets)
-
-            debug("align sample metadata with haplotypes")
-            phased_samples = ds["sample_id"].values.tolist()
-            df_samples_phased = (
-                df_samples.set_index("sample_id").loc[phased_samples].reset_index()
-            )
-
-            debug("apply the query")
-            loc_samples = df_samples_phased.eval(sample_query).values
-            if np.count_nonzero(loc_samples) == 0:
-                raise ValueError(f"No samples found for query {sample_query!r}")
-            ds = ds.isel(samples=loc_samples)
-
-        debug("handle cohort size")
-        if cohort_size is not None:
-            debug("handle cohort size")
-            # overrides min and max
-            min_cohort_size = cohort_size
-            max_cohort_size = cohort_size
-
-        if min_cohort_size is not None:
-            debug("handle min cohort size")
-            n_samples = ds.dims["samples"]
-            if n_samples < min_cohort_size:
-                raise ValueError(
-                    f"not enough samples ({n_samples}) for minimum cohort size ({min_cohort_size})"
-                )
-
-        if max_cohort_size is not None:
-            debug("handle max cohort size")
-            n_samples = ds.dims["samples"]
-            if n_samples > max_cohort_size:
-                rng = np.random.default_rng(seed=random_seed)
-                loc_downsample = rng.choice(
-                    n_samples, size=max_cohort_size, replace=False
-                )
-                loc_downsample.sort()
-                ds = ds.isel(samples=loc_downsample)
-
-        return ds
-
-    @check_types
-    @doc(
         summary="Generate h12 GWSS calibration data for different window sizes.",
         returns="""
             A list of H12 calibration run arrays for each window size, containing
             values and percentiles.
         """,
     )
     def h12_calibration(
@@ -5289,14 +4505,15 @@
         random_seed: base_params.random_seed = 42,
     ) -> Tuple[np.ndarray, np.ndarray]:
         # change this name if you ever change the behaviour of this function, to
         # invalidate any previously cached data
         name = self._g123_gwss_cache_name
 
         if sites == DEFAULT:
+            assert self._default_phasing_analysis is not None
             sites = self._default_phasing_analysis
         valid_sites = self.phasing_analysis_ids + ("all", "segregating")
         if sites not in valid_sites:
             raise ValueError(
                 f"Invalid value for `sites` parameter, must be one of {valid_sites}."
             )
```

### Comparing `malariagen_data-7.8.0/malariagen_data/mjn.py` & `malariagen_data-7.9.0/malariagen_data/mjn.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/pf7.py` & `malariagen_data-7.9.0/malariagen_data/pf7.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/pf7_config.json` & `malariagen_data-7.9.0/malariagen_data/pf7_config.json`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/plasmodium.py` & `malariagen_data-7.9.0/malariagen_data/plasmodium.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/plotly_dendrogram.py` & `malariagen_data-7.9.0/malariagen_data/plotly_dendrogram.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/pv4.py` & `malariagen_data-7.9.0/malariagen_data/pv4.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/pv4_config.json` & `malariagen_data-7.9.0/malariagen_data/pv4_config.json`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/malariagen_data/util.py` & `malariagen_data-7.9.0/malariagen_data/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import pandas as pd
 import plotly.express as px
 import typeguard
 import xarray as xr
 import zarr
 from fsspec.core import url_to_fs
 from fsspec.mapping import FSMap
-from numpydoc_decorator.impl import format_type
+from numpydoc_decorator.impl import humanize_type
 from typing_extensions import TypeAlias, get_type_hints
 
 DIM_VARIANT = "variants"
 DIM_ALLELE = "alleles"
 DIM_SAMPLE = "samples"
 DIM_PLOIDY = "ploidy"
 
@@ -374,21 +374,23 @@
         # parse region string that contains genomic coordinates
         region_split = region_pattern_match.groups()
         contig = region_split[0]
         start = int(region_split[1].replace(",", ""))
         end = int(region_split[2].replace(",", ""))
 
         if contig not in _valid_contigs(resource):
-            raise ValueError(f"Contig {contig} does not exist in the dataset.")
-        elif (
-            start < 0
-            or end <= start
-            or end > resource.genome_sequence(region=contig).shape[0]
-        ):
-            raise ValueError("Provided genomic coordinates are not valid.")
+            raise ValueError(
+                f"The genomic region {region!r} is invalid because contig {contig!r} does not exist in the dataset."
+            )
+        else:
+            contig_length = resource.genome_sequence(region=contig).shape[0]
+            if start < 1 or end < start or end > contig_length:
+                raise ValueError(
+                    f"The genomic region {region!r} is invalid for contig {contig!r} with length {contig_length}."
+                )
 
         return Region(contig, start, end)
 
     else:
         return None
 
 
@@ -909,16 +911,16 @@
         call_args = getcallargs(f, *args, **kwargs)
         for k, t in type_hints.items():
             if k in call_args:
                 v = call_args[k]
                 try:
                     typeguard.check_type(v, t)
                 except typeguard.TypeCheckError as e:
-                    expected_type = format_type(t)
-                    actual_type = format_type(type(v))
+                    expected_type = humanize_type(t)
+                    actual_type = humanize_type(type(v))
                     message = fill(
                         dedent(
                             f"""
                         Parameter {k!r} with value {v!r} in call to function {f.__name__!r} has incorrect type:
                         found {actual_type}, expected {expected_type}. See below for further information.
                     """
                         )
```

### Comparing `malariagen_data-7.8.0/malariagen_data/veff.py` & `malariagen_data-7.9.0/malariagen_data/veff.py`

 * *Files identical despite different names*

### Comparing `malariagen_data-7.8.0/pyproject.toml` & `malariagen_data-7.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "malariagen_data"
-version = "7.8.0"
+version = "7.9.0"
 description = "A package for accessing and analysing MalariaGEN data."
 authors = [
     "Alistair Miles <alistair.miles@sanger.ac.uk>",
     "Chris Clarkson <cc28@sanger.ac.uk>",
     "Lee Hart <lee.hart@sanger.ac.uk>",
     "Kathryn Murie <km22@sanger.ac.uk>",
     "Nace Kranjc <n.kranjc@imperial.ac.uk>",
@@ -45,15 +45,15 @@
 # bug in ipinfo 4.4.1
 ipinfo = "!=4.4.1"
 igv-notebook = ">=0.2.3"
 tqdm = "*"
 dash = "*"
 dash-cytoscape = "*"
 jupyter-dash = "*"
-numpydoc_decorator = ">=2.0.0"
+numpydoc_decorator = ">=2.1.0"
 typing_extensions = "*"
 typeguard = ">=4.0.0"
 protopunica = "*"
 # accelerate plotly - https://plotly.com/python/renderers/#performance
 orjson = "*"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `malariagen_data-7.8.0/PKG-INFO` & `malariagen_data-7.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malariagen-data
-Version: 7.8.0
+Version: 7.9.0
 Summary: A package for accessing and analysing MalariaGEN data.
 License: MIT
 Author: Alistair Miles
 Author-email: alistair.miles@sanger.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,15 @@
 Requires-Dist: ipinfo (!=4.4.1)
 Requires-Dist: ipyleaflet (>0.17.0)
 Requires-Dist: ipywidgets
 Requires-Dist: jupyter-dash
 Requires-Dist: llvmlite (>0.34)
 Requires-Dist: numba
 Requires-Dist: numpy (<1.25)
-Requires-Dist: numpydoc_decorator (>=2.0.0)
+Requires-Dist: numpydoc_decorator (>=2.1.0)
 Requires-Dist: orjson
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: protopunica
 Requires-Dist: scikit-allel
 Requires-Dist: scipy
 Requires-Dist: statsmodels
```

