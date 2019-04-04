# Ansible Role: ansible-role-yum-cron

#### Overview
enables yum cron for yum updates

#### Default Variables
```
---
# CentOS 6.
yum_cron_check_only: 'no'
yum_cron_check_first: 'no'
yum_cron_download_only: 'no'
yum_cron_mailto: ''

# Centos 7.
yum_cron_update_cmd: default
yum_cron_update_messages: 'yes'
yum_cron_download_updates: 'yes'
yum_cron_apply_updates: 'yes'
yum_cron_random_sleep: 360
yum_cron_system_name: None
yum_cron_output_width: 80
yum_cron_email_from: root@localhost
yum_cron_email_to: root
yum_cron_email_host: localhost
yum_cron_group_list: None
yum_cron_group_package_types: 'mandatory, default'
yum_cron_debug_level: -2
yum_cron_mdpolicy: 'group:main'
```


#### Samaple playbook
```
---
- hosts: localhost
  roles:
  - role: ansible-role-yum-cron
  ```
