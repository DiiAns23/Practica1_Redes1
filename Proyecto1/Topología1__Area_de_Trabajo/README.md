# ***TOPOLOGIA NO. 1***
-----------------------------------------
## **INDICE**
-----------------------------------------
1. [**TOPOLOGIA**](#topo)
2. [**CLIENTES**](#cls)
   1. [**ESW1**](#cl1)
   2. [**ESW2**](#cl2)
   3. [**ESW3**](#cl3)
3. [**IP**](#ip)

<div id = "topo">

## **TOPOLOGIA**
-----------------------------------------
![This is a alt text.](../pictures/topologia1.png "Topologia completa")
<div id="cls">

<div id="cl1">

*ESW1*

```shell
conf t
vtp domain GRUPO4
vtp password grupo4
vtp version 2
vtp mode client

int f1/1
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit

int f1/2
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit

int f1/3
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit
```

<div id="cl3">

*ESW2*

```shell
conf t
vtp domain GRUPO4
vtp password grupo4
vtp version 2
vtp mode client

int f1/1
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit

int f1/2
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit

int f1/3
switchport mode access
switchport access  vlan 10
exit

int f1/4
switchport mode access
switchport access  vlan 30
exit

int f1/5
switchport mode access
switchport access  vlan 10
exit
```
<div id="ESW3">

*ESW3*
```shell
conf t
vtp domain GRUPO4
vtp password grupo4
vtp version 2
vtp mode client

int f1/1
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit

int f1/3
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit

int f1/5
switchport mode access
switchport access  vlan 20
exit

int f1/4
switchport mode access
switchport access  vlan 40
exit

int f1/2
switchport mode access
switchport access  vlan 30
exit
```

<div id="ip">

*IPs*
```shell
RRHH1_1: 
ip 192.168.41.10 255.255.255.0 192.168.41.1

RRHH1_2
ip 192.168.41.20 255.255.255.0 192.168.41.1

Conta_1
ip 192.168.43.10 255.255.255.0 192.168.43.1

Conta_2
ip 192.168.43.20 255.255.255.0 192.168.43.1

Ventas_1
ip 192.168.44.10 255.255.255.0 192.168.44.1

Informatica_1
ip 192.168.42.10 255.255.255.0 192.168.42.1
```