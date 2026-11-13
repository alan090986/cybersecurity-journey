Capa de transporte TCP / UDP  Difrencia.

TCP significa protocolo de control de transmisión el cual debe tener una conexión, realiza una negociación en 3 pasos Three-Way Handshake antes de enviar datos.

UDP No requiere una conexión ni una confirmación de recepción envía Data Gramas, paquetes a máxima velocidad, los cuales a veces no llegan completos.

Modelo OSI vs TCP/IP (lo que importa para seguridad)

    OSI: 7 capas (Física, Enlace, Red, Transporte, Sesión, Presentación, Aplicación). TCP/IP lo simplifica en 4: Acceso a red, Internet, Transporte, Aplicación.

    Para seguridad basta con ubicar: IP = capa 3 (Red), TCP/UDP = capa 4 (Transporte), HTTP/DNS = capa 7 (Aplicación). Los firewalls y proxies actúan en capas distintas.


Puertos 

HTTP    -  80  
HTTPS – 443 
DNS   -  53
SSH – 22 
FTP – 21
SMB  - 445 
RDP - 3389
SMTP - 25/587
MySQL - 3307 

DNS (flujo que debes poder explicar)

al excribir example.com el equipo pregunta por el protocolo en este caso DSN en el puerto 53/UDP al resolver 
consulta la jerarquia raiz - TLD Dominio .com - autorizacion del servidor y se devuelve la ip y el equipo
abre la conexion esto si no lo entendia muy bien en realidad se abren los puertos si pasa el protocolo. 

   

HTTP vs HTTPS

    HTTP: puerto 80, texto plano, visible en Wireshark. Métodos GET/POST, códigos 200/301/403/404/500.

    HTTPS: puerto 443, cifrado con TLS. En Wireshark verás el handshake TLS, pero no el contenido.

    Relevancia: User-Agent y URLs son indicadores en análisis de phishing y tráfico malicioso.

NAT, proxy y firewall

    NAT: traduce IPs privadas a una IP pública. 

    Proxy: intermediario que filtra/registra tráfico.

    Firewall: permite/deniega según reglas (IP, puerto, protocolo). 

