# Vector Role

Ansible role for installing and configuring Vector log agent.

## Requirements

- Ansible 2.9+
- Target OS: Debian/Ubuntu

## Role Variables

| Variable | Default | Description |
|----------|---------|-------------|
| `vector_version` | `0.35.0` | Version of Vector to install |
| `clickhouse_host` | `localhost` | ClickHouse server host |
| `clickhouse_port` | `8123` | ClickHouse HTTP port |

## Dependencies

- `AlexeySetevoi.ansible-clickhouse`

## Example Playbook

```yaml
- hosts: servers
  roles:
    - vector-role
```