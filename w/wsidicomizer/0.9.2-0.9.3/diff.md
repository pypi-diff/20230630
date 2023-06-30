# Comparing `tmp/wsidicomizer-0.9.2.tar.gz` & `tmp/wsidicomizer-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidicomizer-0.9.2.tar", max compression
+gzip compressed data, was "wsidicomizer-0.9.3.tar", max compression
```

## Comparing `wsidicomizer-0.9.2.tar` & `wsidicomizer-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1733 2023-05-11 13:26:16.759959 wsidicomizer-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     8191 2023-05-11 13:26:16.751696 wsidicomizer-0.9.2/README.md
--rw-r--r--   0        0        0      921 2023-05-11 13:26:16.764698 wsidicomizer-0.9.2/wsidicomizer/__init__.py
--rw-r--r--   0        0        0    10732 2023-04-03 13:27:43.562194 wsidicomizer-0.9.2/wsidicomizer/cli.py
--rw-r--r--   0        0        0     1197 2023-04-03 06:05:46.207813 wsidicomizer-0.9.2/wsidicomizer/config.py
--rw-r--r--   0        0        0    23475 2023-04-27 11:02:16.094157 wsidicomizer-0.9.2/wsidicomizer/dataset.py
--rw-r--r--   0        0        0     6735 2023-04-27 11:02:16.096375 wsidicomizer-0.9.2/wsidicomizer/dicomizer_source.py
--rw-r--r--   0        0        0     6094 2023-05-11 13:26:16.766698 wsidicomizer-0.9.2/wsidicomizer/encoding.py
--rw-r--r--   0        0        0      789 2023-04-03 13:27:43.575189 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/__init__.py
--rw-r--r--   0        0        0     2228 2023-04-03 13:27:43.576394 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_cli.py
--rw-r--r--   0        0        0     3913 2023-04-27 11:02:16.099286 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_dicomizer.py
--rw-r--r--   0        0        0     4418 2023-04-03 13:27:43.578184 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_image_data.py
--rw-r--r--   0        0        0    14802 2023-04-08 06:20:09.255055 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_reader.py
--rw-r--r--   0        0        0     5403 2023-04-27 11:02:16.100156 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_source.py
--rw-r--r--   0        0        0      769 2023-04-03 06:08:44.876033 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/__init__.py
--rw-r--r--   0        0        0     2227 2023-04-03 06:08:51.748970 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide.py
--rw-r--r--   0        0        0    16631 2023-04-03 13:27:43.582423 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_image_data.py
--rw-r--r--   0        0        0     1476 2023-04-03 13:27:43.593514 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_metadata.py
--rw-r--r--   0        0        0     3787 2023-04-27 11:02:16.102156 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_source.py
--rw-r--r--   0        0        0     2069 2023-04-03 06:06:15.956751 wsidicomizer-0.9.2/wsidicomizer/image_data.py
--rw-r--r--   0        0        0      860 2023-04-03 13:27:43.595183 wsidicomizer-0.9.2/wsidicomizer/sources/__init__.py
--rw-r--r--   0        0        0      746 2023-03-31 14:54:00.564988 wsidicomizer-0.9.2/wsidicomizer/sources/czi/__init__.py
--rw-r--r--   0        0        0    13161 2023-04-03 13:27:43.605550 wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_image_data.py
--rw-r--r--   0        0        0     7933 2023-04-27 11:02:16.105158 wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_metadata.py
--rw-r--r--   0        0        0     2899 2023-04-27 11:02:16.109161 wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_source.py
--rw-r--r--   0        0        0      771 2023-04-16 18:02:33.046081 wsidicomizer-0.9.2/wsidicomizer/sources/opentile/__init__.py
--rw-r--r--   0        0        0     8756 2023-04-08 06:20:09.243941 wsidicomizer-0.9.2/wsidicomizer/sources/opentile/opentile_image_data.py
--rw-r--r--   0        0        0     3102 2023-04-27 11:02:16.111155 wsidicomizer-0.9.2/wsidicomizer/sources/opentile/opentile_source.py
--rw-r--r--   0        0        0      775 2023-04-03 13:27:43.622220 wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/__init__.py
--rw-r--r--   0        0        0    15167 2023-04-27 11:02:16.112156 wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_image_data.py
--rw-r--r--   0        0        0     1443 2023-04-27 11:02:16.114308 wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_metadata.py
--rw-r--r--   0        0        0     3575 2023-04-27 11:02:16.116157 wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_source.py
--rw-r--r--   0        0        0     9593 2023-05-11 13:26:16.769358 wsidicomizer-0.9.2/wsidicomizer/wsidicomizer.py
--rw-r--r--   0        0        0     9768 1970-01-01 00:00:00.000000 wsidicomizer-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1733 2023-05-17 20:38:44.455698 wsidicomizer-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     8191 2023-05-11 13:26:16.751696 wsidicomizer-0.9.3/README.md
+-rw-r--r--   0        0        0      921 2023-05-17 20:38:44.458743 wsidicomizer-0.9.3/wsidicomizer/__init__.py
+-rw-r--r--   0        0        0     7095 2023-05-17 20:38:44.461578 wsidicomizer-0.9.3/wsidicomizer/cli.py
+-rw-r--r--   0        0        0     1197 2023-04-03 06:05:46.207813 wsidicomizer-0.9.3/wsidicomizer/config.py
+-rw-r--r--   0        0        0    23475 2023-04-27 11:02:16.094157 wsidicomizer-0.9.3/wsidicomizer/dataset.py
+-rw-r--r--   0        0        0     6735 2023-04-27 11:02:16.096375 wsidicomizer-0.9.3/wsidicomizer/dicomizer_source.py
+-rw-r--r--   0        0        0     6094 2023-05-11 13:26:16.766698 wsidicomizer-0.9.3/wsidicomizer/encoding.py
+-rw-r--r--   0        0        0      789 2023-04-03 13:27:43.575189 wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/__init__.py
+-rw-r--r--   0        0        0     2322 2023-05-17 20:38:44.464576 wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_cli.py
+-rw-r--r--   0        0        0     3945 2023-05-17 20:38:44.467578 wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_dicomizer.py
+-rw-r--r--   0        0        0     4418 2023-04-03 13:27:43.578184 wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_image_data.py
+-rw-r--r--   0        0        0    14802 2023-04-08 06:20:09.255055 wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_reader.py
+-rw-r--r--   0        0        0     5403 2023-04-27 11:02:16.100156 wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_source.py
+-rw-r--r--   0        0        0      769 2023-04-03 06:08:44.876033 wsidicomizer-0.9.3/wsidicomizer/extras/openslide/__init__.py
+-rw-r--r--   0        0        0     2283 2023-05-17 20:38:37.773666 wsidicomizer-0.9.3/wsidicomizer/extras/openslide/openslide.py
+-rw-r--r--   0        0        0    16631 2023-04-03 13:27:43.582423 wsidicomizer-0.9.3/wsidicomizer/extras/openslide/openslide_image_data.py
+-rw-r--r--   0        0        0     1476 2023-04-03 13:27:43.593514 wsidicomizer-0.9.3/wsidicomizer/extras/openslide/openslide_metadata.py
+-rw-r--r--   0        0        0     3787 2023-04-27 11:02:16.102156 wsidicomizer-0.9.3/wsidicomizer/extras/openslide/openslide_source.py
+-rw-r--r--   0        0        0     2069 2023-04-03 06:06:15.956751 wsidicomizer-0.9.3/wsidicomizer/image_data.py
+-rw-r--r--   0        0        0      860 2023-04-03 13:27:43.595183 wsidicomizer-0.9.3/wsidicomizer/sources/__init__.py
+-rw-r--r--   0        0        0      746 2023-03-31 14:54:00.564988 wsidicomizer-0.9.3/wsidicomizer/sources/czi/__init__.py
+-rw-r--r--   0        0        0    13161 2023-04-03 13:27:43.605550 wsidicomizer-0.9.3/wsidicomizer/sources/czi/czi_image_data.py
+-rw-r--r--   0        0        0     7933 2023-04-27 11:02:16.105158 wsidicomizer-0.9.3/wsidicomizer/sources/czi/czi_metadata.py
+-rw-r--r--   0        0        0     2899 2023-04-27 11:02:16.109161 wsidicomizer-0.9.3/wsidicomizer/sources/czi/czi_source.py
+-rw-r--r--   0        0        0      771 2023-04-16 18:02:33.046081 wsidicomizer-0.9.3/wsidicomizer/sources/opentile/__init__.py
+-rw-r--r--   0        0        0     8756 2023-04-08 06:20:09.243941 wsidicomizer-0.9.3/wsidicomizer/sources/opentile/opentile_image_data.py
+-rw-r--r--   0        0        0     3102 2023-04-27 11:02:16.111155 wsidicomizer-0.9.3/wsidicomizer/sources/opentile/opentile_source.py
+-rw-r--r--   0        0        0      775 2023-04-03 13:27:43.622220 wsidicomizer-0.9.3/wsidicomizer/sources/tiffslide/__init__.py
+-rw-r--r--   0        0        0    15167 2023-04-27 11:02:16.112156 wsidicomizer-0.9.3/wsidicomizer/sources/tiffslide/tiffslide_image_data.py
+-rw-r--r--   0        0        0     1443 2023-04-27 11:02:16.114308 wsidicomizer-0.9.3/wsidicomizer/sources/tiffslide/tiffslide_metadata.py
+-rw-r--r--   0        0        0     3575 2023-04-27 11:02:16.116157 wsidicomizer-0.9.3/wsidicomizer/sources/tiffslide/tiffslide_source.py
+-rw-r--r--   0        0        0     9625 2023-05-17 20:38:44.470636 wsidicomizer-0.9.3/wsidicomizer/wsidicomizer.py
+-rw-r--r--   0        0        0     9768 1970-01-01 00:00:00.000000 wsidicomizer-0.9.3/PKG-INFO
```

### Comparing `wsidicomizer-0.9.2/pyproject.toml` & `wsidicomizer-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wsidicomizer"
-version = "0.9.2"
+version = "0.9.3"
 description = "Tool for reading WSI files from proprietary formats and optionally convert them to to DICOM"
 authors = ["Erik O Gabrielsson <erik.o.gabrielsson@sectra.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/imi-bigpicture/wsidicomizer"
 keywords = ["whole slide image", "digital pathology", "dicom", "converter"]
 classifiers = [
```

### Comparing `wsidicomizer-0.9.2/README.md` & `wsidicomizer-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/__init__.py` & `wsidicomizer-0.9.3/wsidicomizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     create_patient_module,
     create_sample,
     create_specimen_module,
     create_study_module,
 )
 from wsidicomizer.wsidicomizer import WsiDicomizer
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
```

### Comparing `wsidicomizer-0.9.2/wsidicomizer/cli.py` & `wsidicomizer-0.9.3/wsidicomizer/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -67,14 +67,19 @@
             nargs='+',
             help=(
                 'Pyramid levels to include, if not all. E.g. 0 1 for base and '
                 'first pyramid layer. '
             ),
         )
         self._parser.add_argument(
+            '--label',
+            type=Path,
+            help='Optional label image to use instead of label found in file.'
+        )
+        self._parser.add_argument(
             '--no-label',
             action="store_true",
             help='If not to include label'
         )
         self._parser.add_argument(
             '--no-overview',
             action="store_true",
@@ -101,19 +106,19 @@
             '--format',
             type=str,
             default='jpeg',
             help="Encoding format to use if re-encoding. 'jpeg' or 'jpeg2000'."
         )
         self._parser.add_argument(
             '--quality',
-            type=int,
+            type=float,
             default=90,
             help=(
-                "Quality to use if re-encoding. Do not use > 95 for jpeg. "
-                "Use 100 for lossless jpeg2000."
+                "Quality to use if re-encoding. It is recommended to not use > 95 for "
+                "jpeg. Use < 1 or > 1000 for lossless jpeg2000."
             )
         )
         self._parser.add_argument(
             '--subsampling',
             type=str,
             default='420',
             help=(
@@ -143,197 +148,68 @@
             levels = None
         else:
             levels = args.levels
         offset_table: Optional[str] = args.offset_table
         if offset_table == 'None':
             offset_table = None
         self.convert(
-            filepath=str(args.input),
-            output_path=str(args.output),
+            filepath=args.input,
+            output_path=args.output,
             modules=dataset,
             tile_size=args.tile_size,
             include_levels=levels,
             include_label=not args.no_label,
             include_overview=not args.no_overview,
             include_confidential=not args.no_confidential,
             workers=args.workers,
             chunk_size=args.chunk_size,
             encoding_format=args.format,
             encoding_quality=args.quality,
             jpeg_subsampling=args.subsampling,
-            offset_table=offset_table
+            offset_table=offset_table,
+            label=args.label
         )
 
     def convert(
         self,
-        filepath: str,
-        output_path: str,
+        filepath: Path,
+        output_path: Path,
         modules: Optional[Dataset] = None,
         tile_size: int = 512,
         include_levels: Optional[Sequence[int]] = None,
         include_label: bool = True,
         include_overview: bool = True,
         include_confidential: bool = True,
         workers: Optional[int] = None,
         chunk_size: Optional[int] = None,
         encoding_format: str = 'jpeg',
-        encoding_quality: int = 90,
+        encoding_quality: float = 90,
         jpeg_subsampling: str = '420',
-        offset_table: Optional[str] = 'bot'
+        offset_table: Optional[str] = 'bot',
+        label: Optional[Path] = None
     ):
-        return WsiDicomizer.convert(
+        WsiDicomizer.convert(
             filepath=filepath,
             output_path=output_path,
             modules=modules,
             tile_size=tile_size,
             include_levels=include_levels,
             include_label=include_label,
             include_overview=include_overview,
             include_confidential=include_confidential,
             workers=workers,
             chunk_size=chunk_size,
             encoding_format=encoding_format,
             encoding_quality=encoding_quality,
             jpeg_subsampling=jpeg_subsampling,
-            offset_table=offset_table
+            offset_table=offset_table,
+            label=label
         )
 
 
 def main():
-    parser = argparse.ArgumentParser(
-        description=("Convert combatible wsi file to DICOM")
-    )
-
-    parser.add_argument(
-        "-i", "--input", type=Path, required=True, help="Path to input wsi file."
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        type=Path,
-        help=(
-            "Path to output folder. Folder will be created and must not "
-            "excist. If not specified a folder named after the input file is "
-            "created in the same path."
-        ),
-    )
-    parser.add_argument(
-        "-t",
-        "--tile-size",
-        type=int,
-        default=512,
-        help=(
-            "Tile size (same for width and height). Required for ndpi and "
-            "openslide formats E.g. 512"
-        ),
-    )
-    parser.add_argument(
-        "-d",
-        "--dataset",
-        type=Path,
-        help=(
-            "Path to json DICOM dataset. Can be used to define additional "
-            "DICOM modules to include in the files"
-        ),
-    )
-    parser.add_argument(
-        "-l",
-        "--levels",
-        type=int,
-        nargs="+",
-        help=(
-            "Pyramid levels to include, if not all. E.g. 0 1 for base and "
-            "first pyramid layer. "
-        ),
-    )
-    parser.add_argument(
-        "--no-label", action="store_true", help="If not to include label"
-    )
-    parser.add_argument(
-        "--no-overview", action="store_true", help="If not to include overview"
-    )
-    parser.add_argument(
-        "--no-confidential",
-        action="store_true",
-        help="If not to include confidential metadata",
-    )
-    parser.add_argument(
-        "-w",
-        "--workers",
-        type=int,
-        default=os.cpu_count(),
-        help="Number of worker threads to use",
-    )
-    parser.add_argument(
-        "--chunk-size",
-        type=int,
-        default=100,
-        help="Number of tiles to give each worker at a time",
-    )
-    parser.add_argument(
-        "--format",
-        type=str,
-        default="jpeg",
-        help="Encoding format to use if re-encoding. 'jpeg' or 'jpeg2000'.",
-    )
-    parser.add_argument(
-        "--quality",
-        type=int,
-        default=90,
-        help=(
-            "Quality to use if re-encoding. Do not use > 95 for jpeg. "
-            "Use 100 for lossless jpeg2000."
-        ),
-    )
-    parser.add_argument(
-        "--subsampling",
-        type=str,
-        default="420",
-        help=(
-            "Subsampling option if using jpeg for re-encoding. Use '444' for "
-            "no subsampling, '422' for 2x1 subsampling, and '420' for 2x2 "
-            "subsampling."
-        ),
-    )
-    parser.add_argument(
-        "--offset-table",
-        type=str,
-        default="bot",
-        help=(
-            "Offset table to use, 'bot' basic offset table, 'eot' extended "
-            "offset table, 'None' - no offset table."
-        ),
-    )
-
-    args = parser.parse_args()
-    if not args.dataset:
-        dataset = None
-    else:
-        json_file = open(args.dataset)
-        dataset = Dataset.from_json(json.load(json_file))
-    if not args.levels:
-        levels = None
-    else:
-        levels = args.levels
-    offset_table: Optional[str] = args.offset_table
-    if offset_table == "None":
-        offset_table = None
-    WsiDicomizer.convert(
-        filepath=str(args.input),
-        output_path=str(args.output),
-        modules=dataset,
-        tile_size=args.tile_size,
-        include_levels=levels,
-        include_label=not args.no_label,
-        include_overview=not args.no_overview,
-        include_confidential=not args.no_confidential,
-        workers=args.workers,
-        chunk_size=args.chunk_size,
-        encoding_format=args.format,
-        encoding_quality=args.quality,
-        jpeg_subsampling=args.subsampling,
-        offset_table=offset_table,
-    )
+    cli = WsiDicomizerCli()
+    cli.cli()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `wsidicomizer-0.9.2/wsidicomizer/config.py` & `wsidicomizer-0.9.3/wsidicomizer/config.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/dataset.py` & `wsidicomizer-0.9.3/wsidicomizer/dataset.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/dicomizer_source.py` & `wsidicomizer-0.9.3/wsidicomizer/dicomizer_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/encoding.py` & `wsidicomizer-0.9.3/wsidicomizer/encoding.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/__init__.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_cli.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 """Cli for bioformats source."""
 
+from pathlib import Path
 from typing import Optional, Sequence
 
 from pydicom import Dataset
 
 from wsidicomizer.cli import WsiDicomizerCli
 from wsidicomizer.extras.bioformats.bioformats_dicomizer import \
     BioformatsDicomizer
@@ -33,28 +34,31 @@
         include_levels: Optional[Sequence[int]] = None,
         include_label: bool = True,
         include_overview: bool = True,
         include_confidential: bool = True,
         workers: Optional[int] = None,
         chunk_size: Optional[int] = None,
         encoding_format: str = 'jpeg',
-        encoding_quality: int = 90,
+        encoding_quality: float = 90,
         jpeg_subsampling: str = '420',
-        offset_table: Optional[str] = 'bot'
+        offset_table: Optional[str] = 'bot',
+        label: Optional[Path] = None
+
     ):
         with BioformatsDicomizer.open(
             filepath=filepath,
             modules=modules,
             tile_size=tile_size,
             include_levels=include_levels,
             include_label=include_label,
             include_overview=include_overview,
             encoding_format=encoding_format,
             encoding_quality=encoding_quality,
             jpeg_subsampling=jpeg_subsampling,
+            label=label
         ) as wsi:
             wsi.save(
                 output_path=output_path,
                 offset_table=offset_table,
                 workers=workers,
                 chunk_size=chunk_size
             )
```

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_dicomizer.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_dicomizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         modules: Optional[Union[Dataset, Sequence[Dataset]]] = None,
         tile_size: int = 512,
         include_levels: Optional[Sequence[int]] = None,
         include_label: bool = True,
         include_overview: bool = True,
         include_confidential: bool = True,
         encoding_format: str = 'jpeg',
-        encoding_quality: int = 90,
+        encoding_quality: float = 90,
         jpeg_subsampling: str = '420',
         label: Optional[Union[PILImage, str, Path]] = None
     ) -> WsiDicom:
         """Open data in file in filepath as WsiDicom.
 
         Parameters
         ----------
@@ -60,17 +60,17 @@
             Include label(s), default true.
         include_overwiew: bool = True
             Include overview(s), default true.
         include_confidential: bool = True
             Include confidential metadata.
         encoding_format: str = 'jpeg'
             Encoding format to use if re-encoding. 'jpeg' or 'jpeg2000'.
-        encoding_quality: int = 90
-            Quality to use if re-encoding. Do not use > 95 for jpeg. Use 100
-            for lossless jpeg2000.
+        encoding_quality: float = 90
+            Quality to use if re-encoding. It is recommended to not use > 95 for jpeg.
+            Use < 1 or > 1000 for lossless jpeg2000.
         jpeg_subsampling: str = '420'
             Subsampling option if using jpeg for re-encoding. Use '444' for
             no subsampling, '422' for 2x1 subsampling, and '420' for 2x2
             subsampling.
         label: Optional[Union[PILImage, str, Path]] = None
             Optional label image to use instead of label found in file.
```

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_image_data.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_reader.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_reader.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_source.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/bioformats/bioformats_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/__init__.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/openslide/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/openslide/openslide.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-#    Copyright 2021, 2022, 2023 SECTRA AB
-#
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-
-"""Importing openslide module after loading library if needed."""
-
-import os
-from ctypes.util import find_library
-from pathlib import Path
-
-# On windows, use find_library to find directory with openslide dll in
-# the Path environmental variable.
-if os.name == "nt":
-    openslide_lib_path = find_library("libopenslide-0")
-    if openslide_lib_path is not None:
-        openslide_dir = str(Path(openslide_lib_path).parent)
-    else:
-        openslide_lib_dir = os.environ.get("OPENSLIDE")
-        if openslide_lib_dir is not None:
-            openslide_lib_path = Path(openslide_lib_dir).joinpath("libopenslide-0.dll")
-            if not openslide_lib_path.exists():
-                openslide_lib_path = None
-    if openslide_lib_path is None:
-        raise ModuleNotFoundError(
-            "Could not find libopenslide-0.dll in the directories specified "
-            "in the `Path` or `OPENSLIDE` environmental variable. Please add "
-            "the directory with openslide bin content to the `Path` or  "
-            "OPENSLIDE environmental variable."
-        )
-    openslide_dir = str(Path(openslide_lib_path).parent)
-    os.add_dll_directory(openslide_dir)
-
-from openslide import (
-    PROPERTY_NAME_BACKGROUND_COLOR,
-    PROPERTY_NAME_BOUNDS_HEIGHT,
-    PROPERTY_NAME_BOUNDS_WIDTH,
-    PROPERTY_NAME_BOUNDS_X,
-    PROPERTY_NAME_BOUNDS_Y,
-    PROPERTY_NAME_MPP_X,
-    PROPERTY_NAME_MPP_Y,
-    PROPERTY_NAME_OBJECTIVE_POWER,
-    PROPERTY_NAME_VENDOR,
-    OpenSlide,
-)
-from openslide._convert import argb2rgba as convert_argb_to_rgba
-from openslide.lowlevel import _read_region, get_associated_image_names
+#    Copyright 2021, 2022, 2023 SECTRA AB
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
+"""Importing openslide module after loading library if needed."""
+
+import os
+from ctypes.util import find_library
+from pathlib import Path
+
+# On windows, use find_library to find directory with openslide dll in
+# the Path environmental variable.
+if os.name == "nt":
+    openslide_lib_path = find_library("libopenslide-0")
+    if openslide_lib_path is not None:
+        openslide_dir = str(Path(openslide_lib_path).parent)
+    else:
+        openslide_lib_dir = os.environ.get("OPENSLIDE")
+        if openslide_lib_dir is not None:
+            openslide_lib_path = Path(openslide_lib_dir).joinpath("libopenslide-0.dll")
+            if not openslide_lib_path.exists():
+                openslide_lib_path = None
+    if openslide_lib_path is None:
+        raise ModuleNotFoundError(
+            "Could not find libopenslide-0.dll in the directories specified "
+            "in the `Path` or `OPENSLIDE` environmental variable. Please add "
+            "the directory with openslide bin content to the `Path` or  "
+            "OPENSLIDE environmental variable."
+        )
+    openslide_dir = str(Path(openslide_lib_path).parent)
+    os.add_dll_directory(openslide_dir)
+
+from openslide import (
+    PROPERTY_NAME_BACKGROUND_COLOR,
+    PROPERTY_NAME_BOUNDS_HEIGHT,
+    PROPERTY_NAME_BOUNDS_WIDTH,
+    PROPERTY_NAME_BOUNDS_X,
+    PROPERTY_NAME_BOUNDS_Y,
+    PROPERTY_NAME_MPP_X,
+    PROPERTY_NAME_MPP_Y,
+    PROPERTY_NAME_OBJECTIVE_POWER,
+    PROPERTY_NAME_VENDOR,
+    OpenSlide,
+)
+from openslide._convert import argb2rgba as convert_argb_to_rgba
+from openslide.lowlevel import _read_region, get_associated_image_names
```

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_image_data.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/openslide/openslide_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_metadata.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/openslide/openslide_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_source.py` & `wsidicomizer-0.9.3/wsidicomizer/extras/openslide/openslide_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/image_data.py` & `wsidicomizer-0.9.3/wsidicomizer/image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/__init__.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/czi/__init__.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/czi/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_image_data.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/czi/czi_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_metadata.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/czi/czi_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_source.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/czi/czi_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/opentile/__init__.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/opentile/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/opentile/opentile_image_data.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/opentile/opentile_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/opentile/opentile_source.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/opentile/opentile_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/__init__.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/tiffslide/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_image_data.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/tiffslide/tiffslide_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_metadata.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/tiffslide/tiffslide_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_source.py` & `wsidicomizer-0.9.3/wsidicomizer/sources/tiffslide/tiffslide_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.2/wsidicomizer/wsidicomizer.py` & `wsidicomizer-0.9.3/wsidicomizer/wsidicomizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         include_levels: Optional[Sequence[int]] = None,
         include_label: bool = True,
         include_overview: bool = True,
         include_confidential: bool = True,
         workers: Optional[int] = None,
         chunk_size: Optional[int] = None,
         encoding_format: str = "jpeg",
-        encoding_quality: int = 90,
+        encoding_quality: float = 90,
         jpeg_subsampling: str = "420",
         offset_table: Optional[str] = "bot",
         label: Optional[Union[PILImage, str, Path]] = None,
         preferred_source: Optional[Type[DicomizerSource]] = None,
         **source_args,
     ) -> List[str]:
         """Convert data in file to DICOM files in output path. Created
@@ -190,17 +190,17 @@
         workers: Optional[int] = None,
             Maximum number of thread workers to use.
         chunk_size: Optional[int] = None,
             Chunk size (number of tiles) to process at a time. Actual chunk
             size also depends on minimun_chunk_size from image_data.
         encoding_format: str = 'jpeg'
             Encoding format to use if re-encoding. 'jpeg' or 'jpeg2000'.
-        encoding_quality: int = 90
-            Quality to use if re-encoding. Do not use > 95 for jpeg. Use 100
-            for lossless jpeg2000.
+        encoding_quality: float = 90
+            Quality to use if re-encoding. It is recommended to not use > 95 for jpeg.
+            Use < 1 or > 1000 for lossless jpeg2000.
         jpeg_subsampling: str = '420'
             Subsampling option if using jpeg for re-encoding. Use '444' for
             no subsampling, '422' for 2x1 subsampling, and '420' for 2x2
             subsampling.
         offset_table: Optional[str] = 'bot'
             Offset table to use, 'bot' basic offset table, 'eot' extended
             offset table, None - no offset table.
```

### Comparing `wsidicomizer-0.9.2/PKG-INFO` & `wsidicomizer-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsidicomizer
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tool for reading WSI files from proprietary formats and optionally convert them to to DICOM
 Home-page: https://github.com/imi-bigpicture/wsidicomizer
 License: Apache-2.0
 Keywords: whole slide image,digital pathology,dicom,converter
 Author: Erik O Gabrielsson
 Author-email: erik.o.gabrielsson@sectra.com
 Requires-Python: >=3.8,<3.12
```

