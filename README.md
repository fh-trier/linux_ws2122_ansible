# linux_ws2122 - Ansible

Setup gateway and client vm via ansible.

- Adapt IP-Adresse of the client and gateway VM in host_vars.
- Adapt name of the interfaces for booth VMs in host_vars.
- Configure your Router (Fritz!Box, SpeedPort, ect) to route traffic for
  192.168.181.0/24 via gateway.

```bash
ansible-playbook -i hosts.yaml gateway.linuxws2122.de.yaml
ansible-playbook -i hosts.yaml client.linuxws2122.de.yaml
```
