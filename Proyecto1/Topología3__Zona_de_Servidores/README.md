# ***TOPOLOGIA NO. 3***
-----------------------------------------
## **INDICE**
-----------------------------------------
1. [**TOPOLOGIA**](#topo)
2. [**CLIENTES**](#cls)
   1. [**CLIENTE 1**](#cl1)
   2. [**CLIENTE 2**](#cl2)
   3. [**CLIENTE 3**](#cl3)
3. [**TRANSPARENTE**](#trs)


<div id = "topo">

## **TOPOLOGIA**
-----------------------------------------
![This is a alt text.](../pictures/topologia3.png "Topologia completa")

<div id="cls">

## **CLIENTES**
-----------------------------------------

<div id="cl1">

*CLIENTE 1 (SW8)*

```shell
configure terminal
vtp domain GRUPO4
vtp password grupo4
vtp version 2
vtp mode client
exit
sh vtp status
configure terminal
int f1/0
switchport mode access
switchport access vlan 40
exit
int f1/1
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit
int f1/10
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit
```

<div id="cl2">

*CLIENTE 2 (SW9)*

```shell
configure terminal
vtp domain GRUPO4
vtp password grupo4
vtp version 2
vtp mode client
exit
sh vtp status
configure terminal
int f1/0
switchport mode access
switchport access vlan 40
exit
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

*CLIENTE 3 (SW10)*

```shell
configure terminal
vtp domain GRUPO4
vtp password grupo4
vtp version 2
vtp mode client
exit
sh vtp status
configure terminal
int f1/0
switchport mode access
switchport access vlan 40
exit
int f1/1
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit
int f1/2
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit
```

<div id="trs">

## **TRANSPARENTE**
-----------------------------------------

*TRANSPARENT*

```shell
conf t
vtp domain GRUPO4
vtp password grupo4
vtp version 2
vtp mode transparent
vlan 20
name Informatica
exit
sh vtp status
conf t
int f1/0
switchport mode access
switchport access vlan 20
exit
int f1/1
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit
int f1/3
switchport mode trunk
switchport trunk allowed vlan 1,10,20,30,40,1002-1005
exit
```
