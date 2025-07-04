
Perdida de paquete
Tiempos altos de respuesta
Umbral señal de advertencia
Intermitencia significa que la red se cae por momentos
Latencia significa que la red responde lento, Lelay

Protocolo ICMP: este protocolo informa sobre problemas de conectividad

ICMP Ping / Tiempo de respuesta:
1 es normal quiere decir que responde correctamente **Si sube de 0 a 100**: Es una señal de alerta. Tiempos de respuesta elevados indican latencia en la red, lo que puede causar lentitud en aplicaciones y servicios.

ICMP LOSS / Perdidas de paquetes:
- Idealmente debe ser 0% (ninguna pérdida).
- **Si sube de 0 a 100**: Es malo. Un 100% significa pérdida total de comunicación con el dispositivo, lo que indica que el enlace probablemente está caído o tiene problemas graves.

ICMP RESPONSE TIME
- Valores consistentemente bajos indican un enlace saludable.
- **Si sube**: Indica degradación en la calidad del enlace, posiblemente por congestión o problemas en la infraestructura.