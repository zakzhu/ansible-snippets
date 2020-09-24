[TOC]

# To get a passwd hash

An idempotent method to generate unique hashes per system is to use a salt that is consistent between runs:

```jinjia2
{{ 'secretpassword' | password_hash('sha512', 65534 | random(seed=inventory_hostname) | string) }}
```
