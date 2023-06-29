# Comparing `tmp/pymsbuild-1.0.0a1.tar.gz` & `tmp/pymsbuild-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymsbuild-1.0.0a1.tar", last modified: Thu Jun  1 00:08:11 2023, max compression
+gzip compressed data, was "pymsbuild-1.0.0a2.tar", last modified: Thu Jun 29 23:57:20 2023, max compression
```

## Comparing `pymsbuild-1.0.0a1.tar` & `pymsbuild-1.0.0a2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-rw-rw-   0        0        0    19717 2023-06-01 00:07:40.031116 PKG-INFO
--rw-rw-rw-   0        0        0       71 2023-06-01 00:06:39.699320 pyproject.toml
--rw-rw-rw-   0        0        0     2222 2023-06-01 00:06:39.699320 _msbuild.py
--rw-rw-rw-   0        0        0      936 2023-06-01 00:06:39.699320 pymsbuild/cython.py
--rw-rw-rw-   0        0        0     1276 2023-06-01 00:06:39.699320 pymsbuild/dllpack.py
--rw-rw-rw-   0        0        0       74 2023-06-01 00:06:39.699320 pymsbuild/pyproject.toml.in
--rw-rw-rw-   0        0        0    21286 2023-06-01 00:06:39.699320 pymsbuild/_build.py
--rw-rw-rw-   0        0        0    11558 2023-06-01 00:06:39.699320 pymsbuild/_generate.py
--rw-rw-rw-   0        0        0     4892 2023-06-01 00:06:39.699320 pymsbuild/_init.py
--rw-rw-rw-   0        0        0     1505 2023-06-01 00:06:39.699320 pymsbuild/_load_sysconfig.py
--rw-rw-rw-   0        0        0      802 2023-06-01 00:06:39.699320 pymsbuild/_locate_dotnet.py
--rw-rw-rw-   0        0        0     1956 2023-06-01 00:06:39.699320 pymsbuild/_locate_vs.py
--rw-rw-rw-   0        0        0     2013 2023-06-01 00:06:39.699320 pymsbuild/_msbuild.py.in
--rw-rw-rw-   0        0        0     5417 2023-06-01 00:06:39.699320 pymsbuild/_tags.py
--rw-rw-rw-   0        0        0     8560 2023-06-01 00:06:39.699320 pymsbuild/_types.py
--rw-rw-rw-   0        0        0     5557 2023-06-01 00:06:39.699320 pymsbuild/_writer.py
--rw-rw-rw-   0        0        0     1225 2023-06-01 00:06:39.699320 pymsbuild/__init__.py
--rw-rw-rw-   0        0        0     4047 2023-06-01 00:06:39.699320 pymsbuild/__main__.py
--rw-rw-rw-   0        0        0      973 2023-06-01 00:06:39.699320 pymsbuild/targets/common.props
--rw-rw-rw-   0        0        0     4143 2023-06-01 00:06:39.699320 pymsbuild/targets/common.targets
--rw-rw-rw-   0        0        0      119 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-ARM.props
--rw-rw-rw-   0        0        0      690 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-ARM.targets
--rw-rw-rw-   0        0        0      119 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-ARM64.props
--rw-rw-rw-   0        0        0      690 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-ARM64.targets
--rw-rw-rw-   0        0        0      127 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-ARM.props
--rw-rw-rw-   0        0        0      127 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-ARM64.props
--rw-rw-rw-   0        0        0      120 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-POSIX_x64.props
--rw-rw-rw-   0        0        0      127 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-Win32.props
--rw-rw-rw-   0        0        0      127 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-x64.props
--rw-rw-rw-   0        0        0      367 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-POSIX_x64-GCC.props
--rw-rw-rw-   0        0        0      232 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-POSIX_x64.props
--rw-rw-rw-   0        0        0     3572 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-POSIX_x64.targets
--rw-rw-rw-   0        0        0      119 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-Win32.props
--rw-rw-rw-   0        0        0      690 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-Win32.targets
--rw-rw-rw-   0        0        0      119 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-x64.props
--rw-rw-rw-   0        0        0      690 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-x64.targets
--rw-rw-rw-   0        0        0     3921 2023-06-01 00:06:39.699320 pymsbuild/targets/cython.targets
--rw-rw-rw-   0        0        0     6430 2023-06-01 00:06:39.699320 pymsbuild/targets/dllpack-generate.py
--rw-rw-rw-   0        0        0    11010 2023-06-01 00:06:39.699320 pymsbuild/targets/dllpack.c
--rw-rw-rw-   0        0        0     1835 2023-06-01 00:06:39.699320 pymsbuild/targets/dllpack.targets
--rw-rw-rw-   0        0        0     2506 2023-06-01 00:06:39.699320 pymsbuild/targets/dllpack_main.py
--rw-rw-rw-   0        0        0      292 2023-06-01 00:06:39.699320 pymsbuild/targets/package.override.targets
--rw-rw-rw-   0        0        0       23 2023-06-01 00:06:39.699320 pymsbuild/targets/package.props
--rw-rw-rw-   0        0        0     5390 2023-06-01 00:06:39.699320 pymsbuild/targets/package.targets
--rw-rw-rw-   0        0        0      935 2023-06-01 00:06:39.699320 pymsbuild/targets/pyd.props
--rw-rw-rw-   0        0        0      917 2023-06-01 00:06:39.699320 pymsbuild/targets/pyd.targets
--rw-rw-rw-   0        0        0       23 2023-06-01 00:06:39.699320 pymsbuild/targets/sdist.targets
+-rw-rw-rw-   0        0        0    19717 2023-06-29 23:56:53.812623 PKG-INFO
+-rw-rw-rw-   0        0        0       71 2023-06-29 23:56:31.950560 pyproject.toml
+-rw-rw-rw-   0        0        0     2222 2023-06-29 23:56:31.950560 _msbuild.py
+-rw-rw-rw-   0        0        0      936 2023-06-29 23:56:31.950560 pymsbuild/cython.py
+-rw-rw-rw-   0        0        0     1276 2023-06-29 23:56:31.950560 pymsbuild/dllpack.py
+-rw-rw-rw-   0        0        0       74 2023-06-29 23:56:31.950560 pymsbuild/pyproject.toml.in
+-rw-rw-rw-   0        0        0    21304 2023-06-29 23:56:31.950560 pymsbuild/_build.py
+-rw-rw-rw-   0        0        0    11558 2023-06-29 23:56:31.950560 pymsbuild/_generate.py
+-rw-rw-rw-   0        0        0     4892 2023-06-29 23:56:31.950560 pymsbuild/_init.py
+-rw-rw-rw-   0        0        0     1505 2023-06-29 23:56:31.950560 pymsbuild/_load_sysconfig.py
+-rw-rw-rw-   0        0        0      802 2023-06-29 23:56:31.950560 pymsbuild/_locate_dotnet.py
+-rw-rw-rw-   0        0        0     1956 2023-06-29 23:56:31.950560 pymsbuild/_locate_vs.py
+-rw-rw-rw-   0        0        0     2013 2023-06-29 23:56:31.950560 pymsbuild/_msbuild.py.in
+-rw-rw-rw-   0        0        0     5417 2023-06-29 23:56:31.950560 pymsbuild/_tags.py
+-rw-rw-rw-   0        0        0     8560 2023-06-29 23:56:31.950560 pymsbuild/_types.py
+-rw-rw-rw-   0        0        0     5557 2023-06-29 23:56:31.950560 pymsbuild/_writer.py
+-rw-rw-rw-   0        0        0     1225 2023-06-29 23:56:31.950560 pymsbuild/__init__.py
+-rw-rw-rw-   0        0        0     4047 2023-06-29 23:56:31.950560 pymsbuild/__main__.py
+-rw-rw-rw-   0        0        0      973 2023-06-29 23:56:31.950560 pymsbuild/targets/common.props
+-rw-rw-rw-   0        0        0     4143 2023-06-29 23:56:31.950560 pymsbuild/targets/common.targets
+-rw-rw-rw-   0        0        0      119 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-ARM.props
+-rw-rw-rw-   0        0        0      690 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-ARM.targets
+-rw-rw-rw-   0        0        0      119 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-ARM64.props
+-rw-rw-rw-   0        0        0      690 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-ARM64.targets
+-rw-rw-rw-   0        0        0      127 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-default-ARM.props
+-rw-rw-rw-   0        0        0      127 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-default-ARM64.props
+-rw-rw-rw-   0        0        0      120 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-default-POSIX_x64.props
+-rw-rw-rw-   0        0        0      127 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-default-Win32.props
+-rw-rw-rw-   0        0        0      127 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-default-x64.props
+-rw-rw-rw-   0        0        0      367 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-POSIX_x64-GCC.props
+-rw-rw-rw-   0        0        0      232 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-POSIX_x64.props
+-rw-rw-rw-   0        0        0     3572 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-POSIX_x64.targets
+-rw-rw-rw-   0        0        0      119 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-Win32.props
+-rw-rw-rw-   0        0        0      690 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-Win32.targets
+-rw-rw-rw-   0        0        0      119 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-x64.props
+-rw-rw-rw-   0        0        0      690 2023-06-29 23:56:31.950560 pymsbuild/targets/cpp-x64.targets
+-rw-rw-rw-   0        0        0     3921 2023-06-29 23:56:31.950560 pymsbuild/targets/cython.targets
+-rw-rw-rw-   0        0        0     6430 2023-06-29 23:56:31.950560 pymsbuild/targets/dllpack-generate.py
+-rw-rw-rw-   0        0        0    11010 2023-06-29 23:56:31.950560 pymsbuild/targets/dllpack.c
+-rw-rw-rw-   0        0        0     1835 2023-06-29 23:56:31.950560 pymsbuild/targets/dllpack.targets
+-rw-rw-rw-   0        0        0     2506 2023-06-29 23:56:31.950560 pymsbuild/targets/dllpack_main.py
+-rw-rw-rw-   0        0        0      292 2023-06-29 23:56:31.950560 pymsbuild/targets/package.override.targets
+-rw-rw-rw-   0        0        0       23 2023-06-29 23:56:31.950560 pymsbuild/targets/package.props
+-rw-rw-rw-   0        0        0     5390 2023-06-29 23:56:31.950560 pymsbuild/targets/package.targets
+-rw-rw-rw-   0        0        0      935 2023-06-29 23:56:31.950560 pymsbuild/targets/pyd.props
+-rw-rw-rw-   0        0        0      917 2023-06-29 23:56:31.950560 pymsbuild/targets/pyd.targets
+-rw-rw-rw-   0        0        0       23 2023-06-29 23:56:31.950560 pymsbuild/targets/sdist.targets
```

### PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymsbuild
-Version: 1.0.0a1
+Version: 1.0.0a2
 Author: Steve Dower
 Author-email: steve.dower@python.org
 Home-page: https://github.com/zooba/pymsbuild
 Project-url: Bug Tracker, https://github.com/zooba/pymsbuild/issues
 Summary: The pymsbuild build backend.
 Description-Content-Type: text/markdown
 Keywords: build,pep-517,msbuild,packaging,cython
```

### pymsbuild/_build.py

```diff
@@ -387,15 +387,15 @@
 
         rel_files = _relative_to_layout(files, self.layout_dir)
         import gzip, tarfile
         with gzip.open(sdist, "w") as f_gz:
             with tarfile.TarFile.open(tar_name, "w", fileobj=f_gz, format=tarfile.PAX_FORMAT) as f:
                 self.log("Packing files into", sdist)
                 for n, rn in rel_files:
-                    if n == self.state_file:
+                    if n.match(str(self.state_file)):
                         continue
                     self.log("-", rn)
                     f.add(n, arcname=rn)
                 self.log()
         self.write("Wrote sdist to", sdist)
         return sdist.name
 
@@ -450,15 +450,15 @@
         record_files = []
         rel_files = _relative_to_layout(files, self.layout_dir)
 
         import zipfile
         with zipfile.ZipFile(wheel, "w", compression=zipfile.ZIP_DEFLATED) as f:
             self.log("Packing files into", wheel)
             for n, rn in rel_files:
-                if n == self.state_file:
+                if n.match(str(self.state_file)):
                     continue
                 self.log("-", rn)
                 record.append(_add_and_record(f, n, rn))
             for n in self.metadata_dir.glob("*.dist-info"):
                 if n.is_dir():
                     record_files.append(rf"{n.name}/RECORD")
                     record.append(rf"{n.name}/RECORD,,")
```

