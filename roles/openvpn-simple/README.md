# OpenVPN Role

## Deployments

### Simple

#### Ansible

##### Tags

- all
- install
- install-debug
- uninstall
- uninstall-debug
- debug

##### Execute

Install:

```bash
ansible-playbook --inventory inventories/prod/inventories.yaml \
                 --extra-vars @configs/prod/openvpn.yaml \
                 --tags install \
                 roles/openvpn-simple/install.yaml
```

Uninstall:

```bash
ansible-playbook --inventory inventories/prod/inventories.yaml \
                 --extra-vars @configs/prod/openvpn.yaml \
                 --tags uninstall \
                 roles/openvpn-simple/uninstall.yaml
```

### Custom