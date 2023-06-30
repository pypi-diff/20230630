# Comparing `tmp/slpkg-4.9.0b0.tar.gz` & `tmp/slpkg-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slpkg-4.9.0b0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "slpkg-4.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `slpkg-4.9.0b0.tar` & `slpkg-4.9.1.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     1076 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/LICENSE
--rw-r--r--   0        0        0     1863 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/README.md
--rw-r--r--   0        0        0      374 2023-06-23 06:49:52.324363 slpkg-4.9.0b0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-06-23 06:51:26.992355 slpkg-4.9.0b0/slpkg/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/binaries/__init__.py
--rw-r--r--   0        0        0     7698 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/binaries/install.py
--rw-r--r--   0        0        0     1439 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/binaries/queries.py
--rw-r--r--   0        0        0     1892 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/binaries/required.py
--rw-r--r--   0        0        0      916 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/blacklist.py
--rw-r--r--   0        0        0     6373 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/check_updates.py
--rw-r--r--   0        0        0     3637 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/checks.py
--rw-r--r--   0        0        0     1881 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/checksum.py
--rw-r--r--   0        0        0     4004 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/choose_packages.py
--rw-r--r--   0        0        0     3211 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/cleanings.py
--rw-r--r--   0        0        0     4755 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/configs.py
--rw-r--r--   0        0        0     3864 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/dependees.py
--rw-r--r--   0        0        0     1906 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/dialog_box.py
--rw-r--r--   0        0        0     4289 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/dialog_configs.py
--rw-r--r--   0        0        0     3491 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/download_only.py
--rw-r--r--   0        0        0     3507 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/downloader.py
--rw-r--r--   0        0        0      430 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/error_messages.py
--rw-r--r--   0        0        0     1609 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/find_installed.py
--rw-r--r--   0        0        0    65384 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/install_data.py
--rw-r--r--   0        0        0      514 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/logging_config.py
--rw-r--r--   0        0        0     1350 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/logging_deps.py
--rw-r--r--   0        0        0    29917 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/main.py
--rw-r--r--   0        0        0        0 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/models/__init__.py
--rw-r--r--   0        0        0     2655 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/models/models.py
--rw-r--r--   0        0        0     2058 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/multi_process.py
--rw-r--r--   0        0        0    13598 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/new_configs.py
--rw-r--r--   0        0        0     2624 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/progress_bar.py
--rw-r--r--   0        0        0     6716 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/remove_packages.py
--rw-r--r--   0        0        0     4367 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/repo_info.py
--rw-r--r--   0        0        0    31419 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/repositories.py
--rw-r--r--   0        0        0      887 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/rules.py
--rw-r--r--   0        0        0        0 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/sbos/__init__.py
--rw-r--r--   0        0        0     1151 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/sbos/dependencies.py
--rw-r--r--   0        0        0     1605 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/sbos/queries.py
--rw-r--r--   0        0        0     4480 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/sbos/sbo_generate.py
--rw-r--r--   0        0        0    11672 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/sbos/slackbuild.py
--rw-r--r--   0        0        0     3428 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/search.py
--rw-r--r--   0        0        0      587 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/toml_error_message.py
--rw-r--r--   0        0        0     4132 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/tracking.py
--rw-r--r--   0        0        0    36699 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/update_repository.py
--rw-r--r--   0        0        0     4041 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/upgrade.py
--rw-r--r--   0        0        0     7854 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/utilities.py
--rw-r--r--   0        0        0        0 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/views/__init__.py
--rw-r--r--   0        0        0     5935 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/views/asciibox.py
--rw-r--r--   0        0        0     6335 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/views/cli_menu.py
--rw-r--r--   0        0        0     4110 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/views/help_commands.py
--rw-r--r--   0        0        0      632 2023-06-23 06:52:44.488348 slpkg-4.9.0b0/slpkg/views/version.py
--rw-r--r--   0        0        0     6580 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/views/view_package.py
--rw-r--r--   0        0        0    10262 2023-06-23 05:30:07.000000 slpkg-4.9.0b0/slpkg/views/views.py
--rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 slpkg-4.9.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1945 2023-06-30 07:00:04.000000 slpkg-4.9.1/README.md
+-rw-r--r--   0        0        0     1475 2023-06-30 07:00:04.000000 slpkg-4.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/binaries/__init__.py
+-rw-r--r--   0        0        0     7698 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/binaries/install.py
+-rw-r--r--   0        0        0     1439 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/binaries/queries.py
+-rw-r--r--   0        0        0     1892 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/binaries/required.py
+-rw-r--r--   0        0        0      916 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/blacklist.py
+-rw-r--r--   0        0        0     6378 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/check_updates.py
+-rw-r--r--   0        0        0     3637 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/checks.py
+-rw-r--r--   0        0        0     1881 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/checksum.py
+-rw-r--r--   0        0        0     4004 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/choose_packages.py
+-rw-r--r--   0        0        0     4102 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/cleanings.py
+-rw-r--r--   0        0        0     4913 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/configs.py
+-rw-r--r--   0        0        0     3864 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/dependees.py
+-rw-r--r--   0        0        0     1906 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/dialog_box.py
+-rw-r--r--   0        0        0     4362 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/dialog_configs.py
+-rw-r--r--   0        0        0     3491 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/download_only.py
+-rw-r--r--   0        0        0     3507 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/downloader.py
+-rw-r--r--   0        0        0      430 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/error_messages.py
+-rw-r--r--   0        0        0     1609 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/find_installed.py
+-rw-r--r--   0        0        0    65384 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/install_data.py
+-rw-r--r--   0        0        0      522 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/logging_config.py
+-rw-r--r--   0        0        0     1350 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/logging_deps.py
+-rw-r--r--   0        0        0    29917 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/main.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/models/__init__.py
+-rw-r--r--   0        0        0     2655 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/models/models.py
+-rw-r--r--   0        0        0     2078 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/multi_process.py
+-rw-r--r--   0        0        0    13598 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/new_configs.py
+-rw-r--r--   0        0        0     2630 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/progress_bar.py
+-rw-r--r--   0        0        0     6716 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/remove_packages.py
+-rw-r--r--   0        0        0     4367 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/repo_info.py
+-rw-r--r--   0        0        0    31419 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/repositories.py
+-rw-r--r--   0        0        0      887 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/rules.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/sbos/__init__.py
+-rw-r--r--   0        0        0     1151 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/sbos/dependencies.py
+-rw-r--r--   0        0        0     1605 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/sbos/queries.py
+-rw-r--r--   0        0        0     4480 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0        0        0    11672 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/sbos/slackbuild.py
+-rw-r--r--   0        0        0     3428 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/search.py
+-rw-r--r--   0        0        0      587 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/toml_error_message.py
+-rw-r--r--   0        0        0     4132 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/tracking.py
+-rw-r--r--   0        0        0    36699 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/update_repository.py
+-rw-r--r--   0        0        0     4041 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/upgrade.py
+-rw-r--r--   0        0        0     8822 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/utilities.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/views/__init__.py
+-rw-r--r--   0        0        0     5935 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/views/asciibox.py
+-rw-r--r--   0        0        0     6327 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/views/cli_menu.py
+-rw-r--r--   0        0        0     4110 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/views/help_commands.py
+-rw-r--r--   0        0        0      629 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/views/version.py
+-rw-r--r--   0        0        0     6580 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/views/view_package.py
+-rw-r--r--   0        0        0    10262 2023-06-30 07:00:04.000000 slpkg-4.9.1/slpkg/views/views.py
+-rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 slpkg-4.9.1/PKG-INFO
```

### Comparing `slpkg-4.9.0b0/README.md` & `slpkg-4.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 Slpkg is a software package manager that installs, updates and removes packages on <a href="https://www.slackware.com" target="_blank">Slackware</a>-based systems.
 It automatically calculates dependencies and figures out what things need to happen to install packages.
 Slpkg makes it easier to manage groups of machines without the need for manual updates.
 Slpkg works in accordance with the standards of the <a href="https://www.slackbuilds.org" target="_blank">slackbuilds.org</a> organization to build packages.
 It also uses the Slackware Linux instructions for installing, upgrading or removing packages.
 
+## Homepage
+
+Visit the project website [here](https://dslackw.gitlab.io/slpkg/).
+
 ## Source
 
 * <a href="https://gitlab.com/dslackw/slpkg" target="_blank">GitLab</a> repository.
 * <a href="https://slackbuilds.org/repository/15.0/system/slpkg/" target="_blank">SlackBuilds.org</a> repository.
 * <a href="https://sourceforge.net/projects/slpkg/" target="_blank">SourceForge</a> repository.
 * <a href="https://pypi.org/project/slpkg/" target="_blank">PyPi</a> repository.
```

#### html2text {}

```diff
@@ -2,14 +2,16 @@
 dslackw.gitlab.io/slpkg) ## About Slpkg is a software package manager that
 installs, updates and removes packages on Slackware-based systems. It
 automatically calculates dependencies and figures out what things need to
 happen to install packages. Slpkg makes it easier to manage groups of machines
 without the need for manual updates. Slpkg works in accordance with the
 standards of the slackbuilds.org organization to build packages. It also uses
 the Slackware Linux instructions for installing, upgrading or removing
-packages. ## Source * GitLab repository. * SlackBuilds.org repository. *
-SourceForge repository. * PyPi repository. ## License [MIT License](https://
-dslackw.gitlab.io/slpkg/license/) ## Donate Did you know that we developers
-love coffee? [[paypal]](https://www.paypal.me/dslackw) ## Support Please
-support: * Slackware project. * SlackBuilds project. * AlienBob project. Thank
-you all for your support! ## Copyrights SlackwareÂ® is a Registered Trademark
-of Patrick Volkerding. Linux is a Registered Trademark of Linus Torvalds.
+packages. ## Homepage Visit the project website [here](https://
+dslackw.gitlab.io/slpkg/). ## Source * GitLab repository. * SlackBuilds.org
+repository. * SourceForge repository. * PyPi repository. ## License [MIT
+License](https://dslackw.gitlab.io/slpkg/license/) ## Donate Did you know that
+we developers love coffee? [[paypal]](https://www.paypal.me/dslackw) ## Support
+Please support: * Slackware project. * SlackBuilds project. * AlienBob project.
+Thank you all for your support! ## Copyrights SlackwareÂ® is a Registered
+Trademark of Patrick Volkerding. Linux is a Registered Trademark of Linus
+Torvalds.
```

### Comparing `slpkg-4.9.0b0/slpkg/binaries/install.py` & `slpkg-4.9.1/slpkg/binaries/install.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/binaries/queries.py` & `slpkg-4.9.1/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/binaries/required.py` & `slpkg-4.9.1/slpkg/binaries/required.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/blacklist.py` & `slpkg-4.9.1/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/check_updates.py` & `slpkg-4.9.1/slpkg/check_updates.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,26 @@
         if self.option_for_repository:
             self.check_updates_for_repository()
         else:
             self.check_updates_for_repositories()
 
         return self.compare
 
-    def check_updates_for_repository(self):
+    def check_updates_for_repository(self) -> None:
         sbo_repository: dict = {
             self.repos.sbo_repo_name: self.sbo_repository,
             self.repos.ponce_repo_name: self.ponce_repository
         }
 
         if self.is_binary:
             self.binary_repository(self.repository)
         else:
             sbo_repository[self.repository]()
 
-    def check_updates_for_repositories(self):
+    def check_updates_for_repositories(self) -> None:
         if self.repos.sbo_repo:
             self.sbo_repository()
 
         if self.repos.ponce_repo:
             self.ponce_repository()
 
         for repo in list(self.repos.repositories.keys())[2:]:
@@ -87,15 +87,14 @@
     def ponce_repository(self) -> None:
         local_chg_txt: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
         repo_chg_txt: str = f'{self.repos.ponce_repo_mirror[0]}{self.repos.ponce_repo_changelog}'
         self.compare[self.repos.ponce_repo_name] = self.compare_the_changelogs(local_chg_txt, repo_chg_txt)
 
     def compare_the_changelogs(self, local_chg_txt: Path, repo_chg_txt: str) -> bool:
         local_size: int = 0
-        repo_size: int = 0
 
         if self.proxy_address.startswith('http'):
             self.set_http_proxy_server()
 
         if self.proxy_address.startswith('socks'):
             self.set_socks_proxy_server()
 
@@ -118,18 +117,18 @@
                     f'{self.__class__.compare_the_changelogs.__name__}: '
                     f'{local_chg_txt=}, {local_size=}, '
                     f'{repo_chg_txt=}, {repo_size=}, '
                     f'{local_size != repo_size}')
 
         return local_size != repo_size
 
-    def set_http_proxy_server(self):
+    def set_http_proxy_server(self) -> None:
         self.http = ProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
 
-    def set_socks_proxy_server(self):
+    def set_socks_proxy_server(self) -> None:
         try:  # Try to import PySocks if it's installed.
             from urllib3.contrib.socks import SOCKSProxyManager
         except (ModuleNotFoundError, ImportError) as error:
             print(error)
         # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
         self.http = SOCKSProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
```

### Comparing `slpkg-4.9.0b0/slpkg/checks.py` & `slpkg-4.9.1/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/checksum.py` & `slpkg-4.9.1/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/choose_packages.py` & `slpkg-4.9.1/slpkg/choose_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/cleanings.py` & `slpkg-4.9.1/slpkg/cleanings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import shutil
-from pathlib import PosixPath
+from pathlib import Path, PosixPath
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.views.views import ViewMessage
 from slpkg.repositories import Repositories
 from slpkg.models.models import session as Session
 from slpkg.models.models import (Base, engine, LogsDependencies,
@@ -39,27 +39,51 @@
         self.utils.remove_folder_if_exists(self.tmp_slpkg)
         self.utils.create_directory(self.build_path)
         print(f'{self.byellow}Successfully cleared!{self.endc}\n')
 
     def logs_dependencies(self) -> None:
         """ Deletes the log table from the database. """
         dependencies: list = self.session.query(
-            LogsDependencies.name, LogsDependencies.requires).all()  # type: ignore
+            LogsDependencies.name, LogsDependencies.requires).all()
 
         if dependencies:
             self.view.logs_dependencies(dependencies)
-            self.view.question()
-            self.delete_logs_of_dependencies()
+            try:
+                answer: str = input(f'\nDo you want to continue? [y/N] ')
+            except KeyboardInterrupt:
+                raise SystemExit(1)
+            if answer in ['Y', 'y']:
+                self.delete_logs_of_dependencies()
         else:
             print('\nNothing to clean.\n')
 
-    def delete_logs_of_dependencies(self):
+        if any(Path(self.slpkg_log_path).iterdir()):
+            self.delete_process_logs()
+
+    def delete_logs_of_dependencies(self) -> None:
         self.session.query(LogsDependencies).delete()
         self.session.commit()
 
+    def delete_process_logs(self) -> None:
+        """ Deletes of build log files. """
+        print('\n\nThe following log files will be deleted:\n')
+
+        for file in self.slpkg_log_path.glob('*'):
+            print(f"  {self.bred}>{self.endc} '{file}'")
+
+        print(f"\n{self.prog_name}: {self.blink}{self.bold}{self.bred}WARNING!{self.endc}: All the files "
+              f"will delete!")
+
+        self.view.question()
+
+        for file in self.slpkg_log_path.glob('*'):
+            self.utils.remove_file_if_exists(self.slpkg_log_path, str(file))
+
+        print(f'{self.byellow}Successfully cleared!{self.endc}\n')
+
     def db_tables(self) -> None:
         """ Drop all the tables from the database. """
         print('Deleting repositories of local data and the database:\n')
         for item in self.repos.repositories.values():
             if item['path'].exists() and isinstance(item['path'], PosixPath):
                 print(f"  {self.bred}>{self.endc} '{item['path']}'")
```

### Comparing `slpkg-4.9.0b0/slpkg/configs.py` & `slpkg-4.9.1/slpkg/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     tmp_slpkg: Path = Path(tmp_path, prog_name)
     build_path: Path = Path(tmp_path, prog_name, 'build')
     download_only_path: Path = Path(tmp_slpkg, '')
     lib_path: Path = Path('/var/lib', prog_name)
     etc_path: Path = Path('/etc', prog_name)
     db_path: Path = Path(lib_path, 'database')
     log_packages: Path = Path('/var', 'log', 'packages')
+    slpkg_log_path: Path = Path('/var/log/slpkg/')
 
     database_name: str = f'database.{prog_name}'
     file_list_suffix: str = '.pkgs'
     installpkg: str = 'upgradepkg --install-new'
     reinstall: str = 'upgradepkg --reinstall'
     removepkg: str = 'removepkg'
     colors: bool = True
@@ -44,14 +45,15 @@
     parallel_downloads: bool = False
     file_pattern: str = '*'
     spinning_bar: str = True
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
     border_color: str = 'bgreen'
     case_sensitive: bool = True
+    process_log: bool = True
 
     proxy_address: str = ''
     proxy_username: str = ''
     proxy_password: str = ''
 
     try:
         # Load user configuration.
@@ -82,14 +84,15 @@
             parallel_downloads: bool = config['PARALLEL_DOWNLOADS']
             file_pattern_conf: str = config['FILE_PATTERN']
             spinning_bar: str = config['SPINNING_BAR']
             progress_spinner: str = config['PROGRESS_SPINNER']
             spinner_color: str = config['SPINNER_COLOR']
             border_color: str = config['BORDER_COLOR']
             case_sensitive: bool = config['CASE_SENSITIVE']
+            process_log: bool = config['PROCESS_LOG']
             proxy_address: str = config['PROXY_ADDRESS']
             proxy_username: str = config['PROXY_USERNAME']
             proxy_password: str = config['PROXY_PASSWORD']
 
     except (KeyError, tomli.TOMLDecodeError) as error:
         errors.raise_toml_error_message(error, toml_file='/etc/slpkg/slpkg.toml')
 
@@ -129,14 +132,15 @@
     # Creating the paths if not exists
     paths = [
         db_path,
         lib_path,
         etc_path,
         build_path,
         tmp_slpkg,
+        slpkg_log_path,
         download_only_path,
         LoggingConfig.log_path
     ]
 
     for path in paths:
         if not path.is_dir():
             path.mkdir(parents=True, exist_ok=True)
```

### Comparing `slpkg-4.9.0b0/slpkg/dependees.py` & `slpkg-4.9.1/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/dialog_box.py` & `slpkg-4.9.1/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/dialog_configs.py` & `slpkg-4.9.1/slpkg/dialog_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
             'COLORS',
             'DIALOG',
             'SILENT_MODE',
             'ASCII_CHARACTERS',
             'ASK_QUESTION',
             'PARALLEL_DOWNLOADS',
             'SPINNING_BAR',
-            'CASE_INSENSITIVE'
+            'CASE_INSENSITIVE',
+            'PROCESS_LOG'
         ]
         values: list = ['true', 'false']
 
         for key, value in zip(self.configs['CONFIGS'].keys(), tags):
 
             if key in keys and value not in values:
                 self.dialogbox.msgbox(f"\nError: Value for '{key}', it must be 'true' or 'false.'\n",
@@ -116,12 +117,13 @@
                             ('COLORS =',
                              'DIALOG =',
                              'SILENT_MODE =',
                              'ASCII_CHARACTERS =',
                              'ASK_QUESTION =',
                              'PARALLEL_DOWNLOADS =',
                              'SPINNING_BAR =',
-                             'CASE_SENSITIVE =')
+                             'CASE_SENSITIVE =',
+                             'PROCESS_LOG =')
                     ):
                         line: str = line.replace('"', '')
 
                 patch_toml.write(line)
```

### Comparing `slpkg-4.9.0b0/slpkg/download_only.py` & `slpkg-4.9.1/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/downloader.py` & `slpkg-4.9.1/slpkg/downloader.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/find_installed.py` & `slpkg-4.9.1/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/install_data.py` & `slpkg-4.9.1/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/logging_config.py` & `slpkg-4.9.1/slpkg/logging_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 
 
 class LoggingConfig:
     date_now = datetime.now()
     level = logging.INFO
     filemode: str = 'w'
     encoding: str = 'utf-8'
-    log_path: Path = Path('/tmp/slpkg/logs')
-    log_file: Path = Path(log_path, 'slpkg.log')
+    log_path: Path = Path('/var/log/slpkg/')
+    log_file: Path = Path(log_path, 'slpkg_runtime.log')
     date: str = f'{date_now.day}/{date_now.month}/{date_now.year}'
     time: str = f'{date_now.hour}:{date_now.minute}:{date_now.second}'
     date_time: str = f'{date} {time}'
```

### Comparing `slpkg-4.9.0b0/slpkg/logging_deps.py` & `slpkg-4.9.1/slpkg/logging_deps.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/main.py` & `slpkg-4.9.1/slpkg/main.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/models/models.py` & `slpkg-4.9.1/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/multi_process.py` & `slpkg-4.9.1/slpkg/multi_process.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 
         self.option_for_no_silent: bool = self.utils.is_option(
             ('-n', '--no-silent'), flags)
 
     def process(self, command: str, filename: str, progress_message: str) -> None:
         """ Starting multiprocessing install/upgrade process. """
         if self.silent_mode and not self.option_for_no_silent:
-            done: str = f'{self.yellow}{self.ascii.done}{self.endc}'
-            failed: str = f'{self.red}{self.ascii.failed}{self.endc}'
             self.stderr = subprocess.DEVNULL
             self.stdout = subprocess.DEVNULL
+            done: str = f'{self.yellow}{self.ascii.done}{self.endc}'
+            failed: str = f'{self.red}{self.ascii.failed}{self.endc}'
 
             # Starting multiprocessing
-            process_1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
+            process_1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout, filename))
             process_2 = Process(target=self.progress.progress_bar, args=(progress_message, filename))
 
             process_1.start()
             process_2.start()
 
             # Wait until process 1 finish
             process_1.join()
@@ -50,8 +50,8 @@
                     print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} {filename} {failed}{' ' * 17}", end='\r')
                 else:
                     print(f"\r{'':>2}{self.bgreen}{self.ascii.bullet}{self.endc} {filename} {done}{' ' * 17}", end='\r')
 
             # Restore the terminal cursor
             print('\x1b[?25h', self.endc)
         else:
-            self.utils.process(command, self.stderr, self.stdout)
+            self.utils.process(command, self.stderr, self.stdout, filename)
```

### Comparing `slpkg-4.9.0b0/slpkg/new_configs.py` & `slpkg-4.9.1/slpkg/new_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/progress_bar.py` & `slpkg-4.9.1/slpkg/progress_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             try:
                 while True:
                     time.sleep(0.1)
                     bar_spinner.next()
             except KeyboardInterrupt:
                 raise SystemExit(1)
         else:
-            print(f"{'':>2}{self.red}{self.ascii.bullet}{self.endc} {filename}: "
+            print(f"{'':>2}{self.yellow}{self.ascii.bullet}{self.endc} {filename}: "
                   f"{message}... {self.color}", end='')
 
     def assign_spinners(self) -> None:
         self.spinners: dict[str] = {
             'pixel': PixelSpinner,
             'line': LineSpinner,
             'moon': MoonSpinner,
@@ -62,15 +62,15 @@
             'red': self.red,
             'white': self.endc
         }
 
     def set_the_spinner_message(self, filename: str, message: str) -> None:
         self.bar_message: str = f"{self.endc}{message} "
         if filename:
-            self.bar_message: str = (f"{'':>2}{self.red}{self.ascii.bullet}{self.endc} {filename}: "
+            self.bar_message: str = (f"{'':>2}{self.yellow}{self.ascii.bullet}{self.endc} {filename}: "
                                      f"{message}... ")
 
     def set_spinner(self) -> None:
         try:
             self.spinner: str = self.spinners[self.progress_spinner]
         except KeyError:
             self.spinner = PixelSpinner
```

### Comparing `slpkg-4.9.0b0/slpkg/remove_packages.py` & `slpkg-4.9.1/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/repo_info.py` & `slpkg-4.9.1/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/repositories.py` & `slpkg-4.9.1/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/rules.py` & `slpkg-4.9.1/slpkg/rules.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/sbos/dependencies.py` & `slpkg-4.9.1/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/sbos/queries.py` & `slpkg-4.9.1/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/sbos/sbo_generate.py` & `slpkg-4.9.1/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/sbos/slackbuild.py` & `slpkg-4.9.1/slpkg/sbos/slackbuild.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/search.py` & `slpkg-4.9.1/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/toml_error_message.py` & `slpkg-4.9.1/slpkg/toml_error_message.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/tracking.py` & `slpkg-4.9.1/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/update_repository.py` & `slpkg-4.9.1/slpkg/update_repository.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/upgrade.py` & `slpkg-4.9.1/slpkg/upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/utilities.py` & `slpkg-4.9.1/slpkg/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,35 @@
 import logging
 import subprocess
 from pathlib import Path
 from typing import Generator
 
 from slpkg.configs import Configs
 from slpkg.blacklist import Blacklist
+from slpkg.views.version import Version
 from slpkg.error_messages import Errors
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
 
 
 class Utilities(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
 
         self.black = Blacklist()
         self.errors = Errors()
         self.repos = Repositories()
+        self.stderr = None
+        self.stdout = None
+        self.prog_version = Version()
 
         self.installed_packages: dict[str] = dict(self.all_installed())
+        self.process_log_date = LoggingConfig.date.replace('/', '_')
+        self.process_log_time = LoggingConfig.time.replace(':', '_')
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
     def is_package_installed(self, name: str) -> str:
@@ -121,45 +127,62 @@
             for package in packages:
                 if package and not package.startswith('#'):
                     if '#' in package:
                         package = package.split('#')[0].strip()
                     yield package
         except FileNotFoundError:
             logger = logging.getLogger(LoggingConfig.date_time)
-            logger.exception(f'{self.__class__.__name__}: '
-                             f'{self.__class__.read_packages_from_file.__name__}')
+            logger.exception(
+                f'{self.__class__.__name__}: '
+                f'{self.__class__.read_packages_from_file.__name__}'
+            )
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
     def read_text_file(self, file: Path) -> list:
         """ Reads the text file. """
         try:
             with open(file, 'r', encoding='utf-8', errors='replace') as text_file:
                 return text_file.readlines()
         except FileNotFoundError:
             logger = logging.getLogger(LoggingConfig.date_time)
-            logger.exception(f'{self.__class__.__name__}: '
-                             f'{self.__class__.read_text_file.__name__}')
+            logger.exception(
+                f'{self.__class__.__name__}: '
+                f'{self.__class__.read_text_file.__name__}'
+            )
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
-    def process(self, command: str, stderr=None, stdout=None) -> None:
+    def process(self, command: str, stderr=None, stdout=None, filename=None) -> None:
         """ Handle the processes. """
-        output: int = 0
+        output = tee = ''
+        if filename and self.process_log:
+            self.header_process_log(filename)
+            tee: str = (
+                f' | tee -a {self.slpkg_log_path}/{filename}_'
+                f'{self.process_log_date}_{self.process_log_time}.log'
+            )
         try:
-            output: int = subprocess.call(command, shell=True, stderr=stderr, stdout=stdout)
+            output = subprocess.run(f'{command}{tee}', shell=True, stderr=stderr, stdout=stdout)
         except subprocess.CalledProcessError as error:
             logger = logging.getLogger(LoggingConfig.date_time)
-            logger.exception(f'{self.__class__.__name__}'
-                             f'{self.__class__.process.__name__}')
+            logger.exception(
+                f'{self.__class__.__name__}'
+                f'{self.__class__.process.__name__}'
+            )
             self.errors.raise_error_message(str(error), exit_status=20)
         except KeyboardInterrupt:
             raise SystemExit(1)
 
-        if output != 0:
+        if output.returncode != 0:
             raise SystemExit(1)
 
+    def header_process_log(self, filename: str) -> None:
+        """ Creates the build log file and the header. """
+        with open(f'{self.slpkg_log_path}/{filename}_{self.process_log_date}_{self.process_log_time}.log', 'w') as f:
+            f.write(f'{LoggingConfig.date_time}: {filename}: Version: {self.prog_name} {self.prog_version.version}\n')
+
     def get_file_size(self, file: Path) -> str:
         """ Get the local file size and converted to units. """
         size: int = file.stat().st_size
         return self.convert_file_sizes(size)
 
     @staticmethod
     def convert_file_sizes(size: int) -> str:
@@ -189,15 +212,15 @@
     def is_binary_repo(self, repo: str) -> bool:
         """ Checks if the repository is binary. """
         if repo in tuple(self.repos.repositories.keys())[2:]:
             return True
 
     @staticmethod
     def change_owner_privileges(folder: Path) -> None:
-        """ Changes thw owner privileges. """
+        """ Changes the owner privileges. """
         os.chown(folder, 0, 0)
         for file in os.listdir(folder):
             os.chown(Path(folder, file), 0, 0)
 
     @staticmethod
     def case_insensitive_pattern_matching(packages: list, data: dict) -> list:
         """ Case-insensitive pattern matching packages. """
```

### Comparing `slpkg-4.9.0b0/slpkg/views/asciibox.py` & `slpkg-4.9.1/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/views/cli_menu.py` & `slpkg-4.9.1/slpkg/views/cli_menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             f'\n{self.bold}DESCRIPTION:{self.endc}\n  Package manager utility for Slackware.\n'
             f'\n{self.bold}COMMANDS:{self.endc}\n'
             f'  {self.red}-u, update{self.endc}                    Update the package lists.\n'
             f'  {self.cyan}-U, upgrade{self.endc}                   Upgrade all the packages.\n'
             f'  {self.cyan}-c, check-updates{self.endc}             Check for news on ChangeLog.txt.\n'
             f'  {self.cyan}-I, repo-info{self.endc}                 Prints the repositories information.\n'
             f'  {self.cyan}-g, configs{self.endc}                   Edit the configuration file.\n'
-            f'  {self.cyan}-L, clean-logs{self.endc}                Clean dependencies log tracking.\n'
+            f'  {self.cyan}-L, clean-logs{self.endc}                Clean all logging files.\n'
             f'  {self.cyan}-T, clean-data{self.endc}                Clean all the repositories data.\n'
             f'  {self.cyan}-D, clean-tmp{self.endc}                 Delete all the downloaded sources.\n'
             f'  {self.cyan}-b, build{self.endc} [PACKAGES...]       Build only the packages.\n'
             f'  {self.cyan}-i, install{self.endc} [PACKAGES...]     Build and install the packages.\n'
             f'  {self.cyan}-R, remove{self.endc} [PACKAGES...]      Remove installed packages.\n'
             f'  {self.cyan}-d, download{self.endc} [PACKAGES...]    Download only the scripts and sources.\n'
             f'  {self.cyan}-f, find{self.endc} [PACKAGES...]        Find installed packages.\n'
```

### Comparing `slpkg-4.9.0b0/slpkg/views/help_commands.py` & `slpkg-4.9.1/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/views/version.py` & `slpkg-4.9.1/slpkg/views/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 9, '0b')
+        self.version_info: tuple = (4, 9, 1)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.9.0b0/slpkg/views/view_package.py` & `slpkg-4.9.1/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.9.0b0/slpkg/views/views.py` & `slpkg-4.9.1/slpkg/views/views.py`

 * *Files identical despite different names*

