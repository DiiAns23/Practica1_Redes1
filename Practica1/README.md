# **DOCUMENTACION PRACTICA 1 📑**

## Indice 📚

  1. [Introduccion](#introduccion)
  2. [Integrantes](#integrantes)
  3. [Configuracion de la Red Privada](#configuracion-de-la-red-privada)
  4. [Conexiones Ping](#conexiones-ping)
  5. [Ipconfig](#ipconfig)
  6. [Configuracion del Software de VPN (OpenVPN)](#configuracion-del-software-de-vpn-openvpn)
  7. [Integrantes del grupo IAM](#integrantes-del-grupo-iam)
  8. [Creacion y Configuracion de Plataforma Cloud](#creacion-y-configuracion-de-plataforma-cloud)
  9. [Configuracion de las VPCs](#vpc)
  10. [Configuracion de las Nubes](#nubes)
  11. [Pings Entre los Hosts](#hosts)


<div id = 'introduccion'/>

## Introduccion

Durante la realizacion de la _Practica No. 1_ del `Laboratorio de Redes de Computadoras 1` se llevo a cabo la implementacion de una red privada virtual por medio de la plataforma _Google Cloud_. Primeramente, se creo una _Maquina Virtual_, en la cual se ejecuta un proveedor de VPN's (_OpenVPN_). Por medio de OpenVPN, se usaron accesos a clientes y se transfirio los archivos con el acceso a 4 computaodras en diferentes locaciones. Cada computadora realizo pruebas de conexion y se concluyo que la implementacion de una VPN fue un exito. Seguidamente utilizando el programa [GNS3](https://www.gns3.com) se levanto una maquina virtual para poder simular la conexion de una _VPC_ con un _Switch_ conectado a 4 nubes, siendo estas nubes los ordenadores de cada uno de los integrantes del grupo.


<div id = 'integrantes'/>

## Integrantes
| Nombre | Carne | 
|--------|-------|
| Erick Jose Andre Villatoro Revolorio | 201900907 |
| Diego Andrés Obín Rosales | 201903865 | 
| Deivid Alexander Lux Revolorio | 201549059 |
| Josué David Zea Herrera| 201807159 | 
| Juan Diego Alvarado Salguero | 201807335 |

<div id = 'configuracion'/>

## Configuracion de la Red Privada

<div>
    <p align ="center">
        <img width="500" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/confredprivada.jpeg">
    </p>
</div>


<div id = 'ping'/>

## Conexiones Ping

Las pruebas ping se realizaron desde las maquinas conectadas a la VPN que tenian las ip 10.8.0.2-5 hacia la maquina virtual que creo todos los usuarios que se identificaba con la ip 10.8.0.1.

| Cliente 1 | Cliente 2 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/Prueba-2/blob/Master/img/pingcliente1.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/Prueba-2/blob/Master/img/pingcliente2.jpeg">|
| Cliente 3 | Cliente 4 |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/pingcliente3.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/pingcliente4.jpeg">|
| Cliente 5 |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/pingcliente5.jpeg"> | 



<div id = 'ipconfig'/>

## Ipconfig
| Cliente 1 | Cliente 2 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/Prueba-2/blob/Master/img/ipconfig2.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/Prueba-2/blob/Master/img/ipconfig3.jpeg">|
| Cliente 3 | Cliente 4 |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/ipconfig3.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/ipconfig4.jpeg">|
| Cliente 5 |
|  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/ipconfig5.jpeg">|

<div id = 'vpn'/>

## Configuracion del Software de VPN (OpenVPN)

| Cliente 1 | Cliente 2 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/Prueba-2/blob/Master/img/openvpn1.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/Prueba-2/blob/Master/img/openvpn2.jpeg">|
| Cliente 3 | Cliente 4 |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/openvpn3.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/openvpn4.jpeg">|
| Cliente 5 |
|  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/openvpn5.jpeg">|


<div id = 'iam'/>

## Integrantes del grupo IAM

<div>
    <p align ="center">
        <img width="500" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Tarea3_Redes1/IAM.PNG">
    </p>
</div>

<div id = 'cloud'>

## Creacion y Configuracion de Plataforma Cloud

<div>
    <p align ="center">
        <img width="500" src="https://github.com/DiiAns23/Prueba-2/blob/Master/img/configVM.jpeg">
    </p>
</div>


<div id = 'vpc'>

## Configuracion de las VPC's

| Cliente 1 | Cliente 2 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/vpc_1.PNG"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/vpc_2.jpeg">|
| Cliente 3 | Cliente 4 |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/vpc_3.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/vpc_4.jpeg">|
| Cliente 5 |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/vpc_5.jpeg"> | 

<div id = 'nubes'>

## Configuracion de las Nubes

- *_Cliente 1_*
  
| Cliente 2 | Cliente 3 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/obin_erick.PNG"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/obin_deivid.PNG">|
| **Cliente 4** | **Cliente 5** |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/obin_josue.PNG"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/obin_juandi.PNG">|

- *_Cliente 2_*
  
| Cliente 1 | Cliente 3 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/erick_obin.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/erick_deivid.jpeg">|
| **Cliente 4** | **Cliente 5** |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/erick_zea.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/erick_juandi.jpeg">|

- *_Cliente 3_*
  
| Cliente 1 | Cliente 2 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/deivid_obin.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/deivid_erick.jpeg">|
| **Cliente 4** | **Cliente 5** |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/deivid_zea.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/deivid_juandi.jpeg">|

- *_Cliente 4_*
  
| Cliente 1 | Cliente 2 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/zea_obin.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/zea_erick.jpeg">|
| **Cliente 3** | **Cliente 5** |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/zea_deivid.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/zea_juandi.jpeg">|

- *_Cliente 5_*
  
| Cliente 1 | Cliente 2 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/juandi_obin.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/juandi_erick.jpeg">|
| **Cliente 3** | **Cliente 4** |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/juandi_deivid.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/juandi_josue.jpeg">|




<div id='hosts'>

## Pings Entre los Hosts

| Cliente 1 | Cliente 2 |
|:-------------------------:|:-------------------------:|
|<img width="1604" src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/ping_1.PNG"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/ping_2.jpeg">|
| **Cliente 3** | **Cliente 4**  |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/ping_3.jpeg"> |  <img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/ping_4.jpeg">|
| **Cliente 5** |
|<img width="1604"  src="https://github.com/DiiAns23/SoloImagenes/blob/main/Practica_1_Redes_1/ping_5.jpeg"> | 