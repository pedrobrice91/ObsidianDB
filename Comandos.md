
   ==**Comandos extreme Networks**==
- show vlan - `Muestra todas las VLANs configuradas`

==Para interfaces:==
- sh port no-refresh - `Muestra el estado de todos los puertos`
- show ipconfig - `Muestra configuración IP de las interfaces`

==Para protocolos de enrutamiento:==
- show ospf neighbor - `Muestra vecinos OSPF`
- show ospf neighbor detail - `Información detallada de vecinos OSPF`
- show iproute origin ospf - para ver la metrica

==Para enrutamiento:==
- `show iproute` - Tabla de enrutamiento completa

==Para descubrimiento:==
- `show lldp neighbors detailed` - Extreme usa LLDP en lugar de CDP para descubrimiento de dispositivos
- sh edp ports all
- sh iparp
--------------------------------------------------------------------------
 # ==**Comandos huawei**==
display interface description // Muestra información de la interfaz. 
display vlan all // Muestra información de vlan. 
display version // Muestra la información de la versión. 
interface ethernet 0/0/1 // Ingresa a la vista de la interface. 
display ip routing-table 0.0.0.0
display running-configuration 

----------------------------------------------------------------------------------------------
 # ==**Comandos Cisco**==
sh vlan: Muestra todas las VLANs configuradas en el switch y qué puertos pertenecen a cada VLAN.

show interface description 
show interface status :proporciona información sobre el estado de todas las interfaces, incluidas las administrativamente desactivadas
show interface GigabitEthernet1/0/1 status :Muestra el estado (activo/inactivo, velocidad, duplex) de una interfaz específica.
show interface Gi1/0/1 con este veo el trafico de la interface
show ip interface brief :Resumen del estado de todas las interfaces con direcciones IP.
show run interface GigabitEthernet1/0/1: Muestra la configuración específica de una interfaz.
show run interface vlan 905: Muestra la configuración específica de una interfaz VLAN.
sh run view full     cuando no funciona directo la interfaz

==Comandos para protocolos de enrutamiento dinámico (como OSPF, EIGRP y BGP)==
- show ip ospf neighbor - Detalla los vecinos de OSPF.

==Comandos para tablas de enrutamiento y conectividad==
- show ip route 0.0.0.0 Muestra información de enrutamiento para una IP específica.
- show ip route - Muestra la tabla de enrutamiento completa del dispositivo.
- traceroute - Prueba la ruta entre el origen y el destino.

==Descubrimiento y Seguridad==
sh cdp neighbors detail: Muestra información detallada de dispositivos Cisco vecinos usando el protocolo CDP.

sh lldp neighbors detail

sh ip arp | in 10.81.118
sh mac address-table in Gi1/0/22

Incidencia
sh ip route 172.22.17.139
sh ip arp 172.22.17.139 copie la mac
trace mac d4f5.ef72.558c d4f5.ef72.558c para seguir mac desde el mismo boatdcas
sh cdp nei te2/1/1 de pra saltar de sw a sw
traceroute mac pegue la mac dos veces y me dijo en que equipo estaba
sh mac add | i 4 primers hexa
Comandos para Tshoot

**En los BROFF para consultar IP:**  
show ip route 10.200.3.17 y seguir la secuencia hasta llegar a la MPLS  
  
**Para validar segmentos en lista de prefijos con su route-map:**

show ip prefix-list HC_SAN_FELIPE_CLARO

Salida del comando:

CL-DCC-FTC-BA-BROFF-06#show ip prefix-list HC_SAN_FELIPE_CLARO

ip prefix-list HC_SAN_FELIPE_CLARO: 12 entries

**Para revisar los route-map configurados en BROFF:**  
show route-map all

Ejemplo es:

route-map BGP-TO-OSPF, permit, sequence 50

 Match clauses:

   ip address prefix-lists: HC_SAN_FELIPE_CLARO 

 Set clauses:

   metric 30

   metric-type type-2

 Policy routing matches: 0 packets, 0 bytes

show ip route static

show ip route connected

show ip ospf database  
 para validar si recibo la default del proveedor

show run partition ip-static-route ---> para ver el area ospf

show run partition router

show run  config view full | begin gigaXXX

show inter Te1/0/1  transceiver

----------------------------------------------------------------------------------------------
Para buscar el cod de servicio desde el broff 
show inter des | in 52705

-----------------------------
Para cambiar el nombre de la interfaz 
Enable para pasar de modo privilegio
CL-RNO-FTC-BA-01#configure terminal 
CL-RNO-FTC-BA-01(config)#interface Te1/1/8
CL-RNO-FTC-BA-01(config-if)#description ***To CL-RNO-FAL-SA-P12***
CL-RNO-FTC-BA-01(config-if)#do wr

-------------------------------------------------------------------------------------
Terminal cmd
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted -Force #Scope ExecutionPolicy quitar las restricciones
net user /do pbriceno                 #permisos en el AD
----------------------------------------------------------------------------------------------
ssh-keygen -R
----------------------------------------------------------------------------------------------