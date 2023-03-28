## Add and configure zabbix-agent2 6.0

## requirments
* Debian, Ubuntu
* Ansible >= 2.9.6
* ansible-collections:
* * [community.mysql](https://docs.ansible.com/ansible/latest/collections/community/mysql/mysql_info_module.html)
* * [community.general](https://docs.ansible.com/ansible/latest/collections/community/general/sudoers_module.html)

## usage
1. Install community.mysql collection
```bash
ansible-galaxy collection install community.mysql
ansible-galaxy collection install community.general --force
```
2. Enter variables in file **`zabbix-agent2.yaml`**
3. Run 
```Bash
ansible-playbook zabbix-agent2.yaml -e "hosts=YOUR-HOST-NAME"
```