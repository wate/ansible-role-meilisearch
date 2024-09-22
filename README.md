meilisearch
=================

Setup Meilisearch

OS Platform
-----------------

### Debian

- bookworm
- bullseye

Role Variables
--------------

### [defaults/main.yml](defaults/main.yml)

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードなどを参照してください。

#### `meilisearch_version`

インストールするバージョン

#### `meilisearch_master_key`

Meilisearchのマスターキー  
※`meilisearch_cfg.env`が`production`の場合に、16バイト以上のUTF-8文字列を必須

#### `meilisearch_port`

Meilisearchが利用するポート番号

#### `meilisearch_cfg`

Meilisearchの設定

### [vars/main.yml](vars/main.yml)

設定値については[vars/main.yml](vars/main.yml)を参照してください。

#### `meilisearch_user`

#### `meilisearch_group`

#### `meilisearch_home`

#### `meilisearch_bin_dir`

#### `meilisearch_db_dir`

#### `meilisearch_dump_dir`

#### `meilisearch_snapshot_dir`

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: meilisearch
```

License
--------------

Apache License 2.0
