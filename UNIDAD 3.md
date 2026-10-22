## Glosario

### Capa física

- **Bit:** Unidad mínima de información (0 o 1).
    
- **Señal:** Representación física de los datos (eléctrica, óptica o de radiofrecuencia).
    
- **Ancho de banda:** Capacidad máxima de transmisión de un enlace.
    
- **Rendimiento (throughput):** Transferencia real y efectiva de datos en un momento dado.
    
- **Latencia:** Tiempo que tarda un dato en ir del origen al destino.
    
- **Medio de transmisión:** Material o espacio por donde viaja la señal (cobre, fibra, aire).
    

### Cables y medios

- **Par trenzado (UTP / STP):** Cables de cobre trenzados para reducir interferencias eléctricas.
    
- **Conector RJ-45:** Conector estándar de 8 pines para cables de red.
    
- **Cable directo y cruzado:** Directo conecta equipos distintos; cruzado conecta equipos iguales.
    
- **Fibra óptica:** Hilos de vidrio que transmiten datos mediante pulsos de luz.
    
- **Fibra monomodo y multimodo:** Monomodo usa láser (largas distancias); multimodo usa LED (distancias cortas).
    
- **Interferencia electromagnética (EMI):** Ruido eléctrico externo que corrompe los datos en cables de cobre.
    
- **Wi-Fi (IEEE 802.11):** Estándares para redes locales inalámbricas (WLAN).
    
- **Bandas de 2.4 GHz y 5 GHz:** Frecuencias Wi-Fi. 2.4 GHz tiene más alcance; 5 GHz es más rápida.
    
- **Bluetooth:** Tecnología inalámbrica para conexiones personales de corto alcance (WPAN).
    

### Señalización

- **Codificación:** Convertir bits a un formato que el medio físico acepte.
    
- **Señalización:** Regla física para representar los bits (ej. niveles de voltaje).
    
- **Sincronización:** Coordinación de tiempos de reloj entre el equipo que envía y el que recibe.
    
- **Código Manchester:** Codificación donde el valor del bit se define por un cambio de voltaje a mitad del ciclo.
    

### Ethernet y LAN

- **Ethernet (IEEE 802.3):** Estándar principal para redes locales (LAN) cableadas.
    
- **Tarjeta de red (NIC):** Hardware que conecta un dispositivo físico a la red.
    
- **Switch:** Dispositivo inteligente que envía datos únicamente al puerto del destinatario.
    
- **Hub:** Dispositivo obsoleto que repite la señal a ciegas por todos sus puertos.
    
- **Tabla de direcciones MAC:** Memoria del switch que asocia las MAC de los equipos con sus puertos.
    
- **Dúplex (half y full):** Half es transmitir o recibir por turnos; Full permite ambos simultáneamente.
    
- **Colisión:** Choque y pérdida de datos cuando dos equipos transmiten al mismo tiempo.
    

### Direccionamiento

- **Dirección MAC:** Identificador físico y único de 48 bits grabado en la tarjeta de red.
    
- **OUI:** Los primeros 24 bits de la MAC, que identifican al fabricante del equipo.
    
- **Hexadecimal:** Sistema numérico base 16 usado para representar direcciones MAC e IPv6.
    
- **Unicast:** Comunicación de uno a uno.
    
- **Multicast:** Comunicación de uno a un grupo específico.
    
- **Broadcast:** Comunicación de uno hacia todos en la red.
    

### Enlace de datos

- **Trama (frame):** Paquete de datos en la capa de enlace que incluye origen, destino y control de errores.
    
- **Encabezado y tráiler:** El inicio (control/direcciones) y el final (verificación de errores) de la trama.
    
- **FCS / CRC:** Cálculo matemático al final de la trama para comprobar que no llegó corrupta.
    
- **Subcapa LLC:** Mitad superior de la capa de enlace; se comunica con el software y la capa de red.
    
- **Subcapa MAC:** Mitad inferior de la capa de enlace; controla el hardware y el acceso al medio físico.
    
- **CSMA/CD:** Método en redes cableadas antiguas para detectar colisiones.
    
- **CSMA/CA:** Método en redes inalámbricas (Wi-Fi) para evitar colisiones.

## Actividades 
### Actividad 3.1
Figura explicando porque los cables van en pares.
![[Pasted image 20261015163945.png]]

### Actividad 3.2
Por que los puntos de intercambio reducen la latencia ?
Porque la latencia depende de cuantos saltos y los puntos de intercambio reducen esos saltos.
## Clases
### Clase Dia Martes 20 de Octubre 2026

##### Tipos de cable : Cobre
1. UTP
2. FTP
3. STP
4. SFTP  

##### Tipos de cable : Fibra Optica
La fibra optica usa pulsos de luz, llega a mayores distancias y es inmune a la interferencia electromagnetica, pero es mas costosa y delicada de instalar.

### Clase Dia Jueves 22 de Octubre 2026

Nombre: Diego Juarez

Campo 1
Dato de ejemplo: 10101010 10101010 10101010 10101010 10101010 10101010 10101010 10101011 (8 bytes)
Nombre del campo: Preambulo y SFD
Para qué sirve: Los primeros 7 bytes (Preambulo) sincronizan los relojes de los dispositivos emisor y receptor en la red. El último byte (conocido como SFD) marca el inicio exacto de la trama.

Campo 2
Dato de ejemplo: FFFF.FFFF.FFFF (6 bytes)
Nombre del campo: Direccion MAC de destino
Para qué sirve: Identifica al destinatario en la capa de enlace de datos, lo que significa que la trama debe ser procesada por todos los dispositivos en ese segmento de red.

Campo 3
Dato de ejemplo: 0001.4321.ABCD (6 bytes)
Nombre del campo: Direccion MAC de origen
Para qué sirve: Identifica fisicamente al dispositivo que está enviando la trama dentro de la red local.

Campo 4
Dato de ejemplo: 0x0806 (2 bytes)
Nombre del campo: Tipo / EtherType
Para qué sirve: Indica que protocolo de capa de red esta encapsulado en la carga util de la trama para que el receptor sepa como procesarlo.

Campo 5
Dato de ejemplo: ¿Quién tiene la IP 192.168.1.2? Responde a 192.168.1.1 (entre 46 y 1500 bytes)
Nombre del campo: Datos (Payload)
Para qué sirve: Contiene la informacion o el mensaje proveniente de los protocolos de capas superiores que se esta transportando a traves de la red.

Campo 6
Dato de ejemplo: 0x3A7F91C2 (4 bytes)
Nombre del campo: Secuencia de Comprobacion de Trama
Para qué sirve: Es un mecanismo de deteccion de errores de 4 bytes situado al final de la trama. El dispositivo emisor genera un valor matematico basado en el contenido de la trama y lo coloca aqui, el receptor realiza el mismo calculo para asegurarse de que los datos no se hayan corrompido o alterado durante la transmisión fisica.
