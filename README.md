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

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードを参照してください。

### `meilisearch_version`

インストールするバージョン

### `meilisearch_master_key`

Meilisearchのマスターキー  
※`meilisearch_cfg.env`が`production`の場合に、16バイト以上のUTF-8文字列を必須

### `meilisearch_port`

Meilisearchが利用するポート番号

### `meilisearch_cfg`

Meilisearchの設定

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
