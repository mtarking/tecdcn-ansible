# TECDCN: Infra-as-Code for NXOS & NDFC with Ansible

This repo contains the reference playbook with the VXLAN EVPN use case for BRKDCN-2946 at Cisco Live.

![1](./assets/brkdcn-2946-vxlan-evpn-topology.png)

## Cloning Repo

```bash
git clone https://github.com/mtarking/tecdcn-ansible.git
```

## Requirements
```bash
cd tecdcn-ansible/
pip install -r requirements.txt
ansible-galaxy collection install -r requirements.yml
```

## Executing Ansible Playbook

```bash
cd nxos
ansible-playbook -i inventory.yml vxlan.yml
```

or

```bash
cd nd
ansible-playbook -i inventory.yml vxlan.yml
```


Note: You will need to replace the devices in inventory files and host_vars with your devices' information.
