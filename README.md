# loumaris.toolset

Install some handy tools to make the admin life easier.

## usage

Example entry for the `playbook.yml`

```yaml
- name: apply common configuration to all nodes
  hosts: all
  roles:
    - loumaris.toolset
  vars:
    - cloudflare__zone: 'loumaris.cloud'
```

## configuration

You need to set the following parameter (in the vault):
* `cloudflare__email` (your account mail)
* `cloudflare__token` (your api token)
* `cloudflare__zone` (default: _loumaris.cloud_)