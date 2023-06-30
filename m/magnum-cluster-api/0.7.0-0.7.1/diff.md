# Comparing `tmp/magnum_cluster_api-0.7.0.tar.gz` & `tmp/magnum_cluster_api-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.7.0.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.7.1.tar", max compression
```

## Comparing `magnum_cluster_api-0.7.0.tar` & `magnum_cluster_api-0.7.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    10142 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/LICENSE
--rw-r--r--   0        0        0     2795 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-06-29 14:27:28.403267 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-06-29 14:27:28.303258 magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0     1977 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     4019 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4714 2023-06-29 14:27:23.846611 magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     3278 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    14251 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     1219 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/exceptions.py
--rw-r--r--   0        0        0     2888 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3464 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4034 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3307 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     3377 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     3944 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
--rw-r--r--   0        0        0     1513 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     2988 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
--rw-r--r--   0        0        0      143 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
--rw-r--r--   0        0        0     3127 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
--rw-r--r--   0        0        0      170 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
--rw-r--r--   0        0        0     3530 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
--rw-r--r--   0        0        0     1423 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
--rw-r--r--   0        0        0     1526 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     5673 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    11719 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3616 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    85235 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/service.py
--rw-r--r--   0        0        0     3119 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/functional/conftest.py
--rw-r--r--   0        0        0      666 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/functional/test_clusters.py
--rw-r--r--   0        0        0      942 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/conftest.py
--rw-r--r--   0        0        0     3453 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_helm.py
--rw-r--r--   0        0        0     1731 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_image_utils.py
--rw-r--r--   0        0        0     2759 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_images.py
--rw-r--r--   0        0        0     5366 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_objects.py
--rw-r--r--   0        0        0     1717 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_resources.py
--rw-r--r--   0        0        0     1192 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_utils.py
--rw-r--r--   0        0        0    10474 2023-06-29 14:27:23.850612 magnum_cluster_api-0.7.0/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1220 2023-06-29 14:27:23.854614 magnum_cluster_api-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 magnum_cluster_api-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2795 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-06-30 18:33:35.622181 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-06-30 18:33:35.582180 magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0     1977 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     4019 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     4714 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     3278 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    14251 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     1219 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/exceptions.py
+-rw-r--r--   0        0        0     3494 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3464 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-06-30 18:33:31.994088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4034 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3307 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     3377 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     3944 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
+-rw-r--r--   0        0        0     1513 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     2988 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      143 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
+-rw-r--r--   0        0        0     3127 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
+-rw-r--r--   0        0        0      170 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
+-rw-r--r--   0        0        0     3530 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
+-rw-r--r--   0        0        0     1423 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
+-rw-r--r--   0        0        0     1526 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     5673 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    85235 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3119 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/functional/conftest.py
+-rw-r--r--   0        0        0      666 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/functional/test_clusters.py
+-rw-r--r--   0        0        0      942 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/conftest.py
+-rw-r--r--   0        0        0     4035 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_helm.py
+-rw-r--r--   0        0        0     1731 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_image_utils.py
+-rw-r--r--   0        0        0     2759 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_images.py
+-rw-r--r--   0        0        0     5366 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_objects.py
+-rw-r--r--   0        0        0     1717 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_resources.py
+-rw-r--r--   0        0        0     1192 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_utils.py
+-rw-r--r--   0        0        0    10474 2023-06-30 18:33:31.998088 magnum_cluster_api-0.7.1/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1220 2023-06-30 18:33:32.002088 magnum_cluster_api-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 magnum_cluster_api-0.7.1/PKG-INFO
```

### Comparing `magnum_cluster_api-0.7.0/LICENSE` & `magnum_cluster_api-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/README.md` & `magnum_cluster_api-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/cmd/image_loader.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/driver.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/exceptions.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/helm.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,36 +44,56 @@
 
 class GetValuesReleaseCommand(ReleaseCommand):
     COMMAND = ["get", "values"]
 
     def __call__(self):
         try:
             return super().__call__(
-                "--namespace",
-                self.namespace,
-                self.release_name,
                 "--output",
                 "yaml",
             )
         except processutils.ProcessExecutionError as e:
             if "release: not found" in e.stderr:
                 raise exceptions.HelmReleaseNotFound(self.release_name)
             else:
                 raise
 
 
+class GetStatusReleaseCommand(ReleaseCommand):
+    COMMAND = ["status"]
+
+    def __call__(self):
+        try:
+            return super().__call__()
+        except processutils.ProcessExecutionError as e:
+            if "release: not found" in e.stderr:
+                raise exceptions.HelmReleaseNotFound(self.release_name)
+            else:
+                raise
+
+
 class UpgradeReleaseCommand(ReleaseCommand):
     COMMAND = ["upgrade"]
 
     def __init__(self, namespace, release_name, chart_ref, values={}):
         super().__init__(namespace, release_name)
         self.chart_ref = chart_ref
         self.values = values
 
     def __call__(self):
+        try:
+            status = GetStatusReleaseCommand(
+                namespace=self.namespace,
+                release_name=self.release_name,
+            )()
+
+            if "STATUS: pending" in str(status.stdout):
+                return "Other task is in progress"
+        except exceptions.HelmReleaseNotFound:
+            pass
         return super().__call__(
             self.chart_ref,
             "--install",
             "--wait",
             "--values",
             "-",
             process_input=yaml.dump(self.values),
```

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/images.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml` & `magnum_cluster_api-0.7.1/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/proxy/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/proxy/structs.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.7.1/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/resources.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/service.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/functional/conftest.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/functional/test_clusters.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/functional/test_clusters.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/conftest.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_helm.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_helm.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,26 +30,40 @@
         namespace,
         release_name,
         chart_ref,
         values,
     )
     upgrade()
 
-    mock_execute.assert_called_once_with(
-        "helm",
-        "upgrade",
-        "--namespace",
-        namespace,
-        release_name,
-        chart_ref,
-        "--install",
-        "--wait",
-        "--values",
-        "-",
-        process_input=yaml.dump(values),
+    mock_execute.assert_has_calls(
+        [
+            mocker.call(
+                "helm",
+                "status",
+                "--namespace",
+                namespace,
+                release_name,
+            ),
+            #  Note(okozachenko1203): call().__str__() is converted to call() so used tuple here.
+            #                         mocker.call is unittest.mock._Call class alias, and _Call is a subclass of tuple.
+            (("().stdout.__str__", (), {})),
+            mocker.call(
+                "helm",
+                "upgrade",
+                "--namespace",
+                namespace,
+                release_name,
+                chart_ref,
+                "--install",
+                "--wait",
+                "--values",
+                "-",
+                process_input=yaml.dump(values),
+            ),
+        ]
     )
 
 
 def test_helm_delete(mocker):
     namespace = "test-namespace"
     release_name = "test-release"
```

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_image_utils.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_images.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_objects.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_resources.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/tests/unit/test_utils.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.7.1/magnum_cluster_api/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.0/pyproject.toml` & `magnum_cluster_api-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.7.0"
+version = "0.7.1"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `magnum_cluster_api-0.7.0/PKG-INFO` & `magnum_cluster_api-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.7.0
+Version: 0.7.1
 Summary: Cluster API driver for Magnum
 Author: Mohammed Naser
 Author-email: mnaser@vexxhost.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

