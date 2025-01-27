#Teoría

# ¿Qué es una red?
Dispositivos de computación interconectados que pueden intercambiar datos.

# Hablemos de historia 
Internet nació en 1970
- 1970 - 1980: Cada quien lo suyo. Cada vendor tenía su protocolo.
- ISO a finales de 1970
	- Open Systems Interconnection (Modelo OSI). Forma de encapsular los datos para unificar los datos y poder transferir y recibir de todos.
- Modelo TCP/IP vs OSI

Forma de representar cómo se transmite la información.

Módelo OSI
Layer 7: Application.
Layer 6: Presentation 
Layer 5: Session. 
Layer 4: Transport 
Layer 3: Network 
Layer 2: Data Link 
Layer 1: Physical 

Módelo TCP/IP __ PDU(Packet Data Unit )
- Application: Data (correo wa)
- Transport: (Se divide, Segmento). Nos permite identificar una aplicación de otra, se diferencia a través del puerto. En esta capa se guarda el puerto.
- Networking: (Packet). ¿Cómo va a pasar por la red?, nos da la dirección de la casa a qué parte del mundo tengo que llegar, esta dirección tiende a ser única, obtiene la dirección IP, direccionamiento lógico.
- Data link: (Trama/Frame) En el módelo TCP/IP Estás dos con la de abajo son capa 1. La dirección física, la MAC Addres, direccionamiento físico
- Física: Bits No cuenta cómo PDU, aquí se traduce en 1 y 0.


| Bits | D.L trama | NW  | Trans | Data | Footer |
| ---- | --------- | --- | ----- | ---- | ------ |

# Componentes de una red
Endpoints: Todos los dispositivos que se conecten a internet
Intermediate devices: Router, L2 Switch, L3 Switch, Access Point, Wireless Router, IPS (Intrusion Prevention System), Firewall, Virtual Router.
Media: Formas de conectar, 5G,  


Router Inalámbrico: Access Point, Router, Switch


# Application Layer
Los servicios que se consumen: 
- Whatsapp
- El correo para enviar la tarea.
- Las stories de Instagram.
- Tik Tok

El aplicativo más usado es el browser.
HTTP: Hyper Text Transfer Protocol. Cliente - Servidor
Tim Berners Lee - Fundador de WWW en los 90

# Transport Layer
Cómo voy a mandar mi paquete.
- Nos dice que aplicación es.
- La que separa tus aplicaciones al recibir información.
- Dos protocolos importantes.
	- TCP - Transmission Control Protocol.
	- UDP - User Datagram Protocol. Un ejemplo es una video llamada, por ejemplo, porque no se retransmite.
- Una de las funciones más importante de TCP: Error Recovery, es decir, manda respuesta.

# Network Layer
- El famoso protocolo IP ... Internet Protocol.
- Su dirección se considera lógica, no sé que hay, no sé donde es, pero sé que está ....
- Funciona como el servicio Postal.
- Existen direcciones IPv4 y IPv6

# Data - Link and Physical Lawyer
## Data - link layer
- Define el protocolo y el control de uso del medio.
	- Ethernet.
	- Wireless LAN.
- Aquí entra la dirección MAC.
- El direccionamiento es físico.
## Physical Layer.
- Define el medio que se empleará para la transmisión.
	- Cobre.
	- Banda EM.
	- FIbra.

# Data Encapsulation.


SOHO (Small Office HOme Office), tecnicamente hablando todas nuestras casas son SOHO.

El router procesa y envía a internet
Y se envía por switch si estás conectado o por access point si no estás conectado con cable.


## Ethernet LAN
- PAN: Personal Area Network (Bluetooth)
- LAN: Local Area Network () tiende a tener un radio de 100 metros.
- MAN: Metropolitan Area Network.
- WAN: Wide Area Network (Interconectar LAN con otras)

Todos estos términos los define la IEEE ()

Ethernet es un conjunto de estándares LAN de las capas Physical & Data-Link  


En una red empresarial hay diferentes tipos de LAN, 

El cable "ethernet" es un cable UTP(Unshielded Twisted Pair),  la IEEE es quien le puso el nombre
802.3 es ethernet empezó con 10 Mbps (megabytes por segundo). 10 BASE - T

Tiene que estar torcido para anular el campo magnético de los dos cables.
- Existen diferentes tipos 


Conexión.
- Se emplean Ethernet NIC(Network Interphace Card) para conectar al dispositivo. Es decir la tarjeta de red donde está la entrada.
- Se emplea un conector RJ-45 ( La punta del cable)

Transceivers.
¿Qué pasa si el factor de conversión (para dar verlocidad del enlace) no es la suficiente?
- Puedes cambiar algunos puertos por otros convertidores
Algo que le puedo puedo colocar en mi switch para adaptar y enviar más megas.

Frecuencia: Qué tanto tuerces el cable, entre más, da mayor velocidad. Hay una mayor integridad de los datos.



Estándares de Ethernet
Lo qué termina en T es cobre y lo que termina en LX es fibra óptica

| Speed     | Common Name      | Informal IEEE standard | Formal IEEE Standard | Cable Tupe. Maximum Length |
| --------- | ---------------- | ---------------------- | -------------------- | -------------------------- |
| 10 Mbps   | Ethernet         | 10BASE-T               | 802.3                | Cobre, 100m                |
| 100 Mbps  | Fast Ethernet    | 100BASE - T            | 802.2u               | Cobre, 100m                |
| 1000Mbps  | Gigabit Ethernet | 1000BASE - LX          | 802.3z               | Fiber, 5000m               |
| 1000 Mbps | Gigabit Ethernet | 1000BASE-T             | 802.3ab              | Cobre, 100m                |
| 10 Gbps   | 10 Gig Ethernet  | 10GBASE-T              | 802.3an              | Cobre, 100m                |
La señal se degrada en un cable de cobre conforme pasa la distancia, a los 100m la señal ya está muy corrompida, normalmente 80 ya sería lo máximo.

La regla de oro de redes, el que manda es el más débil.

## ¿Cómo se arma un cable UTP?
- Straight:
	- Los pines se conservan en su posición.
	- Entre dispositivos que transmiten en diferentes pines.
- Crossover:
	- Cada par se "cruza" con el otro par.
	- Entre dispositivos que transmiten en los mismo pines.

Automdix: Le decía a la tarjeta, cambia de receptor a transmisor y viceversa, así es cómo se crea el cable directo.

---

Tarea
- [ ] traer cable UTP categoría 6 en steren. 2 metros 
- [ ] Conectores RJ-45, que ya tengan las grecas puestas. x10
- [ ] Pinza ponchacables