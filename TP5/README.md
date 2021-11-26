#Setup DB :

**Install MariaDB :**

*install maria db sur la machine :*
```
sudo dnf install mariadb-server
[...]
Complete!
```
*Le service MariaDB :*
```
sudo systemctl enable mariadb
sudo systemctl start mariadb
systemctl status mariadb
[...]
Active: active (running) since Thu 2021-11-25 12:49:55 CET; 6s ago
[...]
sudo ss -lapt
[...]
LISTEN 0       80                   *:mysql              *:*      users:(("mysqld",pid=26081,fd=21))
[...]
ps -aux | grep mariadb 
marinlo+   26218  0.0  0.1 221928  1156 pts/0    S+   13:38   0:00 grep --color=auto mariadb
"Le processus est lancé par l'user marinlozach
```
*Firewall :*
```
sudo firewall-cmd --add-port=80/tcp --permanent
Success!
sudo firewall-cmd --reload
Success!
"On vérifie"
sudo firewall-cmd --list-all
ports: 80/tcp
```

**Conf MariaDB**

*Configuration élémentaire de la base*
```
