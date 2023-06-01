# proxmox


- nano /etc/hosts

- nano /etc/network/interfaces



'''
auto ens18 iface ens18 inet static address 66.70.243.181 netmask 255.255.255.0 broadcast 66.70.243.255 gateway 66.70.243.254 dns-nameservers 8.8.8.8 8.8.4.4
'''
- service network-manager

-  /etc/hosts

- /etc/network/interfaces

'''
auto lo
iface lo inet loopback

auto vmbr0
iface vmbr0 inet static
address 192.168.3.2
netmask 255.255.255.0
gateway 192.168.3.1
bridge_ports eth0
bridge_stp off
bridge_fd 0
'''


- http://kuwox.blogspot.com/2016/08/proxmox-virtualizando-cambiando.html
