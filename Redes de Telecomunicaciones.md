En los inicios, cada empresa desarrollaba sus propias normas y estándares para crear redes. Esto llevó a la necesidad de
unificar criterios, lo que resultó en la creación de modelos de referencia como el Modelo OSI y el Modelo TCP/IP, que son
los más utilizados en la actualidad.

| OSI             | TCP/IP                   | Protocolo PDU | Protocolos                                              |
| --------------- | ------------------------ | ------------- | ------------------------------------------------------- |
| Aplicación      | Aplicación               | Datos         | telnet, FTP, LPD, SNMP, TFTP,<br>SMTP, NFS, HTTP, HTTPS |
| Presentación    |                          |               |                                                         |
| Sesión          |                          |               |                                                         |
| Transporte      | Transporte               | Segmentos     | TCP, UDP                                                |
| Red             | Internet                 | Paquetes      | ICMP, BOOTP, ARP, IP                                    |
| Enlace de datos | Acceso (Enlace de datos) | Tramas        | Ethernet                                                |
| Física          | Física                   | Bits          |                                                         |
PDU: Representan la forma en que la información se organiza y se transmite entre cada capa.
**Tipos de Redes**
Las redes se clasifican según su alcance geográfico:
1. PAN (Personal Area Network): Red de área personal, como la conexión entre un teléfono y un auricular Bluetooth.
2. LAN (Local Area Network): Red de área local, como la red de una oficina o casa.
3. MAN (Metropolitan Area Network): Red de área metropolitana, que cubre una ciudad o campus.
4. WAN (Wide Area Network): Red de área amplia, como Internet, que conecta redes en diferentes regiones o países.
**Tipos de Comunicación en Redes**
5. Unicast: Comunicación entre un dispositivo emisor y un único dispositivo receptor.
6. Multicast: Comunicación entre un dispositivo emisor y un grupo específico de dispositivos receptores.
7. Broadcast: Comunicación entre un dispositivo emisor y todos los dispositivos conectados a la red.
**Elementos que Componen una Red**
8. Dispositivos Finales: Son los equipos que envían o reciben datos, como computadoras, teléfonos, servidores, etc.
9. Dispositivos Intermedios (Equipos de Acceso ): Facilitan la comunicación entre dispositivos finales. Ejemplos: Router, Switch
10. Medios de físicos de Comunicación:
- Alámbricos: Cables de cobre (como Ethernet) o fibra óptica.
- Inalámbricos: Ondas de radio, Wi-Fi, Bluetooth, etc.

**Funcionamiento de Dispositivos Intermedios**
==Switch:==
- Conecta dispositivos dentro de una misma red.
- Reenvía tramas basándose en direcciones MAC.
- Si no conoce la dirección MAC de destino, realiza un flooding (envía la trama a todos los puertos).
- Opera en la Capa 2 del modelo OSI, aunque; Existen switches de Capa 2 y Capa 3 (estos últimos
pueden realizar funciones de enrutamiento como el reenvío entre VLANs.).

==Router:==
- Conecta redes diferentes.
- Utiliza direcciones IP para enrutar paquetes.
- Implementa algoritmos de enrutamiento (como OSPF, BGP) para determinar la mejor ruta.
- Opera en la Capa 3 del modelo OSI.

Switching es el proceso mediante el cual se transmiten datos dentro de una red local (LAN). El objetivo principal es permitir
la comunicación eficiente entre dispositivos conectados a la misma red.
VLANs (Redes Locales Virtuales): Dividen una red física en múltiples subredes virtuales lógicas. Esto mejora la seguridad y
la organización del tráfico en redes grandes.
Trunking(troncales): Etiquetado de VLANs: En enlaces de trunk, las tramas se etiquetan con identificadores de VLAN para
que los switches sepan a qué VLAN pertenece cada paquete. El protocolo más común para esto es 802.1Q.
Trunk vs Access Ports
Full-Duplex vs Half-Duplex:
 En modo Full-Duplex, el switch permite la comunicación en ambas direcciones simultáneamente, duplicando el
ancho de banda.
 En modo Half-Duplex, solo permite la comunicación en una dirección a la vez.

Routing(Enrutamiento) es el proceso de enviar datos (paquetes) desde un dispositivo en una red hacia otro dispositivo en una red diferente. Los routers son los dispositivos que se encargan de tomar decisiones sobre cómo enviar estos paquetes, basándose en la información de las *tablas de enrutamiento. Estas tablas contienen las rutas que indican cómo llegar a diferentes redes.
Interfaces loopback son interfaces virtuales (no físicas) que existen dentro de un router. No están conectadas a ningún cable o dispositivo físico.
Protocolos de enrutamiento Son reglas y algoritmos que permiten a los routers compartir información sobre cómo llegar a diferentes redes. Los más comunes son: RIP, OSPF y BGP.
OSPF (Open Shortest Path First):
- Más avanzado que RIP.
- Usa el concepto de &quot;costo&quot; (basado en ancho de banda) para determinar la mejor ruta.
- Es adecuado para redes grandes y complejas.
- Es un protocolo de enrutamiento de &quot;estado de enlace&quot;.
**BGP (Border Gateway Protocol):
- Se usa para enrutamiento entre diferentes sistemas autónomos (redes de diferentes organizaciones o proveedores de Internet).
- Es el protocolo que hace posible el funcionamiento de Internet.
- Enfocado en políticas y rutas más que en velocidad.
NAT (Network Address Translation):
Técnica utilizada por routers para traducir direcciones IP privadas en direcciones IP públicas. Es esencial para que dispositivos dentro de una red puedan comunicarse con el exterior (Internet).
NAT estático, dinámico y PAT (Port Address Translation).
Enrutamiento estático: Las rutas son configuradas manualmente. Es adecuado para redes pequeñas y simples. 
Enrutamiento dinámico: Los protocolos como RIP, O SPF y BGP, eBGP permiten que los routers actualicen automáticamente las rutas según los cambios en la red
**Tecnologías comunes en redes WAN**
1. MPLS (Multiprotocol Label Switching): Optimiza el enrutamiento de datos y mejora la velocidad y eficiencia.
2. VPN (Virtual Private Network): Proporciona conexiones seguras a través de redes públicas.
3. Frame Relay y ATM: Tecnologías más antiguas, pero aún en uso en algunas redes.
4. SD-WAN (Software-Defined WAN): Una solución moderna que utiliza software para gestionar y optimizar el tráfico de red.
5. Conexiones inalámbricas: Incluyen tecnologías como LTE, 4G/5G y satélites.
MPLS (Multi-Protocol Label Switching)
- Es una tecnología que mejora el rendimiento de las redes WAN.
- En lugar de usar direcciones IP para enrutar paquetes, MPLS usa &quot;etiquetas&quot; para tomar decisiones de enrutamiento más
rápidas.
- Es muy utilizado por proveedores de servicios para ofrecer conexiones confiables y de alta velocidad.
SD-WAN (Software-Defined Wide Area Network)
- Es una tecnología moderna que permite gestionar y optimizar conexiones WAN de manera inteligente.
- Usa software para decidir automáticamente la mejor ruta para el tráfico (por ejemplo, entre MPLS, Internet o LTE).
La conexión de fibra óptica (FO) punto a punto puede considerarse una tecnología WAN, siempre y cuando se utilice para conectar ubicaciones que estén geográficamente separadas. Por ejemplo, si se utiliza para interconectar oficinas en distintas ciudades o países, se clasifica como una solución WAN.
 Extensión geográfica: Permite comunicación directa entre dos puntos separados por largas distancias.
 Alta velocidad: Proporciona capacidad de transmisión de datos a velocidades muy altas, ideal para aplicaciones
empresariales y telecomunicaciones.
 Infraestructura física: Utiliza cables de fibra óptica, que son comunes en implementaciones WAN para asegurar
estabilidad y baja latencia.
Tipo de clasificación de las redes, la clasificación de las redes según su topología, la llamada &quot;Topología de las Redes&quot;
¿Qué es la Topología de Red?
Se denomina topología de red a la forma en que se organizan los componentes de una red (cables, tarjetas de red, otros
equipos) Dependiendo de la disposición física, es decir la configuración espacial del equipo de red, se distingue las
siguientes topologías:
1) topología en bus
2) topologia en anillo
3) topologia en estrella
4) topología doble anillo
5) topología en arbol
6) red de malla
Switch de borde(Border Access) BA Solo si llegan enlaces y/o son frontera entre una tienda y otra
Switch Accesos SA Todo equipo SW que no sea BA
CEDGE CE dedicado a los CEDGE de SDWAN BANCO
Border Router BR normalmente se da en WIFI que posee un Router
Firewall Perimetral FP
Distribucion / Agregacion AG Cuando un switch conecta a otros switch, pero no Endpoint , se considera
AG cuando posee 5 o menos usuarios
Servicios(Enlace) de internet 
 Correo electrónico, Redes sociales, Aplicaciones móviles, Juegos multijugador en línea
 Telefonía por Internet
 Intercambio de archivos
 Servicios de transmisión de medios
Servicios(enlace) de datos 
 Permiten la transmisión privada de datos a través de una red
 Garantizan la comunicación entre sucursales u oficinas remotas
proveedor de servicios de red o telecomunicaciones es ISP
Balanceo de Carga (Load Balancing)
Es una técnica que distribuye el tráfico de red o las solicitudes entrantes entre múltiples servidores o rutas para:
Optimizar el uso de recursos
Maximizar el rendimiento
Reducir la latencia
Evitar la sobrecarga de un solo dispositivo
Failover (Conmutación por error)
Es un mecanismo de contingencia que:
Detecta automáticamente cuando un dispositivo o enlace falla
Redirige el tráfico hacia un dispositivo o enlace secundario (de respaldo)
Permite mantener la continuidad del servicio sin intervención manual
Se enfoca en la alta disponibilidad y recuperación ante fallos