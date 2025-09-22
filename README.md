# nmap-tcp-sync
Subnet TCP scan lab for cybersecurity practice

## IP Configuration
$ ifconfig
eth0: inet 192.168.183.X  netmask 255.255.255.0
lo:  inet 127.0.0.1

$ nmap -sS 192.168.183.X
Host is up (0.029s latency).
Not shown: 999 filtered tcp ports (no-response)
PORT   STATE SERVICE
80/tcp open  http

$ nmap -sS 192.168.183.X/24

Host: 192.168.183.7
PORT     STATE  SERVICE
1025/tcp closed NFS-or-IIS

Host: 192.168.183.8
PORT     STATE  SERVICE
2800/tcp closed acc-raid

Remaining ports: all 1000 filtered


Summary
Open Ports: 80/tcp (HTTP) on host 192.168.183.X
Closed Ports: 1025/tcp, 2800/tcp
Filtered Ports: Remaining ports did not respond
Observations: Open ports indicate active services; closed ports show no service; filtered ports may be blocked by firewalls.
