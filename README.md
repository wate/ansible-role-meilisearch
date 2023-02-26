meilisearch
=================

Setup Meilisearch

OS Platform
-----------------

### Debian

- bullseye
- buster

Role Variables
--------------

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードを参照してください。

### `meilisearch_version`

インストールするバージョン

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
