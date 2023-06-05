# proxmox



- cd /etc/network
- sudo cat interfaces
- cambiar la ip y luego reiniciar la red
- sudo networkctl  reload


- /etc/interfaces o /etc/network/interfaces
- nano /etc/hosts
-
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




# samba
samba



sudo apt update
sudo apt upgrade
sudo apt install samba

pwd
/home/samba/agora-compartido
sudo nano /etc/samba/smb.conf 

systemctl status smbd --no-pager -l
sudo service smbd restart
sudo service smbd status

sudo ufw allow samba




windows powershell

Get-SmbServerConfiguration | Select EnableSMB2Protocol




- https://linuxconfig.org/how-to-configure-samba-server-share-on-ubuntu-22-04-jammy-jellyfish-linux
- https://www.culturalibre.net/configurar-un-servidor-de-archivos-samba/


https://www.akirah.es/guia-de-instalacion-de-nextcloud-24-en-ubuntu-22-04-apache/

- https://www.muylinux.com/2016/09/23/carpeta-ubuntu-16-04-samba/


