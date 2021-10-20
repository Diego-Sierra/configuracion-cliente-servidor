# **Docker Configuración cliente + servidor DNS**
***
+ Instalación herramientas de red  
Introducimos los comandos para instalar las herramientas tras hacer apt update  
    + ping  
    
      apt install iputils-ping
    + tracepath  
    
      apt install iputils-tracepath
    + traceroute  
    
      apt install traceroute
    + MTR  
    
      apt install mtr
    + ifconfig  
    
      apt install net-tools
    + ifdown-ifup  
    
      apt install ifupdown
    + ip adress show  
    
      apt install iproute2
    + host  
    
      apt install host
    + route  
    
      instalado con net-tools
    + ifplugstatus  
    
      apt install ifplugd.
    + dhclient  
    
      isc-dhcp-client
    + netstat  
    
      instalado con net-tools
    + whois  
    
      apt install whois
    + wget curl  
    
      apt install wget && apt install curl
    + dig  
    
      apt install dnsutils  
      
+ Configura el cliente para que su DNS sea el otro contenedor
    + instalar nano  
    
      apt install nano
    + modificar archivo resolve  
     
      nano /etc/resolv.conf
    + añadir ip del servidor dns en resolve  
    
      nameserver 172.22.0.3
    + comprobar con dig


      dig google.es y el resultado es SERVER: 172.22.0.3
