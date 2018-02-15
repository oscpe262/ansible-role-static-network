# Ansible role 'ansible-role-static-network'

An Ansible role for setting up static network addresses. This role is not intended to cover all purposes and permutations, but rather a personal modular role for local automatization.

## Requirements
Fedora 27

## Role Variables
| Variable		| Default		| Comments (type) |
| :---			| :---			| :---		  |
| `ip_address`| `<none>` | E.g. 192.168.0.10/24 |
| `gw_ip` | `192.168.0.1` | Gateway IP |
| `dns_ip1` | 8.8.8.8 | Primary DNS server |
| `dns_ip2` | 8.8.6.6 | Secondary DNS server |

## Dependencies

## Example Playbook
```Yaml
- hosts: foo
  roles:
    - role: ansible-role-static-network
      ip_address: 192.168.1.10/24
      gw_ip: 192.168.1.1
```

## Testing


## License

BSD

## Contributors

Issues, feature requests, ideas, suggestions, etc. are appreciated and can be posted in the Issues section. Pull requests are also very welcome. Please create a topic branch for your proposed changes, it's the easiest way to merge back into the project.

- [Oscar Petersson](https://github.com/oscpe262/) (Maintainer)
