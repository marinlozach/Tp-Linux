# Checklist

**Choisissez et définissez une IP à la VM**

*Contenu ip a*

    1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
        link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
        inet 127.0.0.1/8 scope host lo
            valid_lft forever preferred_lft forever
        inet6 ::1/128 scope host
            valid_lft forever preferred_lft forever
    2: enp0s3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
        link/ether 08:00:27:91:c0:a1 brd ff:ff:ff:ff:ff:ff
        inet 10.0.2.15/24 brd 10.0.2.255 scope global dynamic noprefixroute enp0s3
            valid_lft 84613sec preferred_lft 84613sec
        inet6 fe80::a00:27ff:fe91:c0a1/64 scope link noprefixroute
            valid_lft forever preferred_lft forever
    3: enp0s8: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
        link/ether 08:00:27:a6:4d:d0 brd ff:ff:ff:ff:ff:ff
        inet 192.168.56.37/24 brd 192.168.56.255 scope global noprefixroute enp0s8
            valid_lft forever preferred_lft forever

