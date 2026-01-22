mariadb
=================

Setup MariaDB

OS Platform
-----------------

### Debian

- trixie
- bookworm

Role Variables
--------------

### [defaults/main.yml](defaults/main.yml)

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードなどを参照してください。

#### `mariadb_packages`

インストールするパッケージ

#### `mariadb_root_password`

rootのパスワード

#### `mariadb_append_mroonga_repository`

mroongaリポジトリを追加するか否か

#### `mariadb_default_charset`

デフォルトのcharset

#### `mariadb_default_collation`

デフォルトのcollation

#### `mariadb_databases`

データベースの設定

#### `mariadb_users`

データベースユーザーの設定

#### `mariadb_max_connections`

max_connectionsの設定値

#### `mariadb_max_table_use_in_query`

table_open_cacheの設定値の自動算出に利用

#### `mariadb_innodb_baffer_pool_rate`

innodb_buffer_pool_sizeの設定値の自動算出に利用

#### `mariadb_myisam_key_baffer_rate`

key_buffer_sizeの設定値の自動算出に利用

#### `mariadb_mysqld_cfg`

MariaDBの設定

### [vars/main.yml](vars/main.yml)

設定値については[vars/main.yml](vars/main.yml)を参照してください。

#### `mariadb_config_base_dir`

#### `mariadb_config_dir`

#### `mariadb_mysql55_default_sql_mode`

#### `mariadb_mysql56_default_sql_mode`

#### `mariadb_mysql57_default_sql_mode`

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
