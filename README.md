# ansible-playbook.-add-zabbix-agent
ansible-playbook. Add and configure zabbix-agent.

Zabbix-agent 3.2 for CentOS 7 and Debian 8 only!

Only for fresh installation!

You have modify 2 files:
1) add-zabbix-agent.yml --- "remote_user" and "hosts"
2) roles/zabbix.agent/tasks/main.yml --- "line: 'ServerActive=XXX.XXX.XXX.XXX'" and "line: 'Server=XXX.XXX.XXX.XXX'" with your server ip-address

Run: ansible-playbook add-zabbix-agent.yml --ask-sudo-pass

Version 0.04
 - added zabbix-agent installation
 - modified zabbix user
 - modified zabbix_agentd.conf
 - create scripts dir
 - main script moved to roles/zabbix.agent/tasks/main.yml

Version 0.03
 - added disrtibution version

Version 0.02
 - added ping hosts
 - added debug message with OS
