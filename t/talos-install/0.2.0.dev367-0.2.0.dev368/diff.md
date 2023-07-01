# Comparing `tmp/talos_install-0.2.0.dev367.tar.gz` & `tmp/talos_install-0.2.0.dev368.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.0.dev367.tar", last modified: Thu Jun 15 16:56:46 2023, max compression
+gzip compressed data, was "talos_install-0.2.0.dev368.tar", last modified: Sat Jul  1 08:45:36 2023, max compression
```

## Comparing `talos_install-0.2.0.dev367.tar` & `talos_install-0.2.0.dev368.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.993787 talos_install-0.2.0.dev367/
--rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/AUTHORS
--rw-rw-r--   0 installer  (3002) installer  (3002)    12013 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/ChangeLog
--rw-rw-r--   0 installer  (3002) installer  (3002)     3378 2023-06-15 16:56:45.993787 talos_install-0.2.0.dev367/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     2740 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/README.md
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.965787 talos_install-0.2.0.dev367/ansible/
--rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/ansible.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.965787 talos_install-0.2.0.dev367/ansible/group_vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      702 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/group_vars/all.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.962787 talos_install-0.2.0.dev367/ansible/roles/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.951787 talos_install-0.2.0.dev367/ansible/roles/cli/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.965787 talos_install-0.2.0.dev367/ansible/roles/cli/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/files/FOUNDMEDEVKEY
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.965787 talos_install-0.2.0.dev367/ansible/roles/cli/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.967787 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1197 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/clone.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1497 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/env.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/logrotate.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      401 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     2718 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/tasks/web.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.969787 talos_install-0.2.0.dev367/ansible/roles/cli/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3814 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/agent.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      484 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/app.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      766 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/cli.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2477 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/env_talos.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1347 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/globals.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/my-httpd.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      379 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/passwords.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/talos-logrotate.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/talos.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/cli/templates/talospass.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.951787 talos_install-0.2.0.dev367/ansible/roles/common/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.969787 talos_install-0.2.0.dev367/ansible/roles/common/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/common/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.970787 talos_install-0.2.0.dev367/ansible/roles/common/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/common/tasks/install_extra_pkgs.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/common/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/common/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.951787 talos_install-0.2.0.dev367/ansible/roles/gather_facts/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.970787 talos_install-0.2.0.dev367/ansible/roles/gather_facts/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/gather_facts/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.971787 talos_install-0.2.0.dev367/ansible/roles/gather_facts/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      930 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/gather_facts/vars/RedHat.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      929 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/gather_facts/vars/Rocky.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.952787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.952787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.971787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/files/inventory_plugins/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.971787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_ansible/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.971787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_ansible/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_ansible/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_ansible/templates/ansible.cfg.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.953787 talos_install-0.2.0.dev367/ansible/roles/install_certificates/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_certificates/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_certificates/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_certificates/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_certificates/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.953787 talos_install-0.2.0.dev367/ansible/roles/install_docker/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_docker/handlers/
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/handlers/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.972787 talos_install-0.2.0.dev367/ansible/roles/install_docker/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.973787 talos_install-0.2.0.dev367/ansible/roles/install_docker/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.973787 talos_install-0.2.0.dev367/ansible/roles/install_docker/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/templates/daemon.json.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_docker/templates/docker-ce.repo.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.954787 talos_install-0.2.0.dev367/ansible/roles/install_python/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.973787 talos_install-0.2.0.dev367/ansible/roles/install_python/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_python/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/install_python/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/install_python/vars/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.958787 talos_install-0.2.0.dev367/ansible/roles/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/nagios/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.955787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.954787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/conf.d/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.974787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/monitor/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/monitor/.ID
--rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/etc/nagios/resource.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.957787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.975787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.955787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/apache2/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.975787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.956787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.975787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/apache/
--rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/apache/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.975787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/nagios/
--rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.976787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/postfix/
--rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.976787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
--rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.957787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.957787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.976787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.977787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.977787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
--rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1585 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
--rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.978787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.978787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
--rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
--rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.957787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.978787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.958787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.958787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/local/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.979787 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/local/bin/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.979787 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.981787 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/cgi.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/contacts.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2765 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/localhost.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/nagios/templates/nagios.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.960787 talos_install-0.2.0.dev367/ansible/roles/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.981787 talos_install-0.2.0.dev367/ansible/roles/opendcim/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.982787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/apache2.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/apache2.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/default.sql
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.959787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.959787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.983787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/drawings/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.983787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/pictures/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/mysqld.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.959787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.959787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.960787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.983787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.984787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
--rw-rw-r--   0 installer  (3002) installer  (3002)    53198 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
--rw-rw-r--   0 installer  (3002) installer  (3002)    20094 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.984787 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/pre-conf.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/files/startup.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.984787 talos_install-0.2.0.dev367/ansible/roles/opendcim/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.985787 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.986787 talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/first-run.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/opendcim.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.961787 talos_install-0.2.0.dev367/ansible/roles/os_tune/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.986787 talos_install-0.2.0.dev367/ansible/roles/os_tune/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/os_tune/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.961787 talos_install-0.2.0.dev367/ansible/roles/talos_users/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.986787 talos_install-0.2.0.dev367/ansible/roles/talos_users/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/talos_users/files/talos
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.987787 talos_install-0.2.0.dev367/ansible/roles/talos_users/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/talos_users/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.987787 talos_install-0.2.0.dev367/ansible/roles/talos_users/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      634 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/talos_users/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.962787 talos_install-0.2.0.dev367/ansible/roles/uninstall/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.987787 talos_install-0.2.0.dev367/ansible/roles/uninstall/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.987787 talos_install-0.2.0.dev367/ansible/roles/uninstall/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.988787 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      682 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/cli.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/docker.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      339 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/user.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.988787 talos_install-0.2.0.dev367/ansible/roles/wiki/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.989787 talos_install-0.2.0.dev367/ansible/roles/wiki/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      572 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.989787 talos_install-0.2.0.dev367/ansible/roles/wiki/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/meta/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/requirements.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.990787 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/compose.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      161 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/init.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      325 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.990787 talos_install-0.2.0.dev367/ansible/roles/wiki/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1275 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/templates/docker-compose.yml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/templates/wiki.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/roles/wiki/templates/wikidump.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1835 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/ansible/site.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.991787 talos_install-0.2.0.dev367/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      293 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/etc/globals.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev367/etc/inventory
--rw-rw-r--   0 installer  (3002) installer  (3002)     1090 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/etc/talos.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-06-15 16:56:45.998787 talos_install-0.2.0.dev367/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-06-15 16:56:29.000000 talos_install-0.2.0.dev367/setup.py
--rwxrwxr-x   0 installer  (3002) installer  (3002)    10147 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev367/talos_install
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-06-15 16:56:45.993787 talos_install-0.2.0.dev367/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3378 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     5618 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/not-zip-safe
--rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/pbr.json
--rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev367/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.948916 talos_install-0.2.0.dev368/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13162 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     4233 2023-07-01 08:45:36.949916 talos_install-0.2.0.dev368/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3573 2023-06-30 16:33:53.000000 talos_install-0.2.0.dev368/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.920916 talos_install-0.2.0.dev368/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.920916 talos_install-0.2.0.dev368/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      672 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.917916 talos_install-0.2.0.dev368/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.905916 talos_install-0.2.0.dev368/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.920916 talos_install-0.2.0.dev368/ansible/roles/cli/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/files/FOUNDMEDEVKEY
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.921916 talos_install-0.2.0.dev368/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.922916 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1197 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1512 2023-06-16 10:28:42.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      467 2023-06-30 16:15:20.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2692 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.924916 talos_install-0.2.0.dev368/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3814 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      453 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      772 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2433 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1381 2023-06-16 10:28:42.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-06-16 12:33:23.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      379 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.906916 talos_install-0.2.0.dev368/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.924916 talos_install-0.2.0.dev368/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.925916 talos_install-0.2.0.dev368/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.906916 talos_install-0.2.0.dev368/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.925916 talos_install-0.2.0.dev368/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.926916 talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      949 2023-06-29 13:29:49.000000 talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      948 2023-06-29 13:29:49.000000 talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.907916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.906916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.926916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.926916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.927916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.927916 talos_install-0.2.0.dev368/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.907916 talos_install-0.2.0.dev368/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.927916 talos_install-0.2.0.dev368/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.927916 talos_install-0.2.0.dev368/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.908916 talos_install-0.2.0.dev368/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.928916 talos_install-0.2.0.dev368/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.928916 talos_install-0.2.0.dev368/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.928916 talos_install-0.2.0.dev368/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.909916 talos_install-0.2.0.dev368/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.913916 talos_install-0.2.0.dev368/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.910916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.909916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.929916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.930916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.930916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.912916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.930916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.910916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.930916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.911916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.912916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.911916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.931916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.932916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.933916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1585 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-06-16 10:28:42.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.933916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.934916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.912916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.934916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.912916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.913916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.934916 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.935916 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.936916 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2765 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.915916 talos_install-0.2.0.dev368/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.936916 talos_install-0.2.0.dev368/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      263 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.938916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.913916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.914916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.938916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.938916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.914916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.914916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.914916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.938916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.939916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53198 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20094 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.939916 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.940916 talos_install-0.2.0.dev368/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.940916 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.941916 talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      635 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      157 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.915916 talos_install-0.2.0.dev368/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.941916 talos_install-0.2.0.dev368/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.916916 talos_install-0.2.0.dev368/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.942916 talos_install-0.2.0.dev368/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.942916 talos_install-0.2.0.dev368/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.942916 talos_install-0.2.0.dev368/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      634 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.917916 talos_install-0.2.0.dev368/ansible/roles/uninstall/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.942916 talos_install-0.2.0.dev368/ansible/roles/uninstall/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.943916 talos_install-0.2.0.dev368/ansible/roles/uninstall/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.943916 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      656 2023-06-30 15:05:58.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/cli.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/docker.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      339 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/user.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.944916 talos_install-0.2.0.dev368/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.944916 talos_install-0.2.0.dev368/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      572 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.944916 talos_install-0.2.0.dev368/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.945916 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      161 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/init.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      325 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.946916 talos_install-0.2.0.dev368/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1275 2023-06-15 16:34:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1844 2023-06-30 16:15:20.000000 talos_install-0.2.0.dev368/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.947916 talos_install-0.2.0.dev368/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      311 2023-06-16 10:28:42.000000 talos_install-0.2.0.dev368/etc/example_globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1090 2023-06-15 07:22:43.000000 talos_install-0.2.0.dev368/etc/example_talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.0.dev368/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-07-01 08:45:36.956916 talos_install-0.2.0.dev368/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-06-15 16:56:29.000000 talos_install-0.2.0.dev368/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)    10898 2023-06-30 16:33:24.000000 talos_install-0.2.0.dev368/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-01 08:45:36.948916 talos_install-0.2.0.dev368/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     4233 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5634 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.0.dev368/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-01 08:45:36.000000 talos_install-0.2.0.dev368/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.0.dev367/ChangeLog` & `talos_install-0.2.0.dev368/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,46 @@
 CHANGES
 =======
 
+*  Add Update in talos\_install to update Env config
+*  add import role (install) and sync PB
+* Fix paths
+* Fix psw query after moving system
+* Fix psw query after moving system
+*  review wikiDB
+* Fix output option show
+* Fix output option show
+* Fix Verbosity level and output
+* Fix find playbook
+* Fix completion
+* Chancge show from run to playbook
+* Fix dependency
+* Fix dependency
+* Fix dependency
+* Fix completion fot talos-run --video
+* Add feature to show ansible output during execution in talos-run Fixed #36
+* Add feature to manage roles in talos-playbook Fixed #34
+* Add feature to manage roles in talos-playbook Fixed #34
+* Add feature to manage roles in talos-playbook Fixed #34
+* Skip IP check for unmanaged infra devices
+* Fixes #32
+* Change clean
+* Fix seach PB md5sum
+* improve clean uncommited changes
+* Rename -config  reload in init, add PB update
+* fix exit code on local PB
+* add dcim\_get\_hostinfo
+*  add utils nagios playbook
+* disable opendcim
+* fix invenotry math group=domain
+*  fix typo range compare
+*  fix typo range compare
+* fix tag typo
+* Restyle web homepage
+* Add customer.domain feature, fix max ansible version
 * Add extension for wiki load config, mino fix
 
 0.2.0
 -----
 
 * Fix Home position
 * Remove SWAP\_USAGE for Talos mgmt
```

### Comparing `talos_install-0.2.0.dev367/PKG-INFO` & `talos_install-0.2.0.dev368/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,27 @@
-Metadata-Version: 2.1
-Name: talos_install
-Version: 0.2.0.dev367
-Summary: E4 CLI Manager
-Home-page: https://www.e4company.com/
-Author: "Marco Cicala"
-Author-email: marco.cicala@e4company.com
-License: GNU General Public License v3 (GPLv3)
-Classifier: Environment :: Console
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Unix Shell
-Description-Content-Type: text/markdown
-
 # All in One installation
 
 ## Deploy requirements
 
 Currrent Talos-cli version is still not public, a dev_key is required for deployment.
 
 Ask a `dev_key` and `dev_key.pub` to save in your `$HOME/.ssh` folder.
 
 ## OS requirements
 
 - The supported OS is Rocky Linux 8. Other Rhel like distributions should works, but aren't tested yet.
 
-- An **user with sudo permissions** is MANDATORY, don't use root directly.
+- An **user with sudo permissions** is MANDATORY, don't use root directly. Due to some restrictions talos user (if already present) can't be used for installation
+
+```
+sudo useradd installer
+sudo visudo
+# add installer as sudo user
+sudo su - installer
+'''
 
 ### Packages
 
 - python = 3.9
 - pip = 3.9
 
 ```bash
@@ -51,40 +41,43 @@
 
 The talos_install package can be runned with these options:
 
 - precheck: to prepare system with base requirements
 - deploy: to install components
 - build: to recreate docker images and pull on docker Hub (only for authorized developper)
 - remove: to remove main settings and confurations.
+- update: Update environment from a newer version
 
 > Note that remove doesn't remove installed packages (like docker)
 and doesn't return to original settings (like selinux or firewalld).
 
+### Configuration Files
+
 #### inventory
 
 File `<pip_environment>/share/talos_install/etc/inventory` is dinamically create at code level.
 Changes to this file by user are tatally ignored during execution.
 
 #### ansible.cfg
 
 The default ansible configuration should not be changed.
 By default the `display_ok_hosts` parameter is set to false.
 If you need to display also the OK state please comment the row in
 `<pip_environment>/share/talos_install/ansible/ansible.cfg`
 
-#### talos.yaml
+#### talos.yaml [ REQUIRED ]
 
-Change configuration of config file `<pip_environment>/share/talos_install/etc/talos.yaml`
-to change users configuration.
+Copy configuration file `<pip_environment>/share/talos_install/etc/example_talos.yaml` to your ${HOME} directory.
+Then change users configuration.
 Is not allow to add or delete master and guest configuration
 
-#### global.yaml
+#### global.yaml [ REQUIRED ]
 
-Change configuration of config file `<pip_environment>/share/talos_install/etc/global.yaml`
-to change customer configuration.
+Copy configuration file `<pip_environment>/share/talos_install/etc/example_global.yaml` to your ${HOME} directory.
+Then change customer configuration.
 
 ### Run Installation precheck
 
 ```bash
 talos_install precheck
 ```
 
@@ -120,22 +113,37 @@
 ```bash
  talos-config setup
 ```
 
 Load initial configuration
 
 ```bash
-talos-config reload
+talos-config init
 ```
 
 Check Key Pairs with Talos-cli (needed for update only)
 
 ```bash
 talos-config git_keys
 ```
 
 Check Overall status
 
 ```bash
 talos-config check
 ```
 
+## Known Issue
+
+ansible-core requires the locale have UTF-8 encoding since 2.14.0
+
+Excerpt from the 2.14.0 release notes1
+
+ansible - At startup the filesystem encoding and locale are checked to verify they are UTF-8. If not, the process exits with an error reporting the errant encoding.
+
+Can you share the output of executing locale in a shell, please?
+You probably just have to fix your system language to a UTF-8 variant.
+Or just run ansible using:
+
+```bash
+LANG=C.UTF-8 talos_install <command>
+```
```

### Comparing `talos_install-0.2.0.dev367/ansible/group_vars/all.yaml` & `talos_install-0.2.0.dev368/ansible/group_vars/all.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -19,11 +19,10 @@
   cli_version: '0.2.0'  # tversion
   cli_repo: 'git@github.com:E4-Computer-Engineering/talos-cli.git'
   data_repo: 'git@github.com:E4-Computer-Engineering/talos-data.git'
   nexus_repo: 'srv-nexus01.e4srv:8081'
   dir: "/opt/talos"
   clidir: "/opt/talos/cli"
   datadir: "/opt/talos/cli/data"
-  repodir: "/opt/talos/repos"
   etcdir: "/etc/e4company/talos"
   webdir: "/opt/talos/web"
   logdir: "/var/log/talos"
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/tasks/clone.yaml` & `talos_install-0.2.0.dev368/ansible/roles/cli/tasks/clone.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/tasks/env.yaml` & `talos_install-0.2.0.dev368/ansible/roles/cli/tasks/env.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -37,12 +37,12 @@
         done
       fi
       BCyan="\[\033[1;36m\]"        # Cyan
       BWhite="\[\033[1;37m\]"       # White
       BGreen="\[\033[1;32m\]"       # Green
       BYellow="\[\033[1;33m\]"      # Yellow
       Color_Off="\[\033[0m\]"       # Text Reset
-      export PS1="\r[${BYellow}MASTER${BWhite}|${BCyan}TALOS-CLI${BWhite}] \h | \w ${Color_Off}\n# "
+      export PS1="\r[${BYellow}{{ customer.domain }}${BWhite}|${BCyan}TALOS-CLI${BWhite}] \h | \w ${Color_Off}\n# "
     marker: '# {mark} ANSIBLE MANAGED BLOCK - talos'
     insertbefore: BOF
     create: true
     mode: '0644'
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/tasks/misc.yaml` & `talos_install-0.2.0.dev368/ansible/roles/cli/tasks/misc.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     - "{{ app.etcdir }}/roles"
     - "{{ app.etcdir }}/pos"
     - "{{ app.etcdir }}/profiles"
     - "{{ app.etcdir }}/templates"
     - "{{ app.etcdir }}/benchmarks"
     - "{{ app.logdir }}"
     - "{{ app.logdir }}/.tlist"
-    - "{{ app.repodir }}"
     - "{{ app.etcdir }}/backup"
     - "{{ app.webdir }}/html/obj"
     - ~/MyPlaybooks
     - "{{ master.home }}/.talos"
 
 - name: Copy master ssh keys
   ansible.builtin.copy:
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/tasks/web.yaml` & `talos_install-0.2.0.dev368/ansible/roles/cli/tasks/web.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/templates/agent.sh.j2` & `talos_install-0.2.0.dev368/ansible/roles/cli/templates/agent.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/templates/cli.conf.j2` & `talos_install-0.2.0.dev368/ansible/roles/cli/templates/cli.conf.j2`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 app.name:              {{ app.name }}
 app.cli_version:       {{ app.cli_version }}
 app.cli_repo:          {{ app.cli_repo }}
 app.data_repo:         {{ app.data_repo }}
 app.dir:               {{ app.dir }}
 app.clidir:            {{ app.clidir }}
 app.datadir:           {{ app.datadir }}
-app.repodir:           {{ app.repodir }}
 app.etcdir:            {{ app.etcdir }}
 app.webdir:            {{ app.webdir }}
 app.logdir:            {{ app.logdir }}
 customer.name:         {{ customer.name }}
+customer.domain:         {{ customer.domain }}
 nexus_repository:      {{ app.nexus_repo }}
 data_repository:       {{ app.data_repo }}
 master.user:      {{ master.user }}
 master.uid:       {{ master.uid }}
 master.password:  {{ master.password }}
 master.mail:      {{ master.mail }}
 mgm_password:          {{ mgm_password }}
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/templates/env_talos.j2` & `talos_install-0.2.0.dev368/ansible/roles/cli/templates/env_talos.j2`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 # PATHS
 export TALOS_PATH="{{ app.dir }}"
 
 export TALOS_CLI_PATH="{{ app.clidir }}"
 export TALOS_ETC_PATH="{{ app.etcdir }}"
 export TALOS_DATA_PATH="{{ app.datadir }}"
-export TALOS_REPOS_PATH="{{ app.repodir }}"
 export TALOS_WEB_PATH="{{ app.webdir }}"
 export TALOS_LOG_PATH="{{ app.logdir }}"
 
 export TALOS_TEMPLATE_PATH="$TALOS_ETC_PATH/templates"
 export TALOS_PROFILE_PATH="$TALOS_ETC_PATH/profiles"
 export TALOS_BENCH_PATH="$TALOS_ETC_PATH/benchmarks"
 export TALOS_ROLE_PATH="$TALOS_ETC_PATH/roles"
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/templates/globals.yaml.j2` & `talos_install-0.2.0.dev368/ansible/roles/cli/templates/globals.yaml.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ### Customer settings
 customer:
   name: '{{ customer.name }}'
   timezone: '{{ customer.timezone }}'
+  domain: '{{ customer.domain }}'
 
 ### IDM
 ca_idm:
   enable: '{{ ca_idm.enable }}'
   ipa: '{{ ca_idm.ipa }}'
   ip: '{{ ca_idm.ip }}'
   force_resolve: '{{ ca_idm.force_resolve }}'
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/templates/my-httpd.conf.j2` & `talos_install-0.2.0.dev368/ansible/roles/cli/templates/my-httpd.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/cli/templates/talos.conf.j2` & `talos_install-0.2.0.dev368/ansible/roles/cli/templates/talos.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/common/tasks/misc.yaml` & `talos_install-0.2.0.dev368/ansible/roles/common/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/gather_facts/vars/RedHat.yaml` & `talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/RedHat.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   - python3-argcomplete
   - rust
   - cargo
   - curl
   - sshpass
 
 pkgansible:
-  - ansible>=7,<8
+  - ansible-core>=2.4,<2.14
 
 ### Certificate
 certdir: /etc/pki/ca-trust/source/anchors/
 
 certcmd: update-ca-trust
 
 ### Common
@@ -56,14 +56,15 @@
   - gcc-c++
   - sysstat
   - pssh
   - ipmitool
   - dnf-plugins-core
   - nfs-utils
   - arp-scan
+  - tree
 
 pkgpowertools:
   - pandoc
 
 
 venvcmd: virtualenv-3
 http_service: httpd
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/gather_facts/vars/Rocky.yaml` & `talos_install-0.2.0.dev368/ansible/roles/gather_facts/vars/Rocky.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   - python3-argcomplete
   - rust
   - cargo
   - curl
   - sshpass
 
 pkgansible:
-  - ansible>=7,<8
+  - ansible-core>=2.4,<2.14
 
 ### Certificate
 certdir: /etc/pki/ca-trust/source/anchors/
 
 certcmd: update-ca-trust
 
 ### Common
@@ -56,14 +56,15 @@
   - gcc-c++
   - sysstat
   - pssh
   - ipmitool
   - dnf-plugins-core
   - nfs-utils
   - arp-scan
+  - tree
 
 pkgpowertools:
   - pandoc
 
 venvcmd: virtualenv-3
 http_service: httpd
 php_service: php
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py` & `talos_install-0.2.0.dev368/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/install_ansible/tasks/main.yaml` & `talos_install-0.2.0.dev368/ansible/roles/install_ansible/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/install_ansible/templates/ansible.cfg.j2` & `talos_install-0.2.0.dev368/ansible/roles/install_ansible/templates/ansible.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/install_certificates/tasks/main.yaml` & `talos_install-0.2.0.dev368/ansible/roles/install_certificates/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/install_docker/tasks/main.yaml` & `talos_install-0.2.0.dev368/ansible/roles/install_docker/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/install_docker/templates/docker-ce.repo.j2` & `talos_install-0.2.0.dev368/ansible/roles/install_docker/templates/docker-ce.repo.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/install_python/tasks/main.yaml` & `talos_install-0.2.0.dev368/ansible/roles/install_python/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/nagios/run` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/nagios/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/etc/sv/postfix/run` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/etc/sv/postfix/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php`

 * *Files 0% similar despite different names*

```diff
@@ -123,12 +123,12 @@
 			<li><a href="<?php echo $cfg["cgi_base_url"];?>/extinfo.cgi?type=7" target="<?php echo $link_target;?>">Scheduling Queue</a></li>
 			<li><a href="<?php echo $cfg["cgi_base_url"];?>/config.cgi" target="<?php echo $link_target;?>">Configuration</a></li>
 		</ul>
 	</div>
 </div>
 
 <div class="footer">
-  <h3>TALOS | © 2002-2022<br>E4 COMPUTER ENGINEERING S.p.A.</h3>
+  <h3>TALOS | © 2020-2023<br>E4 COMPUTER ENGINEERING S.p.A.</h3>
 </div>
 
 </body>
 </html>
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios` & `talos_install-0.2.0.dev368/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/build.yaml` & `talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/misc.yaml` & `talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/tasks/run.yaml` & `talos_install-0.2.0.dev368/ansible/roles/nagios/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/templates/Dockerfile.j2` & `talos_install-0.2.0.dev368/ansible/roles/nagios/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/templates/cgi.cfg.j2` & `talos_install-0.2.0.dev368/ansible/roles/nagios/templates/cgi.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/templates/contacts.cfg.j2` & `talos_install-0.2.0.dev368/ansible/roles/nagios/templates/contacts.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/nagios/templates/localhost.cfg.j2` & `talos_install-0.2.0.dev368/ansible/roles/nagios/templates/localhost.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/apache2.conf` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/apache2.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/default.sql` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/default.sql`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/pre-conf.sh` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/pre-conf.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/files/startup.sh` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/files/startup.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/build.yaml` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/misc.yaml` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/tasks/run.yaml` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/Dockerfile.j2` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/opendcim/templates/first-run.sh.j2` & `talos_install-0.2.0.dev368/ansible/roles/opendcim/templates/first-run.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/os_tune/tasks/main.yaml` & `talos_install-0.2.0.dev368/ansible/roles/os_tune/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/talos_users/tasks/main.yaml` & `talos_install-0.2.0.dev368/ansible/roles/talos_users/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/uninstall/tasks/cli.yaml` & `talos_install-0.2.0.dev368/ansible/roles/uninstall/tasks/cli.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -24,9 +24,8 @@
   ansible.builtin.file:
     path: "{{ item }}"
     state: absent
   loop:
     - "{{ app.dir }}"
     - "{{ app.etcdir }}"
     - "{{ app.logdir }}"
-    - "{{ app.repodir }}"
     - "{{ app.webdir }}"
```

### Comparing `talos_install-0.2.0.dev367/ansible/roles/wiki/defaults/main.yaml` & `talos_install-0.2.0.dev368/ansible/roles/wiki/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/wiki/tasks/compose.yaml` & `talos_install-0.2.0.dev368/ansible/roles/wiki/tasks/compose.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/roles/wiki/templates/docker-compose.yml.j2` & `talos_install-0.2.0.dev368/ansible/roles/wiki/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/ansible/site.yaml` & `talos_install-0.2.0.dev368/ansible/site.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
       become: true
       tags: common
       when: cli_action in ['deploy']
 
     - role: cli
       become: true
       tags: cli
-      when: cli_action in ['deploy']
+      when: cli_action in ['deploy','update']
 
     - role: nagios
       become: true
       tags: nagios
       when: cli_action in ['deploy']
 
     - role: opendcim
```

### Comparing `talos_install-0.2.0.dev367/etc/talos.yaml` & `talos_install-0.2.0.dev368/etc/example_talos.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/setup.cfg` & `talos_install-0.2.0.dev368/setup.cfg`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.0.dev367/talos_install` & `talos_install-0.2.0.dev368/talos_install`

 * *Files 5% similar despite different names*

```diff
@@ -57,19 +57,29 @@
     exit 2
   fi
 
   if ! which ansible &>/dev/null ; then
     echo "Missing ansible"
     exit 2
   fi
+
+  if [[ ! -f ${HOME}/globals.yaml ]]; then
+    echo "Missing ${HOME}/globals.yaml, you can copy a sample from <pip_env>/share/talos_install/etc "
+    exit 2
+  fi
+
+  if [[ ! -f ${HOME}/talos.yaml ]]; then
+    echo "Missing ${HOME}/talos.yaml, you can copy a sample from <pip_env>/share/talos_install/etc "
+    exit 2
+  fi
 }
 
 talos_install_menu(){
   title_message="$1"
-  clear
+  clean
   # Get Terminal info
   echo "TALOS-CLI | HPC Manager Platform "
   printf "# $title_message\n\n"
 }
 
 confirm_precheck(){
   talos_install_menu "Talos Precheck"
@@ -84,14 +94,24 @@
     !!! A REBOOT WILL OCCOUR DURING INSTALLATION !!!
     ------------------------------------------------"
     force_install=false
   fi
   confirm_action
 }
 
+confirm_update(){
+  talos_install_menu "Talos update"
+
+  echo "These actions will be performed:
+  - Udpate Talos environment paths
+  - Udpate Talos-cli dependencies
+  "
+  confirm_action
+}
+
 confirm_deploy(){
   talos_install_menu "Talos deploy"
 
   echo "These actions will be performed:
   - Add an user {{ master.user }} with sudo permission.
   - Install python dependencies
   - Install docker and give to {{ master.user }} permission to run containers
@@ -198,14 +218,15 @@
 
 Environment variables:
     extra_opts                         Additional arguments to pass to ansible-playbook
 
 Commands:
     precheck             Prepare OS for installation
     deploy               Deploy and start main talos containers
+    update               Apply Release change
     build                Build talos custom containers
     remove               Uninstall Talos-cli
 EOF
 }
 
 ### MAIN HERE
 
@@ -259,15 +280,15 @@
 long_opts="help,skip-tags:,tags:,key:,extra:,verbose,limit:,forks:,vault-id:,ask-vault-pass,vault-password-file:"
 
 args=$(getopt -o "${short_opts}" -l "${long_opts}" --name "$0" -- "$@") || { usage >&2; exit 2; }
 
 eval set -- "$args"
 
 ANSIBLE_CONFIG="${basedir}/ansible/ansible.cfg"
-config_dir="${basedir}/etc"
+config_dir="${HOME}"
 inventory="${basedir}/etc/inventory"
 playbook="${basedir}/ansible/site.yml"
 verbosity=""
 extra_opts=""
 target=""
 hostdef="[talos]"
 force_install=false
@@ -326,14 +347,21 @@
     verify_step
     confirm_deploy
     f_action=deploy
     action="Deploying Playbooks"
     playbook="${basedir}/ansible/site.yaml"
     extra_opts="$extra_opts -e cli_action=deploy"
     hostdef="[talos]" ;;
+  (update)
+    confirm_update
+    f_action=update
+    action="Update Environment"
+    playbook="${basedir}/ansible/site.yaml"
+    extra_opts="$extra_opts -e cli_action=update"
+    hostdef="[talos]" ;;
   (remove)
     confirm_destroy
     f_action=deploy
     action="Uninstall talos"
     playbook="${basedir}/ansible/site.yaml"
     extra_opts="$extra_opts -e cli_action=remove"
     hostdef="[talos]" ;;
```

### Comparing `talos_install-0.2.0.dev367/talos_install.egg-info/SOURCES.txt` & `talos_install-0.2.0.dev368/talos_install.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,17 @@
 ansible/roles/wiki/tasks/compose.yaml
 ansible/roles/wiki/tasks/init.yaml
 ansible/roles/wiki/tasks/main.yaml
 ansible/roles/wiki/tasks/misc.yaml
 ansible/roles/wiki/templates/docker-compose.yml.j2
 ansible/roles/wiki/templates/wiki.conf.j2
 ansible/roles/wiki/templates/wikidump.sh.j2
-etc/globals.yaml
+etc/example_globals.yaml
+etc/example_talos.yaml
 etc/inventory
-etc/talos.yaml
 talos_install.egg-info/PKG-INFO
 talos_install.egg-info/SOURCES.txt
 talos_install.egg-info/dependency_links.txt
 talos_install.egg-info/not-zip-safe
 talos_install.egg-info/pbr.json
 talos_install.egg-info/requires.txt
 talos_install.egg-info/top_level.txt
```

