# OpenVPN Role

## Deployments

### Simple

#### Ansible

##### Tags

- all
- install
- debug

##### Execute

```bash
ansible-playbook -i inventories/prod/inventories.yaml roles/openvpn/main.yaml --extra-vars @configs/prod/openvpn.yaml --tags install,debug
```

### Custom