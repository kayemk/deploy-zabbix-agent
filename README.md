# Deploy Zabbix Agents via Ansible
deploy zabbix agents on debian (linux) nodes using ansible

### Agent Info

Zabbix Agent Version 3.0

### Installation

### Usage

<i>ansible 2.1 at least as control node</i>

* Activate ssh connection for root user in sshd.
* Modify hosts.ini and if needed ansible.cfg. Don't modify the `gather_facts` because they are needed for hostname validation on zabbix_agentd.conf. 
* After that you're good to go.

```
ansible-playbook site.yml --ask-pass
```

* Deactivate ssh connection for root user in sshd.
