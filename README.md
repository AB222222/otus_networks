# otus_networks

Теоретическая часть.

Сеть office1

```
e@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.2.0 26 
  Network address: 192.168.2.0/26

          Netmask: 255.255.255.192
         Wildcard: 0.0.0.63

       IP address: 192.168.2.0 (OK)
Broadcast address: 192.168.2.63
       First host: 192.168.2.1
        Last host: 192.168.2.62
  Number of hosts: 62
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.2.64 26
  Network address: 192.168.2.64/26

          Netmask: 255.255.255.192
         Wildcard: 0.0.0.63

       IP address: 192.168.2.64 (OK)
Broadcast address: 192.168.2.127
       First host: 192.168.2.65
        Last host: 192.168.2.126
  Number of hosts: 62
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.2.128 26
  Network address: 192.168.2.128/26

          Netmask: 255.255.255.192
         Wildcard: 0.0.0.63

       IP address: 192.168.2.128 (OK)
Broadcast address: 192.168.2.191
       First host: 192.168.2.129
        Last host: 192.168.2.190
  Number of hosts: 62
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.2.192 26
  Network address: 192.168.2.192/26

          Netmask: 255.255.255.192
         Wildcard: 0.0.0.63

       IP address: 192.168.2.192 (OK)
Broadcast address: 192.168.2.255
       First host: 192.168.2.193
        Last host: 192.168.2.254
  Number of hosts: 62
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ 
```

Сеть office2

```
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.1.0 25
  Network address: 192.168.1.0/25

          Netmask: 255.255.255.128
         Wildcard: 0.0.0.127

       IP address: 192.168.1.0 (OK)
Broadcast address: 192.168.1.127
       First host: 192.168.1.1
        Last host: 192.168.1.126
  Number of hosts: 126
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.1.128 26
  Network address: 192.168.1.128/26

          Netmask: 255.255.255.192
         Wildcard: 0.0.0.63

       IP address: 192.168.1.128 (OK)
Broadcast address: 192.168.1.191
       First host: 192.168.1.129
        Last host: 192.168.1.190
  Number of hosts: 62
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.1.192 26
  Network address: 192.168.1.192/26

          Netmask: 255.255.255.192
         Wildcard: 0.0.0.63

       IP address: 192.168.1.192 (OK)
Broadcast address: 192.168.1.255
       First host: 192.168.1.193
        Last host: 192.168.1.254
  Number of hosts: 62
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ 
```

Сеть central

```
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.0.0 28
  Network address: 192.168.0.0/28

          Netmask: 255.255.255.240
         Wildcard: 0.0.0.15

       IP address: 192.168.0.0 (OK)
Broadcast address: 192.168.0.15
       First host: 192.168.0.1
        Last host: 192.168.0.14
  Number of hosts: 14
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.0.32 28
  Network address: 192.168.0.32/28

          Netmask: 255.255.255.240
         Wildcard: 0.0.0.15

       IP address: 192.168.0.32 (OK)
Broadcast address: 192.168.0.47
       First host: 192.168.0.33
        Last host: 192.168.0.46
  Number of hosts: 14
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.0.64 26
  Network address: 192.168.0.64/26

          Netmask: 255.255.255.192
         Wildcard: 0.0.0.63

       IP address: 192.168.0.64 (OK)
Broadcast address: 192.168.0.127
       First host: 192.168.0.65
        Last host: 192.168.0.126
  Number of hosts: 62
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ 
```

Тогда свободные подсети есть только в сети Central:

```
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.0.16 28
  Network address: 192.168.0.16/28

          Netmask: 255.255.255.240
         Wildcard: 0.0.0.15

       IP address: 192.168.0.16 (OK)
Broadcast address: 192.168.0.31
       First host: 192.168.0.17
        Last host: 192.168.0.30
  Number of hosts: 14
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.0.48 28
  Network address: 192.168.0.48/28

          Netmask: 255.255.255.240
         Wildcard: 0.0.0.15

       IP address: 192.168.0.48 (OK)
Broadcast address: 192.168.0.63
       First host: 192.168.0.49
        Last host: 192.168.0.62
  Number of hosts: 14
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ netcalc 192.168.0.128 25
  Network address: 192.168.0.128/25

          Netmask: 255.255.255.128
         Wildcard: 0.0.0.127

       IP address: 192.168.0.128 (OK)
Broadcast address: 192.168.0.255
       First host: 192.168.0.129
        Last host: 192.168.0.254
  Number of hosts: 126
me@me-HP-260-G3-DM:~/otus-linux/DZ_networks_20210221$ 
```

Практическая часть.

Прилагаю Vagrantfile.

