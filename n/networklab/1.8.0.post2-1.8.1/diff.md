# Comparing `tmp/networklab-1.8.0.post2.tar.gz` & `tmp/networklab-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.8.0.post2.tar", last modified: Sat Mar 16 08:14:05 2024, max compression
+gzip compressed data, was "networklab-1.8.1.tar", last modified: Mon Apr  8 09:30:57 2024, max compression
```

## Comparing `networklab-1.8.0.post2.tar` & `networklab-1.8.1.tar`

### file list

```diff
@@ -1,736 +1,741 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.906695 networklab-1.8.0.post2/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-03-16 08:14:05.906695 networklab-1.8.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netlab
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.786695 networklab-1.8.0.post2/netsim/
--rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.786695 networklab-1.8.0.post2/netsim/ansible/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)      757 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)     2236 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/create-config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)     2772 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/initial-config.ansible
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/reload-config.ansible
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.790695 networklab-1.8.0.post2/netsim/ansible/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/create-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/create-custom-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.794695 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.794695 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.798695 networklab-1.8.0.post2/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.798695 networklab-1.8.0.post2/netsim/ansible/tasks/frr/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/frr/mpls-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/initial-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.798695 networklab-1.8.0.post2/netsim/ansible/tasks/iosxr/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/iosxr/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.798695 networklab-1.8.0.post2/netsim/ansible/tasks/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/linux/dhcp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.798695 networklab-1.8.0.post2/netsim/ansible/tasks/nxos/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.798695 networklab-1.8.0.post2/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/readiness-check/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/readiness-check/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/readiness-check/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/readiness-check/vsrx.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.798695 networklab-1.8.0.post2/netsim/ansible/tasks/vmx/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/vmx/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/tasks/wait-for-ready.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.798695 networklab-1.8.0.post2/netsim/ansible/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.802695 networklab-1.8.0.post2/netsim/ansible/templates/bfd/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.806695 networklab-1.8.0.post2/netsim/ansible/templates/bgp/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/frr.bgp-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.806695 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/dnsmasq.j2
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/eos.server.j2
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/ios.server.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/dhcp/linux.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.810695 networklab-1.8.0.post2/netsim/ansible/templates/eigrp/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.810695 networklab-1.8.0.post2/netsim/ansible/templates/evpn/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.810695 networklab-1.8.0.post2/netsim/ansible/templates/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.818695 networklab-1.8.0.post2/netsim/ansible/templates/initial/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.818695 networklab-1.8.0.post2/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.822695 networklab-1.8.0.post2/netsim/ansible/templates/isis/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.826695 networklab-1.8.0.post2/netsim/ansible/templates/mpls/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/srlinux.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/sros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.834695 networklab-1.8.0.post2/netsim/ansible/templates/ospf/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/junos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/junos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.834695 networklab-1.8.0.post2/netsim/ansible/templates/sr/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.838695 networklab-1.8.0.post2/netsim/ansible/templates/srv6/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.838695 networklab-1.8.0.post2/netsim/ansible/templates/vlan/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/vptx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.846695 networklab-1.8.0.post2/netsim/ansible/templates/vrf/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.850695 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/ansible/templates/vxlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.850695 networklab-1.8.0.post2/netsim/api/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.850695 networklab-1.8.0.post2/netsim/augment/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/addressing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/augment/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.858695 networklab-1.8.0.post2/netsim/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10222 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/alias.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/clab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.858695 networklab-1.8.0.post2/netsim/cli/clab_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/clab_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/clab_actions/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/clab_actions/tarball.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/down.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/external_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show-usage.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.858695 networklab-1.8.0.post2/netsim/cli/show_commands/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/module_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/show_commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/up.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/usage.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25341 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/cli/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.858695 networklab-1.8.0.post2/netsim/daemons/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/daemons/bird.yml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/daemons/dnsmasq.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.862695 networklab-1.8.0.post2/netsim/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/data/filemaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/data/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/data/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28960 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/data/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.862695 networklab-1.8.0.post2/netsim/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/defaults/addressing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/defaults/attributes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/defaults/automation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/defaults/hints.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/defaults/multilab.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/defaults/paths.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/defaults/ports.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.870694 networklab-1.8.0.post2/netsim/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/arubacx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/asav.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/asav.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/csr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/eos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/fortios.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/iosv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/iosv.yml
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/junos.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/none.yml
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/unknown.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/vmx.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/vmx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/vptx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/vsrx.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/vsrx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/devices/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.782695 networklab-1.8.0.post2/netsim/extra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.870694 networklab-1.8.0.post2/netsim/extra/bgp.domain/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.domain/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.domain/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.870694 networklab-1.8.0.post2/netsim/extra/bgp.originate/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.originate/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.originate/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.870694 networklab-1.8.0.post2/netsim/extra/bgp.policy/
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/_route_map_aoscx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/_route_map_ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/simple-attributes.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.policy/srlinux.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.874695 networklab-1.8.0.post2/netsim/extra/bgp.session/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/_sample_bfd_template.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/bird.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/default-originate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/topology.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/bgp.session/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.878695 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/frr.bgp-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.multihop/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.878695 networklab-1.8.0.post2/netsim/extra/ebgp.utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/ebgp.utils/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.878695 networklab-1.8.0.post2/netsim/extra/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/fabric/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/fabric/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.878695 networklab-1.8.0.post2/netsim/extra/multilab/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/multilab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.878695 networklab-1.8.0.post2/netsim/extra/none/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/none/none.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.878695 networklab-1.8.0.post2/netsim/extra/proxy-arp/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.878695 networklab-1.8.0.post2/netsim/install/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2190 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/ansible.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/containerlab.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/grpc.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.882695 networklab-1.8.0.post2/netsim/install/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.882695 networklab-1.8.0.post2/netsim/install/libvirt/asav/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/asav.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/csr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/eos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/iosv.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.882695 networklab-1.8.0.post2/netsim/install/libvirt/vptx/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/vptx/juniper.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/vptx/make-config.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/vptx/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/vptx.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/vptx.xml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.882695 networklab-1.8.0.post2/netsim/install/libvirt/vsrx/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/libvirt.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/install/ubuntu.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.890694 networklab-1.8.0.post2/netsim/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    19797 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/_dataplane.py
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/bfd.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/bfd.yml
--rw-r--r--   0 runner    (1001) docker     (127)    24386 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/bgp.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/dhcp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/eigrp.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/eigrp.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/evpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/evpn.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/gateway.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/isis.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/isis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/mpls.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/mpls.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/ospf.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/sr.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/sr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/srv6.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/srv6.yml
--rw-r--r--   0 runner    (1001) docker     (127)    60006 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/vlan.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20374 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/vrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/vrf.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/vxlan.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/modules/vxlan.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.890694 networklab-1.8.0.post2/netsim/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/d2.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/d2.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/graph.yml
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/graphite.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.894694 networklab-1.8.0.post2/netsim/providers/
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/clab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/external.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/virtualbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/providers/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.894694 networklab-1.8.0.post2/netsim/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.786695 networklab-1.8.0.post2/netsim/templates/provider/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.894694 networklab-1.8.0.post2/netsim/templates/provider/clab/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.894694 networklab-1.8.0.post2/netsim/templates/provider/clab/cumulus/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/clab/cumulus/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/clab/cumulus/interfaces.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.894694 networklab-1.8.0.post2/netsim/templates/provider/clab/frr/
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/clab/frr/daemons.j2
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/clab/frr/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.894694 networklab-1.8.0.post2/netsim/templates/provider/clab/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.894694 networklab-1.8.0.post2/netsim/templates/provider/external/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.898695 networklab-1.8.0.post2/netsim/templates/provider/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/forwarded-ports.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/vptx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.902695 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/virtualbox-ports.j2
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/provider/virtualbox/vsrx-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.902695 networklab-1.8.0.post2/netsim/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/tests/clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/tests/grpc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.902695 networklab-1.8.0.post2/netsim/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/tools/graphite.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/tools/graphite.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.902695 networklab-1.8.0.post2/netsim/tools/suzieq/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/tools/suzieq.yml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/topology-defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.906695 networklab-1.8.0.post2/netsim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/netsim/utils/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.906695 networklab-1.8.0.post2/networklab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-03-16 08:14:05.000000 networklab-1.8.0.post2/networklab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24645 2024-03-16 08:14:05.000000 networklab-1.8.0.post2/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 08:14:05.000000 networklab-1.8.0.post2/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-16 08:14:05.000000 networklab-1.8.0.post2/networklab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-16 08:14:05.000000 networklab-1.8.0.post2/networklab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 08:14:05.906695 networklab-1.8.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 08:14:05.906695 networklab-1.8.0.post2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3377 2024-03-16 08:13:59.000000 networklab-1.8.0.post2/tests/test_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.480151 networklab-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-08 09:30:50.000000 networklab-1.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 09:30:50.000000 networklab-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-08 09:30:57.480151 networklab-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-08 09:30:50.000000 networklab-1.8.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-04-08 09:30:50.000000 networklab-1.8.1/netlab
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.364151 networklab-1.8.1/netsim/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.364151 networklab-1.8.1/netsim/ansible/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2342 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/create-config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/reload-config.ansible
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.368151 networklab-1.8.1/netsim/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/create-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/create-custom-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.368151 networklab-1.8.1/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.372151 networklab-1.8.1/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.372151 networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.372151 networklab-1.8.1/netsim/ansible/tasks/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/frr/mpls-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/initial-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.372151 networklab-1.8.1/netsim/ansible/tasks/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/linux/dhcp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/iosxr-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/vmx/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/wait-for-ready.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/templates/bfd/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.384151 networklab-1.8.1/netsim/ansible/templates/bgp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.384151 networklab-1.8.1/netsim/ansible/templates/dhcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/dnsmasq.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/eos.server.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/ios.server.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/linux.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.384151 networklab-1.8.1/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.384151 networklab-1.8.1/netsim/ansible/templates/evpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.388151 networklab-1.8.1/netsim/ansible/templates/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.392151 networklab-1.8.1/netsim/ansible/templates/initial/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.392151 networklab-1.8.1/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.396151 networklab-1.8.1/netsim/ansible/templates/isis/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.400151 networklab-1.8.1/netsim/ansible/templates/mpls/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/srlinux.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/sros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.408151 networklab-1.8.1/netsim/ansible/templates/ospf/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/junos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.408151 networklab-1.8.1/netsim/ansible/templates/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.408151 networklab-1.8.1/netsim/ansible/templates/srv6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.412151 networklab-1.8.1/netsim/ansible/templates/vlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.420151 networklab-1.8.1/netsim/ansible/templates/vrf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/junos.ospf-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.424151 networklab-1.8.1/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.424151 networklab-1.8.1/netsim/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.424151 networklab-1.8.1/netsim/augment/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/addressing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.432151 networklab-1.8.1/netsim/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10608 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/alias.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/clab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.432151 networklab-1.8.1/netsim/cli/clab_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/clab_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/clab_actions/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/clab_actions/tarball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/down.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/external_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show-usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.432151 networklab-1.8.1/netsim/cli/show_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/module_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/up.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.432151 networklab-1.8.1/netsim/daemons/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/daemons/bird.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/daemons/dnsmasq.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.436151 networklab-1.8.1/netsim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/filemaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28960 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.436151 networklab-1.8.1/netsim/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/addressing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/automation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/hints.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/multilab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/paths.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/ports.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.440151 networklab-1.8.1/netsim/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/arubacx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/asav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/asav.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/csr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/eos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/iosv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/iosv.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/junos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/none.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/unknown.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vmx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vsrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vsrx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.360151 networklab-1.8.1/netsim/extra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.440151 networklab-1.8.1/netsim/extra/bgp.domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.domain/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.domain/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.440151 networklab-1.8.1/netsim/extra/bgp.originate/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.originate/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.originate/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.444151 networklab-1.8.1/netsim/extra/bgp.policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/_route_map_aoscx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/_route_map_ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/simple-attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/srlinux.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/bgp.session/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/_sample_bfd_template.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/bird.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/default-originate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/topology.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/ebgp.multihop/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/ebgp.utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.utils/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/fabric/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/fabric/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/multilab/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/multilab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/none/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/none/none.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/proxy-arp/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/ansible.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/containerlab.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/grpc.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/libvirt/asav/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/iosv.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/libvirt/vptx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.460151 networklab-1.8.1/netsim/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    19815 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/_dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/bfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/bfd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/bgp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/dhcp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/eigrp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/eigrp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/evpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/evpn.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/gateway.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/isis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/isis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/mpls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/mpls.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/ospf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/sr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/sr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/srv6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/srv6.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    60006 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vlan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20374 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vrf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vxlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vxlan.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/d2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/d2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/graph.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/clab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/external.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/virtualbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.364151 networklab-1.8.1/netsim/templates/provider/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/clab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/clab/cumulus/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/cumulus/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/cumulus/interfaces.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/frr/daemons.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/frr/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/external/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.472151 networklab-1.8.1/netsim/templates/provider/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/forwarded-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.472151 networklab-1.8.1/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/vsrx-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.472151 networklab-1.8.1/netsim/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/tests/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/tests/grpc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.472151 networklab-1.8.1/netsim/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/graphite.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.476151 networklab-1.8.1/netsim/tools/suzieq/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/suzieq.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/topology-defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.476151 networklab-1.8.1/netsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.476151 networklab-1.8.1/netsim/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/validate/frr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/validate/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.480151 networklab-1.8.1/networklab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24814 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 09:30:50.000000 networklab-1.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:30:57.480151 networklab-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 09:30:50.000000 networklab-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.476151 networklab-1.8.1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3377 2024-04-08 09:30:50.000000 networklab-1.8.1/tests/test_transformation.py
```

### Comparing `networklab-1.8.0.post2/LICENSE.md` & `networklab-1.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/PKG-INFO` & `networklab-1.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.8.0.post2
+Version: 1.8.1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0). It contains [numerous new features](https://netlab.tools/release/1.8/) that might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use [release 1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.0.post2/README.md` & `networklab-1.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0). It contains [numerous new features](https://netlab.tools/release/1.8/) that might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use [release 1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/collect-configs.ansible` & `networklab-1.8.1/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/config.ansible` & `networklab-1.8.1/netsim/ansible/config.ansible`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
   - fail: msg="Specify configuration template name with an external variable"
     when: config is not defined
     run_once: true
 
   - name: Set variables that cannot be set with VARS
     set_fact:
       netlab_device_type: "{{ netlab_device_type|default(ansible_network_os) }}"
+      netlab_interfaces: "{{ ([ loopback ] if loopback is defined else []) + interfaces|default([]) }}"
       custom_config: "{{ config }}"
 
   - name: Deploy custom configuration templates
     include_tasks: "tasks/deploy-custom-config.yml"
     args:
       apply:
         tags: [ always ]
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/create-config.ansible` & `networklab-1.8.1/netsim/ansible/create-config.ansible`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   vars:
     config_dir: "{{ lookup('env','PWD') }}/config"
   tasks:
   - block:
     - name: Set variables that cannot be set with VARS
       set_fact:
         netlab_device_type: "{{ netlab_device_type|default(ansible_network_os) }}"
+        netlab_interfaces: "{{ ([ loopback ] if loopback is defined else []) + interfaces|default([]) }}"
 
     - name: Create config directory in {{ config_dir }}
       file:
         path: "{{ config_dir }}"
         state: directory
       run_once: true
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/initial-config.ansible` & `networklab-1.8.1/netsim/ansible/initial-config.ansible`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   hosts: all:!unprovisioned
   strategy: "{{ netlab_strategy|default('linear') }}"
   gather_facts: false
   tasks:
   - name: Set variables that cannot be set with VARS
     set_fact:
       netlab_device_type: "{{ netlab_device_type|default(ansible_network_os) }}"
+      netlab_interfaces: "{{ ([ loopback ] if loopback is defined else []) + interfaces|default([]) }}"
       search_path: "{{ paths_templates.dirs }}"
     tags: [ always ]
 
   - import_tasks: tasks/wait-for-ready.yml
   - import_tasks: tasks/initial-config.yml
 
 #
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/reload-config.ansible` & `networklab-1.8.1/netsim/ansible/reload-config.ansible`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     fail: msg="Specify initial configuration directory with the 'config' external variable"
     when: config is not defined
     run_once: true
 
   - name: Set variables that cannot be set with VARS
     set_fact:
       netlab_device_type: "{{ netlab_device_type|default(ansible_network_os) }}"
+      netlab_interfaces: "{{ ([ loopback ] if loopback is defined else []) + interfaces|default([]) }}"
       search_path: "{{ paths_templates.dirs }}"
       custom_config: "{{ config }}"
     tags: [ always ]
 
   - import_tasks: tasks/wait-for-ready.yml
   - include_tasks: tasks/initial-config.yml
     when: netlab_initial|default(False) in ['always']
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/create-config.yml` & `networklab-1.8.1/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.8.1/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/cumulus.yml` & `networklab-1.8.1/netsim/ansible/tasks/fetch-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.8.1/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.8.1/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/iosxr/initial.yml` & `networklab-1.8.1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+---
 # Find the temporary IP address
 #
 - name: "Get current IOS XR IP address from Vagrant"
   shell: "vagrant ssh-config {{ inventory_hostname }}|grep -i hostname|grep -o '[0-9.]*'"
   register: ssh_config
-  when: netlab_provider == 'libvirt'
 
 # Add secondary IP address to the IOS XR management interface if the DHCP server gave
 # it an unexpected IP address due to its use of ASCII DHCP client ID
 #
 - block:
   - name: "Change ansible_hostname for IOS XR to temporary Vagrant-supplied IP address"
     set_fact:
@@ -16,12 +16,8 @@
   - name: "Configure secondary IP address on IOS XR management interface"
     iosxr_config:
       parents:
       - interface {{ mgmt.ifname }}
       lines:
       - ip address {{ mgmt.ipv4 }} 255.255.255.0 secondary
 
-  when: netlab_provider == 'libvirt' and ssh_config is defined and ansible_host != ssh_config.stdout
-
-- name: "iosxr_config: deploying initial config from {{ config_template }}"
-  iosxr_config:
-    src: "{{ config_template }}"
+  when: ssh_config is defined and ansible_host != ssh_config.stdout
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/linux/dhcp.yml` & `networklab-1.8.1/netsim/ansible/tasks/linux/dhcp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.8.1/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/readiness-check/vptx.yml` & `networklab-1.8.1/netsim/ansible/tasks/readiness-check/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.8.1/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.8.1/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.8.1/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.8.1/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/ios.j2`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,51 @@
-{% import "eos.macro.j2" as bgpcfg %}
+{% import "ios.macro.j2" as bgpcfg %}
 !
-route-map next-hop-self-ipv4 permit 10
-   match route-type external
-   set ip next-hop peer-address
-!
-route-map next-hop-self-ipv4 permit 20
-!
-route-map next-hop-self-ipv6 permit 10
-   match route-type external
-   set ipv6 next-hop peer-address
-!
-route-map next-hop-self-ipv6 permit 20
+ip bgp-community new-format
 !
 router bgp {{ bgp.as }}
-  bgp advertise-inactive
-  bgp log-neighbor-changes
   no bgp default ipv4-unicast
-  no bgp default ipv6-unicast
+  bgp update-delay 5
+  bgp nopeerup-delay cold-boot 1
+  bgp nopeerup-delay user-initiated 1
 {% if bgp.router_id|ipv4 %}
-  router-id {{ bgp.router_id }}
+  bgp router-id {{ bgp.router_id }}
 {% endif %}
 {% if bgp.rr|default(False) and bgp.rr_cluster_id|default(False) %}
   bgp cluster-id {{ bgp.rr_cluster_id }}
 {% endif %}
+{#
+    Configure IPv4 and IPv6 BGP neighbors
+#}
 {% for n in bgp.neighbors %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
-{{     bgpcfg.neighbor(n,n[af],bgp) }}
+{{     bgpcfg.neighbor_global(n,n[af]) }}
 {%   endfor %}
 {% endfor %}
 !
-{# Activate address families #}
-{% for af in ['ipv4','ipv6'] %}
-{%   if bgp[af] is defined %}
-!
+{# Configure BGP address families #}
+{% for af in ['ipv4','ipv6'] if bgp[af] is defined %}
  address-family {{ af }}
+  bgp scan-time 5
 !
-{%     if loopback[af] is defined and bgp.advertise_loopback %}
-  network {{ loopback[af]|ipaddr('0') }}
-{%     endif %}
-!
-{%     for l in interfaces|default([]) if l.bgp.advertise|default("") and l[af] is defined and not 'vrf' in l %}
-  network {{ l[af]|ipaddr('0') }}
-{%     endfor %}
-!
-{%     for pfx in bgp.originate|default([]) if af == 'ipv4' %}
-  network {{ pfx|ipaddr('0') }}
-{%     endfor %}
-!
-{%     for n in bgp.neighbors if n[af] is defined and n.activate[af] is defined and n.activate[af] %}
-  neighbor {{ n[af] }} activate
-{%       if n.type == 'ibgp' and bgp.next_hop_self|default(False) %}
-  neighbor {{ n[af] }} route-map next-hop-self-{{ af }} out
-{%       endif %}
-{%     endfor %}
+{%   if loopback[af] is defined and bgp.advertise_loopback %}
+{{     bgpcfg.bgp_network(af,loopback[af]) }}
 {%   endif %}
+!
+{%   for l in interfaces|default([]) if l.bgp.advertise|default("") and l[af] is defined and not 'vrf' in l %}
+{{     bgpcfg.bgp_network(af,l[af]) }}
+{%   endfor %}
+{%   for pfx in bgp.originate|default([]) if af == 'ipv4' %}
+{{     bgpcfg.bgp_network(af,pfx) }}
+{%   endfor %}
+!
+{%   for n in bgp.neighbors if n[af] is defined and n.activate[af] is defined and n.activate[af] %}
+{{     bgpcfg.neighbor_af(n,n[af],bgp) }}
+{%   endfor %}
 {% endfor %}
 !
+{#
+  Add extra IPv4 prefixes
+#}
 {% for pfx in bgp.originate|default([]) %}
-ip route {{ pfx|ipaddr('0') }} Null0
+ip route {{ pfx|ipaddr('network') }} {{ pfx|ipaddr('netmask') }} null 0
 {% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 {#
   Define a BGP neighbor
 #}
-{% macro neighbor(n,ip,bgp) %}
+{% macro neighbor(n,af,bgp) %}
 !
-  neighbor {{ ip }} remote-as {{ n.as }}
-  neighbor {{ ip }} description {{ n.name }}
+{%   if n.local_if is defined %}
+  neighbor ebgp_intf_{{ n.local_if }} peer group
+  neighbor interface {{ n.local_if }} peer-group ebgp_intf_{{ n.local_if }}
+{%   endif %}
+{%   set peer = 'ebgp_intf_' + n.local_if if n.local_if is defined else n[af] %}
+  neighbor {{ peer }} remote-as {{ n.as }}
+  neighbor {{ peer }} description {{ n.name }}
 {%     if n.local_as is defined %}
-  neighbor {{ ip }} local-as {{ n.local_as }} no-prepend replace-as
+  neighbor {{ peer }} local-as {{ n.local_as }} no-prepend replace-as
 {%     endif %}
 {%     if n.type == 'ibgp' %}
-  neighbor {{ ip }} update-source Loopback0
+  neighbor {{ peer }} update-source Loopback0
 {%     endif %}
 {%     if n.type == 'localas_ibgp' %}
-  neighbor {{ ip }} next-hop-peer
+  neighbor {{ peer }} next-hop-peer
 {%     endif %}
 {%     if 'ibgp' in n.type %}
 {%       if bgp.rr|default('') and not n.rr|default('') %}
-  neighbor {{ ip }} route-reflector-client
+  neighbor {{ peer }} route-reflector-client
 {%       endif %}
 {%     endif %}
 {%     if n.type in bgp.community|default({}) %}
-  neighbor {{ ip }} send-community {% 
+  neighbor {{ peer }} send-community {% 
     for ckw in bgp._cprop_order if ckw in bgp.community[n.type] %}{{ ckw }} {% endfor %}
 {%     endif %}
 {%- endmacro %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/frr.bgp-config.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/frr.j2`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #}
 {% for af in ['ipv4','ipv6'] %}
 {%   for n in bgp.neighbors if n[af] is defined %}
 {%     set peer = n[af] if n[af] is string else n.local_if|default('?') %}
   neighbor {{ peer }}{{ ' interface' if peer!=n[af] else '' }} remote-as {{ n.as }}
   neighbor {{ peer }} description {{ n.name }}
 {%     if n.type == 'ibgp' %}
-  neighbor {{ peer }} update-source {{ loopback_name }}
+  neighbor {{ peer }} update-source {{ loopback.ifname }}
 {%     elif n.local_as is defined %}
   neighbor {{ peer }} local-as {{ n.local_as }} {{ 'no-prepend replace-as' if n.replace_global_as|default(True) else '' }}
 {%     endif %}
 !
 {%   endfor %}
 {% endfor %}
 {#
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/routeros.j2`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,39 @@
-{% import "ios.macro.j2" as bgpcfg %}
-!
-ip bgp-community new-format
-!
-router bgp {{ bgp.as }}
-  no bgp default ipv4-unicast
-  bgp update-delay 5
-  bgp nopeerup-delay cold-boot 1
-  bgp nopeerup-delay user-initiated 1
+{% import "routeros.macro.j2" as bgpcfg %}
+
+/routing bgp instance set 0 as={{ bgp.as }}
+
 {% if bgp.router_id|ipv4 %}
-  bgp router-id {{ bgp.router_id }}
+  /routing bgp instance set 0 router-id={{ bgp.router_id }}
 {% endif %}
-{% if bgp.rr|default(False) and bgp.rr_cluster_id|default(False) %}
-  bgp cluster-id {{ bgp.rr_cluster_id }}
-{% endif %}
-{#
-    Configure IPv4 and IPv6 BGP neighbors
-#}
+
 {% for n in bgp.neighbors %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
-{{     bgpcfg.neighbor_global(n,n[af]) }}
+{{     bgpcfg.neighbor(n,n[af],bgp,'default') }}
 {%   endfor %}
 {% endfor %}
-!
-{# Configure BGP address families #}
-{% for af in ['ipv4','ipv6'] if bgp[af] is defined %}
- address-family {{ af }}
-!
-{%   if loopback[af] is defined and bgp.advertise_loopback %}
-{{     bgpcfg.bgp_network(af,loopback[af]) }}
+
+{# Set networks to announce #}
+{% for af in ['ipv4','ipv6'] %}
+{%   if bgp[af] is defined %}
+
+{%     if loopback[af] is defined and bgp.advertise_loopback %}
+{{       bgpcfg.bgp_network(af,loopback[af]) }}
+{%     endif %}
+
+{%     for l in interfaces|default([]) if l.bgp.advertise|default("") and l[af] is defined and not 'vrf' in l %}
+{{       bgpcfg.bgp_network(af,l[af]) }}
+{%     endfor %}
+
+{%     for pfx in bgp.originate|default([]) if af == 'ipv4' %}
+{{       bgpcfg.bgp_network(af,pfx) }}
+{%     endfor %}
+
 {%   endif %}
-!
-{%   for l in interfaces|default([]) if l.bgp.advertise|default("") and l[af] is defined and not 'vrf' in l %}
-{{     bgpcfg.bgp_network(af,l[af]) }}
-{%   endfor %}
-{%   for pfx in bgp.originate|default([]) if af == 'ipv4' %}
-{{     bgpcfg.bgp_network(af,pfx) }}
-{%   endfor %}
-!
-{%   for n in bgp.neighbors if n[af] is defined and n.activate[af] is defined and n.activate[af] %}
-{{     bgpcfg.neighbor_af(n,n[af],bgp) }}
-{%   endfor %}
 {% endfor %}
-!
+
 {#
   Add extra IPv4 prefixes
 #}
 {% for pfx in bgp.originate|default([]) %}
-ip route {{ pfx|ipaddr('network') }} {{ pfx|ipaddr('netmask') }} null 0
+/ip route add type=blackhole dst-address={{ pfx|ipaddr('0') }}
 {% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 {% endif %}
 {%- endmacro %}
 {#
    Address family BGP neighbor definition
 #}
 {% macro neighbor_af(n,ip,bgp) %}
   neighbor {{ ip }} activate
+  neighbor {{ ip }} advertisement-interval 0
 {% if 'ibgp' in n.type %}
 {%   if bgp.next_hop_self is defined and bgp.next_hop_self %}
   neighbor {{ ip }} next-hop-self{% if n.type == 'localas_ibgp' %} all{% endif +%}
 {%   endif %}
 {%   if bgp.rr|default('') and (not n.rr|default('') or n.type == 'localas_ibgp') %}
   neighbor {{ ip }} route-reflector-client
 {%   endif %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/dhcp/cumulus.j2` & `networklab-1.8.1/netsim/ansible/templates/dhcp/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/dhcp/dnsmasq.j2` & `networklab-1.8.1/netsim/ansible/templates/dhcp/dnsmasq.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/dhcp/eos.j2` & `networklab-1.8.1/netsim/ansible/templates/dhcp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/dhcp/eos.server.j2` & `networklab-1.8.1/netsim/ansible/templates/dhcp/eos.server.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/dhcp/ios.j2` & `networklab-1.8.1/netsim/ansible/templates/dhcp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/dhcp/ios.server.j2` & `networklab-1.8.1/netsim/ansible/templates/dhcp/ios.server.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2` & `networklab-1.8.1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.8.1/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.8.1/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.8.1/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/asa.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/eos.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/eos.j2`

 * *Files 8% similar despite different names*

```diff
@@ -22,29 +22,19 @@
 {% endfor %}
 {% if mtu is defined %}
 !
 interface defaults
  mtu {{ mtu }}
 {% endif %}
 !
-{% if loopback is defined %}
-interface {{ loopback.ifname }}
-{%   if 'ipv4' in loopback %}
- ip address {{ loopback.ipv4 }}
-{%   endif %}
-{%   if 'ipv6' in loopback %}
- ipv6 address {{ loopback.ipv6 }}
-{%   endif %}
-{% endif %}
-!
 interface {{ mgmt.ifname|default('Management1') }}
  no lldp transmit
  no lldp receive
 !
-{% for l in interfaces|default([]) %}
+{% for l in netlab_interfaces %}
 interface {{ l.ifname }}
  no shutdown
 {% if l.virtual_interface is not defined %}
  no switchport
 {% endif %}
 {% if l.vrf is defined %}
  vrf {{ l.vrf }}
@@ -69,14 +59,15 @@
 ! Invalid IPv4 address {{ l.ipv4 }}
 {%   endif %}
 {% endif %}
 {#
     Set interface IPv6 addresses
 #}
 {% if 'ipv6' in l %}
+ ipv6 nd ra interval 5
 {%   if l.ipv6 == True %}
  ipv6 enable
 {%   elif l.ipv6|ipv6 %}
  ipv6 address {{ l.ipv6 }}
 {%   else %}
 ! Invalid IPv6 address {{ l.ipv6 }}
 {%   endif %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/frr.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/frr.j2`

 * *Files 7% similar despite different names*

```diff
@@ -62,85 +62,80 @@
 
 /usr/lib/frr/frrinit.sh restart
 {% endif %}
 
 #
 # Create loopbacks and stub devices
 #
-{% for i in (interfaces+[{ 'type': 'loopback', 'ifname': 'lo0'}]) if i.type in ['loopback','stub'] %}
+{% for i in netlab_interfaces if i.type in ['loopback','stub'] %}
 if [ ! -e /sys/class/net/{{ i.ifname }} ]; then
   if [ ! -e /sys/devices/virtual/net/{{ i.ifname }} ]; then
     ip link add {{ i.ifname }} type dummy
     ip link set dev {{ i.ifname }} up
   fi
 fi
 {% endfor %}
 
+# Disable IPv6 (for IPv4-only interfaces) or SLAAC (if the device is a router)
+#
+{% for l in interfaces if l.type in ['lan','p2p','stub'] %}
+{%   if l.ipv6 is not defined %}
+sysctl -qw net.ipv6.conf.{{ l.ifname }}.disable_ipv6=1
+{%   elif role|default('router') != 'host' %}
+sysctl -qw net.ipv6.conf.{{ l.ifname }}.autoconf=0
+sysctl -qw net.ipv6.conf.{{ l.ifname }}.accept_ra=0
+ip link set {{ l.ifname }} down
+ip link set {{ l.ifname }} up
+{%   endif %}
+{% endfor %}
+
 #
 # Add vtysh.conf file
 echo "service integrated-vtysh-config" >/etc/frr/vtysh.conf
 #
 # Set Ethernet interface MTU
-{% for l in interfaces|default([]) if l.mtu is defined %}
+{% for l in interfaces if l.mtu is defined %}
 ip link set {{ l.ifname }} mtu {{ l.mtu }}
 {% endfor %}
 #
 # Rest of initial configuration done through VTYSH
 #
 cat >/tmp/config <<CONFIG
 hostname {{ inventory_hostname }}
 !
 {% if 'ipv6' in af %}
 ipv6 forwarding
 {% endif %}
 {% set frr_defaults = netlab_frr_defaults|default('datacenter') %}
 frr defaults {{ frr_defaults }}
 !
-{% if loopback is defined %}
-interface {{ loopback.ifname }}
- no shutdown
-{%  if loopback.ipv4 is defined %}
- ip address {{ loopback.ipv4 }}
-{%  endif %}
-{%  if loopback.ipv6 is defined %}
- ipv6 address {{ loopback.ipv6 }}
-{%  endif %}
-!
-{% endif %}
-{% for l in interfaces|default([]) %}
+{% for l in netlab_interfaces %}
 interface {{ l.ifname }}
-! no shutdown
+ no shutdown
 {% if l.name is defined %}
  description {{ l.name }}{{ " ["+l.role+"]" if l.role is defined else "" }}
 {% elif l.type|default("") == "stub" %}
  description Stub interface
 {% endif %}
 {% if l.ipv4 is defined and (l.ipv4 is string or l._parent_ipv4 is defined) %}
  ip address {{ l.ipv4 if l.ipv4 is string else l._parent_ipv4 }}
 {% else %}
  ! no ip address
 {% endif %}
 {% if l.ipv6 is defined %}
 {%  if l.ipv6 is string and l.ipv6|ipv6 %}
  ipv6 address {{ l.ipv6 }}
 {%  endif %}
+{%  if l.type != 'loopback' %}
  ipv6 nd ra-interval 5
  no ipv6 nd suppress-ra
-{% else %}
- ! Note, currently does not take for OS configured interfaces; known issue
- ipv6 nd suppress-ra
+{%  endif %}
 {% endif %}
 {% if l.bandwidth is defined %}
  bandwidth {{ l.bandwidth  }}
 {% endif %}
 !
 {% endfor %}
 do write
 CONFIG
 vtysh -f /tmp/config
-
-# Workaround for FRR issue with disabling ipv6 (https://github.com/FRRouting/frr/issues/7738)
-{% for l in interfaces if l.type in ['lan','p2p','stub'] and l.ipv6 is not defined %}
-sysctl -qw net.ipv6.conf.{{ l.ifname }}.disable_ipv6=1
-{% endfor %}
-
 exit 0
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/ios.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/junos.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/junos.j2`

 * *Files 12% similar despite different names*

```diff
@@ -15,39 +15,24 @@
 {% include 'junos.vrf.j2' %}
 {% endif %}
 {% if vlans is defined %}
 {% include 'junos.vlan.j2' %}
 {% endif %}
 
 interfaces {
-  lo0 {
-    unit 0 {
-{% if 'ipv4' in loopback %}
-      family inet {
-        address {{ loopback.ipv4 }};
-      }
-{% endif %}
-{% if 'ipv6' in loopback %}
-      family inet6 {
-        address {{ loopback.ipv6 }};
-      }
-{% endif %}
-    }
-  }
-
 {# Handle MTU outside the main interface loop, since it needs to be applied only to the master interface #}
 {% for l in interfaces|default([]) %}
 {%   if l.mtu is defined %}
   {{ l.junos_interface }} {
     mtu {{ l.mtu + 14 }};
   }
 {%   endif %}
 {% endfor %}
 
-{% for l in interfaces|default([]) %}
+{% for l in netlab_interfaces %}
   {{ l.ifname }} {
 {% if l.name is defined %}
     description "{{ l.name }}{{ " ["+l.role+"]" if l.role is defined else "" }}";
 {% elif l.type|default("") == "stub" %}
     description "Stub interface"
 {% endif %}
     
@@ -91,8 +76,17 @@
 protocols {
   lldp {
     interface {{ mgmt.ifname|default('fxp0') }} {
       disable;
     }
     interface all;
   }
+{% for l in netlab_interfaces if 'ipv6' in l and l.type != 'loopback' %}
+{%   if loop.first %}
+  router-advertisement {
+{%   endif %}
+    interface {{ l.ifname }};
+{%   if loop.last %}
+  }
+{%   endif %}
+{% endfor %}
 }
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/nxos.j2`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,23 @@
 {% if vlans is defined %}
 feature interface-vlan
 {% endif %}
 {% if vrfs is defined %}
 {% include 'nxos.vrf.j2' %}
 !
 {% endif %}
-interface {{ loopback.ifname }}
-{% if 'ipv4' in loopback %}
- ip address {{ loopback.ipv4 }}
-{% endif %}
-{% if 'ipv6' in loopback %}
- ipv6 address {{ loopback.ipv6 }}
-{% endif %}
 !
 interface {{ mgmt.ifname|default('GigabitEthernet0/0') }}
  no lldp transmit
  no lldp receive
 !
-{% for l in interfaces|default([]) %}
+{% for l in netlab_interfaces %}
 interface {{ l.ifname }}
  no shutdown
-{% if l.virtual_interface is not defined and l.vlan is not defined %}
+{% if l.virtual_interface is not defined %}
  no switchport
  mac-address {{ '52dc.cafe.%02d%02d' % ( id,l.ifindex ) }}
 {% endif %}
 {% if l.vrf is defined %}
   vrf member {{ l.vrf }}
 {% endif %}
 {% if l.name is defined %}
@@ -73,10 +66,11 @@
 {%   if l.ipv6 == True %}
  ipv6 address use-link-local-only
 {%   elif l.ipv6|ipv6 %}
  ipv6 address {{ l.ipv6 }}
 {%   else %}
 ! Invalid IPv6 address {{ l.ipv6 }}
 {%   endif %}
+ ipv6 nd ra-interval 5 min 3
 {% endif %}
 !
 {% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.8.1/netsim/ansible/templates/initial/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/asa.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/eos.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/frr.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/frr.j2`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {% elif isis.area is defined %}
   net {{ "%s.0000.0000.%04d.00" % (isis.area,id) }}
 {% endif %}
 {% if isis.af.ipv6 is defined %}
   topology ipv6-unicast
 {% endif %}
 !
-interface lo0
+interface {{ loopback.ifname }}
 {% if 'ipv4' in loopback and 'ipv4' in isis.af %}
   ip router isis Gandalf
 {% endif %}
 {% if 'ipv6' in loopback and 'ipv6' in isis.af %}
   ipv6 router isis Gandalf
 {% endif %}
 !
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/ios.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/junos.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.8.1/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/srlinux.ldp.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/srlinux.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/sros.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/sros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files 6% similar despite different names*

```diff
@@ -38,7 +38,21 @@
 {% endif %}
 {% if 'isis' in module %}
 - path: configure/router[router-name=Base]/isis[isis-instance=0]
   val:
    ldp-sync: False
 {% endif %}
 {% endif %}
+
+{# If BGP is used, allow next hop resolution via LDP #}
+{% if 'bgp' in module %}
+- path: configure/router[router-name=Base]/bgp/next-hop-resolution
+  val:
+   shortcut-tunnel:
+    family:
+{%  for af in ('ipv4','ipv6') if af in loopback %}
+    - family-type: {{ af }}
+      resolution: filter
+      resolution-filter:
+       ldp: True
+{%  endfor %}
+{% endif %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/sros.mplsvpn.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/sros.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.8.1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
  passive-interface {{ l.ifname }}
 {% endfor %}
 {% if ospf.reference_bandwidth is defined %}
  auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
 {% endif %}
 !
 {% if 'ipv4' in loopback %}
-interface {{ loopback_name }}
+interface {{ loopback.ifname }}
  ip ospf area {{ ospf.area }}
 {% endif %}
 !
 {% for l in interfaces|default([]) if 'ospf' in l and ('ipv4' in l or 'ipv4' in l.dhcp.client|default({})) %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
  ip ospf area {{ l.ospf.area }}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 router ospf6
  ospf6 router-id {{ ospf.router_id }}
 {% if ospf.reference_bandwidth is defined %}
  auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
 {% endif %}
 {% if 'ipv6' in loopback %}
- interface {{ loopback_name }} area {{ ospf.area }}
+ interface {{ loopback.ifname }} area {{ ospf.area }}
 {% endif %}
 {% for l in interfaces|default([]) if 'ospf' in l and ('ipv6' in l or 'ipv6' in l.dhcp.client|default({})) %}
  interface {{ l.ifname }} area {{ l.ospf.area }}
 {% endfor %}
 !
 {% for l in interfaces|default([]) if 'ospf' in l and ('ipv6' in l or 'ipv6' in l.dhcp.client|default({})) %}
 interface {{ l.ifname }}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-router ospf {{ pid }}
-{% if ospf.router_id|ipv4 %}
- router-id {{ ospf.router_id }}
-{% endif %}
-{% if ospf.unnumbered is defined %}
- interface unnumbered hello mask tx 0.0.0.0
-{% endif %}
+!
+router ospf {{ vdata.vrfidx }} vrf {{ vname }}
+ router-id {{ vdata.ospf.router_id|default(ospf.router_id) }}
 {% if ospf.reference_bandwidth is defined %}
  auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
 {% endif %}
-{% for l in interfaces|default([]) if l.ospf.passive|default(False) %}
+{% for l in vdata.ospf.interfaces|default([]) if l.ospf.passive|default(False) %}
  passive-interface {{ l.ifname }}
 {% endfor %}
+{% if bgp.as is defined %}
+ redistribute bgp {{ bgp.as }} subnets
+{% endif %}
 !
-interface Loopback0
- ip ospf area {{ ospf.area }}
-!
-{% for l in interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
+{% for l in vdata.ospf.interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ip ospf area {{ l.ospf.area }}
-{%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
-{%     if l.ospf.network_type == "broadcast" %}
- no ip ospf network
-{%     else %}
+ ip ospf {{ vdata.vrfidx }} area {{ l.ospf.area }}
+{%   if l.ospf.network_type is defined %}
  ip ospf network {{ l.ospf.network_type }}
-{%     endif %}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
  ip ospf cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
- ip ospf neighbor bfd
+ ip ospf bfd
 {%   endif %}
 !
 {% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-ipv6 router ospf {{ pid }}
- router-id {{ ospf.router_id }}
-{% if ospf.reference_bandwidth is defined %}
- auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
+{% set pid = ospf.process|default(1) %}
+feature ospfv3
+{% if ospf.bfd|default(False) %}
+feature bfd
 {% endif %}
-{% for l in interfaces|default([]) if l.ospf.passive|default(False) %}
- passive-interface {{ l.ifname }}
-{% endfor %}
 !
-{% if 'ipv6' in loopback %}
-interface Loopback0
- ipv6 ospf {{ pid }} area {{ ospf.area }}
+router ospfv3 {{ pid }}
+{% if ospf.router_id|ipv4 %}
+ router-id {{ ospf.router_id }}
+{% endif %}
+{% if ospf.reference_bandwidth is defined %}
+ auto-cost reference-bandwidth {{ ospf.reference_bandwidth }} Mbps
 {% endif %}
 !
-{% for l in interfaces|default([]) if 'ospf' in l and 'ipv6' in l %}
+{% for l in netlab_interfaces if 'ospf' in l and 'ipv6' in l %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ipv6 ospf {{ pid }} area {{ l.ospf.area }}
+ ipv6 router ospfv3 {{ pid }} area {{ l.ospf.area }}
 {%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
-{%     if l.ospf.network_type == "broadcast" %}
- no ipv6 ospf network
-{%     else %}
- ipv6 ospf network {{ l.ospf.network_type }}
-{%     endif %}
+ ospfv3 network {{ l.ospf.network_type }}
+{%   elif l.type == 'loopback' %}
+ ospfv3 network point-to-point
 {%   endif %}
 {%   if l.ospf.cost is defined %}
- ipv6 ospf cost {{ l.ospf.cost }}
+ ospfv3 cost {{ l.ospf.cost }}
+{%   endif %}
+{%   if l.ospf.passive|default(False) %}
+ ospfv3 passive-interface
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
- ipv6 ospf bfd
+ ospfv3 bfd
 {%   endif %}
 !
 {% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-router ospf
-{% if ospf.router_id|ipv4 %}
- ospf router-id {{ ospf.router_id }}
+!
+route-map all
+!
+{% set pid = vdata.vrfidx %}
+feature ospf
+{% if vdata.ospf.bfd|default(False) %}
+feature bfd
+{% endif %}
+!
+router ospf {{ pid }}
+ vrf {{ vname }}
+  timers throttle spf 100 200 500
+  timers throttle lsa 0 100 500
+{% if vdata.ospf.router_id|ipv4 %}
+  router-id {{ vdata.ospf.router_id }}
 {% endif %}
 {% if ospf.reference_bandwidth is defined %}
- auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
+  auto-cost reference-bandwidth {{ ospf.reference_bandwidth }} Mbps
 {% endif %}
-exit
 !
-{% if 'ipv4' in loopback %}
-interface {{ loopback_name }}
- ip ospf area {{ ospf.area }}
+  redistribute direct route-map all
+{% if bgp.as is defined %}
+  redistribute bgp {{ bgp.as }} route-map all
 {% endif %}
 !
-{% for l in interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
+{% for l in vdata.ospf.interfaces|default([]) %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ip ospf area {{ l.ospf.area }}
-{%   if l.ospf.network_type is defined %}
+ ip router ospf {{ pid }} area {{ l.ospf.area }}
+{%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
  ip ospf network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
  ip ospf cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.passive|default(False) %}
- ip ospf passive
+ ip ospf passive-interface
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
-{%     set link_bfd = l.bfd|default({}) %}
- ip ospf bfd {{
-   link_bfd.multiplier|default(bfd.multiplier)|default(3)
-   }} {{ 
-   link_bfd.min_rx|default(bfd.min_rx)|default(500) }} {{ 
-   link_bfd.min_tx|default(bfd.min_tx)|default(500) }}
+ ip ospf bfd
 {%   endif %}
 !
 {% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-{% if 'ipv6' in loopback %}
-interface {{ loopback_name }}
- ipv6 ospf6 area {{ ospf.area }}
-!
+{% macro config(ospf_pid,ospf_vrf,ospf_data,intf_data,bgp={}) %}
+{% if ospf_vrf %}
+router ospf {{ ospf_pid }} vrf {{ ospf_vrf }}
+{% else %}
+router ospf {{ ospf_pid }}
+{% endif %}
+{% if ospf_data.router_id|ipv4 %}
+ router-id {{ ospf_data.router_id }}
+{% endif %}
+{% if ospf_data.reference_bandwidth is defined %}
+ auto-cost reference-bandwidth {{ ospf_data.reference_bandwidth }}
+{% endif %}
+{% for l in intf_data if l.ospf.passive|default(False) %}
+ passive-interface {{ l.ifname }}
+{% endfor %}
+{% if ospf_vrf %}
+ redistribute connected
+{%   if bgp.as is defined %}
+ redistribute bgp {{ bgp.as }} subnets
+{%   endif %}
 {% endif %}
-{% for l in interfaces|default([]) if 'ospf' in l and 'ipv6' in l %}
+!
+{% for l in intf_data if 'ospf' in l and ('ipv4' in l or 'ipv4' in l.dhcp.client|default({})) %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ipv6 ospf6 area {{ l.ospf.area }}
+ ip ospf {{ ospf_pid }} area {{ l.ospf.area }}
 {%   if l.ospf.network_type is defined %}
- ipv6 ospf6 network {{ l.ospf.network_type }}
+ ip ospf network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
- ipv6 ospf6 cost {{ l.ospf.cost }}
-{%   endif %}
-{%   if l.ospf.passive|default(False) %}
- ipv6 ospf6 passive
+ ip ospf cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
-{%     set link_bfd = l.bfd|default({}) %}
- ipv6 ospf6 bfd {{
-   link_bfd.multiplier|default(bfd.multiplier)|default(3)
-   }} {{ 
-   link_bfd.min_rx|default(bfd.min_rx)|default(500) }} {{ 
-   link_bfd.min_tx|default(bfd.min_tx)|default(500) }}
+ ip ospf bfd
 {%   endif %}
 !
 {% endfor %}
-!
-router ospf6
- ospf6 router-id {{ ospf.router_id }}
-{% if ospf.reference_bandwidth is defined %}
- auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
-{% endif %}
-exit
+{% endmacro %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv2.j2`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-{% set pid = ospf.process|default(1) %}
-router ospf {{ pid }}
-{% if ospf.router_id|ipv4 %}
- router-id {{ ospf.router_id }}
+{% macro config(ospf_pid,ospf_vrf,ospf_data,intf_data,bgp={}) %}
+{% if ospf_vrf %}
+router ospf {{ ospf_pid }} vrf {{ ospf_vrf }}
+{% else %}
+router ospf {{ ospf_pid }}
 {% endif %}
-{% if ospf.reference_bandwidth is defined %}
- auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
+{% if ospf_data.router_id|ipv4 %}
+ router-id {{ ospf_data.router_id }}
 {% endif %}
-{% for l in interfaces|default([]) if l.ospf.passive|default(False) %}
+{% if ospf_data.reference_bandwidth is defined %}
+ auto-cost reference-bandwidth {{ ospf_data.reference_bandwidth }}
+{% endif %}
+{% for l in intf_data if l.ospf.passive|default(False) %}
  passive-interface {{ l.ifname }}
 {% endfor %}
-!
-{% if 'ipv4' in loopback %}
-interface Loopback0
- ip ospf {{ pid }} area {{ ospf.area }}
+{% if ospf_vrf %}
+ redistribute connected
+{%   if bgp.as is defined %}
+ redistribute bgp {{ bgp.as }} subnets
+{%   endif %}
 {% endif %}
 !
-{% for l in interfaces|default([]) if 'ospf' in l and ('ipv4' in l or 'ipv4' in l.dhcp.client|default({})) %}
+{% for l in intf_data if 'ospf' in l and ('ipv4' in l or 'ipv4' in l.dhcp.client|default({})) %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ip ospf {{ pid }} area {{ l.ospf.area }}
+ ip ospf {{ ospf_pid }} area {{ l.ospf.area }}
 {%   if l.ospf.network_type is defined %}
  ip ospf network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
  ip ospf cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
  ip ospf bfd
 {%   endif %}
 !
 {% endfor %}
+{% endmacro %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 {% set pid = ospf.process|default(1) %}
-ipv6 router ospf {{ pid }}
+feature ospf
+{% if ospf.bfd|default(False) %}
+feature bfd
+{% endif %}
+!
+router ospf {{ pid }}
+{% if ospf.router_id|ipv4 %}
  router-id {{ ospf.router_id }}
+ timers throttle spf 100 200 500
+ timers throttle lsa 0 100 500
+{% endif %}
 {% if ospf.reference_bandwidth is defined %}
- auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
+ auto-cost reference-bandwidth {{ ospf.reference_bandwidth }} Mbps
 {% endif %}
-{% for l in interfaces|default([]) if l.ospf.passive|default(False) %}
- passive-interface {{ l.ifname }}
-{% endfor %}
 !
-{% if 'ipv6' in loopback %}
-interface Loopback0
- ipv6 ospf {{ pid }} area {{ ospf.area }}
-{% endif %}
+{% if 'ipv4' in loopback %}
+interface loopback0
+ ip router ospf {{ pid }} area {{ ospf.area }}
 !
-{% for l in interfaces|default([]) if 'ospf' in l and ('ipv6' in l or 'ipv6' in l.dhcp.client|default({})) %}
+{% endif %}
+{% for l in interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ipv6 ospf {{ pid }} area {{ l.ospf.area }}
-{%   if l.ospf.network_type is defined %}
- ipv6 ospf network {{ l.ospf.network_type }}
+ ip router ospf {{ pid }} area {{ l.ospf.area }}
+{%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
+ ip ospf network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
- ipv6 ospf cost {{ l.ospf.cost }}
+ ip ospf cost {{ l.ospf.cost }}
+{%   endif %}
+{%   if l.ospf.passive|default(False) %}
+ ip ospf passive-interface
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
- ipv6 ospf bfd
+ ip ospf bfd
 {%   endif %}
 !
 {% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-{% set pid = ospf.process|default(1) %}
-feature ospf
-{% if ospf.bfd|default(False) %}
-feature bfd
+{% macro config(ospf_pid,ospf_vrf,ospf_data,intf_data,bgp={}) %}
+router ospfv3 {{ ospf_pid }}
+ router-id {{ ospf_data.router_id }}
+{% if ospf_data.reference_bandwidth is defined %}
+ auto-cost reference-bandwidth {{ ospf_data.reference_bandwidth }}
 {% endif %}
-!
-router ospf {{ pid }}
-{% if ospf.router_id|ipv4 %}
- router-id {{ ospf.router_id }}
+{% if ospf_vrf %}
+ address-family ipv6 unicast vrf {{ ospf_vrf }}
+{% else %}
+ address-family ipv6 unicast
 {% endif %}
-{% if ospf.reference_bandwidth is defined %}
- auto-cost reference-bandwidth {{ ospf.reference_bandwidth }} Mbps
+{% for l in intf_data if l.ospf.passive|default(False) %}
+  passive-interface {{ l.ifname }}
+{% endfor %}
+{% if ospf_vrf %}
+  redistribute connected
+{%   if bgp.as is defined %}
+  redistribute bgp {{ bgp.as }}
+{%   endif %}
 {% endif %}
 !
-{% if 'ipv4' in loopback %}
-interface loopback0
- ip router ospf {{ pid }} area {{ ospf.area }}
-!
-{% endif %}
-{% for l in interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
+{% for l in intf_data if 'ospf' in l and ('ipv6' in l or 'ipv6' in l.dhcp.client|default({})) %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ip router ospf {{ pid }} area {{ l.ospf.area }}
-{%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
- ip ospf network {{ l.ospf.network_type }}
+ ospfv3 {{ ospf_pid }} ipv6 area {{ l.ospf.area }}
+{%   if l.type == 'loopback' %}
+ ospfv3 network point-to-point
+{%   elif l.ospf.network_type is defined %}
+ ospfv3 network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
- ip ospf cost {{ l.ospf.cost }}
-{%   endif %}
-{%   if l.ospf.passive|default(False) %}
- ip ospf passive-interface
+ ospfv3 cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
- ip ospf bfd
+ ospfv3 bfd
 {%   endif %}
 !
 {% endfor %}
+{% endmacro %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv3.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-{% set pid = ospf.process|default(1) %}
-feature ospfv3
-{% if ospf.bfd|default(False) %}
-feature bfd
+{% macro config(ospf_pid,ospf_vrf,ospf_data,intf_data,bgp={}) %}
+router ospfv3 {{ ospf_pid }}
+ router-id {{ ospf_data.router_id }}
+{% if ospf_data.reference_bandwidth is defined %}
+ auto-cost reference-bandwidth {{ ospf_data.reference_bandwidth }}
 {% endif %}
-!
-router ospfv3 {{ pid }}
-{% if ospf.router_id|ipv4 %}
- router-id {{ ospf.router_id }}
+{% if ospf_vrf %}
+ address-family ipv6 unicast vrf {{ ospf_vrf }}
+{% else %}
+ address-family ipv6 unicast
 {% endif %}
-{% if ospf.reference_bandwidth is defined %}
- auto-cost reference-bandwidth {{ ospf.reference_bandwidth }} Mbps
+{% for l in intf_data if l.ospf.passive|default(False) %}
+  passive-interface {{ l.ifname }}
+{% endfor %}
+{% if ospf_vrf %}
+  redistribute connected
+{%   if bgp.as is defined %}
+  redistribute bgp {{ bgp.as }}
+{%   endif %}
 {% endif %}
 !
-{% if 'ipv6' in loopback %}
-interface loopback0
- ipv6 router ospfv3 {{ pid }} area {{ ospf.area }}
-!
-{% endif %}
-{% for l in interfaces|default([]) if 'ospf' in l and 'ipv6' in l %}
+{% for l in intf_data if 'ospf' in l and ('ipv6' in l or 'ipv6' in l.dhcp.client|default({})) %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ipv6 router ospfv3 {{ pid }} area {{ l.ospf.area }}
-{%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
+ ospfv3 {{ ospf_pid }} ipv6 area {{ l.ospf.area }}
+{%   if l.type == 'loopback' %}
+ ospfv3 network point-to-point
+{%   elif l.ospf.network_type is defined %}
  ospfv3 network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
  ospfv3 cost {{ l.ospf.cost }}
 {%   endif %}
-{%   if l.ospf.passive|default(False) %}
- ospfv3 passive-interface
-{%   endif %}
 {%   if l.ospf.bfd|default(False) %}
  ospfv3 bfd
 {%   endif %}
 !
 {% endfor %}
+{% endmacro %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/sr/junos.j2` & `networklab-1.8.1/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/sr/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.8.1/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/vptx.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/vptx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.8.1/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 {#
   Define a BGP neighbor
 #}
-{% macro neighbor(n,ip,bgp) %}
+{% macro neighbor(n,af,bgp) %}
 !
-  neighbor {{ ip }} remote-as {{ n.as }}
-  neighbor {{ ip }} description {{ n.name }}
+{%   if n.local_if is defined %}
+  neighbor ebgp_intf_{{ n.local_if }} peer group
+  neighbor interface {{ n.local_if }} peer-group ebgp_intf_{{ n.local_if }}
+{%   endif %}
+{%   set peer = 'ebgp_intf_' + n.local_if if n.local_if is defined else n[af] %}
+  neighbor {{ peer }} remote-as {{ n.as }}
+  neighbor {{ peer }} description {{ n.name }}
 {%     if n.local_as is defined %}
-  neighbor {{ ip }} local-as {{ n.local_as }} no-prepend replace-as
+  neighbor {{ peer }} local-as {{ n.local_as }} no-prepend replace-as
 {%     endif %}
 {%     if n.type == 'ibgp' %}
-  neighbor {{ ip }} update-source Loopback0
+  neighbor {{ peer }} update-source Loopback0
 {%     endif %}
 {%     if n.type == 'localas_ibgp' %}
-  neighbor {{ ip }} next-hop-peer
+  neighbor {{ peer }} next-hop-peer
 {%     endif %}
 {%     if 'ibgp' in n.type %}
 {%       if bgp.rr|default('') and not n.rr|default('') %}
-  neighbor {{ ip }} route-reflector-client
+  neighbor {{ peer }} route-reflector-client
 {%       endif %}
 {%     endif %}
 {%     if n.type in bgp.community|default({}) %}
-  neighbor {{ ip }} send-community {% 
+  neighbor {{ peer }} send-community {% 
     for ckw in bgp._cprop_order if ckw in bgp.community[n.type] %}{{ ckw }} {% endfor %}
 {%     endif %}
 {%- endmacro %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.8.1/netsim/extra/bgp.session/arubacx.j2`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,64 @@
-{% import "eos.bgp-macro.j2" as bgpcfg %}
-!
-mpls ip
+{% macro ebgp_session(n,af,bgp) -%}
+{%   if n.password is defined %}
+  neighbor {{ n[af] }} password plaintext {{ n.password }}
+{%   endif %}
+{%   if n.gtsm is defined %}
+  neighbor {{ n[af] }} ttl-security-hops {{ n.gtsm }}
+{%   endif %}
+{%   if n.timers is defined %}
+  neighbor {{ n[af] }} timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
+{%   endif %}
+{%   if n.bfd is defined %}
+  neighbor {{ n[af] }} fall-over bfd
+{%   endif %}
+{%   if n.remove_private_as|default([]) %}
+  neighbor {{ n[af] }} remove-private-as
+{%   endif %}
+{%- endmacro %}
+
+{% macro ebgp_neighbor(n,af) -%}
+{%   if n.default_originate is defined %}
+  neighbor {{ n[af] }} default-originate
+{%   endif %}
+{%   if n.allowas_in is defined %}
+  neighbor {{ n[af] }} allowas-in {{ n.allowas_in }}
+{%   endif %}
+{%- endmacro %}
+
 !
 router bgp {{ bgp.as }}
-{% for vname,vdata in vrfs.items() %}
+{% for af in ['ipv4','ipv6'] %}
+{%   for n in bgp.neighbors if n[af] is defined %}
+{{     ebgp_session(n,af,bgp) -}}
+{%   endfor %}
+{% endfor %}
 !
- vrf {{ vname }}
-  redistribute connected
-  router-id {{ vdata.bgp.router_id|default(bgp.router_id) }}
-  rd {{ vdata.rd }}
-{%   if 'ospf' in vdata %}
-  redistribute ospf
-{%   endif %}
-{%   for af in ['ipv4','ipv6'] if af in vdata.af|default({}) %}
-{%     for rt in vdata.import %}
-  route-target import vpn-{{ af }} {{ rt }}
-{%     endfor %}
-{%     for rt in vdata.export %}
-  route-target export vpn-{{ af }} {{ rt }}
-{%     endfor %}
+{% for af in ['ipv4','ipv6'] %}
+{%   for n in bgp.neighbors if n[af] is defined %}
+{%     if loop.first %}
+ address-family {{ af }} unicast
+{%     endif %}
+{{     ebgp_neighbor(n,af) -}}
 {%   endfor %}
-{%   for n in vdata.bgp.neighbors|default([]) %}
-{%     for af in ['ipv4','ipv6'] if n[af] is defined %}
-{{       bgpcfg.neighbor(n,n[af],bgp) }}
-{%     endfor %}
+{% endfor %}
+!
+{% if vrfs is defined %}
+{% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
+ vrf {{ vname }}
+{% for af in ['ipv4','ipv6'] %}
+{%   for n in bgp.neighbors if n[af] is defined %}
+{{     ebgp_session(n,af,bgp) -}}
 {%   endfor %}
+{% endfor %}
+!
 {%   for af in ['ipv4','ipv6'] %}
-{%     for n in vdata.networks|default([]) if af in n %}
-{%       if loop.index == 1 %}
-  address-family {{ af }}
+{%     for n in vdata.bgp.neighbors if n[af] is defined %}
+{%       if loop.first %}
+   address-family {{ af }} unicast
 {%       endif %}
-   network {{ n[af]|ipaddr('0') }}
-{%     endfor %}
-{%     for n in vdata.bgp.neighbors|default([]) if n[af] is defined %}
-{%       if loop.index == 1 %}
-  address-family {{ af }}
-{%       endif %}
-   neighbor {{ n[af] }} activate
+{{       ebgp_neighbor(n,af) -}}
 {%     endfor %}
 {%   endfor %}
 {% endfor %}
+{% endif %}
+!
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,47 @@
+{% macro config(ospf_pid,ospf_vrf,ospf_data,intf_data,bgp={}) %}
 !
-router ospf {{ vdata.vrfidx }} vrf {{ vname }}
- router-id {{ vdata.ospf.router_id|default(ospf.router_id) }}
- interface unnumbered hello mask tx 0.0.0.0
-{% if bgp.as is defined %}
- redistribute bgp include leaked
-{% endif %}
-{% if ospf.reference_bandwidth is defined %}
- auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
-{% endif %}
-{% for l in vdata.ospf.interfaces|default([]) if l.ospf.passive|default(False) %}
- passive-interface {{ l.ifname }}
-{% endfor %}
+! OSPFv3 FRR configuration
 !
-{% for l in vdata.ospf.interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
+{% for l in intf_data if 'ospf' in l and 'ipv6' in l %}
 interface {{ l.ifname }}
 ! {{ l.name|default("") }}
- ip ospf area {{ l.ospf.area }}
-{%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
-{%     if l.ospf.network_type == "broadcast" %}
- no ip ospf network
-{%     else %}
- ip ospf network {{ l.ospf.network_type }}
-{%     endif %}
+ ipv6 ospf6 area {{ l.ospf.area }}
+{%   if l.ospf.network_type is defined %}
+ ipv6 ospf6 network {{ l.ospf.network_type }}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
- ip ospf cost {{ l.ospf.cost }}
+ ipv6 ospf6 cost {{ l.ospf.cost }}
+{%   endif %}
+{%   if l.ospf.passive|default(False) %}
+ ipv6 ospf6 passive
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
- ip ospf neighbor bfd
+{%     set link_bfd = l.bfd|default({}) %}
+ ipv6 ospf6 bfd {{
+   link_bfd.multiplier|default(bfd.multiplier)|default(3)
+   }} {{ 
+   link_bfd.min_rx|default(bfd.min_rx)|default(500) }} {{ 
+   link_bfd.min_tx|default(bfd.min_tx)|default(500) }}
 {%   endif %}
 !
 {% endfor %}
+!
+{% if ospf_vrf %}
+router ospf6 vrf {{ ospf_vrf }}
+{% else %}
+router ospf6
+{% endif %}
+ ospf6 router-id {{ ospf_data.router_id }}
+ timers lsa min-arrival 100
+ timers throttle spf 10 50 500
+{% if ospf_vrf %}
+{%   if bgp.as is defined %}
+ redistribute bgp
+{%   endif %}
+ redistribute connected
+{% endif %}
+{% if ospf_data.reference_bandwidth is defined %}
+ auto-cost reference-bandwidth {{ ospf_data.reference_bandwidth }}
+{% endif %}
+exit
+{% endmacro %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.8.1/netsim/extra/bgp.session/nxos.j2`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,55 @@
+{% macro ebgp_session(n,af,bgp) -%}
+{%   if n.password is defined %}
+      password {{ n.password }}
+{%   endif %}
+{%   if n.gtsm is defined %}
+      ttl-security hops {{ n.gtsm }}
+{%   endif %}
+{%   if n.timers is defined %}
+      timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
+{%   endif %}
+{%   if n.passive|default(False) %}
+      transport connection-mode passive
+{%   endif %}
+{%   if n.remove_private_as|default([]) %}
+{%     set rpa = { 'on': '', 'replace': 'replace-as', 'all': 'all' } %}
+{%     for rpo in n.remove_private_as if rpo in rpa %}
+      neighbor {{ n[af] }} remove-private-as {{ rpa[rpo] }}
+{%     endfor %}
+{%   endif %}
+{%- endmacro %}
 !
-router bgp {{ vdata.as|default(bgp.as) }} vrf {{ vname }}
- no bgp ebgp-requires-policy
- no bgp default ipv4-unicast
-{% for n in vdata.bgp.neighbors|default([]) %}
-{%   for af in ['ipv4','ipv6'] if n[af] is defined %}
-{%     set peer = n[af] if n[af] is string else n.local_if|default('?') %}
-{%     if n[af] is string %}
- neighbor {{ peer }} remote-as {{ n.as }}
-{%     else %}
- neighbor {{ peer }} interface remote-as {{ n.as }}
+{% macro ebgp_neighbor(n,af) -%}
+{%     if n.allowas_in is defined %}
+        allowas-in {{ n.allowas_in }}
 {%     endif %}
- neighbor {{ peer }} description {{ n.name }}
-{%     if n.local_as is defined %}
-  neighbor {{ peer }} local-as {{ n.local_as }} {{ 'no-prepend replace-as' if n.replace_global_as|default(True) else '' }}
+{%     if n.as_override|default(False) %}
+        as-override
 {%     endif %}
-{%   endfor %}
-{% endfor %}
-{% for af in ['ipv4','ipv6'] if vdata.af[af]|default(False) %}
- address-family {{ af }} unicast
-  redistribute connected
-  label vpn export auto
-  export vpn
-  import vpn
-  rd vpn export {{ vdata.rd }}
-  rt vpn import {{ vdata.import|join(" ") }}
-  rt vpn export {{ vdata.export|join(" ") }}
-{%   if af == 'ipv4' and 'ospf' in vdata %}
-  redistribute ospf
-{%   endif %}
-{%   for n in vdata.networks|default([]) if af in n %}
-  network {{ n[af]|ipaddr('0') }}
-{%   endfor %}
-{%   for n in vdata.bgp.neighbors|default([]) if n[af] is defined %}
-{%     set peer = n[af] if n[af] is string else n.local_if|default('?') %}
-  neighbor {{ peer }} activate
-{%     if n.type in bgp.community|default({}) %}
-{%       for c_type in bgp.community[n.type] %}
-  neighbor {{ peer }} send-community {{ c_type }}
-{%       endfor %}
+{%     if n.default_originate|default(False) %}
+        default-originate
 {%     endif %}
-{%   endfor %}
- exit-address-family
+{%- endmacro %}
+!
+router bgp {{ bgp.as }}
+{% for af in ['ipv4','ipv6'] %}
+{%   for n in bgp.neighbors if n[af] is defined %}
+  neighbor {{ n[af] }}
+{{     ebgp_session(n,af,bgp) }}
+      address-family {{ af }} unicast
+{{     ebgp_neighbor(n,af) }}
+{%  endfor %}
 {% endfor %}
+{% set vrfs = vrfs|default({}) %}
+{% for vname, vdata in vrfs.items() %}
+  vrf {{ vname }}
 !
+{%   for af in ['ipv4','ipv6'] %}
+{%     for n in vdata.bgp.neighbors|default([]) if af in n %}
+    neighbor {{ n[af] }} remote-as {{ n.as }}
+{{       ebgp_session(n,af,vdata.bgp) }}
+      address-family {{ af }} unicast
+{{       ebgp_neighbor(n,af) }}
+{%     endfor %}
+{%   endfor %}
+{% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 {% endif %}
 {%- endmacro %}
 {#
    Address family BGP neighbor definition
 #}
 {% macro neighbor_af(n,ip,bgp) %}
   neighbor {{ ip }} activate
+  neighbor {{ ip }} advertisement-interval 0
 {% if 'ibgp' in n.type %}
 {%   if bgp.next_hop_self is defined and bgp.next_hop_self %}
   neighbor {{ ip }} next-hop-self{% if n.type == 'localas_ibgp' %} all{% endif +%}
 {%   endif %}
 {%   if bgp.rr|default('') and (not n.rr|default('') or n.type == 'localas_ibgp') %}
   neighbor {{ ip }} route-reflector-client
 {%   endif %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 !
 router bgp {{ bgp.as }}
 {% for vname,vdata in vrfs.items() %}
 {%   for af in ('ipv4','ipv6') if af in vdata.af|default({}) %}
  address-family {{ af }} vrf {{ vname }}
   bgp router-id {{ vdata.bgp.router_id|default(bgp.router_id) }}
   redistribute connected
-{%     if af == 'ipv4' and 'ospf' in vdata %}
+{%     if 'ospf' in vdata %}
   redistribute ospf {{ vdata.vrfidx }}
 {%     endif %}
 !
 {%     for n in vdata.networks|default([]) if af in n %}
 {{       bgpcfg.bgp_network(af,n[af]) }}
 {%     endfor %}
 !
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,20 @@
     }
     term redis_ospf {
       from {
         protocol ospf;
       }
       then accept;
     }
+    term redis_ospf3 {
+      from {
+        protocol ospf3;
+      }
+      then accept;
+    }
 {%   if bgp.next_hop_self is defined and bgp.next_hop_self %}
     term next-hop-self {
       from {
         route-type external;
       }
       then {
         next-hop self;
@@ -38,14 +44,20 @@
     }
     term redis_ospf {
       from {
         protocol ospf;
       }
       then accept;
     }
+    term redis_ospf3 {
+      from {
+        protocol ospf3;
+      }
+      then accept;
+    }
   }
 
 {% endfor %}
 }
 
 {# apply VRF BGP & routing settings #}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/junos.j2`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,50 @@
-{% set KW_NETWORK_TYPE = {'point-to-point': 'p2p','point-to-multipoint': 'p2mp', 'non-broadcast': 'nbma' } %}
+{% import "junos.ospf-macro.j2" as ospf_cfg %}
+{% if bgp.as is defined %}
+{% include 'junos.bgp.j2' %}
+{% endif %}
 
+{% for vname,vdata in vrfs.items() if 'ospf' in vdata %}
+{# 
+   generic policy to redistribute bgp + leaked(imported) into ospf
+#}
+{% if vdata.ospf.router_id is defined and vdata.ospf.router_id|ipv4 %}
 routing-instances {
-  {{vname}} {
-    protocols {
-      ospf {
-        export vrf-{{vname}}-ospf-export;
+  {{ vname }} {
+    routing-options {
+      router-id {{ vdata.ospf.router_id }}
+    }
+  }
+}
+{% endif %}
+{% set ns = namespace(import_list=[]) %}
+{%   for i in vdata.import|default([]) %}
+{{ ns.import_list.append('tg_'+i|replace(':', '_')|replace('.', '_')) }}
+{%   endfor %}
 
-{% for l in vdata.ospf.interfaces|default([]) %}
-        area {{ l.ospf.area }} {
-          interface {{ l.ifname }} {
-{%   if l.ospf.network_type is defined and l.ospf.network_type != 'broadcast' %}
-            interface-type {{ KW_NETWORK_TYPE[l.ospf.network_type] }};
-{%   endif %}
-{%   if l.ospf.passive|default(False) or l.type|default('') == 'loopback' %}
-            passive;
-{%   endif %}
-{%   if l.ospf.cost is defined %}
-            metric {{ l.ospf.cost }};
-{%   endif %}
-{%   if l.ospf.bfd|default(False) %}
-            bfd-liveness-detection {
-              minimum-receive-interval {{ l.bfd.min_rx|default(bfd.min_rx)|default(500) }};
-              multiplier {{ l.bfd.multiplier|default(bfd.multiplier)|default(3) }};
-              transmit-interval {
-                minimum-interval {{ l.bfd.min_tx|default(bfd.min_tx)|default(500) }};
-              }
-            }
-{%   endif %}
-          }
-        }
-{% endfor %}
+policy-options {
+  policy-statement vrf-{{vname}}-ospf-export {
+    term redis_direct {
+      from {
+        protocol direct;
+      }
+      then accept;
+    }
+    term redis_bgp {
+      from protocol bgp;
+      then {
+        accept;
       }
     }
+    term redis_local_target {
+      from community [ {{ ns.import_list|join(' ') }} ];
+      then accept;
+    }
   }
 }
+{%   if vdata.af.ipv4|default(False) %}
+{{     ospf_cfg.config('ospf',vname,vdata.ospf,vdata.ospf.interfaces|default([]),bgp|default({})) }}
+{%   endif %}
+{%   if vdata.af.ipv6|default(False) %}
+{{     ospf_cfg.config('ospf3',vname,vdata.ospf,vdata.ospf.interfaces|default([]),bgp|default({})) }}
+{%   endif %}
+{% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,32 @@
-!
-route-map all
-!
-{% set pid = vdata.vrfidx %}
-feature ospf
-{% if vdata.ospf.bfd|default(False) %}
-feature bfd
+
+{% if vdata.ospf.router_id|ipv4 or ospf.router_id|ipv4 %}
+set protocols ospf parameters router-id {{ vdata.ospf.router_id|default(ospf.router_id) }}
 {% endif %}
-!
-router ospf {{ pid }}
- vrf {{ vname }}
-{% if vdata.ospf.router_id|ipv4 %}
-  router-id {{ vdata.ospf.router_id }}
+
+set protocols ospf redistribute connected
+{% if bgp.as is defined %}
+set protocols ospf redistribute bgp
 {% endif %}
+
 {% if ospf.reference_bandwidth is defined %}
-  auto-cost reference-bandwidth {{ ospf.reference_bandwidth }} Mbps
-{% endif %}
-!
-{% if bgp.as is defined %}
-  redistribute bgp {{ bgp.as }} route-map all
+set protocols ospf auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
 {% endif %}
-!
-{% for l in vdata.ospf.interfaces|default([]) %}
-interface {{ l.ifname }}
-! {{ l.name|default("") }}
- ip router ospf {{ pid }} area {{ l.ospf.area }}
-{%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
- ip ospf network {{ l.ospf.network_type }}
+
+{% for l in vdata.ospf.interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
+
+set protocols ospf interface {{ l.ifname }} area {{ l.ospf.area }}
+
+{%   if l.ospf.passive|default(False) %}
+set protocols ospf interface {{ l.ifname }} passive
 {%   endif %}
-{%   if l.ospf.cost is defined %}
- ip ospf cost {{ l.ospf.cost }}
+{%   if l.ospf.network_type is defined %}
+set protocols ospf interface {{ l.ifname }} network {{ l.ospf.network_type }}
 {%   endif %}
-{%   if l.ospf.passive|default(False) %}
- ip ospf passive-interface
+{%   if l.ospf.cost is defined %}
+set protocols ospf interface {{ l.ifname }} cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
- ip ospf bfd
+set protocols ospf interface {{ l.ifname }} bfd
 {%   endif %}
-!
+
 {% endfor %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.8.1/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.8.1/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,46 @@
-
-{% if vdata.ospf.router_id|ipv4 or ospf.router_id|ipv4 %}
-set protocols ospf parameters router-id {{ vdata.ospf.router_id|default(ospf.router_id) }}
-{% endif %}
-
-set protocols ospf redistribute connected
-{% if bgp.as is defined %}
-set protocols ospf redistribute bgp
-{% endif %}
-
-{% if ospf.reference_bandwidth is defined %}
-set protocols ospf auto-cost reference-bandwidth {{ ospf.reference_bandwidth }}
-{% endif %}
-
-{% for l in vdata.ospf.interfaces|default([]) if 'ospf' in l and 'ipv4' in l %}
-
-set protocols ospf interface {{ l.ifname }} area {{ l.ospf.area }}
-
-{%   if l.ospf.passive|default(False) %}
-set protocols ospf interface {{ l.ifname }} passive
-{%   endif %}
-{%   if l.ospf.network_type is defined %}
-set protocols ospf interface {{ l.ifname }} network {{ l.ospf.network_type }}
+{% macro config(ospf_pid,ospf_vrf,ospf_data,intf_data,bgp={}) %}
+!
+! OSPFv3 configuration
+!
+{% for l in intf_data if 'ospf' in l and 'ipv6' in l %}
+interface {{ l.ifname }}
+! {{ l.name|default("") }}
+ ipv6 ospf {{ ospf_pid }} area {{ l.ospf.area }}
+{%   if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
+{%     if l.ospf.network_type == "broadcast" %}
+ no ipv6 ospf network
+{%     else %}
+ ipv6 ospf network {{ l.ospf.network_type }}
+{%     endif %}
 {%   endif %}
 {%   if l.ospf.cost is defined %}
-set protocols ospf interface {{ l.ifname }} cost {{ l.ospf.cost }}
+ ipv6 ospf cost {{ l.ospf.cost }}
 {%   endif %}
 {%   if l.ospf.bfd|default(False) %}
-set protocols ospf interface {{ l.ifname }} bfd
+ ipv6 ospf bfd
 {%   endif %}
-
+!
+{% endfor %}
+!
+{% if ospf_vrf %}}
+ipv6 router ospf {{ ospf_pid }} vrf {{ ospf_vrf }}
+{% else %}
+ipv6 router ospf {{ ospf_pid }}
+{% endif %}
+ router-id {{ ospf_data.router_id }}
+ timers spf delay initial 100 200 500
+ timers lsa rx min interval 100
+ timers lsa tx delay initial 100 200 500
+{% if ospf_data.reference_bandwidth is defined %}
+ auto-cost reference-bandwidth {{ ospf_data.reference_bandwidth }}
+{% endif %}
+{% if ospf_vrf %}
+{%   if bgp.as is defined %}
+ redistribute bgp include leaked
+{%   endif %}
+ redistribute connected
+{% endif %}
+{% for l in intf_data if l.ospf.passive|default(False) %}
+ passive-interface {{ l.ifname }}
 {% endfor %}
+{% endmacro %}
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.8.1/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.8.1/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.8.1/netsim/ansible/templates/vxlan/frr.j2`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,14 @@
 {% if vxlan.vlans is defined %}
 {%   for vname in vxlan.vlans if vlans[vname].vni is defined %}
 {%     set vlan = vlans[vname] %}
 # Create VXLAN L2 interface per vni
 {{ create_vxlan_interface(vlan.vni, "vlan" + vlan.id|string,None,max_mtu) }}
 {%     if vlan.vtep_list is defined %}
 {%       for remote_vtep in vlan.vtep_list %}
-ip link set vxlan{{vlan.vni}} type vxlan remote {{ remote_vtep }}
+bridge fdb append 00:00:00:00:00:00 dev vxlan{{vlan.vni}} dst {{ remote_vtep }}
 {%       endfor %}
 {%     endif %}
 {%   endfor %}
 {% endif %}
 
 exit $?
```

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.8.1/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.8.1/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.8.1/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.8.1/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/api/__init__.py` & `networklab-1.8.1/netsim/api/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/addressing.py` & `networklab-1.8.1/netsim/augment/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/components.py` & `networklab-1.8.1/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/config.py` & `networklab-1.8.1/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/devices.py` & `networklab-1.8.1/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/groups.py` & `networklab-1.8.1/netsim/augment/groups.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/links.py` & `networklab-1.8.1/netsim/augment/links.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/main.py` & `networklab-1.8.1/netsim/augment/main.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/nodes.py` & `networklab-1.8.1/netsim/augment/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,15 @@
     if n.get('role','') != 'host':
       lbname = devices.get_loopback_name(n,topology)
       if lbname:
         n.loopback.ifname = lbname
         n.loopback.ifindex = 0
         n.loopback.type = 'loopback'
         n.loopback.neighbors = []
+        n.loopback.virtual_interface = True
 
     augment_mgmt_if(n,defaults,topology.addressing.mgmt)
     providers.execute_node("augment_node_data",n,topology)
 
 '''
 Final cleanup of node data
 '''
```

### Comparing `networklab-1.8.0.post2/netsim/augment/plugin.py` & `networklab-1.8.1/netsim/augment/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/tools.py` & `networklab-1.8.1/netsim/augment/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/topology.py` & `networklab-1.8.1/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/augment/validate.py` & `networklab-1.8.1/netsim/augment/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/__init__.py` & `networklab-1.8.1/netsim/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,22 +135,26 @@
 
 def load_snapshot_or_topology(args: typing.Union[argparse.Namespace,Box]) -> typing.Optional[Box]:
   log.set_logging_flags(args)
   if args.device or args.provider or args.settings:     # If we have -d, -p or -s flag
     if not args.topology:                               # ... then the user wants to use the topology file
       args.topology = 'topology.yml'                    # ... so let's set the default value if needed
 
+  topology = None
   if args.topology:
     topology = load_topology(args)
     augment.main.transform(topology)
     log.exit_on_error()
-    return topology
   else:
     args.snapshot = args.snapshot or 'netlab.snapshot.yml'
-    return _read.read_yaml(filename=args.snapshot)
+    topology = _read.read_yaml(filename=args.snapshot)
+
+  if topology:
+    global_vars.init(topology)
+  return topology
 
 # get_message: get action-specific message from topology file
 #
 
 def get_message(topology: Box, action: str, default_message: bool = False) -> typing.Optional[str]:
   global DRY_RUN
   if not 'message' in topology or DRY_RUN:
@@ -184,43 +188,56 @@
   if not lab_id in status:
     status[lab_id].dir = os.getcwd()                        # Map lab ID into current directory
   if not 'providers' in status[lab_id]:                     # Initialize provider list
     status[lab_id].providers = []
 
   if update is not None:                                    # Update lab status from a dictionary
     status[lab_id] = status[lab_id] + update
-    if 'status' in update:                                  # Append change in lab status to log        
+    if 'status' in update:                                  # Append change in lab status to log
+      update['log_line'] = update['status']
+
+    if 'log_line' in update:
       if not 'log' in status[lab_id]:                       # Create empty log if needed
         status[lab_id].log = []
 
       # Append status change to log if it's not a duplicate of the last entry
       # This is to avoid excessive log entries when the status is updated multiple times
       # in a row (e.g. when a lab is being created)
       #
-      if not status[lab_id].log or not f': {update["status"]}' in status[lab_id].log[-1]:
+      if not status[lab_id].log or not f': {update["log_line"]}' in status[lab_id].log[-1]:
         timestamp = datetime.datetime.now(datetime.timezone.utc).astimezone().isoformat()
-        status[lab_id].log.append(f'{timestamp}: {update["status"]}')
+        status[lab_id].log.append(f'{timestamp}: {update["log_line"]}')
 
   if cb is not None:                                        # If needed, perform status-specific callback        
     cb(status[lab_id])
 
 """
 lab_status_change -- change current lab status
 """
 def lab_status_change(topology: Box, new_status: str) -> None:
   global DRY_RUN
   if DRY_RUN:                                              # Don't update status if we're in dry-run mode 
     return
 
   _status.change_status(
     topology,
-    callback = lambda s,t: 
+    callback = lambda s,t:
       lab_status_update(t,s,
         update = { 'status': new_status }))
 
+"""
+lab_status_log -- change current lab status
+"""
+def lab_status_log(topology: Box, log_line: str) -> None:
+  _status.change_status(
+    topology,
+    callback = lambda s,t:
+      lab_status_update(t,s,
+        update = { 'log_line': log_line }))
+
 #
 # Main command dispatcher
 #
 # The command to execute is the first CLI argument. We try to load a module with the same name
 # and if the module load fails for whatever reason we generate an error and exit.
 #
 # However, the module load could fail due to coding errors within the module (not because the module
```

### Comparing `networklab-1.8.0.post2/netsim/cli/ansible.py` & `networklab-1.8.1/netsim/cli/ansible.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import subprocess
 import sys
 import os
 import json
 from pathlib import Path
 
 from ..utils import log
+from . import external_commands
 
 try:
   from importlib import resources
 except ImportError:
   import importlib_resources as resources # type: ignore
 
 def find_playbook(name: str) -> typing.Union[str,None]:
@@ -50,11 +51,10 @@
 
   if log.VERBOSE:
     print("Running Ansible playbook %s" % pbname)
 
   cmd = ['ansible-playbook',pbname]
   cmd.extend(args)
 
-  try:
-    subprocess.check_call(cmd)
-  except Exception as ex:
-    log.fatal(f"Executing Ansible playbook {pbname} failed:\n  {ex}")
+  OK = external_commands.run_command(cmd)
+  if not OK:
+    log.fatal(f"Executing Ansible playbook {pbname} failed")
```

### Comparing `networklab-1.8.0.post2/netsim/cli/clab.py` & `networklab-1.8.1/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/clab_actions/build.py` & `networklab-1.8.1/netsim/cli/clab_actions/build.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/clab_actions/tarball.py` & `networklab-1.8.1/netsim/cli/clab_actions/tarball.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/collect.py` & `networklab-1.8.1/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/config.py` & `networklab-1.8.1/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/connect.py` & `networklab-1.8.1/netsim/cli/connect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/create.py` & `networklab-1.8.1/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/down.py` & `networklab-1.8.1/netsim/cli/down.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     '--dry-run',
     dest='dry_run',
     action='store_true',
     help='Print the commands that would be executed, but do not execute them')
   parser.add_argument(
     '--force',
     dest='force',
-    action='store_true',
+    action='count', default = 0,
     help='Force shutdown or cleanup (use at your own risk)')
   parser.add_argument(
     '--snapshot',
     dest='snapshot',
     action='store',
     nargs='?',
     default='netlab.snapshot.yml',
@@ -103,22 +103,25 @@
   p_module.call('pre_stop_lab',p_topology)
   external_commands.stop_lab(topology.defaults,p_name,"netlab down",exec_command)
   p_module.call('post_stop_lab',p_topology)
 
 '''
 lab_dir_mismatch -- check if the lab instance is running in the current directory
 '''
-def lab_dir_mismatch(topology: Box) -> bool:
+def lab_dir_mismatch(topology: Box, args: argparse.Namespace) -> bool:
   lab_id = status.get_lab_id(topology)
   lab_status = status.read_status(topology)       # Find current running instance(s)
   if not lab_id in lab_status:                    # This could be a lab instance from pre-status days
     return False                                  # ... in which case we can shut it down
   if lab_id in lab_status and lab_status[lab_id].dir == os.getcwd():
     return False                                 # Lab instance is known  and this is the correct directory        
 
+  if args.force >= 2:
+    return True
+
   print(f'''
 According to the netlab status file, the lab instance '{lab_id}' is running
 in directory {lab_status[lab_id].dir}.
 
 You could proceed if you want to clean up the netlab artifacts from this
 directory, but you might impact the running lab instance.
 ''')
@@ -173,17 +176,18 @@
 def run(cli_args: typing.List[str]) -> None:
   args = down_parse(cli_args)
   set_dry_run(args)
 
   topology = load_snapshot(args)
   print(f"Read transformed lab topology from snapshot file {args.snapshot}")
 
-  mismatch = lab_dir_mismatch(topology)
+  mismatch = lab_dir_mismatch(topology,args)
 
   probes_OK = True
+  external_commands.LOG_COMMANDS = True
   lab_status_change(topology,f'lab shutdown requested{" in conflicting directory" if mismatch else ""}')
   try:
     provider_probes(topology)
   except:
     probes_OK = False
     if not args.force:
       return
```

### Comparing `networklab-1.8.0.post2/netsim/cli/external_commands.py` & `networklab-1.8.1/netsim/cli/external_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # Run external commands from netlab CLI
 #
 import typing
 import os
 import subprocess
 from box import Box
 
-from . import is_dry_run
+from . import is_dry_run,lab_status_log
 from ..utils import strings,log
+from ..data import global_vars
 
 def print_step(n: int, txt: str, spacing: typing.Optional[bool] = False) -> None:
   if spacing:
     print()
   print("Step %d: %s" % (n,txt))
   print("=" * 72)
 
@@ -44,14 +45,29 @@
 run_command: Execute an external command specified as a string or a list of CLI parameters
 
 Flags:
 * check_result -- return False if the command does not produce any output
 * ignore_errors -- do not print errors to the console
 * return_stdout -- return the command output instead of True/False
 """
+LOG_COMMANDS: bool = False
+
+def log_command(cmd: typing.Union[str,list], status: str) -> None:
+  global LOG_COMMANDS
+  if not LOG_COMMANDS:
+    return
+
+  topology = global_vars.get_topology()
+  if not topology:
+    log.fatal('Internal error: topology not set',module='log_command')
+    return
+
+  cmd_text = cmd if isinstance(cmd,str) else ' '.join(cmd)
+  lab_status_log(topology,f'{status}: {cmd_text}')
+
 def run_command(
     cmd : typing.Union[str,list],
     check_result : bool = False,
     ignore_errors: bool = False,
     return_stdout: bool = False) -> typing.Union[bool,str]:
 
   if log.debug_active('cli'):
@@ -73,19 +89,24 @@
     return True
 
   try:
     result = subprocess.run(cmd,capture_output=check_result,check=True,text=True)
     if log.debug_active('external') or log.VERBOSE >= 3:
       print(f'... run result: {result}')
     if not check_result:
+      log_command(cmd,'OK')
       return True
     if return_stdout:
+      log_command(cmd,'OK')
       return result.stdout
+
+    log_command(cmd,'OK' if result.stdout != "" else 'FAIL')
     return result.stdout != ""
   except Exception as ex:
+    log_command(cmd,'ERROR')
     if not log.QUIET and not ignore_errors:
       print(f"Error executing {stringify(cmd)}:\n  {ex}")
     return False
 
 def test_probe(p : typing.Union[str,list,Box],quiet : bool = False) -> bool:
   if isinstance(p,str):
     return bool(run_command(p,check_result=True,ignore_errors=quiet))
@@ -197,18 +218,31 @@
 def docker_is_used(topology: Box) -> bool:
   if topology.provider == 'clab':
     return True
 
   return 'clab' in topology[topology.provider].providers
 
 #
+# Get local IP address, either the endpoint of the SSH connection or loopback
+#
+def get_local_addr() -> str:
+  ssh_connection = os.environ.get("SSH_CONNECTION")
+  if ssh_connection:
+    ssh_list = ssh_connection.split(" ")
+    if len(ssh_list) >= 4:
+      return ssh_list[2]
+    
+  return "127.0.0.1"
+
+#
 # Execute external tool commands
 #
 def execute_tool_commands(cmds: list, topology: Box) -> None:
   topology.sys.docker_net = ""
+  topology.sys.ipaddr = get_local_addr()
   if docker_is_used(topology):
     topology.sys.docker_net = f"--network={topology.addressing.mgmt.get('_network',None) or 'netlab_mgmt'}"
 
   for cmd in cmds:
     cmd = strings.eval_format(cmd,topology)
     run_command(cmd = [ 'bash', '-c', cmd ],check_result=True)
```

### Comparing `networklab-1.8.0.post2/netsim/cli/graph.py` & `networklab-1.8.1/netsim/cli/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     nargs='?',
     default='netlab.snapshot.yml',
     const='netlab.snapshot.yml',
     help='Transformed topology snapshot file')
   parser.add_argument(
     '-t','--type',
     dest='g_type', action='store',
-    choices=['topology,bgp'],
+    choices=['topology','bgp'],
     help='Graph type')
   parser.add_argument(
     '-e','--engine',
     dest='engine', action='store',
     default='graphviz',
     choices=['graphviz','d2'],
     help='Graphing engine')
```

### Comparing `networklab-1.8.0.post2/netsim/cli/initial.py` & `networklab-1.8.1/netsim/cli/initial.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # Deploys initial device configurations
 #
 import typing
 import os
 import argparse
 
 from . import common_parse_args,get_message,load_snapshot_or_topology,lab_status_change
+from . import external_commands
 from . import ansible
+from ..utils import status as _status
 from box import Box
 
 #
 # CLI parser for 'netlab initial' command
 #
 def initial_config_parse(args: typing.List[str]) -> typing.Tuple[argparse.Namespace, typing.List[str]]:
   parser = argparse.ArgumentParser(
@@ -82,18 +84,23 @@
   if args.logging or args.verbose:
     print("Ansible playbook args: %s" % rest)
 
   if args.output:
     ansible.playbook('create-config.ansible',rest)
     print("\nInitial configurations have been created in the %s directory" % args.output)
   else:
+    external_commands.LOG_COMMANDS = True
+
     topology = load_snapshot_or_topology(Box({},default_box=True,box_dots=True))
     deploy_text = ', '.join(deploy_parts) or 'complete configuration'
     if not topology is None:
       lab_status_change(topology,f'deploying configuration: {deploy_text}')
 
     ansible.playbook('initial-config.ansible',rest)
     if topology and not args.no_message:
       message = get_message(topology,'initial',True)
       if message:
         print(f"\n\n{message}")
       lab_status_change(topology,f'configuration deployment complete')
+
+  if _status.is_directory_locked():                   # If we're using the lock file, touch it after we're done
+    _status.lock_directory()                          # .. to have a timestamp of when the lab was started
```

### Comparing `networklab-1.8.0.post2/netsim/cli/inspect.py` & `networklab-1.8.1/netsim/cli/inspect.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from box import Box
 
 from . import load_snapshot
 from ..outputs import _TopologyOutput
 from ..outputs import common as outputs_common
 from ..utils import strings,log
+from ..data.types import must_be_id
+from ..data import global_vars
 
 #
 # CLI parser for 'netlab inspect' command
 #
 def inspect_parse(args: typing.List[str]) -> argparse.Namespace:
   parser = argparse.ArgumentParser(
     prog="netlab inspect",
@@ -52,14 +54,22 @@
   topology = load_snapshot(args)
 
   o_module = args.format or 'yaml'
   o_param  = f'{o_module}:{args.expr or "."}'
   inspect_module = _TopologyOutput.load(o_param,topology.defaults.outputs[o_module])
 
   if args.node:
+    log.init_log_system(False)
+    must_be_id(
+      parent=None,
+      key=args.node,
+      path=f'NOATTR:--node parameter',
+      max_length=global_vars.get_const('MAX_NODE_ID_LENGTH',16),
+      module='inspect')
+    log.exit_on_error()
     if args.node in topology.nodes:
       topology = outputs_common.adjust_inventory_host(
                 node=topology.nodes[args.node],
                 defaults=topology.defaults,
                 group_vars=True)
     else:
       log.fatal(
```

### Comparing `networklab-1.8.0.post2/netsim/cli/install.py` & `networklab-1.8.1/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/libvirt.py` & `networklab-1.8.1/netsim/cli/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/read.py` & `networklab-1.8.1/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/report.py` & `networklab-1.8.1/netsim/cli/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/restart.py` & `networklab-1.8.1/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show-usage.txt` & `networklab-1.8.1/netsim/cli/show-usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show.py` & `networklab-1.8.1/netsim/cli/show.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,10 +105,13 @@
   topology.name = 'empty'
 #  topology.nodes = data.get_empty_box()
   topology.nodes.dummy.device = 'none'                  # Add a dummy node
   topology.nodes.dummy.module = []                      # ... and disable all modules on that node
   if 'plugin' in args and args.plugin:
     topology.plugin = args.plugin
 
+  if args.action in ['defaults']:                       # Save original paths for the "show defaults" command
+    topology.defaults._original_paths = data.get_box(topology.defaults.paths)
+
   main.transform_setup(topology)
   settings = topology.defaults
   show_dispatch[args.action]['exec'](settings,args)
```

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/__init__.py` & `networklab-1.8.1/netsim/cli/show_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/attributes.py` & `networklab-1.8.1/netsim/cli/show_commands/attributes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/devices.py` & `networklab-1.8.1/netsim/cli/show_commands/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/images.py` & `networklab-1.8.1/netsim/cli/show_commands/images.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/module_support.py` & `networklab-1.8.1/netsim/cli/show_commands/module_support.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/modules.py` & `networklab-1.8.1/netsim/cli/show_commands/modules.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/outputs.py` & `networklab-1.8.1/netsim/cli/show_commands/outputs.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/providers.py` & `networklab-1.8.1/netsim/cli/show_commands/providers.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/show_commands/reports.py` & `networklab-1.8.1/netsim/cli/show_commands/reports.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/test.py` & `networklab-1.8.1/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/up.py` & `networklab-1.8.1/netsim/cli/up.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from . import create
 from . import external_commands, set_dry_run, is_dry_run
 from . import common_parse_args, get_message
 from . import lab_status_update, lab_status_change
 from .. import providers
 from ..utils import log,strings,status as _status, read as _read
+from ..data import global_vars
 
 #
 # Extra arguments for 'netlab up' command
 #
 def up_parse_args(standalone: bool) -> argparse.ArgumentParser:
   parse_parents = [ common_parse_args() ] if standalone else []
   parser = argparse.ArgumentParser(
@@ -57,14 +58,19 @@
   parser.add_argument(
     '--snapshot',
     dest='snapshot',
     action='store',
     nargs='?',
     const='netlab.snapshot.yml',
     help='Use netlab snapshot file created by a previous lab run')
+  parser.add_argument(
+    '--validate',
+    dest='validate',
+    action='store_true',
+    help=argparse.SUPPRESS)
   return parser
 
 """
 Get lab topology from the snapshot file or run the transformation process
 """
 def get_topology(args: argparse.Namespace, cli_args: typing.List[str]) -> Box:
   up_args_parser = up_parse_args(bool(args.snapshot))         # (re)create the correct parser
@@ -74,14 +80,15 @@
     log.set_logging_flags(args)                               # ... use these arguments to set logging flags and read the snapshot
 
     topology = _read.read_yaml(filename=args.snapshot)
     if topology is None:
       log.fatal(f'Cannot read snapshot file {args.snapshot}, aborting...')
 
     print(f"Using transformed lab topology from snapshot file {args.snapshot}")
+    global_vars.init(topology)    
   else:                                                       # No snapshot file, use 'netlab create' parser
     log.section_header('Creating','configuration files')
     topology = create.run(cli_args,'up','Create configuration files, start a virtual lab, and configure it',up_args_parser)
 
   return topology
 
 """
@@ -299,14 +306,15 @@
   if not is_dry_run():
     check_lab_instance(topology)
 
   settings = topology.defaults
   if log.QUIET:
     os.environ["ANSIBLE_STDOUT_CALLBACK"] = "selective"
 
+  external_commands.LOG_COMMANDS = True
   provider_probes(topology)
 
   p_provider = topology.provider
   p_module = providers._Provider.load(p_provider,topology.defaults.providers[p_provider])
   providers.mark_providers(topology)
   p_module.call('pre_output_transform',topology)
 
@@ -330,8 +338,14 @@
   else:
     deploy_initial_config(args,topology)
   start_external_tools(args,topology)
   lab_status_change(topology,'started')
   if _status.is_directory_locked():                   # If we're using the lock file, touch it after we're done
     _status.lock_directory()                          # .. to have a timestamp of when the lab was started
 
-  log.repeat_warnings('netlab up')
+  log.repeat_warnings('netlab up')
+
+  if args.validate:
+    if args.no_config:
+      log.error('Lab is not configured, skipping the validation phase',Warning,'')
+    else:
+      external_commands.run_command('netlab validate')
```

### Comparing `networklab-1.8.0.post2/netsim/cli/usage.txt` & `networklab-1.8.1/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/cli/validate.py` & `networklab-1.8.1/netsim/cli/validate.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import traceback
 
 from box import Box
 
 from . import load_snapshot,parser_add_debug,parser_add_verbose
 from ..utils import log,templates,strings,status as _status, files as _files
 from ..data import global_vars
+from ..augment import devices
 from .. import data
 from .connect import connect_to_node,LogLevel
 
 #
 # CLI parser for 'netlab validate' command
 #
 def validate_parse(args: typing.List[str]) -> argparse.Namespace:
@@ -47,20 +48,40 @@
     dest='nodes', action='store',
     help='Execute validation tests only on selected node(s)')
   parser.add_argument(
     '--skip-wait',
     dest='nowait', action='store_true',
     help='Skip the waiting period')
   parser.add_argument(
+    '-e','--error-only',
+    dest='error_only', action='store_true',
+    help='Display only validation errors (on stderr)')
+  parser.add_argument(
+    '--skip-missing',
+    dest='skip_missing', action='store_true',
+    help=argparse.SUPPRESS)
+  parser.add_argument(
+    '--dump',
+    action='store',
+    choices=['result'],
+    nargs='+',
+    default=[],
+    help='Dump additional information during validation process')
+  parser.add_argument(
     dest='tests', action='store',
     nargs='*',
     help='Validation test(s) to execute (default: all)')
 
   return parser.parse_args(args)
 
+# I'm cheating. Declaring a global variable is easier than passing 'args' argument around
+#
+ERROR_ONLY: bool = False
+TEST_HEADER: dict = {}
+
 '''
 list_tests: display validation tests defined for the current lab topology
 '''
 def list_tests(topology: Box) -> None:
   heading = [ 'Test','Description','Nodes','Devices' ]
   rows = [
     [ v_entry.name,
@@ -72,41 +93,62 @@
 
 # The following routines print colored test status and offer
 # various levels of abstraction, from "give me a colored text"
 # to "tell the user the lab was a great success"
 
 # Prints test status (colored text in fixed width)
 #
-def p_status(txt: str, color: str, topology: Box) -> None:
+def p_status(txt: str, color: str, topology: Box, stderr: bool = False) -> None:
   txt = f'[{txt}]{" " * 80}'[:topology._v_len+3]
-  strings.print_colored_text(txt,color)
+  strings.print_colored_text(txt,color,stderr=stderr)
 
 # Print test header
 #
 def p_test_header(v_entry: Box,topology: Box) -> None:
+  global TEST_HEADER
+  h_text = v_entry.get('description','Starting test') + \
+           (f' [ node(s): {",".join(v_entry.nodes)} ]' if v_entry.nodes else '')
+
+  if ERROR_ONLY:
+    TEST_HEADER = { 'name': v_entry.name, 'text': h_text }
+    return
+
   p_status(v_entry.name,"bright_cyan",topology)
-  print(
-    v_entry.get('description','Starting test') + \
-    (f' [ node(s): {",".join(v_entry.nodes)} ]' if v_entry.nodes else ''))
+  print(h_text)
 
 # Print generic "test failed" message
 #
 def log_failure(msg: str, topology: Box, f_status: str = 'FAIL') -> None:
-  p_status(f_status,'bright_red',topology)
-  print(msg)
+  global TEST_HEADER,ERROR_ONLY
+  if TEST_HEADER:
+    print(file=sys.stderr)
+    p_status(TEST_HEADER['name'],'red',topology,stderr=True)
+    print(TEST_HEADER['text'],file=sys.stderr)
+    TEST_HEADER = {}
+
+  p_status(f_status,'bright_red',topology,stderr=ERROR_ONLY)
+  print(msg,file=sys.stderr if ERROR_ONLY else sys.stdout)
 
 # Print generic "making progress" message
 #
 def log_progress(msg: str, topology: Box, f_status: str = 'PASS') -> None:
+  global ERROR_ONLY
+  if ERROR_ONLY:
+    return
+
   p_status(f_status,'light_green',topology)
   print(msg)
 
 # Print generic "ambivalent info" message
 #
 def log_info(msg: str, topology: Box, f_status: str = 'INFO') -> None:
+  global ERROR_ONLY
+  if ERROR_ONLY:
+    return
+
   p_status(f_status,'yellow',topology)
   print(msg)
 
 # Print "test failed on node"
 #
 def p_test_fail(n_name: str, v_entry: Box, topology: Box) -> None:
   err = v_entry.get('fail','')
@@ -118,14 +160,51 @@
 def p_test_pass(v_entry: Box, topology: Box) -> None:
   msg = v_entry.get('pass','Test succeeded')
   log_progress(msg,topology)
 
 _validation_plugins: dict = {}
 
 '''
+extend_first_wait_time: some devices need extra time to start working, even when
+the configuration process has completed. Assuming we can't (or don't want to)
+catch that during the device readiness check, we should add extra delay to the
+validation process.
+
+This function walks through the lab nodes, checks the features.initial.delay of
+each device, and adds the maximum delay to the first 'wait' parameter.
+'''
+
+def extend_first_wait_time(args: argparse.Namespace, topology: Box) -> None:
+  max_delay = 0
+  d_device  = None
+  for n_data in topology.nodes.values():
+    d_features = devices.get_device_features(n_data,topology.defaults)
+    d_delay = d_features.get('initial.delay',None)
+    if not d_delay:
+      continue
+    if d_delay > max_delay:                                           # Found a device that requires a delay
+      max_delay = d_delay                                             # ... take the max value of the delay
+      d_device  = n_data.device                                       # ... and remember the device causing it
+
+  if not max_delay:                                                   # No slow devices in lab topology, exit
+    return
+
+  for v_entry in topology.validate:
+    if not v_entry.get('wait',0):                                     # No wait associated with this entry, move on
+      continue
+
+    v_entry.wait = v_entry.wait + max_delay
+    if not args.error_only:
+      log.error(
+        f'Initial wait time extended by {max_delay} seconds required by {d_device}',
+        category=Warning,
+        module='')
+    return
+
+'''
 load_plugin: try to load the validation plugin for the specified device
 '''
 
 def load_plugin(device: str) -> typing.Any:
   topology = global_vars.get_topology()
   if topology is None:                                                # Abort if we can't get a point to the topology
     return None
@@ -213,14 +292,15 @@
   exec_data = data.get_box(global_vars.get_topology() or {}) + v_entry.vars
   exec_data.node = node
 
   plugin = find_plugin(node.device)               # Find device-specific validation plugin
   if plugin is None:                              # Not found, the test is skipped
     return None
   plugin._result = result
+  global_vars.set_result_dict('_result',result or Box({}))
   exec_data[p_name] = plugin
 
   try:
     return eval(exec,{},exec_data)
   except AttributeError as ex:
     if p_name in str(ex):
       return None
@@ -235,15 +315,15 @@
 * If the validation entry is a dictionary, use device-specific item
 * If the result of the above is not a string we have a failure, get out
 * If the resulting string contains '{{' run it through Jinja2 engine
 
 If we try to get the string to pass to the device from a plugin, then any
 plugin evaluation errors indicate something is badly broken, so we log the
 error with as much data as feasible... and if the end-user ever sees that
-error message, the author of the validation plugin did a lousy job ¯\_(ツ)_/¯
+error message, the author of the validation plugin did a lousy job.
 '''
 def get_entry_value(v_entry: Box, action: str, node: Box, topology: Box) -> typing.Any:
   n_device = node.device
   if action in v_entry:
     value = v_entry[action][n_device] if isinstance(v_entry[action],dict) else v_entry[action]
   elif 'plugin' in v_entry:
     try:
@@ -301,15 +381,15 @@
     return err_value
 
   if verbosity >= 3:                                        # Extra-verbose: print command to execute
     print(f'Preparing to execute {v_cmd}')
 
   # Set up arguments for the 'netlab connect' command and execute it
   #
-  args = argparse.Namespace(quiet=True,host=n_name,output=True,show=v_cmd)
+  args = argparse.Namespace(quiet=True,host=n_name,output=True,show=v_cmd,verbose=False)
   result = connect_to_node(args=args,rest=[],topology=topology,log_level=LogLevel.NONE)
 
   if verbosity >= 3:                                        # Extra-verbose: print the results we got
     print(f'Executed {v_cmd} got {result}')
 
   # If the result we got back is not a string, the 'netlab connect' command
   # failed in one way or another
@@ -329,58 +409,69 @@
       f'Failed to parse result output of "{" ".join(v_cmd)}" on {n_name} (device {node.device}) as JSON',
       topology=topology)
     return err_value
 
 '''
 Execute a command on the device and return stdout
 '''
-def get_result_string(v_entry: Box, n_name: str, topology: Box) -> typing.Union[bool,str]:
+def get_result_string(
+      v_entry: Box,
+      n_name: str,
+      topology: Box,
+      report_error: bool = True) -> typing.Union[bool,str]:
+
   node = topology.nodes[n_name]                             # Get the node data
   v_cmd = get_exec_list(v_entry,'exec',node,topology)       # ... and the 'exec' action for the current node
   if not v_cmd:                                             # We should not get here, but we could...
     log.error(
       f'Test {v_entry.name}: have no idea what command to execute on node {n_name} / device {node.device}',
       category=log.MissingValue,
       module='validation')
     return False
 
   # Set up arguments for the 'netlab connect' command and execute it
   #
-  args = argparse.Namespace(quiet=True,host=n_name,output=True,show=None)
+  args = argparse.Namespace(quiet=True,host=n_name,output=True,show=None,verbose=False)
   result = connect_to_node(args=args,rest=v_cmd,topology=topology,log_level=LogLevel.NONE)
 
   if result is False:                                       # Report an error if 'netlab connect' failed
-    log_failure(
-      f'Failed to execute command {v_cmd} on {n_name} (device {node.device})',topology)
+    if report_error:
+      log_failure(
+        f'Failed to execute command "{" ".join(v_cmd)}" on {n_name} (device {node.device})',topology)
 
   return result
 
 '''
 find_test_action -- find something that can be executed on current node
 
 * Try 'show' and 'exec' actions
 * If an action value is a string, the user doesn't care about multi-vendor
   setup. Run with whatever the user specified
 * If the user specified a multi-vendor setup, try to use the device-specific
   action
+* If there's no relevant 'show' or 'exec' action, try the plugin
+* If there's no plugin, but we have 'wait' action, return 'wait'
 * If everything fails, return None (nothing usable for the current node)
 '''
 def find_test_action(v_entry: Box, node: Box) -> typing.Optional[str]:
-  for kw in ('show','exec','wait'):
+  for kw in ('show','exec'):
     if kw not in v_entry:
       continue
     if isinstance(v_entry[kw],(str,int)):
       return kw
     if node.device in v_entry[kw]:
       return kw
 
-  if 'plugin' not in v_entry:
-    return None
+  if 'plugin' in v_entry:
+    return find_plugin_action(v_entry,node)
 
-  return find_plugin_action(v_entry,node)
+  if 'wait' in v_entry:
+    return 'wait'
+
+  return None
 
 '''
 wait_before_testing -- wait for specified time since lab start time or previous test
 '''
 def wait_before_testing(
       v_entry: Box,
       start_time: typing.Optional[typing.Union[int,float]],
@@ -434,15 +525,16 @@
 }
 
 def execute_validation_expression(
       v_entry: Box,
       node: Box,
       topology: Box,
       result: Box,
-      verbosity: int) -> typing.Optional[bool]:
+      verbosity: int,
+      report_error: bool) -> typing.Optional[bool]:
 
   global test_skip_count,test_result_count,test_pass_count
   global BUILTINS
 
   v_test = get_entry_value(v_entry,'valid',node,topology)
   if not v_test:                              # Do we have a validation expression for the current device?
     log_info(                                 # ... nope, have to skip it
@@ -469,16 +561,17 @@
         print(f'Test expression: {v_test}\n')
         print(f'Evaluated result {OK}')
       for kw in ('re','result'):              # Remove stuff that will crash JSON serialization
         result.pop(kw,None)
       print(f'Result received from {node.name}\n{"-" * 80}\n{result.to_json()}\n')
 
   if OK is not None and not OK:               # We have a real result (not skipped) that is not OK
-    p_test_fail(node.name,v_entry,topology)
-    test_result_count += 1
+    if report_error:
+      p_test_fail(node.name,v_entry,topology)
+      test_result_count += 1
     return bool(OK)
   elif OK:                                    # ... or we might have a positive result
     log_progress(f'Validation succeeded on {node.name}',topology)
     test_result_count += 1
     test_pass_count += 1
     return bool(OK)
 
@@ -495,114 +588,173 @@
 * If the 'exec_plugin_function' throws an exception, log the failure and assume the test has failed
 """
 def execute_validation_plugin(
       v_entry: Box,
       node: Box,
       topology: Box,
       result: Box,
-      verbosity: int) -> typing.Optional[bool]:
+      verbosity: int,
+      report_error: bool) -> typing.Optional[bool]:
 
   global test_skip_count,test_result_count,test_pass_count
 
   try:
     OK = exec_plugin_function('valid',v_entry,node,result)
     if OK is not None and not OK:
-      p_test_fail(node.name,v_entry,topology)
+      if report_error:
+        p_test_fail(node.name,v_entry,topology)
   except Exception as ex:
-    log_failure(f'{node.name}: {str(ex)}',topology)
+    if report_error:
+      log_failure(f'{node.name}: {str(ex)}',topology)
     OK = False
 
   if (not OK and verbosity) or verbosity >= 2:
     print(f'Input data: {result.to_json()}')
     print(f'Plugin expression: {v_entry.plugin}\n')
     print(f'Evaluated result {OK}')
 
   if OK is not None:
-    test_result_count += 1
+    if report_error or OK:
+      test_result_count += 1
     if OK:
       msg = f'{node.name}: {OK}' if isinstance(OK,str) else f'Validation succeeded on {node.name}'
       log_progress(msg,topology)
       test_pass_count += 1
 
   return bool(OK)
 
 '''
+Execute node validation
+'''
+def execute_node_validation(
+      v_entry: Box,
+      topology: Box,
+      n_name: str,
+      report_error: bool,
+      args: argparse.Namespace) -> typing.Tuple[typing.Optional[bool],typing.Optional[bool]]:
+
+  global test_skip_count,test_result_count,test_pass_count
+
+  node = topology.nodes[n_name]
+  result = data.get_empty_box()
+
+  action = find_test_action(v_entry,node)       # Find the action to show/execute/wait
+  if action == 'wait':                          # Test with pure 'wait'
+    return (True,True)                          # is assumed to be successful
+
+  if action is None:                            # None found, skip this node
+    log_info(
+      f'Test action not defined for device {node.device} / node {n_name}',
+      f_status='SKIPPED',
+      topology=topology)
+    test_skip_count += 1                        # Increment skip count for test results summary
+    return (True,None)                          # Processed, unknown result
+
+  if args.verbose >= 2:                         # Print out what will be executed
+    cmd = get_entry_value(v_entry,action,node,topology)
+    print(f'{action} on {node.name}/{node.device}: {cmd}')
+
+  if action == 'show':                          # We got a 'show' action, try to get parsed results
+    result = get_parsed_result(v_entry,n_name,topology,args.verbose)
+    if '_error' in result:                      # OOPS, we failed (unrecoverable)
+      test_result_count += 1                    # Increase result count
+      return (True, False)                      # ... and return (processed, failed)
+  elif action == 'exec':                        # We got an 'exec' action, try to get something out of the device
+    result.stdout = get_result_string(v_entry,n_name,topology,report_error)
+    if result.stdout is False:                  # Did the exec command fail?
+      if report_error:
+        test_result_count += 1
+        return (True, False)                    # Return (processed, failed)
+
+  OK = None
+  if 'valid' in v_entry:                        # Do we have a validation expression in the test entry?
+    OK = execute_validation_expression(v_entry,node,topology,result,args.verbose,report_error)
+  elif 'plugin' in v_entry:                     # If not, try to call the plugin function
+    OK = execute_validation_plugin(v_entry,node,topology,result,args.verbose,report_error)
+
+  if OK is False:                               # Validation failed...
+    if not report_error:                        # ... but we still don't have to report it?
+      return (False, None)                      # ... return (not processed, unknown)
+    if 'result' in args.dump:                   # Do we have to dump the result for further troubleshooting?
+      for kw in ['re']:                         # ... remove extra keys first
+        result.pop(kw,None)
+      # ... and remove the 'result' key if it's not needed
+      if 'result' in result and isinstance(result.result,Box):
+        result.pop('result',None)
+      print(f'Returned result\n{"=" * 80}\n{result.to_yaml()}')
+  return (True, OK)                             # ... otherwise return (processed, validation result)
+
+'''
 Execute a single validation test on all specified nodes
 '''
 def execute_validation_test(
       v_entry: Box,
       topology: Box,
       start_time: typing.Optional[typing.Union[int,float]],
       args: argparse.Namespace) -> typing.Optional[bool]:
   global test_skip_count,test_result_count,test_pass_count
 
   # Return value uses ternary logic: OK (True), Fail(False), Skipped (None)
   ret_value = None
 
   p_test_header(v_entry,topology)                 # Print test header
-  if 'wait' in v_entry and not args.nowait:
-    wait_before_testing(v_entry,start_time,topology)
+  if 'wait' in v_entry and not v_entry.nodes:     # Handle pure wait case
+    if not args.nowait:
+      wait_before_testing(v_entry,start_time,topology)
+    return None
 
   if not v_entry.nodes:
-    if 'wait' in v_entry:
-      return None
-
     log_info(
       f'There are no nodes specified for this test, skipping...',
       f_status='SKIPPED',
       topology=topology)
     test_skip_count += 1
     return None
 
-  for n_name in v_entry.nodes:                    # Iterate over all specified nodes
-    node = topology.nodes[n_name]
-    result = data.get_empty_box()
-
-    action = find_test_action(v_entry,node)       # Find the action to show/execute/wait
-    if action == 'wait':                          # Skip tests with pure wait action
-      continue                                    # ... note that wait is the last action keyword considered
+  wait_time = 0 if args.nowait else v_entry.get('wait',0)
+  start_time= time.time()
+  stop_time = start_time + wait_time              # Time to wait for successful result
+  wait_msg  = v_entry.get('wait_msg',None)        # Message to display if starting sleep after the first try
+  wait_time = time.time()                         # Time to display first 'waiting' message
+  wait_cnt  = 0                                   # How many 'waiting' messages did we display?
+  n_remaining: list = v_entry.nodes               # Start with all nodes specified in the validation entry
+
+  while n_remaining:                              # Keep retrying 
+    for n_name in n_remaining:                    # Iterate over remaining nodes
+      (proc,OK) = execute_node_validation(v_entry,topology,n_name,time.time() >= stop_time,args)
+
+      if proc:                                    # Have we processed this node? Remove node from remaining list
+        n_remaining = [ x for x in n_remaining if x != n_name ]
+
+      # The result could be 'True', 'False', or 'None' (don't know)
+      if OK is True and ret_value is None:        # If we have a True result and we don't know the composite result yet
+        ret_value = True                          # ... set composite result to True
+      elif OK is False:                           # But if we have a single failure ...
+        ret_value = False                         # ... set composite result to False (failure)
+
+    if ret_value is not False and n_remaining and wait_msg:
+      if wait_time < time.time():
+        if 'wait' in v_entry and wait_cnt == 0:
+          extra_msg = f' (retrying for {v_entry.wait} seconds)'
+        else:
+          extra_msg = f' ({int(stop_time - time.time())} seconds left)'
+        log_info(
+          wait_msg + extra_msg,
+          f_status = 'WAITING',
+          topology=topology)
+        wait_cnt += 1                             # Next message will be X seconds left
+        wait_time += 15                           # ... and it will happen after 15 seconds
+      time.sleep(1)
 
-    if action is None:                            # None found, skip this node
+  if ret_value:                                   # If we got to 'True'
+    if wait_cnt:
       log_info(
-        f'Test action not defined for device {node.device} / node {n_name}',
-        f_status='SKIPPED',
+        f'Succeeded in { round(time.time() - start_time,1) } seconds',
+        f_status = 'PASS',
         topology=topology)
-      test_skip_count += 1                        # Increment skip count for test results summary
-      continue
-
-    if args.verbose >= 2:                         # Print out what will be executed
-      cmd = get_entry_value(v_entry,action,node,topology)
-      print(f'{action} on {node.name}/{node.device}: {cmd}')
-
-    if action == 'show':                          # We got a 'show' action, try to get parsed results
-      result = get_parsed_result(v_entry,n_name,topology,args.verbose)
-      if '_error' in result:                      # OOPS, we failed
-        ret_value = False
-        test_result_count += 1
-        continue
-    elif action == 'exec':                        # We got an 'exec' action, try to get something out of the device
-      result.stdout = get_result_string(v_entry,n_name,topology)
-      if result.stdout is False:                  # Store device printout in 'stdout'
-        test_result_count += 1
-        ret_value = False
-        continue
-
-    OK = None
-    if 'valid' in v_entry:                        # Do we have a validation expression in the test entry?
-      OK = execute_validation_expression(v_entry,node,topology,result,args.verbose)
-    elif 'plugin' in v_entry:                     # If not, try to call the plugin function
-      OK = execute_validation_plugin(v_entry,node,topology,result,args.verbose)
-
-    # The result could be 'True', 'False', or 'None' (don't know)
-    if OK is True and ret_value is None:          # If we have a True result and we don't know the composite result yet
-      ret_value = True                            # ... set composite result to True
-    elif OK is False:                             # But if we have a single failure ...
-      ret_value = False                           # ... set composite result to False (failure)
-
-  if ret_value:                                   # If we got to 'True'
     p_test_pass(v_entry,topology)                 # ... declare Mission Accomplished
 
   return ret_value
 
 '''
 filter_by_test: select only tests specified in arguments
 '''
@@ -654,42 +806,47 @@
   for v_entry in topology.validate:
     v_entry.nodes = [ n for n in v_entry.nodes if n in node_list ]
 
 '''
 Main routine: run all tests, handle validation errors, print summary results
 '''
 def run(cli_args: typing.List[str]) -> None:
-  global test_skip_count,test_result_count,test_pass_count
+  global test_skip_count,test_result_count,test_pass_count,ERROR_ONLY
   args = validate_parse(cli_args)
   log.set_logging_flags(args)
   topology = load_snapshot(args)
 
   if 'validate' not in topology:
-    log.fatal('No validation tests defined for the current lab, exiting')
+    if args.skip_missing:
+      sys.exit(2)
+    else:
+      log.fatal('No validation tests defined for the current lab, exiting')
 
   if args.list:
     list_tests(topology)
     return
 
   filter_by_tests(args,topology)
   filter_by_nodes(args,topology)
+  extend_first_wait_time(args,topology)
   log.exit_on_error()
 
   templates.load_ansible_filters()
 
+  ERROR_ONLY = args.error_only
   status = True
   cnt = 0
   test_skip_count = 0
   test_result_count = 0
   test_pass_count = 0
   topology._v_len = max([ len(v_entry.name) for v_entry in topology.validate ] + [ 7 ])
-  start_time = _status.lock_timestamp()
+  start_time = _status.lock_timestamp() or time.time()
 
   for v_entry in topology.validate:
-    if cnt:
+    if cnt and not ERROR_ONLY:
       print()
 
     try:
       result = execute_validation_test(v_entry,topology,start_time,args)
     except KeyboardInterrupt:
       print("")
       log.fatal('Validation test interrupted')
@@ -705,17 +862,18 @@
         sys.exit(1)
 
     if 'wait' in v_entry:
       start_time = time.time()
 
     cnt = cnt + 1
 
-  print()
-  if test_pass_count and test_pass_count == test_result_count:
-    log_progress(f'Tests passed: {test_pass_count}',topology,f_status='SUCCESS')
-  elif test_result_count:
-    log_failure('Tests completed, validation failed',topology)
+  if not ERROR_ONLY:
+    print()
+    if test_pass_count and test_pass_count == test_result_count:
+      log_progress(f'Tests passed: {test_pass_count}',topology,f_status='SUCCESS')
+    elif test_result_count:
+      log_failure('Tests completed, validation failed',topology)
 
-  if test_skip_count:
-    log_info('Some tests were skipped, the results are not reliable',topology)
+    if test_skip_count:
+      log_info('Some tests were skipped, the results are not reliable',topology)
 
   sys.exit(0 if status else 1)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `networklab-1.8.0.post2/netsim/common.py` & `networklab-1.8.1/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/daemons/bird.yml` & `networklab-1.8.1/netsim/daemons/bird.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/data/__init__.py` & `networklab-1.8.1/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/data/filemaps.py` & `networklab-1.8.1/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/data/global_vars.py` & `networklab-1.8.1/netsim/data/global_vars.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #
 
 import typing
 from box import Box
 
 _topology: typing.Optional[Box] = None
 _globals:  typing.Optional[Box] = None
+_glob_dict: dict = {}
 
 '''
 init -- create 'globals' entry in 'topology.defaults' and save a pointer to it
 
 It would be ideal to get a pointer to topology in every call to 'get', but
 that's not realistic.
 '''
@@ -24,24 +25,40 @@
   _globals  = topology.defaults._globals
 
 
 '''
 get -- get a pointer to a global Box (referenced by name) hidden in topology
 '''
 
+def missing_globals(varname: str) -> typing.NoReturn:
+  from ..utils.log import fatal
+  fatal(f'Trying to use global variable {varname} before the global_vars subsystem is initialized')
+
 def get(varname: str) -> Box:
+  global _globals
   if _globals is None:
-    from ..utils.log import fatal
-    from ..data import get_empty_box
-
-    fatal(f'Trying to get global variable {varname} before the global_vars subsystem is initialized')
-    return get_empty_box()              # pragma: no cover -- fatal aborts, but we need to return the right object to keep mypy happy
+    missing_globals(varname)
 
   return _globals[varname]
 
+def set(varname: str, value: typing.Any) -> None:
+  global _globals
+  if _globals is None:
+    missing_globals(varname)
+
+  _globals[varname] = value
+
+def get_result_dict(varname: str) -> Box:
+  global _glob_dict
+  return _glob_dict.get(varname,Box({}))
+
+def set_result_dict(varname: str, value: Box) -> None:
+  global _glob_dict
+  _glob_dict[varname] = value
+
 def get_topology() -> typing.Optional[Box]:
   global _topology
 
   return _topology
 
 def get_const(varname: str, default: typing.Any) -> typing.Any:
   topology = get_topology()
```

### Comparing `networklab-1.8.0.post2/netsim/data/types.py` & `networklab-1.8.1/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/data/validate.py` & `networklab-1.8.1/netsim/data/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/defaults/attributes.yml` & `networklab-1.8.1/netsim/defaults/attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/defaults/hints.yml` & `networklab-1.8.1/netsim/defaults/hints.yml`

 * *Files 16% similar despite different names*

```diff
@@ -6,12 +6,15 @@
     participating nodes and list VLANs in the 'vlans' attribute of that group
   node_bundle: |
     evpn.bundle attribute can be used only in global VRF definition
   asn: >
     You could use 'bgp.as' parameter to specify the global AS. Otherwise, specify
     the global AS used by EVPN in 'vrf.as' parameter if you use VRFs, or in
     'evpn.as' parameter if you use EVPN in bridging-only scenarios.
+bgp:
+  igp: >
+    Add a supported IGP (ospf, isis, eigrp) to the list of modules.
 report:
   source: >
     A report can be specified in a file with .j2 suffix within 'reports' subdirectory in
     package-, system-, user- or current directory. You can also specify a report in a
     defaults.outputs.report setting.
```

### Comparing `networklab-1.8.0.post2/netsim/defaults/paths.yml` & `networklab-1.8.1/netsim/defaults/paths.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ---
 validate:                       # Search path for validation plugins
 - topology:validate
 - validate
+- package:validate
 
 custom:                         # Custom configuration templates
   dirs:                         # ... search directories
   - "topology:"
   - "."
   - "~/.netlab"
   - "package:extra"
```

### Comparing `networklab-1.8.0.post2/netsim/devices/__init__.py` & `networklab-1.8.1/netsim/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/arubacx.py` & `networklab-1.8.1/netsim/devices/arubacx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/arubacx.yml` & `networklab-1.8.1/netsim/devices/arubacx.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: ArubaOS-CX
 interface_name: 1/1/{ifindex}
 mgmt_if: mgmt
 loopback_interface_name: "loopback {ifindex}"
 tunnel_interface_name: "tunnel {ifindex}"
 ifindex_offset: 1
 libvirt:
@@ -16,15 +17,15 @@
   node:
     kind: vr-aoscx
   interface:
     name: eth{ifindex}
 group_vars:
   ansible_network_os: arubanetworks.aoscx.aoscx
   ansible_connection: network_cli
-  #ansible_connection: arubanetworks.aoscx.aoscx
+  # ansible_connection: arubanetworks.aoscx.aoscx
   ansible_user: admin
   ansible_ssh_pass: admin
   netlab_device_type: arubacx
 features:
   bfd: true
   bgp:
     activate_af: true
@@ -37,18 +38,20 @@
   gateway:
     protocol: [ anycast, vrrp ]
   mpls:
     ldp: true
     vpn: true
   ospf: true
   vlan:
-    #model: l3-switch
+    # model: l3-switch
     model: switch
     svi_interface_name: vlan{vlan}
     # ArubaOS-CX supports subinterfaces... but not on virtual devices.
-    #subif_name: "{ifname}.{vlan.access_id}"
-    #native_routed: False
-  vrf: true
+    # subif_name: "{ifname}.{vlan.access_id}"
+    # native_routed: False
+  vrf:
+    ospfv2: True
+    bgp: True
   vxlan: true
 external:
   image: none
 graphite.icon: switch
```

### Comparing `networklab-1.8.0.post2/netsim/devices/asav.py` & `networklab-1.8.1/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/asav.yml` & `networklab-1.8.1/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/csr.yml` & `networklab-1.8.1/netsim/devices/csr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/cumulus.yml` & `networklab-1.8.1/netsim/devices/cumulus.yml`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,17 @@
     protocol: [ anycast, vrrp ]
   ospf:
     unnumbered: True
   vlan:
     model: switch
     svi_interface_name: "vlan{vlan}"
     subif_name: "{ifname}.{vlan.access_id}"
-  vrf: True
+  vrf:
+    ospfv2: True
+    bgp: True
   vxlan: True
 clab:
   mtu: 1500
   node:
     kind: cvx
     runtime: docker
     config_templates:
```

### Comparing `networklab-1.8.0.post2/netsim/devices/cumulus_nvue.yml` & `networklab-1.8.1/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/dellos10.yml` & `networklab-1.8.1/netsim/devices/dellos10.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Dell OS10
 interface_name: ethernet1/1/{ifindex}
 mgmt_if: mgmt1/1/1
 loopback_interface_name: loopback{ifindex}
 features:
   initial:
     ipv4:
@@ -19,15 +20,17 @@
     irb: true
   gateway:
     protocol: [ anycast, vrrp ]
   ospf: true
   vlan:
     model: switch
     svi_interface_name: virtual-network{vlan}
-  vrf: true
+  vrf:
+    ospfv2: True
+    bgp: True
   vxlan: true
 clab:
   image: vrnetlab/vr-ftosv
   node:
     kind: vr-ftosv
   interface:
     name: eth{ifindex}
```

### Comparing `networklab-1.8.0.post2/netsim/devices/eos.py` & `networklab-1.8.1/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/eos.yml` & `networklab-1.8.1/netsim/devices/eos.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Arista vEOS VM or cEOS container
 interface_name: Ethernet{ifindex}
 mgmt_if: Management1
 loopback_interface_name: Loopback{ifindex}
 tunnel_interface_name: Tunnel{ifindex}
 virtualbox:
   image: arista/veos
@@ -16,16 +17,18 @@
     ipv4:
       unnumbered: true
     ipv6:
       lla: true
   bfd: true
   bgp:
     activate_af: true
+    ipv6_lla: true
     local_as: true
     local_as_ibgp: true
+    rfc8950: true
     vrf_local_as: true
     community:
       standard: [ standard, large ]
       large: [ large ]
       extended: [ extended ]
       2octet: [ standard ]
   dhcp:
@@ -54,34 +57,39 @@
     unnumbered: true
   sr: true
   vlan:
     model: l3-switch
     native_routed: true
     subif_name: '{ifname}.{subif_index}'
     svi_interface_name: Vlan{vlan}
-  vrf: true
+  vrf:
+    ospfv2: True
+    ospfv3: True
+    bgp: True
   vxlan: true
 clab:
   interface:
     name: et{ifindex}
   node:
     kind: ceos
     env:
       INTFTYPE: et
       CLAB_MGMT_VRF: management
   mgmt_if: Management0
-  image: ceos:4.26.4M
+  image: ceos:4.31.2F
   group_vars:
     ansible_user: admin
     ansible_ssh_pass: admin
     ansible_become: yes
     ansible_become_method: enable
 libvirt:
   image: arista/veos
   create_template: eos.xml.j2
-#      create: |
-#        virt-install --connect=qemu:///system --name=vm_box --os-type=linux --arch=x86_64 --cpu host --vcpus=2 --hvm
-#          --ram=2048 --disk path=vm.qcow2,bus=ide,format=qcow2 --network=network:vagrant-libvirt,model=virtio --graphics none --import
+# create: |
+#   virt-install --connect=qemu:///system --name=vm_box --os-type=linux
+#     --arch=x86_64 --cpu host --vcpus=2 --hvm
+#     --ram=2048 --disk path=vm.qcow2,bus=ide,format=qcow2
+#     --network=network:vagrant-libvirt,model=virtio --graphics none --import
 external:
   image: none
 graphite.icon: switch
 bgp._cprop_order: [ standard, extended, large, link-bandwidth ]
```

### Comparing `networklab-1.8.0.post2/netsim/devices/fortios.yml` & `networklab-1.8.1/netsim/devices/fortios.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/frr.yml` & `networklab-1.8.1/netsim/devices/frr.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 description: FRR container
 interface_name: eth{ifindex}
 mgmt_if: eth0
-loopback_interface_name: "lo{ifindex}"
+loopback_interface_name: lo{ifindex if ifindex else ""}
 tunnel_interface_name: "tun{ifindex}"
 group_vars:
   ansible_network_os: frr
   ansible_python_interpreter: auto_silent
   netlab_initial: always
 clab:
   # image: frrouting/frr:v7.5.0
@@ -71,10 +71,14 @@
     mixed_trunk: true
     model: router
     native_routed: true
     subif_name: '{ifname}.{vlan.access_id}'
     svi_interface_name: vlan{vlan}
   vrf:
     keep_module: true
-  vxlan: true
+    ospfv2: True
+    ospfv3: True
+    bgp: True
+  vxlan:
+    vtep6: true
 
 graphite.icon: router
```

### Comparing `networklab-1.8.0.post2/netsim/devices/iosv.py` & `networklab-1.8.1/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/iosv.yml` & `networklab-1.8.1/netsim/devices/iosv.yml`

 * *Files 7% similar despite different names*

```diff
@@ -60,13 +60,16 @@
     6pe: true
   vlan:
     model: router
     svi_interface_name: BVI{bvi}
     subif_name: "{ifname}.{subif_index}"
     mixed_trunk: true
     native_routed: true
-  vrf: true
+  vrf:
+    ospfv2: True
+    ospfv3: True
+    bgp: True
   gateway:
     protocol: [ vrrp ]
 external:
   image: none
 graphite.icon: router
```

### Comparing `networklab-1.8.0.post2/netsim/devices/iosxr.yml` & `networklab-1.8.1/netsim/devices/iosxr.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Cisco IOS XRv
 mgmt_if: MgmtEth0/RP0/CPU0/0
 interface_name: GigabitEthernet0/0/0/{ifindex}
 ifindex_offset: 0
 group_vars:
   ansible_user: vagrant
   ansible_ssh_pass: vagrant
@@ -30,9 +31,19 @@
   image: cisco/iosxr
   create:
     virt-install --connect=qemu:///system --network network=vagrant-libvirt,model=e1000 --name=vm_box
       --cpu host --arch=x86_64 --vcpus=2 --ram=8192
       --virt-type=kvm
       --disk path=vm.qcow2,format=qcow2,device=disk,bus=ide
       --graphics none --import
-##      create_iso: iosxr
-##          --disk path=bootstrap.iso,format=iso,device=cdrom
+clab:
+  node:
+    kind: cisco_xrd
+    runtime: docker
+  mgmt_if: MgmtEth0/RP0/CPU0/0
+  interface:
+    name: Gi0-0-0-{ifindex}
+  image: ios-xr/xrd-control-plane:7.11.1
+  group_vars:
+    ansible_user: clab
+    ansible_ssh_pass: clab@123
+    ansible_become_password: clab@123
```

### Comparing `networklab-1.8.0.post2/netsim/devices/junos.py` & `networklab-1.8.1/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/junos.yml` & `networklab-1.8.1/netsim/devices/junos.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Generic Juniper device (meta device, used only as parent)
 loopback_interface_name: "lo0.{ifindex}"
 ifindex_offset: 0
 interface_name: ge-0/0/{ifindex}
 mgmt_if: fxp0
 group_vars:
   ansible_user: vagrant
@@ -12,23 +13,27 @@
 
 features:
   initial:
     ipv4:
       unnumbered: true
     ipv6:
       lla: true
+    delay: 90
   bfd: true
   bgp: true
   isis:
     unnumbered:
       ipv4: true
       ipv6: true
   mpls:
     ldp: true
     vpn: true
   ospf:
     unnumbered: true
   sr: true
-  vrf: true
+  vrf:
+    ospfv2: True
+    ospfv3: True
+    bgp: True
 
 external:
   image: none
```

### Comparing `networklab-1.8.0.post2/netsim/devices/linux.py` & `networklab-1.8.1/netsim/devices/linux.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/linux.yml` & `networklab-1.8.1/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/none.yml` & `networklab-1.8.1/netsim/devices/none.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Dummy device used to test topology transformation
 #
 # Most features are enabled on the dummy device -- this file is a pretty
 # good template if you want to figure out what device features there are.
 #
 interface_name: eth{ifindex}
 loopback_interface_name: Loopback{ifindex}
@@ -53,9 +54,12 @@
     model: l3-switch
     svi_interface_name: Vlan{vlan}
     subif_name: "{ifname}.{vlan.access_id}"
     mixed_trunk: True
     native_routed: True
   sr: True
   srv6: True
-  vrf: True
+  vrf:
+    ospfv2: True
+    ospfv3: True
+    bgp: True
   vxlan: True
```

### Comparing `networklab-1.8.0.post2/netsim/devices/nxos.yml` & `networklab-1.8.1/netsim/devices/nxos.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Cisco Nexus 9300v
 interface_name: Ethernet1/{ifindex}
 mgmt_if: mgmt0
 loopback_interface_name: loopback{ifindex}
 virtualbox:
   image: cisco/nexus9300v
 group_vars:
@@ -32,15 +33,17 @@
   ospf:
     unnumbered: true
   vlan:
     model: l3-switch
     native_routed: true
     subif_name: '{ifname}.{subif_index}'
     svi_interface_name: vlan{vlan}
-  vrf: true
+  vrf:
+    ospfv2: True
+    bgp: True
   vxlan: true
 
 libvirt:
   create_template: nxos.xml.j2
   image: cisco/nexus9300v
 external:
   image: none
```

### Comparing `networklab-1.8.0.post2/netsim/devices/routeros.yml` & `networklab-1.8.1/netsim/devices/routeros.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Mikrotik RouterOS version 6
 interface_name: ether{ifindex}
 mgmt_if: ether1
 ifindex_offset: 2
 libvirt:
   image: mikrotik/chr
 group_vars:
@@ -17,11 +18,13 @@
   ospf: true
   vlan:
     model: router
     svi_interface_name: bridge{vlan}
     subif_name: "{ifname}-{vlan.access_id}"
     mixed_trunk: true
     native_routed: true
-  vrf: true
+  vrf:
+    ospfv2: True
+    bgp: True
 external:
   image: none
 graphite.icon: router
```

### Comparing `networklab-1.8.0.post2/netsim/devices/routeros7.yml` & `networklab-1.8.1/netsim/devices/routeros7.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Mikrotik RouterOS version 7
 interface_name: ether{ifindex}
 mgmt_if: ether1
 loopback_interface_name: loopback{ifindex}
 ifindex_offset: 2
 libvirt:
   image: mikrotik/chr7
@@ -22,15 +23,17 @@
     vpn: true
   ospf: true
   vlan:
     model: l3-switch
     svi_interface_name: "vlan{vlan}"
     subif_name: "{ifname}-{vlan.access_id}"
     native_routed: true
-  vrf: true
+  vrf:
+    ospfv2: True
+    bgp: True
 clab:
   image: vrnetlab/vr-routeros:7.6
   node:
     kind: vr-ros
   interface:
     name: eth{ifindex-1}
 external:
```

### Comparing `networklab-1.8.0.post2/netsim/devices/srlinux.yml` & `networklab-1.8.1/netsim/devices/srlinux.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+---
 description: Nokia SR Linux container
 mgmt_if: mgmt0
 interface_name: ethernet-1/{ifindex}
 loopback_interface_name: "lo0.{ifindex}"
 group_vars:
   ansible_user: admin
   ansible_ssh_pass: NokiaSrl1!
   ansible_network_os: srlinux
   ansible_connection: paramiko
   netlab_console_connection: ssh
 sr:
   srgb_range_start: 500000
   srgb_range_size: 1000
   ipv6_sid_offset: 100
-bfd:           # SR Linux supports lower BFD timers than the global default
+bfd:                                    # SR Linux supports lower BFD timers than the global default
   min_tx: 100
   min_rx: 100
 clab:
-  image: ghcr.io/nokia/srlinux:23.3.1 # latest version, changes YANG model
+  image: ghcr.io/nokia/srlinux:23.3.1   # latest version, changes YANG model
   node:
     kind: srl
     type: ixrd2
   interface:
     name: e1-{ifindex}
   group_vars:
     srlinux_grpc_port: 57400
@@ -41,28 +42,30 @@
     local_as: True
     vrf_local_as: True
     local_as_ibgp: True
     activate_af: True
     ipv6_lla: True
     rfc8950: True
   vxlan:
-    requires: [ evpn ] # vrf for l3 vxlan
+    requires: [ evpn ]                  # vrf for l3 vxlan
   evpn:
     irb: True
     asymmetrical_irb: True
   ospf:
     unnumbered: False
   isis:
     unnumbered:
       ipv4: False
       ipv6: True
       network: False
   vrf:
     keep_module: True
+    ospfv2: True
+    bgp: True
   gateway:
     protocol: [ anycast ]
   sr: True
   mpls:
-   ldp: True # on 7250 IXR only
+    ldp: True                           # on 7250 IXR only
 external:
   image: none
 graphite.icon: router
```

### Comparing `networklab-1.8.0.post2/netsim/devices/sros.yml` & `networklab-1.8.1/netsim/devices/sros.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 description: Nokia SR OS container
 mgmt_if: A/1
 interface_name: 1/1/c{ifindex}
 loopback_interface_name: "loopback.{ifindex}"
 group_vars:
   ansible_user: admin
   ansible_ssh_pass: admin
@@ -9,60 +10,62 @@
   ansible_connection: paramiko_ssh
   netlab_console_connection: ssh
   sros_use_openconfig: False
 sr:
   srgb_range_start: 500000
   srgb_range_size: 1000
   ipv6_sid_offset: 100
-bfd:           # SR OS supports lower BFD timers than the global default
+bfd:                          # SR OS supports lower BFD timers than the global default
   min_tx: 100
   min_rx: 100
 features:
   initial:
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
   ospf:
     unnumbered: True
-    strict_bfd: True # RFC9355 support
+    strict_bfd: True          # RFC9355 support
   isis:
     unnumbered:
       ipv4: True
       ipv6: True
-      network: False # SROS treats the interfaces as point-to-point and forms at most 1 adjacency
+      network: False          # SROS treats the interfaces as point-to-point and forms at most 1 adjacency
   bfd: True
   bgp:
     local_as: True
     vrf_local_as: True
     local_as_ibgp: True
     activate_af: True
     ipv6_lla: True
-    rfc8950: False   # Not implemented yet, may be possible
+    rfc8950: False            # Not implemented yet, may be possible
   evpn:
     irb: True
     asymmetrical_irb: True
   mpls:
     ldp: True
-    bgp: True  # BGP-LU
+    bgp: True                 # BGP-LU
     vpn: True
-    6pe: True  # also implies BGP-LU
+    6pe: True                 # also implies BGP-LU
   vxlan:
-    requires: [ evpn ] # Current implementation focuses on VXLAN+EVPN, device supports static too
+    requires: [ evpn ]        # Current implementation focuses on VXLAN+EVPN, device supports static too
   vlan:
     model: router
     svi_interface_name: "svi.{vlan}"
     subif_name: "{ifname}/1:{vlan.access_id}"
     mixed_trunk: True
     native_routed: True
   gateway:
     protocol: [ anycast, vrrp ]
   sr: True
   srv6: True
-  vrf: True
+  vrf:
+    ospfv2: True
+    bgp: True
 
 clab:
   image: vrnetlab/vr-sros
   mtu: 1500
   node:
     kind: vr-sros
     type: sr-1 # By default emulate SR-1
```

### Comparing `networklab-1.8.0.post2/netsim/devices/unknown.py` & `networklab-1.8.1/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/vmx.py` & `networklab-1.8.1/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/vptx.py` & `networklab-1.8.1/netsim/devices/vptx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/vsrx.py` & `networklab-1.8.1/netsim/devices/vsrx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/devices/vsrx.yml` & `networklab-1.8.1/netsim/devices/vsrx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.domain/plugin.py` & `networklab-1.8.1/netsim/extra/bgp.domain/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.originate/plugin.py` & `networklab-1.8.1/netsim/extra/bgp.originate/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/_route_map_aoscx.j2` & `networklab-1.8.1/netsim/extra/bgp.policy/_route_map_aoscx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/_route_map_ios.j2` & `networklab-1.8.1/netsim/extra/bgp.policy/_route_map_ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/arubacx.j2` & `networklab-1.8.1/netsim/extra/bgp.policy/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/cumulus.j2` & `networklab-1.8.1/netsim/extra/bgp.policy/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/defaults.yml` & `networklab-1.8.1/netsim/extra/bgp.policy/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/eos.j2` & `networklab-1.8.1/netsim/extra/bgp.policy/eos.j2`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 {% import '_route_map_ios.j2' as routemap with context %}
 {% macro ebgp_neighbor(n,af) -%}
+{%   set peer = 'ebgp_intf_' + n.local_if if n.local_if is defined else n[af] %}
 {%   if 'weight' in n %}
-    neighbor {{ n[af] }} weight {{ n.weight }}
+    neighbor {{ peer }} weight {{ n.weight }}
+{%   endif %}
+{%   if 'policy' in n %}
+{%     for direction in [ 'in','out' ] if direction in n.policy %}
+    neighbor {{ peer }} route-map bp-{{ n._policy_name }}-{{ direction }} {{ direction }}
+{%     endfor %}
 {%   endif %}
-{{   routemap.apply_route_map(n,af) }}
 {%- endmacro %}
 !
 {% call(p_entry) routemap.create_route_maps(bgp,vrfs|default({})) -%}
 {{   routemap.common_route_map_entry(p_entry) }}
 {%- endcall %} 
 !
 router bgp {{ bgp.as }}
```

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/frr.j2` & `networklab-1.8.1/netsim/extra/bgp.policy/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/ios.j2` & `networklab-1.8.1/netsim/extra/bgp.policy/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/plugin.py` & `networklab-1.8.1/netsim/extra/bgp.policy/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/simple-attributes.yml` & `networklab-1.8.1/netsim/extra/bgp.policy/simple-attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.policy/srlinux.j2` & `networklab-1.8.1/netsim/extra/bgp.policy/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/_sample_bfd_template.j2` & `networklab-1.8.1/netsim/extra/bgp.session/_sample_bfd_template.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/arubacx.j2` & `networklab-1.8.1/netsim/extra/ebgp.multihop/frr.j2`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,24 @@
-{% macro ebgp_session(n,af,bgp) -%}
-{%   if n.password is defined %}
-  neighbor {{ n[af] }} password plaintext {{ n.password }}
-{%   endif %}
-{%   if n.gtsm is defined %}
-  neighbor {{ n[af] }} ttl-security-hops {{ n.gtsm }}
-{%   endif %}
-{%   if n.timers is defined %}
-  neighbor {{ n[af] }} timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
-{%   endif %}
-{%   if n.bfd is defined %}
-  neighbor {{ n[af] }} fall-over bfd
-{%   endif %}
-{%   if n.remove_private_as|default([]) %}
-  neighbor {{ n[af] }} remove-private-as
-{%   endif %}
-{%- endmacro %}
-
-{% macro ebgp_neighbor(n,af) -%}
-{%   if n.default_originate is defined %}
-  neighbor {{ n[af] }} default-originate
-{%   endif %}
-{%   if n.allowas_in is defined %}
-  neighbor {{ n[af] }} allowas-in {{ n.allowas_in }}
+{% macro ebgp_session(n,af) -%}
+{%   if n.multihop is defined %}
+  neighbor {{ n[af] }} ebgp-multihop {{ n.multihop if n.multihop < 255 else '' }}
+  neighbor {{ n[af] }} update-source {{ loopback.ifname }}
 {%   endif %}
 {%- endmacro %}
-
 !
 router bgp {{ bgp.as }}
 {% for af in ['ipv4','ipv6'] %}
 {%   for n in bgp.neighbors if n[af] is defined %}
-{{     ebgp_session(n,af,bgp) -}}
-{%   endfor %}
-{% endfor %}
-!
-{% for af in ['ipv4','ipv6'] %}
-{%   for n in bgp.neighbors if n[af] is defined %}
-{%     if loop.first %}
- address-family {{ af }} unicast
-{%     endif %}
-{{     ebgp_neighbor(n,af) -}}
+{{     ebgp_session(n,af) -}}
 {%   endfor %}
 {% endfor %}
 !
 {% if vrfs is defined %}
-{% for vname,vdata in vrfs.items() if vdata.bgp is defined %}
- vrf {{ vname }}
-{% for af in ['ipv4','ipv6'] %}
-{%   for n in bgp.neighbors if n[af] is defined %}
-{{     ebgp_session(n,af,bgp) -}}
-{%   endfor %}
-{% endfor %}
-!
-{%   for af in ['ipv4','ipv6'] %}
-{%     for n in vdata.bgp.neighbors if n[af] is defined %}
-{%       if loop.first %}
-   address-family {{ af }} unicast
-{%       endif %}
-{{       ebgp_neighbor(n,af) -}}
+{%   for vname,vdata in vrfs.items() if vdata.bgp is defined %}
+router bgp {{ vdata.as|default(bgp.as) }} vrf {{ vname }}
+{%     for af in ['ipv4','ipv6'] %}
+{%       for n in bgp.neighbors if n[af] is defined %}
+{{         ebgp_session(n,af) -}}
+{%       endfor %}
 {%     endfor %}
 {%   endfor %}
-{% endfor %}
 {% endif %}
-!
```

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/cumulus.j2` & `networklab-1.8.1/netsim/extra/bgp.session/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/default-originate.yml` & `networklab-1.8.1/netsim/extra/bgp.session/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/defaults.yml` & `networklab-1.8.1/netsim/extra/bgp.session/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/eos.j2` & `networklab-1.8.1/netsim/extra/bgp.session/eos.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 {% macro ebgp_session(n,af,bgp) -%}
+{%   set peer = 'ebgp_intf_' + n.local_if if n.local_if is defined else n[af] %}
 {%   if n.tcp_ao is defined %}
 {%     set idx = bgp._ao_secrets.index(n.password) + 1 %}
 {%     set algo = { 'aes-128-cmac': 'aes-128-cmac-96', 'hmac-sha-1': 'hmac-sha1-96' } %}
-  neighbor {{ n[af] }} password shared-secret profile tcp-ao-{{ idx }} algorithm {{ algo[n.tcp_ao] }}
+  neighbor {{ peer }} password shared-secret profile tcp-ao-{{ idx }} algorithm {{ algo[n.tcp_ao] }}
 {%   elif n.password is defined %}
-  neighbor {{ n[af] }} password {{ n.password }}
+  neighbor {{ peer }} password {{ n.password }}
 {%   endif %}
 {%   if n.gtsm is defined %}
-  neighbor {{ n[af] }} ttl maximum-hops {{ n.gtsm }}
+  neighbor {{ peer }} ttl maximum-hops {{ n.gtsm }}
 {%   endif %}
 {%   if n.timers is defined %}
-  neighbor {{ n[af] }} timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
+  neighbor {{ peer }} timers {{ n.timers.keepalive|default(60) }} {{ n.timers.hold|default(180) }}
 {%   endif %}
 {%   if n.bfd|default(False) %}
-  neighbor {{ n[af] }} bfd
+  neighbor {{ peer }} bfd
 {%   endif %}
 {%   if n.passive|default(False) %}
-  neighbor {{ n[af] }} passive
+  neighbor {{ peer }} passive
 {%   endif %}
 {%   if n.remove_private_as|default([]) %}
 {%     set rpa = { 'on': '', 'replace': 'all replace', 'all': 'all', 
                    'ingress': 'ingress', 'ingress-replace': 'ingress replace' } %}
 {%     for rpo in n.remove_private_as if rpo in rpa %}
-  neighbor {{ n[af] }} remove-private-as {{ rpa[rpo] }}
+  neighbor {{ peer }} remove-private-as {{ rpa[rpo] }}
 {%     endfor %}
 {%   endif %}
 {%- endmacro %}
 
 {% macro ebgp_neighbor(n,af) -%}
+{%   set peer = 'ebgp_intf_' + n.local_if if n.local_if is defined else n[af] %}
 {%   if n.default_originate|default(False) %}
-  neighbor {{ n[af] }} default-originate always
+  neighbor {{ peer }} default-originate always
 {%   endif %}
 {%   if n.allowas_in is defined %}
-  neighbor {{ n[af] }} allowas-in {{ n.allowas_in }}
+  neighbor {{ peer }} allowas-in {{ n.allowas_in }}
 {%   endif %}
 {%   if n.as_override|default(False) %}
-  neighbor {{ n[af] }} as-path remote-as replace out
+  neighbor {{ peer }} as-path remote-as replace out
 {%   endif %}
 {%- endmacro %}
 
 !
 {% for pwd in bgp._ao_secrets|default([]) %}
 {%   if loop.first %}
 management security
```

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/frr.j2` & `networklab-1.8.1/netsim/extra/bgp.session/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/ios.j2` & `networklab-1.8.1/netsim/extra/bgp.session/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/junos.j2` & `networklab-1.8.1/netsim/extra/bgp.session/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/plugin.py` & `networklab-1.8.1/netsim/extra/bgp.session/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/routeros7.j2` & `networklab-1.8.1/netsim/extra/bgp.session/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/srlinux.j2` & `networklab-1.8.1/netsim/extra/bgp.session/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/sros.j2` & `networklab-1.8.1/netsim/extra/bgp.session/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/bgp.session/vyos.j2` & `networklab-1.8.1/netsim/extra/bgp.session/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/arubacx.j2` & `networklab-1.8.1/netsim/extra/ebgp.multihop/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/defaults.yml` & `networklab-1.8.1/netsim/extra/ebgp.multihop/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml` & `networklab-1.8.1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/eos.j2` & `networklab-1.8.1/netsim/extra/ebgp.multihop/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml` & `networklab-1.8.1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/frr.bgp-config.j2` & `networklab-1.8.1/netsim/extra/ebgp.multihop/ios.j2`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 {% macro ebgp_session(n,af) -%}
 {%   if n.multihop is defined %}
   neighbor {{ n[af] }} ebgp-multihop {{ n.multihop if n.multihop < 255 else '' }}
-  neighbor {{ n[af] }} update-source {{ loopback_name }}
+  neighbor {{ n[af] }} update-source Loopback0
 {%   endif %}
 {%- endmacro %}
 !
 router bgp {{ bgp.as }}
 {% for af in ['ipv4','ipv6'] %}
 {%   for n in bgp.neighbors if n[af] is defined %}
 {{     ebgp_session(n,af) -}}
 {%   endfor %}
 {% endfor %}
 !
 {% if vrfs is defined %}
-{%   for vname,vdata in vrfs.items() if vdata.bgp is defined %}
-router bgp {{ vdata.as|default(bgp.as) }} vrf {{ vname }}
-{%     for af in ['ipv4','ipv6'] %}
+{%   for vname,vdata in vrfs.items() %}
+{%     for af in ('ipv4','ipv6') if af in vdata.af|default({}) %}
+ address-family {{ af }} vrf {{ vname }}
 {%       for n in bgp.neighbors if n[af] is defined %}
 {{         ebgp_session(n,af) -}}
 {%       endfor %}
 {%     endfor %}
 {%   endfor %}
 {% endif %}
```

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/plugin.py` & `networklab-1.8.1/netsim/extra/ebgp.multihop/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/srlinux.j2` & `networklab-1.8.1/netsim/extra/ebgp.multihop/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/ebgp.multihop/sros.j2` & `networklab-1.8.1/netsim/extra/ebgp.multihop/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/fabric/plugin.py` & `networklab-1.8.1/netsim/extra/fabric/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/multilab/__init__.py` & `networklab-1.8.1/netsim/extra/multilab/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/proxy-arp/plugin.py` & `networklab-1.8.1/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.8.1/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/extra/proxy-arp/sros.j2` & `networklab-1.8.1/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/ansible.sh` & `networklab-1.8.1/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/containerlab.sh` & `networklab-1.8.1/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/grpc.sh` & `networklab-1.8.1/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/arubacx.txt` & `networklab-1.8.1/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/asav/day0-config` & `networklab-1.8.1/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/csr.txt` & `networklab-1.8.1/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/dellos10.txt` & `networklab-1.8.1/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/eos.txt` & `networklab-1.8.1/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/eos.xml.j2` & `networklab-1.8.1/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/iosv.txt` & `networklab-1.8.1/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.8.1/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/iosxr.txt` & `networklab-1.8.1/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/nxos.txt` & `networklab-1.8.1/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.8.1/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/routeros7.txt` & `networklab-1.8.1/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/vptx/juniper.conf` & `networklab-1.8.1/netsim/install/libvirt/vptx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/vptx/make-config.sh` & `networklab-1.8.1/netsim/install/libvirt/vptx/make-config.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/vptx.txt` & `networklab-1.8.1/netsim/install/libvirt/vptx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/vptx.xml.j2` & `networklab-1.8.1/netsim/install/libvirt/vptx.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.8.1/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt/vsrx.txt` & `networklab-1.8.1/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/libvirt.sh` & `networklab-1.8.1/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/install/ubuntu.sh` & `networklab-1.8.1/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/__init__.py` & `networklab-1.8.1/netsim/modules/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from ..data.validate import must_be_list
 from ..utils.callback import Callback
 from ..augment import devices
 
 # List of attributes we don't want propagated from defaults to global/node
 #
 no_propagate_list = [
-  "attributes","extra_attributes","features",
-  "requires","supported_on","no_propagate",
-  "config_after","transform_after"]
+  "attributes", "extra_attributes", "features",
+  "requires", "supported_on", "no_propagate",
+  "config_after", "transform_after", "warnings" ]
 
 """
 Return the authoritative list of all modules.
 
 A module is a top-level 'defaults' dictionary key if the value is a dictionary with 'supported_on' key
 """
 def list_of_modules(topology: Box) -> list:
```

### Comparing `networklab-1.8.0.post2/netsim/modules/_dataplane.py` & `networklab-1.8.1/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/_routing.py` & `networklab-1.8.1/netsim/modules/_routing.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 from box import Box
 import typing
 import netaddr
 
 from ..utils import log
-from ..augment import addressing
+from ..augment import addressing,devices
 from .. import data
 
 # Build routing protocol address families
 #
 # * If the address families are not set, calculate them based on interface address families
 # * Otherwise parse and validate the AF attribute
 #
@@ -274,14 +274,48 @@
       continue
     if not vdata[proto] is False:                                           # Not a false flag
       continue
 
     vdata.pop(proto,None)                                                   # Got rid of the false flag
 
 """
+check_vrf_support: Check whether a node supports the desired routing protocol in a VRF
+
+Inputs:
+* Node to check
+* netlab protocol (ospf / bgp)
+* protocol address family (ipv4 for ospfv2, ipv6 for ospfv3)
+* feature to check in device features
+* topology (to get defaults)
+"""
+def check_vrf_protocol_support(
+      node: Box,
+      proto: str,
+      af: typing.Optional[str],
+      feature: str,
+      topology: Box) -> None:
+  if not 'vrfs' in node:                          # No VRFs in the current node, nothing to check
+    return
+  
+  for v_name,v_data in node.vrfs.items():         # Iterate over VRFs
+    if not proto in v_data:                       # Are we running the target protocol in the VRF?
+      continue
+    if af and not af in v_data.af:                # Does the VRF use the target address family?
+      continue
+
+    # We found the protocol to check in the current VRF, time to check device features
+    d_feature = devices.get_device_features(node,topology.defaults)
+    if not d_feature.get(f'vrf.{feature}',False): # Does the device support the target protocol/AF combo?
+      log.error(
+        f'Device {node.device} (node {node.name}) does not support {feature} in VRFs (found in VRF {v_name})',
+        category=log.IncorrectValue,
+        module=proto)
+      return
+
+"""
 get_remote_cp_endpoint: find the remote control-plane endpoint
 
 Return loopback interface or the first physical interface
 """
 def get_remote_cp_endpoint(n: Box) -> Box:
   if 'loopback' in n and n.get('role') != 'host':           # The node has loopback and is not a host
     return n.loopback                                       # ... can't use loopback if the node has no routing
```

### Comparing `networklab-1.8.0.post2/netsim/modules/bfd.py` & `networklab-1.8.1/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/bfd.yml` & `networklab-1.8.1/netsim/modules/bfd.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/bgp.py` & `networklab-1.8.1/netsim/modules/bgp.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,36 +146,62 @@
 build_ibgp_sessions: create IBGP session data structure
 
 * BGP route reflectors need IBGP session with all other nodes in the same AS
 * Other nodes need IBGP sessions with all RRs in the same AS
 """
 def build_ibgp_sessions(node: Box, sessions: Box, topology: Box) -> None:
   rrlist = find_bgp_rr(node.bgp.get("as"),topology)
+  has_ibgp     = False                            # Assume we have no IBGP sessions (yet)
 
   # If we don't have route reflectors, or if the current node is a route
   # reflector, we need BGP sessions to all other nodes in the same AS
   if not(rrlist) or node.bgp.get("rr",None):
     for name,n in topology.nodes.items():
       if "bgp" in n:
         if n.bgp.get("as") == node.bgp.get("as") and n.name != node.name:
           n_intf = get_remote_ibgp_endpoint(n)
           neighbor_data = bgp_neighbor(n,n_intf,'ibgp',sessions,get_neighbor_rr(n))
           if not neighbor_data is None:
             node.bgp.neighbors.append(neighbor_data)
+            has_ibgp = True
 
   #
   # The node is not a route reflector, and we have a non-empty RR list
   # We need BGP sessions with the route reflectors
   else:
     for n in rrlist:
       if n.name != node.name:
         n_intf = get_remote_ibgp_endpoint(n)
         neighbor_data = bgp_neighbor(n,n_intf,'ibgp',sessions,get_neighbor_rr(n))
         if not neighbor_data is None:
           node.bgp.neighbors.append(neighbor_data)
+          has_ibgp = True
+
+  if not has_ibgp:
+    return
+
+  # Do we have to warn the user that IBGP sessions work better with IGP?
+  # The warning could be disabled in the settings, and we assume it doesn't make
+  # sense complaining if the node has no loopback interfaces (routing on hosts)
+  #
+  ibgp_warning = topology.defaults.bgp.warnings.missing_igp and 'loopback' in node
+  igp_list     = topology.defaults.bgp.warnings.igp_list
+
+  if ibgp_warning:                                # Does the user want to get the warning?
+    for igp in igp_list:                          # If so, check the viable IGPs
+      if igp in node.module:                      # ... and if any one of them is in the list of node modules
+        ibgp_warning = False                      # ... life is good, turn off the warning
+        break
+
+  if ibgp_warning:
+    log.error(
+      f'Node {node.name} has IBGP sessions but no IGP',
+      category=Warning,
+      module='bgp',
+      hint='igp')
 
 """
 build_ebgp_sessions: create EBGP session data structure
 
 * EBGP sessions are established whenever two nodes on the same link have different AS
 """
 def build_ebgp_sessions(node: Box, sessions: Box, topology: Box) -> None:
@@ -612,8 +638,9 @@
     if not "bgp" in node:   # pragma: no cover (this should have been caught in check_bgp_parameters)
       log.fatal(f"Internal error: node {node.name} has BGP module enabled but no BGP parameters","bgp")
       return
     build_bgp_sessions(node,topology)
     bgp_set_advertise(node,topology)
     bgp_set_originate_af(node,topology)
     _routing.remove_vrf_routing_blocks(node,'bgp')
-    bgp_transform_community_list(node,topology)
+    bgp_transform_community_list(node,topology)
+    _routing.check_vrf_protocol_support(node,'bgp',None,'bgp',topology)
```

### Comparing `networklab-1.8.0.post2/netsim/modules/bgp.yml` & `networklab-1.8.1/netsim/modules/bgp.yml`

 * *Files 4% similar despite different names*

```diff
@@ -79,7 +79,10 @@
   local_as: Supports local-as functionality
   vrf_local_as: Supports local-as within a VRF
   local_as_ibgp: Can use local-as to create IBGP sesssion
   activate_af: Can control activation of individual address families
   ipv6_lla: Can run EBGP sessions over IPv6 link-local addresses
   rfc8950: Can run IPv4 AF over IPv6 LLA EBGP session
   community: Granular BGP community propagation
+warnings:
+  missing_igp: True
+  igp_list: [ ospf, eigrp, isis ]
```

### Comparing `networklab-1.8.0.post2/netsim/modules/dhcp.py` & `networklab-1.8.1/netsim/modules/dhcp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/dhcp.yml` & `networklab-1.8.1/netsim/modules/dhcp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/evpn.py` & `networklab-1.8.1/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/evpn.yml` & `networklab-1.8.1/netsim/modules/evpn.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/gateway.py` & `networklab-1.8.1/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/gateway.yml` & `networklab-1.8.1/netsim/modules/gateway.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/isis.py` & `networklab-1.8.1/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/isis.yml` & `networklab-1.8.1/netsim/modules/isis.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/mpls.py` & `networklab-1.8.1/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/mpls.yml` & `networklab-1.8.1/netsim/modules/mpls.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/ospf.py` & `networklab-1.8.1/netsim/modules/ospf.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,14 +48,39 @@
         f'Device {node.device} used on node {node.name} cannot run OSPF over unnumbered interface',
         log.IncorrectValue,
         'interfaces')
       OK = False
 
   return OK
 
+"""
+Propagate node attributes into VRFs and loopback interface:
+
+* OSPF area, reference_bandwidth, and router_id are copied into vrfs.x.ospf if needed
+* OSPF area is copied into the loopback interface
+"""
+
+def propagate_node_attributes(node: Box, topology: Box) -> None:
+  if 'ospf' not in node:
+    return
+
+  if 'loopback' in node and 'area' in node.ospf:
+    node.loopback.ospf.area = node.ospf.area
+
+  if not 'vrfs' in node:
+    return
+
+  for vname,vdata in node.vrfs.items():
+    if not 'ospf' in vdata:
+      continue
+
+    for kw in topology.defaults.ospf.attributes.vrf_copy:
+      if kw in node.ospf and kw not in vdata.ospf:
+        vdata.ospf[kw] = node.ospf[kw]
+
 class OSPF(_Module):
 
   def node_post_transform(self, node: Box, topology: Box) -> None:
     features = devices.get_device_features(node,topology.defaults)
 
     _routing.router_id(node,'ospf',topology.pools)
     
@@ -92,13 +117,17 @@
 
     #
     # Final steps:
     # * move OSPF-enabled VRF interfaces into VRF dictionary
     # * Calculate address families
     # * Enable BFD
     # * Remove OSPF module if there are no OSPF-enabled global or VRF interfaces
+    # * Propagate OSPF attributes into loopback interface and VRFs
     #
     _routing.remove_unaddressed_intf(node,'ospf')
     _routing.build_vrf_interface_list(node,'ospf',topology)
     _routing.routing_af(node,'ospf')
     _routing.remove_vrf_routing_blocks(node,'ospf')
+    propagate_node_attributes(node,topology)
     _routing.remove_unused_igp(node,'ospf')
+    _routing.check_vrf_protocol_support(node,'ospf','ipv4','ospfv2',topology)
+    _routing.check_vrf_protocol_support(node,'ospf','ipv6','ospfv3',topology)
```

### Comparing `networklab-1.8.0.post2/netsim/modules/ospf.yml` & `networklab-1.8.1/netsim/modules/ospf.yml`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     area:
     process:
     reference_bandwidth:
     bfd:
     router_id: { type: ipv4, use: id }
   node_copy: [ area ]
   vrf_aware: [ area ]
+  vrf_copy: [ area, router_id, reference_bandwidth ]
   vrf:
     active: bool
     router_id: { type: ipv4, use: id }
   link:
     cost: { type: int, min_value: 1, max_value: 65534 }
     area: { type: ipv4, use: id }
     bfd: bool
```

### Comparing `networklab-1.8.0.post2/netsim/modules/srv6.py` & `networklab-1.8.1/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/vlan.py` & `networklab-1.8.1/netsim/modules/vlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/vlan.yml` & `networklab-1.8.1/netsim/modules/vlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/vrf.py` & `networklab-1.8.1/netsim/modules/vrf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/vrf.yml` & `networklab-1.8.1/netsim/modules/vrf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/modules/vxlan.py` & `networklab-1.8.1/netsim/modules/vxlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,20 +103,27 @@
   # Search for additional loopback interfaces with vxlan.vtep' flag, and use the first one
   for intf in node.interfaces:
     if intf.get('type', '') == 'loopback' and 'vxlan' in intf and intf.vxlan.get('vtep', False):
       vtep_interface = intf
       loopback_name = intf.ifname
       break
 
-  if topology.defaults.vxlan.use_v6_vtep and not 'ipv6' in vtep_interface:
-    log.error(
-      f'You want to use IPv6 VTEP -- VXLAN module needs an IPv6 address on loopback interface of {node.name}',
-      log.IncorrectValue,
-      'vxlan')
-    return False
+  if topology.defaults.vxlan.use_v6_vtep:
+    features = devices.get_device_features(node,topology.defaults)
+    if not features.get('vxlan.vtep6'):
+      log.error(
+        f'Device {node.device} (node {node.name}) does not support VXLAN over IPv6',
+        log.IncorrectValue,
+        'vxlan')
+    if 'ipv6' not in vtep_interface:
+      log.error(
+        f'You want to use IPv6 VTEP -- VXLAN module needs an IPv6 address on loopback interface of {node.name}',
+        log.IncorrectValue,
+        'vxlan')
+      return False
 
   if not 'ipv4' in vtep_interface and not topology.defaults.vxlan.use_v6_vtep:
     log.error(
       f'VXLAN module needs an IPv4 address on loopback interface of {node.name}',
       log.IncorrectValue,
       'vxlan')
     return False
```

### Comparing `networklab-1.8.0.post2/netsim/outputs/__init__.py` & `networklab-1.8.1/netsim/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/ansible.py` & `networklab-1.8.1/netsim/outputs/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/common.py` & `networklab-1.8.1/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/d2.py` & `networklab-1.8.1/netsim/outputs/d2.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/d2.yml` & `networklab-1.8.1/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/devices.py` & `networklab-1.8.1/netsim/outputs/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/graph.py` & `networklab-1.8.1/netsim/outputs/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/graphite.py` & `networklab-1.8.1/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/provider.py` & `networklab-1.8.1/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/report.py` & `networklab-1.8.1/netsim/outputs/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/tools.py` & `networklab-1.8.1/netsim/outputs/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/outputs/yaml.py` & `networklab-1.8.1/netsim/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/providers/__init__.py` & `networklab-1.8.1/netsim/providers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,20 @@
 
   def post_stop_lab(self, topology: Box) -> None:
     pass
 
   def post_configuration_create(self, topology: Box) -> None:
     pass
 
+  def get_lab_status(self) -> Box:
+    return get_empty_box()
+  
+  def get_node_name(self, node: str, topology: Box) -> str:
+    return node
+
   """
   Generic provider pre-transform processing: Mark multi-provider links
   """
   def pre_transform(self,topology : Box) -> None:
     if not 'links' in topology:
       return
```

### Comparing `networklab-1.8.0.post2/netsim/providers/clab.py` & `networklab-1.8.1/netsim/providers/clab.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #
 # Containerlab provider module
 #
-import subprocess
 import typing
-import shutil
+import json
 from box import Box
 
 from . import _Provider,get_forwarded_ports
 from ..utils import log
-from ..data import filemaps
+from ..data import filemaps, get_empty_box
 from ..cli import is_dry_run,external_commands
 
 def list_bridges( topology: Box ) -> typing.Set[str]:
   return { l.bridge for l in topology.links if l.bridge and l.node_count != 2 and not 'external_bridge' in l.clab }
 
 def use_ovs_bridge( topology: Box ) -> bool:
     return topology.defaults.providers.clab.bridge_type == "ovs-bridge"
@@ -129,7 +128,37 @@
   def post_stop_lab(self, topology: Box) -> None:
     log.print_verbose('post-stop hook for Containerlab, cleaning up any bridges')
     for brname in list_bridges(topology):
       if use_ovs_bridge(topology):
         destroy_ovs_bridge(brname)
       else:
         destroy_linux_bridge(brname)
+
+  def get_lab_status(self) -> Box:
+    try:
+      status = external_commands.run_command(
+                  'docker ps --format json',
+                  check_result=True,
+                  ignore_errors=True,
+                  return_stdout=True)
+      
+      stat_box = get_empty_box()
+      if not isinstance(status,str):
+        return stat_box
+      try:
+        for line in status.split('\n'):
+          if not line.startswith('{'):
+            continue
+          docker_stats = json.loads(line)
+          stat_box[docker_stats['Names']].status = docker_stats['Status']
+          stat_box[docker_stats['Names']].image = docker_stats['Image']
+      except Exception as ex:
+        log.error(f'Cannot get Docker status: {ex}',category=log.FatalError,module='clab')
+        return stat_box
+
+      return stat_box
+    except:
+      log.error('Cannot execute "docker ps": {ex}',category=log.FatalError,module='clab')
+      return get_empty_box()
+
+  def get_node_name(self, node: str, topology: Box) -> str:
+    return f'clab-{ topology.name }-{ node }'
```

### Comparing `networklab-1.8.0.post2/netsim/providers/clab.yml` & `networklab-1.8.1/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/providers/external.py` & `networklab-1.8.1/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/providers/libvirt.py` & `networklab-1.8.1/netsim/providers/libvirt.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 import os
 import typing
 from box import Box
 import pathlib
 import tempfile
 import netaddr
 
-from ..data import types
+from ..data import types,get_empty_box
 from ..utils import log
 from ..utils import files as _files
 from . import _Provider
+from ..augment import devices
 from ..augment.links import get_link_by_index
 from ..cli import is_dry_run,external_commands
 
 LIBVIRT_MANAGEMENT_NETWORK_NAME  = "vagrant-libvirt"
 LIBVIRT_MANAGEMENT_BRIDGE_NAME   = "libvirt-mgmt"
 LIBVIRT_MANAGEMENT_TEMPLATE_PATH = "templates/provider/libvirt"
 LIBVIRT_MANAGEMENT_TEMPLATE_NAME = "vagrant-libvirt.xml"
@@ -181,15 +182,16 @@
   types.must_be_int(libvirt_defaults,'batch_size','defaults.providers.libvirt',module='libvirt',min_value=1,max_value=50)
   types.must_be_int(libvirt_defaults,'batch_interval','defaults.providers.libvirt',module='libvirt',min_value=1,max_value=1000)
   log.exit_on_error()
 
   batch_size = libvirt_defaults.batch_size
   start_cmd  = libvirt_defaults.start
   libvirt_defaults.start = []
-  node_list = list(topology.nodes.keys())
+  node_list = [ n_name for n_name in topology.nodes.keys() 
+                  if devices.get_provider(topology.nodes[n_name],topology.defaults) == 'libvirt' ]
 
   while True:
     libvirt_defaults.start.append(start_cmd + " " + " ".join(node_list[:batch_size]))     # Add up to batch_size nodes to the start command
     if len(node_list) <= batch_size:
       break
     node_list = node_list[batch_size:]
     if libvirt_defaults.batch_interval:
@@ -215,15 +217,15 @@
     _Provider.pre_transform(self,topology)
 
     for l in topology.links:
       if l.get('libvirt.uplink',None):                           # Set 'public' attribute if the link has an uplink
         if not 'public' in l.libvirt:                            # ... but no 'public' libvirt attr
           l.libvirt.public = 'bridge'                            # ... default mode is bridge (MACVTAP)
 
-      if l.get('libvirt.provider',None):
+      if l.get('libvirt.provider',None) and 'vlan' not in l.type:
         l.type = 'lan'
         if not 'bridge' in l:
           l.bridge = "%s_%d" % (topology.name[0:10],l.linkindex)
 
   def transform_node_images(self, topology: Box) -> None:
     self.node_image_version(topology)
 
@@ -320,7 +322,36 @@
       log.print_verbose(f"... network {brname} maps into {linux_bridge}")
       if not external_commands.run_command(
           ['sudo','sh','-c',f'echo 0x4000 >/sys/class/net/{linux_bridge}/bridge/group_fwd_mask']):
         log.error(f"Cannot set forwarding mask on Linux bridge {linux_bridge}")
         continue
 
       log.print_verbose(f"... setting LLDP enabled flag on {linux_bridge}")
+
+  def get_lab_status(self) -> Box:
+    try:
+      status = external_commands.run_command(
+                  'vagrant status --machine-readable',
+                  check_result=True,
+                  ignore_errors=True,
+                  return_stdout=True)
+      
+      stat_box = get_empty_box()
+      if not isinstance(status,str):
+        return stat_box
+      try:
+        for line in status.split('\n'):
+          items = line.split(',')
+          if len(items) >= 4:
+            if items[2] == 'state-human-short':
+              stat_box[items[1]].status = items[3]
+      except Exception as ex:
+        log.error(f'Cannot get Vagrant status: {ex}',category=log.FatalError,module='libvirt')
+        return stat_box
+
+      return stat_box
+    except:
+      log.error('Cannot execute "vagrant status --machine-readable": {ex}',category=log.FatalError,module='libvirt')
+      return get_empty_box()
+
+  def get_node_name(self, node: str, topology: Box) -> str:
+    return f'{ topology.name.split(".")[0] }_{ node }'
```

### Comparing `networklab-1.8.0.post2/netsim/providers/libvirt.yml` & `networklab-1.8.1/netsim/providers/libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/clab/clab.j2` & `networklab-1.8.1/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/clab/cumulus/hosts.j2` & `networklab-1.8.1/netsim/templates/provider/clab/cumulus/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.8.1/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/clab/frr/hosts.j2` & `networklab-1.8.1/netsim/templates/provider/clab/frr/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.8.1/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/external/external.j2` & `networklab-1.8.1/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
     guest_name = "{{ name }}"
 
     {{ name }}.vm.synced_folder ".", "/vagrant", disabled: true
     {{ name }}.vm.allow_fstab_modification = false
     {{ name }}.vm.allow_hosts_modification = false
     {{ name }}.ssh.insert_key = false
     {{ name }}.ssh.password = "vagrant"
-    {{ name }}.vm.boot_timeout = 300
+    {{ name }}.vm.boot_timeout = 600
     {{ name }}.vm.guest = :freebsd
 
     {{ name }}.vm.provider :libvirt do |domain|
       domain.default_prefix = "#{cwd}_"
       domain.features = ['acpi','apic','pae']
-      domain.cpus = 2
+      domain.cpus = 4
       domain.memory = 8192
       domain.disk_bus = "ide"
       domain.driver = "kvm"
       domain.nic_model_type = "e1000"
       domain.graphics_type = "none"
     end
```

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.8.1/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/vptx-domain.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/vptx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.8.1/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.8.1/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/tools/__init__.py` & `networklab-1.8.1/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/tools/graphite.py` & `networklab-1.8.1/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/tools/graphite.yml` & `networklab-1.8.1/netsim/tools/graphite.yml`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     docker run -d --rm
       {sys.docker_net}
       -v "$(pwd)/graphite/graphite-default.json":/htdocs/default/default.json
       -p { 8080 + defaults.multilab.id if defaults.multilab.id else 8080 }:80
       --name '{name}_graphite'
       netreplica/graphite
   message:
-    Open http://127.0.0.1:{ 8080 + defaults.multilab.id if defaults.multilab.id else 8080 }/graphite/ in your browser
+    Open http://{sys.ipaddr}:{ 8080 + defaults.multilab.id if defaults.multilab.id else 8080 }/graphite/ in your browser
   down:
     docker kill '{name}_graphite'
 config:
 - dest: graphite-default.json
   render: graphite
 attributes:
   node:
```

### Comparing `networklab-1.8.0.post2/netsim/tools/suzieq.yml` & `networklab-1.8.1/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/topology-defaults.yml` & `networklab-1.8.1/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/utils/bgp.py` & `networklab-1.8.1/netsim/utils/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/utils/callback.py` & `networklab-1.8.1/netsim/utils/callback.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,11 +32,13 @@
     except (ImportError, AttributeError):
       if abort:
         log.fatal(f"Failed to load specific module: {sys.exc_info()[1]}")
       else:
         print(f"Failed to load specific module: {sys.exc_info()[1]}")
       return None
 
-  def call(self, name: str, *args: typing.Any, **kwargs: typing.Any) -> None:
+  def call(self, name: str, *args: typing.Any, **kwargs: typing.Any) -> typing.Any:
     method = getattr(self,name,None)
     if method:
-      method(*args, **kwargs)
+      return method(*args, **kwargs)
+    else:
+      return None
```

### Comparing `networklab-1.8.0.post2/netsim/utils/files.py` & `networklab-1.8.1/netsim/utils/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import pathlib
 import importlib
 import importlib.util
 import os
 import sys
 import typing
-import fnmatch
 
 from . import log
 from ..data import global_vars
 
 try:
   from importlib import resources
   new_resources = hasattr(resources,'files')
@@ -75,26 +74,33 @@
 
 """
 Transform a search path into an absolute search path
 
 * replace 'package:' with get_moddir()
 * add topology directory to any other path
 """
+def expand_package(path: str) -> pathlib.Path:
+  return get_moddir () / path.replace('package:','')
+
 def absolute_search_path(
       path: typing.List[str],
       curdir: str = '.') -> typing.List[str]:
   a_path = []
   for p_entry in path:
     if 'package:' in p_entry:
-      p_abs = get_moddir () / p_entry.replace('package:','')
+      p_abs = expand_package(p_entry)
     elif 'topology:' in p_entry:
       topology = global_vars.get_topology()
       if topology:
-        topo_dir = os.path.dirname(topology.input[0])+"/"
-        p_abs = pathlib.Path(p_entry.replace('topology:',topo_dir))
+        topo_name = topology.input[0]
+        if topo_name.startswith('package:'):
+          p_abs = expand_package(os.path.dirname(topo_name))
+        else:
+          topo_dir = os.path.dirname(topo_name)+"/"
+          p_abs = pathlib.Path(p_entry.replace('topology:',topo_dir))
       else:
         continue
     elif p_entry.find('~') == 0:
       p_abs = pathlib.Path(os.path.expanduser(p_entry))
     elif p_entry[0] in ['.','/']:
       p_abs = pathlib.Path(p_entry)    
     else:
@@ -117,19 +123,20 @@
 
   return None
 
 #
 # Get a list of files matching a glob pattern
 #
 def get_globbed_files(path: typing.Any, glob: str) -> list:
+  if isinstance(path,str):
+    path = pathlib.Path(path)
   if isinstance(path,pathlib.Path):
     return [ str(fname) for fname in list(path.glob(glob)) ]
   else:
-    file_names = list(path.iterdir())
-    return fnmatch.filter(file_names,glob)
+    log.fatal(f'Internal error: invalid argument to get_globbed_files: {path}')
 
 #
 # Get a path object that can be used to find files in a file system or in the package
 #
 
 def get_traversable_path(dir_name : str) -> typing.Any:
   if 'package:' in dir_name:
```

### Comparing `networklab-1.8.0.post2/netsim/utils/log.py` & `networklab-1.8.1/netsim/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 * Append hints to error log (needed for CI test cases), then print them to
   terminal or file
 """
 def print_more_hints(
       h_list: typing.Union[list,str],   # Hint split into lines
       h_name: str='HINT',               # Hint header
       h_color: str='green',             # Color of hint header
+      h_warning: bool=False,            # is this a warning hint?
       cleanup: bool=True) -> None:      # Remove empty lines from hint lines?
 
   if isinstance(h_list,str):
     h_width = min(strings.rich_err_width,100)
     if strings.rich_err_color:
       h_width = h_width - 10
 
@@ -146,15 +147,16 @@
     h_list = [ line for line in h_list if line ]
   if not h_list:
     return
 
   global _ERROR_LOG
   h_first = True
   for line in h_list:
-    _ERROR_LOG.append(f"... {line}")                        # Convention: hints in traditional output are prefaced with ...
+    if not h_warning:
+      _ERROR_LOG.append(f"... {line}")                      # Convention: hints in traditional output are prefaced with ...
     if strings.rich_err_color:
       if h_first:                                           # First hint line on color-capable TTY: print hint header
         strings.print_colored_text(strings.pad_err_code(h_name),h_color,stderr=True)
         print(line,file=sys.stderr)
         h_first = False
       else:
         print(" "*10+line,file=sys.stderr)                  # Otherwise print another line indented to align with the previous one
@@ -198,18 +200,18 @@
         stderr=True)
       mod_txt = f'{module}: ' if module else ''                     # Skip module header if it's explicitly set to empty
       print(f'{mod_txt}{text}',file=sys.stderr)
     else:
       print(err_line,file=sys.stderr)
 
   if more_hints is not None:                                        # Caller supplied hints, print them with HINT label
-    print_more_hints(more_hints)
+    print_more_hints(more_hints,h_warning=category is Warning)
 
   if more_data is not None:                                         # Caller supplied data, print it with DATA label
-    print_more_hints(more_data,'DATA','bright_black')
+    print_more_hints(more_data,'DATA','bright_black',h_warning=category is Warning)
 
   if hint is None:                                                  # No pointers to static hints
     return
 
   from ..data.global_vars import get_topology
   from .strings import extra_data_printout
 
@@ -217,19 +219,20 @@
   if topology is None:                                              # No valid topology ==> no static hints
     return
 
   mod_hints = topology.defaults.hints[module]                       # Get static hints for current module
 
   if mod_hints[hint]:                                               # Do we know what to do?
     hint_printout = extra_data_printout(mod_hints[hint],width=90)   # Format the hint for traditional printout
-    _ERROR_LOG.extend(hint_printout.split("\n"))
+    if category is not Warning:
+      _ERROR_LOG.extend(hint_printout.split("\n"))
     if strings.rich_err_color:
       l_width = min(strings.rich_err_width-10,100)
       hint_lines = strings.wrap_text_into_lines(mod_hints[hint],width=l_width)
-      print_more_hints(hint_lines,'HINT','green')
+      print_more_hints(hint_lines,'HINT','green',h_warning=category is Warning)
     else:
       print(hint_printout,file=sys.stderr)
 
     mod_hints[hint] = ''
 
 def exit_on_error() -> None:
   global _ERROR_LOG
```

### Comparing `networklab-1.8.0.post2/netsim/utils/read.py` & `networklab-1.8.1/netsim/utils/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 
     k = k.lower()                                 # Normalize to lowercase
     if not k.startswith('netlab_'):               # Skip non-netlab variables
       continue
 
     k = k.replace('netlab_','',1)                 # Drop the netlab_ prefix
     k = k.replace('_','.')                        # Replace underscores with dots
+    k = k.replace('..','_')                       # Turn __ (..) back into a single underscore
     topology.defaults[k] = v                      # And set the value
 
 #
 # Load the topology and defaults
 #
 # * Read the topology from fname
 # * Build the list of defaults
```

### Comparing `networklab-1.8.0.post2/netsim/utils/sort.py` & `networklab-1.8.1/netsim/utils/sort.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/utils/status.py` & `networklab-1.8.1/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/utils/strings.py` & `networklab-1.8.1/netsim/utils/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,20 +111,25 @@
 
 """
 confirm: print the prompt and wait for a yes/no answer
 """
 def confirm(prompt: str) -> bool:
   prompt = f'{prompt} [y/n]'
 
-  while True:
-    answer = input(prompt).lower()
-    if answer in ['y','yes']:
-      return True
-    if answer in ['n','no']:
-      return False
+  try:
+    while True:
+      answer = input(prompt).lower()
+      if answer in ['y','yes']:
+        return True
+      if answer in ['n','no']:
+        return False
+  except KeyboardInterrupt as ex:
+    from . import log
+    print()
+    log.fatal('Aborted by user')
 
 """
 print text table
 """
 def print_table(
       heading: typing.List[str],
       rows: typing.List[typing.List[str]],
```

### Comparing `networklab-1.8.0.post2/netsim/utils/templates.py` & `networklab-1.8.1/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/netsim/utils/versioning.py` & `networklab-1.8.1/netsim/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/networklab.egg-info/PKG-INFO` & `networklab-1.8.1/networklab.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.8.0.post2
+Version: 1.8.1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0). It contains [numerous new features](https://netlab.tools/release/1.8/) that might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use [release 1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.0.post2/networklab.egg-info/SOURCES.txt` & `networklab-1.8.1/networklab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,21 +59,22 @@
 netsim/ansible/tasks/fetch-config/srlinux.yml
 netsim/ansible/tasks/fetch-config/sros.yml
 netsim/ansible/tasks/fetch-config/vyos.yml
 netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
 netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
 netsim/ansible/tasks/frr/deploy-config.yml
 netsim/ansible/tasks/frr/mpls-clab.yml
-netsim/ansible/tasks/iosxr/initial.yml
 netsim/ansible/tasks/linux/dhcp.yml
 netsim/ansible/tasks/linux/initial-clab.yml
 netsim/ansible/tasks/nxos/initial.yml
 netsim/ansible/tasks/readiness-check/arubacx.yml
 netsim/ansible/tasks/readiness-check/dellos10.yml
 netsim/ansible/tasks/readiness-check/eos-clab.yml
+netsim/ansible/tasks/readiness-check/iosxr-clab.yml
+netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml
 netsim/ansible/tasks/readiness-check/routeros7.yml
 netsim/ansible/tasks/readiness-check/vptx.yml
 netsim/ansible/tasks/readiness-check/vsrx.yml
 netsim/ansible/tasks/vmx/initial.yml
 netsim/ansible/templates/missing.j2
 netsim/ansible/templates/bfd/arubacx.j2
 netsim/ansible/templates/bfd/cumulus.j2
@@ -92,15 +93,14 @@
 netsim/ansible/templates/bgp/asa.macro.j2
 netsim/ansible/templates/bgp/cumulus.j2
 netsim/ansible/templates/bgp/cumulus_nvue.j2
 netsim/ansible/templates/bgp/dellos10.j2
 netsim/ansible/templates/bgp/dellos10.macro.j2
 netsim/ansible/templates/bgp/eos.j2
 netsim/ansible/templates/bgp/eos.macro.j2
-netsim/ansible/templates/bgp/frr.bgp-config.j2
 netsim/ansible/templates/bgp/frr.j2
 netsim/ansible/templates/bgp/ios.j2
 netsim/ansible/templates/bgp/ios.macro.j2
 netsim/ansible/templates/bgp/iosxr.j2
 netsim/ansible/templates/bgp/junos.j2
 netsim/ansible/templates/bgp/none.j2
 netsim/ansible/templates/bgp/nxos.j2
@@ -253,16 +253,15 @@
 netsim/ansible/templates/ospf/ios.j2
 netsim/ansible/templates/ospf/ios.ospfv2.j2
 netsim/ansible/templates/ospf/ios.ospfv3.j2
 netsim/ansible/templates/ospf/iosxr.j2
 netsim/ansible/templates/ospf/iosxr.ospfv2.j2
 netsim/ansible/templates/ospf/iosxr.ospfv3.j2
 netsim/ansible/templates/ospf/junos.j2
-netsim/ansible/templates/ospf/junos.ospfv2.j2
-netsim/ansible/templates/ospf/junos.ospfv3.j2
+netsim/ansible/templates/ospf/junos.macro.j2
 netsim/ansible/templates/ospf/none.j2
 netsim/ansible/templates/ospf/nxos.j2
 netsim/ansible/templates/ospf/nxos.ospfv2.j2
 netsim/ansible/templates/ospf/nxos.ospfv3.j2
 netsim/ansible/templates/ospf/routeros.j2
 netsim/ansible/templates/ospf/routeros7.j2
 netsim/ansible/templates/ospf/routeros7.ospf-include.j2
@@ -307,26 +306,30 @@
 netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
 netsim/ansible/templates/vrf/dellos10.bgp.j2
 netsim/ansible/templates/vrf/dellos10.j2
 netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
 netsim/ansible/templates/vrf/eos.bgp-macro.j2
 netsim/ansible/templates/vrf/eos.bgp.j2
 netsim/ansible/templates/vrf/eos.j2
-netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
+netsim/ansible/templates/vrf/eos.ospfv2.j2
+netsim/ansible/templates/vrf/eos.ospfv3.j2
 netsim/ansible/templates/vrf/frr.bgp.j2
 netsim/ansible/templates/vrf/frr.frr-config.j2
 netsim/ansible/templates/vrf/frr.j2
-netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
+netsim/ansible/templates/vrf/frr.ospfv2.j2
+netsim/ansible/templates/vrf/frr.ospfv3.j2
 netsim/ansible/templates/vrf/ios.bgp-macro.j2
 netsim/ansible/templates/vrf/ios.bgp.j2
 netsim/ansible/templates/vrf/ios.j2
 netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+netsim/ansible/templates/vrf/ios.ospfv2.j2
+netsim/ansible/templates/vrf/ios.ospfv3.j2
 netsim/ansible/templates/vrf/junos.bgp.j2
 netsim/ansible/templates/vrf/junos.j2
-netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
+netsim/ansible/templates/vrf/junos.ospf-macro.j2
 netsim/ansible/templates/vrf/nxos.bgp.j2
 netsim/ansible/templates/vrf/nxos.j2
 netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
 netsim/ansible/templates/vrf/routeros.bgp-macro.j2
 netsim/ansible/templates/vrf/routeros.bgp.j2
 netsim/ansible/templates/vrf/routeros.j2
 netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
@@ -489,15 +492,14 @@
 netsim/extra/bgp.session/vyos.j2
 netsim/extra/ebgp.multihop/arubacx.j2
 netsim/extra/ebgp.multihop/cumulus.j2
 netsim/extra/ebgp.multihop/defaults.yml
 netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
 netsim/extra/ebgp.multihop/eos.j2
 netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
-netsim/extra/ebgp.multihop/frr.bgp-config.j2
 netsim/extra/ebgp.multihop/frr.j2
 netsim/extra/ebgp.multihop/ios.j2
 netsim/extra/ebgp.multihop/plugin.py
 netsim/extra/ebgp.multihop/srlinux.j2
 netsim/extra/ebgp.multihop/sros.j2
 netsim/extra/ebgp.utils/plugin.py
 netsim/extra/fabric/defaults.yml
@@ -649,13 +651,16 @@
 netsim/utils/log.py
 netsim/utils/read.py
 netsim/utils/sort.py
 netsim/utils/status.py
 netsim/utils/strings.py
 netsim/utils/templates.py
 netsim/utils/versioning.py
+netsim/validate/__init__.py
+netsim/validate/frr.py
+netsim/validate/linux.py
 networklab.egg-info/PKG-INFO
 networklab.egg-info/SOURCES.txt
 networklab.egg-info/dependency_links.txt
 networklab.egg-info/requires.txt
 networklab.egg-info/top_level.txt
 tests/test_transformation.py
```

### Comparing `networklab-1.8.0.post2/setup.py` & `networklab-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.0.post2/tests/test_transformation.py` & `networklab-1.8.1/tests/test_transformation.py`

 * *Files identical despite different names*

