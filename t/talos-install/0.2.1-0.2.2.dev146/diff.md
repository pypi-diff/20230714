# Comparing `tmp/talos_install-0.2.1.tar.gz` & `tmp/talos_install-0.2.2.dev146.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talos_install-0.2.1.tar", last modified: Fri Jul  7 16:44:50 2023, max compression
+gzip compressed data, was "talos_install-0.2.2.dev146.tar", last modified: Fri Jul 14 12:48:41 2023, max compression
```

## Comparing `talos_install-0.2.1.tar` & `talos_install-0.2.2.dev146.tar`

### file list

```diff
@@ -1,225 +1,226 @@
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.716694 talos_install-0.2.1/
--rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-07-07 16:44:50.000000 talos_install-0.2.1/AUTHORS
--rw-rw-r--   0 installer  (3002) installer  (3002)    14160 2023-07-07 16:44:50.000000 talos_install-0.2.1/ChangeLog
--rw-rw-r--   0 installer  (3002) installer  (3002)     4825 2023-07-07 16:44:50.716694 talos_install-0.2.1/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     4172 2023-07-04 12:06:47.000000 talos_install-0.2.1/README.md
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.688694 talos_install-0.2.1/ansible/
--rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/ansible.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.689694 talos_install-0.2.1/ansible/group_vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      603 2023-07-07 16:42:14.000000 talos_install-0.2.1/ansible/group_vars/all.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.685694 talos_install-0.2.1/ansible/roles/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.674694 talos_install-0.2.1/ansible/roles/cli/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.689694 talos_install-0.2.1/ansible/roles/cli/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/files/FOUNDMEDEVKEY
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.689694 talos_install-0.2.1/ansible/roles/cli/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.690694 talos_install-0.2.1/ansible/roles/cli/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1197 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/tasks/clone.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1512 2023-06-16 10:28:42.000000 talos_install-0.2.1/ansible/roles/cli/tasks/env.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/tasks/logrotate.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      434 2023-07-02 09:06:27.000000 talos_install-0.2.1/ansible/roles/cli/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     2692 2023-07-02 09:06:27.000000 talos_install-0.2.1/ansible/roles/cli/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/tasks/web.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.693694 talos_install-0.2.1/ansible/roles/cli/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3814 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/agent.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      418 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/cli/templates/app.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      745 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/cli/templates/cli.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2388 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/cli/templates/env_talos.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1381 2023-06-16 10:28:42.000000 talos_install-0.2.1/ansible/roles/cli/templates/globals.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-06-16 12:33:23.000000 talos_install-0.2.1/ansible/roles/cli/templates/my-httpd.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      379 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/passwords.yaml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/talos-logrotate.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1088 2023-07-07 16:42:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/talos.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/cli/templates/talospass.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.675694 talos_install-0.2.1/ansible/roles/common/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.693694 talos_install-0.2.1/ansible/roles/common/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/common/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.694694 talos_install-0.2.1/ansible/roles/common/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/common/tasks/install_extra_pkgs.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/common/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      818 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/common/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.675694 talos_install-0.2.1/ansible/roles/gather_facts/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.694694 talos_install-0.2.1/ansible/roles/gather_facts/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/gather_facts/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.694694 talos_install-0.2.1/ansible/roles/gather_facts/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)      949 2023-06-29 13:29:49.000000 talos_install-0.2.1/ansible/roles/gather_facts/vars/RedHat.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      948 2023-06-29 13:29:49.000000 talos_install-0.2.1/ansible/roles/gather_facts/vars/Rocky.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.676694 talos_install-0.2.1/ansible/roles/install_ansible/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.675694 talos_install-0.2.1/ansible/roles/install_ansible/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.694694 talos_install-0.2.1/ansible/roles/install_ansible/files/inventory_plugins/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.695694 talos_install-0.2.1/ansible/roles/install_ansible/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_ansible/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.695694 talos_install-0.2.1/ansible/roles/install_ansible/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_ansible/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.695694 talos_install-0.2.1/ansible/roles/install_ansible/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      512 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_ansible/templates/ansible.cfg.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.676694 talos_install-0.2.1/ansible/roles/install_certificates/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.695694 talos_install-0.2.1/ansible/roles/install_certificates/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_certificates/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.696694 talos_install-0.2.1/ansible/roles/install_certificates/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_certificates/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.677694 talos_install-0.2.1/ansible/roles/install_docker/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.696694 talos_install-0.2.1/ansible/roles/install_docker/handlers/
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/handlers/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.696694 talos_install-0.2.1/ansible/roles/install_docker/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.696694 talos_install-0.2.1/ansible/roles/install_docker/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.697694 talos_install-0.2.1/ansible/roles/install_docker/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/templates/daemon.json.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_docker/templates/docker-ce.repo.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.677694 talos_install-0.2.1/ansible/roles/install_python/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.697694 talos_install-0.2.1/ansible/roles/install_python/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_python/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.697694 talos_install-0.2.1/ansible/roles/install_python/vars/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/install_python/vars/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.682694 talos_install-0.2.1/ansible/roles/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.697694 talos_install-0.2.1/ansible/roles/nagios/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.679694 talos_install-0.2.1/ansible/roles/nagios/files/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.678694 talos_install-0.2.1/ansible/roles/nagios/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/conf.d/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/monitor/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/monitor/.ID
--rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/etc/nagios/resource.cfg
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.679694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/apache2/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.698694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.680694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/apache/
--rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/apache/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/nagios/
--rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/postfix/
--rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
--rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.680694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.699694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.700694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.701694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
--rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1585 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
--rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-06-16 10:28:42.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.701694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
--rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.701694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
--rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
--rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.702694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.681694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/local/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.702694 talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/local/bin/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.703694 talos_install-0.2.1/ansible/roles/nagios/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.704694 talos_install-0.2.1/ansible/roles/nagios/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/cgi.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/contacts.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     2765 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/localhost.cfg.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/nagios/templates/nagios.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.684694 talos_install-0.2.1/ansible/roles/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.704694 talos_install-0.2.1/ansible/roles/opendcim/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      295 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/opendcim/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.706694 talos_install-0.2.1/ansible/roles/opendcim/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/apache2.conf
--rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/apache2.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/default.sql
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.682694 talos_install-0.2.1/ansible/roles/opendcim/files/etc/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.683694 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.706694 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/drawings/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.706694 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/pictures/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/mysqld.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.683694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.683694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.683694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.706694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.707694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
--rw-rw-r--   0 installer  (3002) installer  (3002)    53198 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
--rw-rw-r--   0 installer  (3002) installer  (3002)    20094 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.707694 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
--rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
--rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
--rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/pre-conf.sh
--rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/files/startup.sh
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.707694 talos_install-0.2.1/ansible/roles/opendcim/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.708694 talos_install-0.2.1/ansible/roles/opendcim/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/tasks/build.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/tasks/misc.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/tasks/run.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.709694 talos_install-0.2.1/ansible/roles/opendcim/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/opendcim/templates/Dockerfile.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      712 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/opendcim/templates/first-run.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      168 2023-07-04 12:06:47.000000 talos_install-0.2.1/ansible/roles/opendcim/templates/opendcim.conf.j2
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.684694 talos_install-0.2.1/ansible/roles/os_tune/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.709694 talos_install-0.2.1/ansible/roles/os_tune/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/os_tune/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.685694 talos_install-0.2.1/ansible/roles/talos_users/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.709694 talos_install-0.2.1/ansible/roles/talos_users/files/
--rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/talos_users/files/talos
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.710694 talos_install-0.2.1/ansible/roles/talos_users/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/talos_users/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.710694 talos_install-0.2.1/ansible/roles/talos_users/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      634 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/talos_users/tasks/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.685694 talos_install-0.2.1/ansible/roles/uninstall/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.710694 talos_install-0.2.1/ansible/roles/uninstall/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.710694 talos_install-0.2.1/ansible/roles/uninstall/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/meta/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.711694 talos_install-0.2.1/ansible/roles/uninstall/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      656 2023-07-02 09:06:27.000000 talos_install-0.2.1/ansible/roles/uninstall/tasks/cli.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/tasks/docker.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      339 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/uninstall/tasks/user.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.711694 talos_install-0.2.1/ansible/roles/wiki/
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.712694 talos_install-0.2.1/ansible/roles/wiki/defaults/
--rw-rw-r--   0 installer  (3002) installer  (3002)      572 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/wiki/defaults/main.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.712694 talos_install-0.2.1/ansible/roles/wiki/meta/
--rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/meta/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/requirements.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.713694 talos_install-0.2.1/ansible/roles/wiki/tasks/
--rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/tasks/compose.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      161 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/wiki/tasks/init.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      325 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/wiki/tasks/main.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/tasks/misc.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.713694 talos_install-0.2.1/ansible/roles/wiki/templates/
--rw-rw-r--   0 installer  (3002) installer  (3002)     1275 2023-06-15 16:34:43.000000 talos_install-0.2.1/ansible/roles/wiki/templates/docker-compose.yml.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/templates/wiki.conf.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-06-15 07:22:43.000000 talos_install-0.2.1/ansible/roles/wiki/templates/wikidump.sh.j2
--rw-rw-r--   0 installer  (3002) installer  (3002)     1844 2023-07-02 09:06:27.000000 talos_install-0.2.1/ansible/site.yaml
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.714694 talos_install-0.2.1/etc/
--rw-rw-r--   0 installer  (3002) installer  (3002)      311 2023-07-02 09:06:27.000000 talos_install-0.2.1/etc/example_globals.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)     1090 2023-07-02 09:06:27.000000 talos_install-0.2.1/etc/example_talos.yaml
--rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.1/etc/inventory
--rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-07-07 16:44:50.722694 talos_install-0.2.1/setup.cfg
--rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-06-15 16:56:29.000000 talos_install-0.2.1/setup.py
--rwxrwxr-x   0 installer  (3002) installer  (3002)    10898 2023-07-02 09:06:27.000000 talos_install-0.2.1/talos_install
-drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-07 16:44:50.716694 talos_install-0.2.1/talos_install.egg-info/
--rw-rw-r--   0 installer  (3002) installer  (3002)     4825 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/PKG-INFO
--rw-rw-r--   0 installer  (3002) installer  (3002)     5634 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/SOURCES.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/dependency_links.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.1/talos_install.egg-info/not-zip-safe
--rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/pbr.json
--rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/requires.txt
--rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-07 16:44:50.000000 talos_install-0.2.1/talos_install.egg-info/top_level.txt
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:41.000151 talos_install-0.2.2.dev146/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      347 2023-07-14 12:48:40.000000 talos_install-0.2.2.dev146/AUTHORS
+-rw-rw-r--   0 installer  (3002) installer  (3002)    15013 2023-07-14 12:48:40.000000 talos_install-0.2.2.dev146/ChangeLog
+-rw-rw-r--   0 installer  (3002) installer  (3002)     4830 2023-07-14 12:48:41.001151 talos_install-0.2.2.dev146/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     4170 2023-07-12 08:45:00.000000 talos_install-0.2.2.dev146/README.md
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.969151 talos_install-0.2.2.dev146/ansible/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      334 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/ansible.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.970151 talos_install-0.2.2.dev146/ansible/group_vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      603 2023-07-14 12:42:47.000000 talos_install-0.2.2.dev146/ansible/group_vars/all.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.967151 talos_install-0.2.2.dev146/ansible/roles/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.956151 talos_install-0.2.2.dev146/ansible/roles/cli/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.970151 talos_install-0.2.2.dev146/ansible/roles/cli/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/files/FOUNDMEDEVKEY
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.970151 talos_install-0.2.2.dev146/ansible/roles/cli/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.971151 talos_install-0.2.2.dev146/ansible/roles/cli/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1197 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/tasks/clone.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1512 2023-06-16 10:28:42.000000 talos_install-0.2.2.dev146/ansible/roles/cli/tasks/env.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      301 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/tasks/logrotate.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      434 2023-07-02 09:06:27.000000 talos_install-0.2.2.dev146/ansible/roles/cli/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2662 2023-07-12 08:45:00.000000 talos_install-0.2.2.dev146/ansible/roles/cli/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1675 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/tasks/web.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.977151 talos_install-0.2.2.dev146/ansible/roles/cli/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3814 2023-06-15 16:34:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/agent.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      418 2023-07-04 12:06:47.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/app.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      785 2023-07-11 11:55:47.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/cli.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2388 2023-07-04 12:06:47.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/env_talos.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1379 2023-07-12 08:44:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/globals.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1711 2023-06-16 12:33:23.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/my-httpd.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      379 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/passwords.yaml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      506 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/talos-logrotate.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1160 2023-07-14 11:45:24.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/talos.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)       22 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/cli/templates/talospass.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.956151 talos_install-0.2.2.dev146/ansible/roles/common/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.977151 talos_install-0.2.2.dev146/ansible/roles/common/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       59 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/common/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.978151 talos_install-0.2.2.dev146/ansible/roles/common/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      360 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/common/tasks/install_extra_pkgs.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      155 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/common/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      815 2023-07-11 11:55:47.000000 talos_install-0.2.2.dev146/ansible/roles/common/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.957151 talos_install-0.2.2.dev146/ansible/roles/gather_facts/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.978151 talos_install-0.2.2.dev146/ansible/roles/gather_facts/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      495 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/gather_facts/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.978151 talos_install-0.2.2.dev146/ansible/roles/gather_facts/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      949 2023-06-29 13:29:49.000000 talos_install-0.2.2.dev146/ansible/roles/gather_facts/vars/RedHat.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      948 2023-06-29 13:29:49.000000 talos_install-0.2.2.dev146/ansible/roles/gather_facts/vars/Rocky.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.958151 talos_install-0.2.2.dev146/ansible/roles/install_ansible/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.957151 talos_install-0.2.2.dev146/ansible/roles/install_ansible/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.978151 talos_install-0.2.2.dev146/ansible/roles/install_ansible/files/inventory_plugins/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3333 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.979151 talos_install-0.2.2.dev146/ansible/roles/install_ansible/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_ansible/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.979151 talos_install-0.2.2.dev146/ansible/roles/install_ansible/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1764 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_ansible/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.979151 talos_install-0.2.2.dev146/ansible/roles/install_ansible/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      466 2023-07-13 07:54:09.000000 talos_install-0.2.2.dev146/ansible/roles/install_ansible/templates/ansible.cfg.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.958151 talos_install-0.2.2.dev146/ansible/roles/install_certificates/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.979151 talos_install-0.2.2.dev146/ansible/roles/install_certificates/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_certificates/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.980151 talos_install-0.2.2.dev146/ansible/roles/install_certificates/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      689 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_certificates/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.959151 talos_install-0.2.2.dev146/ansible/roles/install_docker/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.980151 talos_install-0.2.2.dev146/ansible/roles/install_docker/handlers/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_docker/handlers/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.980151 talos_install-0.2.2.dev146/ansible/roles/install_docker/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       84 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_docker/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.980151 talos_install-0.2.2.dev146/ansible/roles/install_docker/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1526 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_docker/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.981151 talos_install-0.2.2.dev146/ansible/roles/install_docker/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      183 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_docker/templates/daemon.json.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1919 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_docker/templates/docker-ce.repo.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.959151 talos_install-0.2.2.dev146/ansible/roles/install_python/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.981151 talos_install-0.2.2.dev146/ansible/roles/install_python/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      590 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_python/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.981151 talos_install-0.2.2.dev146/ansible/roles/install_python/vars/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/install_python/vars/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.963151 talos_install-0.2.2.dev146/ansible/roles/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.981151 talos_install-0.2.2.dev146/ansible/roles/nagios/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      253 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.960151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.960151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.982151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/etc/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.982151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/etc/nagios/conf.d/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/etc/nagios/conf.d/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.982151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/etc/nagios/monitor/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/etc/nagios/monitor/.ID
+-rw-rw-r--   0 installer  (3002) installer  (3002)      499 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/etc/nagios/resource.cfg
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.963151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.982151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.960151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/apache2/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.982151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1615 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      245 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/rsyslog.conf
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.961151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.983151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/apache/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      140 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/apache/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.983151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/nagios/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      835 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/nagios/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.983151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/postfix/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      752 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/postfix/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.983151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       51 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/rsyslog/run
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.962151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.962151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.984151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/etc/.ID
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.984151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.985151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13613 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13958 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1614 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1585 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5972 2023-06-16 10:28:42.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.985151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-footer.ssi
+-rw-rw-r--   0 installer  (3002) installer  (3002)        0 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/ssi/common-header.ssi
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.986151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     9882 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css
+-rw-rw-r--   0 installer  (3002) installer  (3002)     7391 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.962151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagiosgraph/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.986151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      950 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.963151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/usr/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.963151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/usr/local/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.986151 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/usr/local/bin/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1147 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.987151 talos_install-0.2.2.dev146/ansible/roles/nagios/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      748 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      349 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1070 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1098 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.988151 talos_install-0.2.2.dev146/ansible/roles/nagios/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    14403 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)    11609 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/templates/cgi.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3808 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/templates/contacts.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     2765 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/templates/localhost.cfg.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      116 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/nagios/templates/nagios.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.965151 talos_install-0.2.2.dev146/ansible/roles/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.989151 talos_install-0.2.2.dev146/ansible/roles/opendcim/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      295 2023-07-04 12:06:47.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.990151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1167 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/apache2.conf
+-rw-rw-r--   0 installer  (3002) installer  (3002)      106 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/apache2.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)    60057 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/default.sql
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.964151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/etc/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.964151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/etc/opendcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.990151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/etc/opendcim/drawings/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.990151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/etc/opendcim/pictures/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)      233 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/mysqld.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.964151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.964151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.964151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.991151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.991151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/css/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    53198 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)    20094 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.991151 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/images/
+-rw-rw-r--   0 installer  (3002) installer  (3002)    13138 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png
+-rw-rw-r--   0 installer  (3002) installer  (3002)    38561 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1350 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/pre-conf.sh
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1114 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/files/startup.sh
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.992151 talos_install-0.2.2.dev146/ansible/roles/opendcim/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)        4 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.993151 talos_install-0.2.2.dev146/ansible/roles/opendcim/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1052 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/tasks/build.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      353 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      725 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/tasks/misc.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1131 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/tasks/run.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.993151 talos_install-0.2.2.dev146/ansible/roles/opendcim/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     3023 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/templates/Dockerfile.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      712 2023-07-04 12:06:47.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/templates/first-run.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      168 2023-07-04 12:06:47.000000 talos_install-0.2.2.dev146/ansible/roles/opendcim/templates/opendcim.conf.j2
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.965151 talos_install-0.2.2.dev146/ansible/roles/os_tune/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.993151 talos_install-0.2.2.dev146/ansible/roles/os_tune/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1403 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/os_tune/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.966151 talos_install-0.2.2.dev146/ansible/roles/talos_users/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.994151 talos_install-0.2.2.dev146/ansible/roles/talos_users/files/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       75 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/talos_users/files/talos
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.994151 talos_install-0.2.2.dev146/ansible/roles/talos_users/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/talos_users/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.994151 talos_install-0.2.2.dev146/ansible/roles/talos_users/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      634 2023-06-15 16:34:43.000000 talos_install-0.2.2.dev146/ansible/roles/talos_users/tasks/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.966151 talos_install-0.2.2.dev146/ansible/roles/uninstall/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.994151 talos_install-0.2.2.dev146/ansible/roles/uninstall/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       89 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/uninstall/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.995151 talos_install-0.2.2.dev146/ansible/roles/uninstall/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/uninstall/meta/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.995151 talos_install-0.2.2.dev146/ansible/roles/uninstall/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      656 2023-07-02 09:06:27.000000 talos_install-0.2.2.dev146/ansible/roles/uninstall/tasks/cli.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      315 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/uninstall/tasks/docker.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      176 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/uninstall/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      339 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/uninstall/tasks/user.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.996151 talos_install-0.2.2.dev146/ansible/roles/wiki/
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.996151 talos_install-0.2.2.dev146/ansible/roles/wiki/defaults/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      572 2023-06-15 16:34:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/defaults/main.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.996151 talos_install-0.2.2.dev146/ansible/roles/wiki/meta/
+-rw-rw-r--   0 installer  (3002) installer  (3002)       41 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/meta/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      110 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/requirements.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.997151 talos_install-0.2.2.dev146/ansible/roles/wiki/tasks/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      542 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/tasks/compose.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      161 2023-06-15 16:34:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/tasks/init.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      325 2023-06-15 16:34:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/tasks/main.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      240 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/tasks/misc.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.998151 talos_install-0.2.2.dev146/ansible/roles/wiki/templates/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1275 2023-06-15 16:34:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/templates/docker-compose.yml.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      327 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/templates/wiki.conf.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)      436 2023-06-15 07:22:43.000000 talos_install-0.2.2.dev146/ansible/roles/wiki/templates/wikidump.sh.j2
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1844 2023-07-02 09:06:27.000000 talos_install-0.2.2.dev146/ansible/site.yaml
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:40.999151 talos_install-0.2.2.dev146/etc/
+-rw-rw-r--   0 installer  (3002) installer  (3002)      235 2023-07-12 14:19:48.000000 talos_install-0.2.2.dev146/etc/example_cluster.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)      311 2023-07-12 13:19:52.000000 talos_install-0.2.2.dev146/etc/example_globals.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1228 2023-07-12 08:45:00.000000 talos_install-0.2.2.dev146/etc/example_talos.yaml
+-rw-rw-r--   0 installer  (3002) installer  (3002)       46 2023-04-16 16:14:10.000000 talos_install-0.2.2.dev146/etc/inventory
+-rw-rw-r--   0 installer  (3002) installer  (3002)     1188 2023-07-14 12:48:41.014151 talos_install-0.2.2.dev146/setup.cfg
+-rw-rw-r--   0 installer  (3002) installer  (3002)      321 2023-06-15 16:56:29.000000 talos_install-0.2.2.dev146/setup.py
+-rwxrwxr-x   0 installer  (3002) installer  (3002)    11080 2023-07-12 13:27:06.000000 talos_install-0.2.2.dev146/talos_install
+drwxrwxr-x   0 installer  (3002) installer  (3002)        0 2023-07-14 12:48:41.000151 talos_install-0.2.2.dev146/talos_install.egg-info/
+-rw-rw-r--   0 installer  (3002) installer  (3002)     4830 2023-07-14 12:48:40.000000 talos_install-0.2.2.dev146/talos_install.egg-info/PKG-INFO
+-rw-rw-r--   0 installer  (3002) installer  (3002)     5659 2023-07-14 12:48:40.000000 talos_install-0.2.2.dev146/talos_install.egg-info/SOURCES.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-14 12:48:40.000000 talos_install-0.2.2.dev146/talos_install.egg-info/dependency_links.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-06-15 16:56:45.000000 talos_install-0.2.2.dev146/talos_install.egg-info/not-zip-safe
+-rw-rw-r--   0 installer  (3002) installer  (3002)       47 2023-07-14 12:48:40.000000 talos_install-0.2.2.dev146/talos_install.egg-info/pbr.json
+-rw-rw-r--   0 installer  (3002) installer  (3002)       94 2023-07-14 12:48:40.000000 talos_install-0.2.2.dev146/talos_install.egg-info/requires.txt
+-rw-rw-r--   0 installer  (3002) installer  (3002)        1 2023-07-14 12:48:40.000000 talos_install-0.2.2.dev146/talos_install.egg-info/top_level.txt
```

### Comparing `talos_install-0.2.1/ChangeLog` & `talos_install-0.2.2.dev146/ChangeLog`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,54 @@
 CHANGES
 =======
 
+* Release 0.2.2
+* fix ipmi check
+* fix ipmi check
+* fix bmc
+* fix bmc
+* fix bmc
+* fix home setting
+* fix collect sequence
+* new playbook slurm
+* new playbook slurm
+* new playbook slurm
+* new playbook slurm
+* new playbook slurm
+* new playbook ofed
+* new playbook ofed
+* new playbook ofed
+* new playbook ofed
+* new playbook
+* Update libplay
+* fix add files
+* Clean talos repo on update and review flow
+* Dynamic authorization in dcim call
+* add htpasswd update
+* add htpasswd update
+* add htpasswd update
+* fix ncpa\_nvme
+* fix ncpa\_ipmi
+* fix ncpa\_nvme
+* fix bmc\_profile
+* fix bmc\_profile
+* fix playbook completion
+* fix playbook completion
+* fix playbook Add
+* Update libplay
+* fix show role and job (local)
 * Release 0.2.1
+* fix documentation
+* fix update
+* fix samples sudoers
+* fix BMC default
+* fix BMC default
+* fix BMC default
+* fix BMC default
+* fix sudoers
 * fix SSH-o batchmode=yes
 * fix SSH checks for key:ok-host:no
 * fix SSH checks
 *  fix check config
 *  fix check config
 * Skip for unecessary run
 * Skip for unecessary run
@@ -75,15 +118,15 @@
 *  fix typo range compare
 *  fix typo range compare
 * fix tag typo
 * Restyle web homepage
 * Add customer.domain feature, fix max ansible version
 * Add extension for wiki load config, mino fix
 
-0.2.0
+0.2.1
 -----
 
 * Fix Home position
 * Remove SWAP\_USAGE for Talos mgmt
 * Add Init Playbook on Reload
 * Add Init Playbook on Reload
 * Add Init Playbook on Reload
```

### Comparing `talos_install-0.2.1/PKG-INFO` & `talos_install-0.2.2.dev146/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos_install
-Version: 0.2.1
+Version: 0.2.2.dev146
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -129,15 +129,15 @@
 ```
 
 By default setup is automatically done during deploy:
 
 ```bash
 <pip_environment>/share/talos_cli/etc/talos.yaml
 
-talos_conf: use_default: 'true'
+talos_conf: use_default: true
 ```
 
 If necessary run setup
 
 ```bash
  talos-config setup
 ```
```

### Comparing `talos_install-0.2.1/README.md` & `talos_install-0.2.2.dev146/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 ```
 
 By default setup is automatically done during deploy:
 
 ```bash
 <pip_environment>/share/talos_cli/etc/talos.yaml
 
-talos_conf: use_default: 'true'
+talos_conf: use_default: true
 ```
 
 If necessary run setup
 
 ```bash
  talos-config setup
 ```
```

### Comparing `talos_install-0.2.1/ansible/group_vars/all.yaml` & `talos_install-0.2.2.dev146/ansible/group_vars/all.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   namespace: "ilciko"
   nagios_tag: 1.0
   opendcim_tag: 1.0
 
 ### TALOS
 app:
   name: 'talos'
-  cli_version: '0.2.1'  # tversion
+  cli_version: '0.2.2'  # tversion
   cli_repo: 'git@github.com:E4-Computer-Engineering/talos-cli.git'
   nexus_repo: 'srv-nexus01.e4srv:8081'
   dir: "/opt/talos"
   clidir: "/opt/talos/cli"
   datadir: "/opt/talos/cli/data"
   etcdir: "/etc/e4company/talos"
   webdir: "/opt/talos/web"
```

### Comparing `talos_install-0.2.1/ansible/roles/cli/tasks/clone.yaml` & `talos_install-0.2.2.dev146/ansible/roles/cli/tasks/clone.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/cli/tasks/env.yaml` & `talos_install-0.2.2.dev146/ansible/roles/cli/tasks/env.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/cli/tasks/misc.yaml` & `talos_install-0.2.2.dev146/ansible/roles/cli/tasks/misc.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -39,36 +39,36 @@
 - name: Configure Talos
   ansible.builtin.template:
     src: talos.conf.j2
     dest: "{{ app.etcdir }}/talos.conf"
     mode: '0660'
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
-  when: talos_conf.use_default == 'true'
+  when: talos_conf.use_default
 
 - name: Generate CUSTOMER keypair
   community.crypto.openssh_keypair:
     path: "{{ master.home }}/.ssh/{{ item }}"
     size: 2048
     type: rsa
     force: false
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
   loop:
     - CUSTOMER_CLI
-  when: talos_conf.use_default == 'true'
+  when: talos_conf.use_default
 
 - name: Get CUSTOMER keypair
   ansible.builtin.fetch:
     src: "{{ master.home }}/.ssh/{{ item }}.pub"
     dest: "/tmp/{{ customer.name }}.{{ item }}.pub"
     flat: true
   loop:
     - CUSTOMER_CLI
-  when: talos_conf.use_default == 'true'
+  when: talos_conf.use_default
 
 - name: Set Permissions
   ansible.builtin.file:
     dest: "{{ item }}"
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
     recurse: true
```

### Comparing `talos_install-0.2.1/ansible/roles/cli/tasks/web.yaml` & `talos_install-0.2.2.dev146/ansible/roles/cli/tasks/web.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/cli/templates/agent.sh.j2` & `talos_install-0.2.2.dev146/ansible/roles/cli/templates/agent.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/cli/templates/cli.conf.j2` & `talos_install-0.2.2.dev146/ansible/roles/cli/templates/cli.conf.j2`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 customer.name:         {{ customer.name }}
 customer.domain:       {{ customer.domain }}
 master.user:           {{ master.user }}
 master.uid:            {{ master.uid }}
 master.password:       {{ master.password }}
 master.home:           {{ master.home }}
 master.mail:           {{ master.mail }}
+guest.user:            {{ guest.user }}
 mgm_password:          {{ mgm_password }}
```

### Comparing `talos_install-0.2.1/ansible/roles/cli/templates/env_talos.j2` & `talos_install-0.2.2.dev146/ansible/roles/cli/templates/env_talos.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/cli/templates/globals.yaml.j2` & `talos_install-0.2.2.dev146/ansible/roles/cli/templates/globals.yaml.j2`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 # ansible_inventory_enable: set to true to add/remove nodes on Ansible inventory (Default = true)
 # ansible_init_mode: set to true to run init sequence on node added. (Default = false)
 # dcim_inventory_enable: set to true to add/remove nodes on DCIM inventory (Default = false)
 # nagios_enable: set to true to add/remove nodes Monitoring (Default = true)
 # default_domain: set to true to use a fixed domain for host resolution (Default = true)
 # talos_domain: set extension, dont forget dot! (Default = .e4red)
 talos_conf:
-  use_default: '{{ talos_conf.use_default }}'
+  use_default: {{ talos_conf.use_default }}
   ansible_inventory_enable: '{{ talos_conf.ansible_inventory_enable }}'
   ansible_init_mode: '{{ talos_conf.ansible_init_mode }}'
   dcim_inventory_enable: '{{ talos_conf.dcim_inventory_enable }}'
   nagios_enable: '{{ talos_conf.nagios_enable }}'
   default_domain: '{{ talos_conf.default_domain }}'
   talos_domain: '{{ talos_conf.talos_domain }}'
```

### Comparing `talos_install-0.2.1/ansible/roles/cli/templates/my-httpd.conf.j2` & `talos_install-0.2.2.dev146/ansible/roles/cli/templates/my-httpd.conf.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/cli/templates/talos.conf.j2` & `talos_install-0.2.2.dev146/ansible/roles/cli/templates/talos.conf.j2`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Default = true
 ANSIBLE_INVENTORY_ENABLE = {{ talos_conf.ansible_inventory_enable }}
 
 # Set Ansible init_mode to true to configure node during add node
 # Default = false
 ANSIBLE_INIT_MODE = {{ talos_conf.ansible_init_mode }}
 
-# Set DCIM invetory to true to add/remove nodes on DCIM inventory
+# Set DCIM inventory to true to add/remove nodes on DCIM inventory
 # Default = true
 DCIM_INVENTORY_ENABLE = {{ talos_conf.dcim_inventory_enable }}
 
 # Set NAGIOS to true to add/remove nodes Monitoring
 # Default = true
 NAGIOS_ENABLE = {{ talos_conf.nagios_enable }}
 
@@ -29,7 +29,12 @@
 # Set Talos Domain extension (i.e .example)
 # Default = null
 TALOS_DOMAIN = {{ talos_conf.talos_domain }}
 
 # Set Default Talos Verbosity Level (0-2)
 # Default = 0 (no Verbose)
 TALOS_VERBOSITY = 0
+
+# Set Default bmc host extension
+# Default = -bmc
+
+DEFAULT_BMC = -bmc
```

### Comparing `talos_install-0.2.1/ansible/roles/common/tasks/misc.yaml` & `talos_install-0.2.2.dev146/ansible/roles/common/tasks/misc.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     - "{{ app.etcdir }}/html"
     - "{{ app.etcdir }}/conf"
 
 - name: Set master user pass
   community.general.htpasswd:
     path: "{{ item }}"
     name: "{{ master.user }}"
-    password: "{{ master.password }}"
+    password: "{{ mgm_password }}"
     owner: "{{ master.user }}"
     group: "{{ master.group }}"
     mode: '0644'
   loop:
     - "{{ app.etcdir }}/html/htpasswd"
 
 - name: Set guest user pass
```

### Comparing `talos_install-0.2.1/ansible/roles/gather_facts/vars/RedHat.yaml` & `talos_install-0.2.2.dev146/ansible/roles/gather_facts/vars/RedHat.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/gather_facts/vars/Rocky.yaml` & `talos_install-0.2.2.dev146/ansible/roles/gather_facts/vars/Rocky.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py` & `talos_install-0.2.2.dev146/ansible/roles/install_ansible/files/inventory_plugins/yamlgroup.py`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/install_ansible/tasks/main.yaml` & `talos_install-0.2.2.dev146/ansible/roles/install_ansible/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/install_certificates/tasks/main.yaml` & `talos_install-0.2.2.dev146/ansible/roles/install_certificates/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/install_docker/tasks/main.yaml` & `talos_install-0.2.2.dev146/ansible/roles/install_docker/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/install_docker/templates/docker-ce.repo.j2` & `talos_install-0.2.2.dev146/ansible/roles/install_docker/templates/docker-ce.repo.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/install_python/tasks/main.yaml` & `talos_install-0.2.2.dev146/ansible/roles/install_python/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/apache2/sites-available/nagios.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/nagios/run` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/nagios/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/etc/sv/postfix/run` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/etc/sv/postfix/run`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/images/LOGO_E4_NERO.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/images/talos.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/index.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/infobox.html`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/side.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/common.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagios/share/stylesheets/status.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/opt/nagiosgraph/etc/fix-nagiosgraph-multiple-selection.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios` & `talos_install-0.2.2.dev146/ansible/roles/nagios/files/overlay/usr/local/bin/start_nagios`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/tasks/build.yaml` & `talos_install-0.2.2.dev146/ansible/roles/nagios/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/tasks/misc.yaml` & `talos_install-0.2.2.dev146/ansible/roles/nagios/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/tasks/run.yaml` & `talos_install-0.2.2.dev146/ansible/roles/nagios/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/templates/Dockerfile.j2` & `talos_install-0.2.2.dev146/ansible/roles/nagios/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/templates/cgi.cfg.j2` & `talos_install-0.2.2.dev146/ansible/roles/nagios/templates/cgi.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/templates/contacts.cfg.j2` & `talos_install-0.2.2.dev146/ansible/roles/nagios/templates/contacts.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/nagios/templates/localhost.cfg.j2` & `talos_install-0.2.2.dev146/ansible/roles/nagios/templates/localhost.cfg.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/apache2.conf` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/apache2.conf`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/default.sql` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/default.sql`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/etc/opendcim/drawings/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/etc/opendcim/pictures/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/css/inventory.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/images/logo.png`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/overlay/var/www/dcim/misc.inc.php`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/pre-conf.sh` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/pre-conf.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/files/startup.sh` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/files/startup.sh`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/tasks/build.yaml` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/tasks/build.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/tasks/misc.yaml` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/tasks/misc.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/tasks/run.yaml` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/tasks/run.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/templates/Dockerfile.j2` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/opendcim/templates/first-run.sh.j2` & `talos_install-0.2.2.dev146/ansible/roles/opendcim/templates/first-run.sh.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/os_tune/tasks/main.yaml` & `talos_install-0.2.2.dev146/ansible/roles/os_tune/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/talos_users/tasks/main.yaml` & `talos_install-0.2.2.dev146/ansible/roles/talos_users/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/uninstall/tasks/cli.yaml` & `talos_install-0.2.2.dev146/ansible/roles/uninstall/tasks/cli.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/wiki/defaults/main.yaml` & `talos_install-0.2.2.dev146/ansible/roles/wiki/defaults/main.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/wiki/tasks/compose.yaml` & `talos_install-0.2.2.dev146/ansible/roles/wiki/tasks/compose.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/roles/wiki/templates/docker-compose.yml.j2` & `talos_install-0.2.2.dev146/ansible/roles/wiki/templates/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/ansible/site.yaml` & `talos_install-0.2.2.dev146/ansible/site.yaml`

 * *Files identical despite different names*

### Comparing `talos_install-0.2.1/etc/example_talos.yaml` & `talos_install-0.2.2.dev146/etc/example_talos.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 ---
 master:
   user: 'talos'
   group: 'talos'
-  uid: 1000
-  gid: 1000
+  uid: 3000
+  gid: 3000
   debug: false
-  password: 'E4company!TM'
-  mail: 'talosmaster@e4company.com'
+  password: 'Tpassword'
+  mail: 'talos@e4company.com'
   home: '/usr/talos'
 
+# Guest credential are for nagios and DCIM not-administrative user.
+# admin user are above .user .password
 guest:
   user: 'guest'
-  password: 'guest'
+  password: 'Tpassword'
 
-mgm_password: 'E4password!'
+# BMC and web service admin password
+mgm_password: 'E4company!TM'
 
 ### Talos configuration
 # Set use_default to enable the default setting, if 'false' on client you'll need to run talos-setup config
 # ansible_inventory_enable: set to true to add/remove nodes on Ansible inventory (Default = true)
 # ansible_init_mode: set to true to run init sequence on node added. (Default = false)
 # dcim_inventory_enable: set to true to add/remove nodes on DCIM inventory (Default = false)
 # nagios_enable: set to true to add/remove nodes Monitoring (Default = true)
 # default_domain: set to true to use a fixed domain for host resolution (Default = true)
 # talos_domain: set extension, dont forget dot! (Default = .e4red)
 talos_conf:
-  use_default: 'true'
+  use_default: true
   ansible_inventory_enable: 'true'
   ansible_init_mode: 'false'
   dcim_inventory_enable: 'false'
   nagios_enable: 'true'
   default_domain: 'true'
   talos_domain: '.e4red'
```

### Comparing `talos_install-0.2.1/setup.cfg` & `talos_install-0.2.2.dev146/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = talos_install
-version = 0.2.1
+version = 0.2.2
 summary = E4 CLI Manager
 description_file = 
 	README.md
 author = "Marco Cicala"
 author_email = marco.cicala@e4company.com
 home_page = https://www.e4company.com/
 license = GNU General Public License v3 (GPLv3)
```

### Comparing `talos_install-0.2.1/talos_install` & `talos_install-0.2.2.dev146/talos_install`

 * *Files 3% similar despite different names*

```diff
@@ -58,21 +58,27 @@
   fi
 
   if ! which ansible &>/dev/null ; then
     echo "Missing ansible"
     exit 2
   fi
 
+  missing_files=""
   if [[ ! -f ${HOME}/globals.yaml ]]; then
-    echo "Missing ${HOME}/globals.yaml, you can copy a sample from <pip_env>/share/talos_install/etc "
-    exit 2
+    missing_files="${missing_files}\n${HOME}/globals.yaml"
   fi
 
   if [[ ! -f ${HOME}/talos.yaml ]]; then
-    echo "Missing ${HOME}/talos.yaml, you can copy a sample from <pip_env>/share/talos_install/etc "
+    missing_files="${missing_files}\n${HOME}/talos.yaml "
+  fi
+  if [[ ! -f ${HOME}/cluster.yaml ]]; then
+    missing_files="${missing_files}\n${HOME}/cluster.yaml"
+  fi
+  if [[ $missing_files != "" ]]; then
+    echo -e  "Missing Files:\n${missing_files}\nyou can copy a sample from <pip_env>/share/talos_install/etc "
     exit 2
   fi
 }
 
 talos_install_menu(){
   title_message="$1"
   clean
```

### Comparing `talos_install-0.2.1/talos_install.egg-info/PKG-INFO` & `talos_install-0.2.2.dev146/talos_install.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talos-install
-Version: 0.2.1
+Version: 0.2.2.dev146
 Summary: E4 CLI Manager
 Home-page: https://www.e4company.com/
 Author: "Marco Cicala"
 Author-email: marco.cicala@e4company.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -129,15 +129,15 @@
 ```
 
 By default setup is automatically done during deploy:
 
 ```bash
 <pip_environment>/share/talos_cli/etc/talos.yaml
 
-talos_conf: use_default: 'true'
+talos_conf: use_default: true
 ```
 
 If necessary run setup
 
 ```bash
  talos-config setup
 ```
```

### Comparing `talos_install-0.2.1/talos_install.egg-info/SOURCES.txt` & `talos_install-0.2.2.dev146/talos_install.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 ansible/roles/wiki/tasks/compose.yaml
 ansible/roles/wiki/tasks/init.yaml
 ansible/roles/wiki/tasks/main.yaml
 ansible/roles/wiki/tasks/misc.yaml
 ansible/roles/wiki/templates/docker-compose.yml.j2
 ansible/roles/wiki/templates/wiki.conf.j2
 ansible/roles/wiki/templates/wikidump.sh.j2
+etc/example_cluster.yaml
 etc/example_globals.yaml
 etc/example_talos.yaml
 etc/inventory
 talos_install.egg-info/PKG-INFO
 talos_install.egg-info/SOURCES.txt
 talos_install.egg-info/dependency_links.txt
 talos_install.egg-info/not-zip-safe
```

