## Add and configure zabbix-agent2 6.0

## requirments
* Debian, Ubuntu
* Ansible >= 2.9.6
* ansible-collection [community.mysql](https://docs.ansible.com/ansible/latest/collections/community/mysql/mysql_info_module.html#examples)

## usage
1. Install community.mysql collection
```bash
ansible-galaxy collection install community.mysql
```
2. Enter variables in file **`zabbix-agent2.yaml`**
3. Run 
```Bash
ansible-playbook zabbix-agent2.yaml -e "hosts=YOUR-HOST-NAME"
```