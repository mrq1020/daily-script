> **READ**

`iptables -L -n --line-number`

`iptables -L --verbose --line-number`

`...`

> **CREATE/UPDATE/DELETE**

`iptables -I DOCKER-USER -s 10.91.21.18 -j ACCEPT`

`iptables -A IN_public_allow -p TCP --dport 6379 -j ACCEPT`

`iptables -R INPUT 2 -s 192.168.1.1 -p TCP --dport 22 -j DROP`

`iptables -R IN_public_allow 21 -s 172.17.0.0/12 -d 127.0.0.1 -p TCP --dport 3306 -j ACCEPT`

`iptables -D DOCKER-USER 188`

`...`

> **save**

`iptables-save > /etc/sysconfig/iptables`

`cat /etc/sysconfig/iptables`

`service iptbales save`

`service iptables restart`

`...`
