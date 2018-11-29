# backup-restore

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-backup-restore.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-memcached)

Ansible role for backup-restore

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.backup-restore`

# Default settings

```
restore_postgresql: false
backup_postgresql_db: ""
backup_postgresql_user: ""
backup_postgresql_pass: ""
backup_postgresql_host: 'localhost'
backup_postgres_size_threshold: 1000000
backup_postgresql_backup_file_name: "backup.sql"

restore_mysql: false
backup_mysql_db: ""
backup_mysql_user: ""
backup_mysql_pass: ""
backup_mysql_backup_file_name: "backup.sql"

restore_redis: false
backup_redis_save_path: "/var/lib/redis"

restore_elasticsearch: false

restore_mongodb: false
backup_mongodb_backup_file_name: "mongodb_backup"
backup_mongodb_admin_db: admin
backup_mongodb_backup_user: backup
backup_mongodb_backup_pass: ""
backup_mongodb_root_user: root
backup_mongodb_root_pass: ""
backup_mongodb_db: dbname
backup_mongodb_user: username
backup_mongodb_pass: secret

restore_files: false
backup_files_paths: []

backup_tmp_path: "{{ ansible_env.HOME}}/backup"
backup_folder_prefix: ""

```
