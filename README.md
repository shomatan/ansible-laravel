# Ansible role: laravel
Configures task schedule for laravel.

## Requirements
None.

### Role variables
|Key|Type|Description|Default|
|:--|:---|:----------|:------|
|laravel_user|String|Execute user.|nginx|
|laravel_cron|Dict|Cron entries.|{}|

### Dependencies
+ php

### Example Playbook

```yaml
- hosts: all
  roles:
    - { role: laravel }
  vars:
    laravel_cron:
      sample_app:
        path: /var/www/html
```
