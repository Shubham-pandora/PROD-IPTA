ansible-playbook deploy.yml -i HOSTFILE  --limit "192.168.0.104" -e "IPTABLES='NO' IPTABLESAUDIT='YES'" -k -v

ansible-playbook deploy.yml -i INV  --limit "192.168.0.104" -e "IPTABLES='NO' IPTABLESAUDIT='YES'" -k -v

ansible-playbook deploy.yml -i inventory/hosts.ini -i inventory/groups.ini -u root --limit "192.168.0.104" -e "IPTABLES='YES' IPTABLESAUDIT='YES' NAGIOS='YES'" -k -v   





[STREAMS_VLAN48]
192.168.0.104

[STREAMS_REACT_VLAN48]
10.30.48.157
10.30.48.61
10.30.48.98
192.168.0.104