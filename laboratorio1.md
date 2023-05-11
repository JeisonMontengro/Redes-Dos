# Laboratorio de redes 1 
<p><code>Laboratorio 1 de redes 2</code></p>
<p>Realizado <code>Jeison Daneiro Montenegro Cuasialpud</code>

## 1. [Configurar el entorno de trabajo](#) ✔ 
 1. Instalar [VSCode][1_1] 
 2. Instalar [Git][1_2] 
 3. Crear una cuenta en [github][1_3] 
 4. Crear el repositorio en Github llamado <code>Redes-dos</code> 
 5. Instalar la [extension de github][1_4] para VScode 
 6. Agregar <code>Usuario</code> y <code>Correo</code> globalmente para Git. 
 7. Clonar el repositorio remoto desde VScode. 
  
 bash 
 # Para agregar Usuario y Contraseña a GIT 
 $ git config --global user.name "John Doe" 
 $ git config --global user.email johndoe@example.com 
  
  
 [1_1]:https://code.visualstudio.com/download 
 [1_2]:https://git-scm.com/download/win 
 [1_3]:https://github.com/ 
 [1_4]:https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github 
  
  
  
 ## 2. [Preguntas de conocimiento](#) ✔ 
  
 <ol type="a"> 
 <li>¿Cual es la dirección de red y de broadcast de un host que tiene una ip 192.168.10.10/30 .?</li> 

   Ip = 192.168.10.10/30 
   
   Dirección de Red = 192.168.10.8/30

   Direccion de Broadcast = 192.168.10.11

   Host Minimo = 192.168.10.9

   Host Maximo= 192.168.10.10

 <li>¿Cuantos clientes puede tener la sub red 172.16.0.0/22?.</li> 
 <li>¿Que clase y tipo de dirección es 10.10.10.0/24?.</li>

   Es de clase A y es de tipo Privada
 <li>¿Que información se puede inferir de la dirección 169.254.255.200/26?.</li> 

   Se puede inferir que es de clase B porque su primer octeto esta en el rango de 128 a 191 y es de tipo publica
 </ol> 
  
 ## 3. [Caracterización de los adaptadores](#) ✔ 
 |Parámetro||Valor| 
 |--|:--:|--:| 
 |Número de adaptadores Físicos|-->|3| 
 |Número de adaptadores Virtuales|-->|1| 
 |Tipo de Adaptador principal|-->|Ethernet| 
 |Fabricante del Adaptador principal|-->|Realke PCle Family Controller| 
 |Código MAC del fabricante|-->|| 
 |MAC|-->|1C-BF-C0-35-CF-C6| 
  
 >Nota: Para obtener los parámetros de la red, usaremos los comandos [ipconfig][10], [ifconfig][8], [getmac][9]. 
  
  
 ## 4. [Caracterización de la red](#) ✔ 
 |Parámetro|Valor| 
 |--|--:| 
 |_Subnet_|| 
 |IPv4|192.168.1.43| 
 |Subnet Mask decimal|24| 
 |Subnet Mask octetos|255.255.255.0| 
 |Número de direcciones de Host|254| 
 |Rango de direcciones de Host|108.177.13.188| 
 |IP Broadcast|192.168.1.255| 
 |Server DHCP|192.168.1.1| 
 |Server DNS|8.20.247.20| 
  
 >Nota: Para obtener los parámetros de la red, usaremos el comando [ipconfig][10] o [ifconfig][8]. 
  
  
 ## 5. [Caracterización de la puerta de enlace](#) ✔ 
 |Parámetro|Valor| 
 |--|--:| 
 |Número de Entradas en la tabla ARP |8| 
 |IPv4 Gateway|26.0.0.1| 
 |MAC Gateway|| 
 |ISP|Sistemas palacios| 
 |[IP Publica][5]|8.242.185.2| 
 |Sistema Autónomo|| 
  
  
 >Nota: Para obtener los parámetros de la red, usaremos el comando [arp][11] y algún servicio web/HTTP. 
  
  
 ## 6. [Retardo de la red](#) ✔ 
 |Servidor|IP|Tiempo promedio/ms| 
 |--|--|--| 
 |DNS Google|8.8.8.8|11ms| 
 |DNS Cloudflare|1.1.1.1|78ms| 
 |OpenDNS|208.67.222.222|95 ms| 
 |Alternate DNS|208.67.220.220|113 ms| 
 |DNS Quad9|9.9.9.9|125 ms| 
 |AdGuard DNS|94.140.14.14|80 ms| 
  
 >Nota: Para calcular el retardo de la red, usaremos el protocolo ICMP/[ping][12] con al menos 10 paquetes. 
  
  
 ## 7. [Capacidad del canal](#) ✔ 
 |Servidor|Ping/ms|Down/MB|Up/MB| 
 |--|:--:|--:|--:| 
 |[speed test][1]|Tiempo de Espera Agotado para Esta Solicitud||| 
 |[Netflix][2]|Tiempo de Espera Agotado para Esta Solicitud||| 
 |[Claro][3]|Tiempo de Espera Agotado para Esta Solicitud||| 
 |[nperf][4]|164 ms||| 
  
 >Nota: Para calcular el retardo de la red, usaremos el protocolo HTTP via servicio WEB. 
  
  
 ## 8. [Distancia desde el host](#) ✔ 
 |Servidor|Ping/ms|Numero de Saltos| 
 |--|:--:|--:| 
 |google.com|144 ms|10| 
 |GMail.com|83 ms|9| 
 |YouTube.com|102 ms|11| 
 |dns.google|73 ms|12| 
 |aws.amazon.com|32 ms|20| 
 |portal.azure.com|156 ms|28| 
 |login.live.com|209 ms|23| 
 |Facebook.com|414 ms|13| 
 |c.ns.WhatsApp.net|1478 ms|2| 
 |claro.com.co|Tiempo de espera agotado para esta solicitud|3| 
 |platzi.com|933 ms|No se puede resolver el nombre del sistema de destino Platzi.com.| 
 |rappi.com.co|Tiempo de espera agotado para esta solicitud|2| 
  
 >Nota: Para calcular el retardo de la red, usaremos el comando ICMP/[tracert][13]. 
  
 ## 9. [Diagrama de Red](#) ✔ 
 - Realice un diagrama topológico de la red que le ofrece conectividad a internet. 
 - Incluya todos los detalles de la red de area local a la que se encuentra conectado. 
 - Incluya los saltos conocidos incluyendo el equipo de borde de su ISP. 
  
 ## 10. [Preguntas de conocimiento](#) ✔ 
 1. Cual es la dirección de red y de broadcast de un host que tiene una ip 192.168.10.10/30. 
 1. Cuantos equipos o. 
 1. Incluya los saltos conocidos incluyendo el equipo de borde de su ISP.