mariadb
=================

Setup MariaDB

OS Platform
-----------------

### Debian

- bullseye
- buster

Role Variables
--------------

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードを参照してください。

### `mariadb_packages`

インストールするパッケージ

### `mariadb_root_password`

rootのパスワード

### `mariadb_default_charset`

デフォルトのcharset

### `mariadb_default_collation`

デフォルトのcollation

### `mariadb_databases`

データベースの設定

### `mariadb_users`

データベースユーザーの設定

### `mariadb_max_connections`

max_connectionsの設定値

### `mariadb_max_table_use_in_query`

table_open_cacheの設定値の自動算出に利用

### `mariadb_innodb_baffer_pool_rate`

innodb_buffer_pool_sizeの設定値の自動算出に利用

### `mariadb_myisam_key_baffer_rate`

key_buffer_sizeの設定値の自動算出に利用

### `mariadb_mysqld_cfg`

MariaDBの設定

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: mariadb
```

License
--------------

Apache License 2.0
