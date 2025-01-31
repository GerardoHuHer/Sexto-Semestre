Using the command line interface (CLI)
¿Cómo nos conectamos a un dispositivo?
Consola. Cable azulito
Telnet: texto plano
SSH: Encriptado
GUI

Por consola se necesita un requisito: 
- Baud rate: 9600 bits/seg
- No hardware Flow control
- 8-bit ASCII (Data bits).
- No parity bits.
- 1 stop bit.
Informalmente a los últimos 3 se les llaman 8n1

## Analyzing Ethernet LAN Switching
### ¿Cómo envía un switch su información realmente?
- Utiliza las MAC address.
- Guarda esas direcciones en una tabla "especial":
	- MAC address table.
	- Más conocida como la CAM (Content-Addressable )
Toda trama que llega al switch, toda **MAC address origen** la va a guardar en al MAC Address table, "yo sé donde vives"

PDU: Packet Data Unit

# Configurin