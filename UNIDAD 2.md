## <mark style="background:#ff4d4f">NOTAS</mark>
Los IXP sirven para crear rutas mas cortas para el trafico de intenet.
### Clase Dia Martes 22 de Septiembre 2026

##### Clasificacion de Redes :

Red de Area Personal (PAN)
Las redes PAN conecta dispositivos que pertenecen a una misma persona y estan a una distacia muy corta entre si, alcence maximo de 10 m.

Red de Area Local (LAN)
Las redes LAN conecta dispositivos dentro de un espacio fisico unico : una casa, una oficina, un salon de clases o un solo edificio. Sus caracteristicas son que una sola organizacion controla y administra por completo, suele tener una alta velocidad y bajo costo por su alcance limitado.

Red Inalambrica de Area Local (WLAN)
Las redes WLAN son una LAN que usa el espectro radioelectronico en lugar de cables para conectar los dispositivos dentro del mismo espacio. Sus caracteristicas son el acceso se hace atraves de cables o mas puntos de acceso (AP), el medio es compartido y mas sensible a interferencia.

Red de Area Amplia (WAN)
Las redes WAN conecta redes que estan geograficamente distantes, a veces en distintas ciudades, paises o continentes. Sus caracteristicas son que no la administra una organizacion, suele depender de proveedores de telecomunicaciones, su costo y latencia son mayores a la LAN.

Comparacion de alcances de Menor a Mayor :
1. PAN (Una Persona)
2. WLAN (Un Edificio)
3. Campus Area Network CAN (Varios Edificios de una Organizacion)
4. WAN (Distintas Ciudades o Paises)
La diferencias entre ellas no es que tecnologia usan, sino quien las administra y que tan lejos llega, eso determina si es PAN, LAN, CAN O WAN


#### ACTIVIDAD 2.1


|                     | PAN                                                                                                                                                | LAN                                                                                                                                | WLAN                                                                                                                                           | CAN                                                                                                                                            | WAN                                                                                                                                                  |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **DEFINICION**      | Las redes PAN conecta dispositivos que pertenecen a una misma persona y estan a una distacia muy corta entre si.                                   | Las redes LAN conecta dispositivos dentro de un espacio fisico unico.                                                              | Las redes WLAN son una LAN que usa el espectro radioelectronico en lugar de cables para conectar los dispositivos dentro del mismo espacio.    | Las redes CAN conectan redes de área local dentro de una misma zona geográfica delimitada.                                                     | Las redes WAN conecta redes que estan geograficamente distantes, a veces en distintas ciudades, paises o continentes.                                |
| **CARACTERISTICAS** | Cobertura de unos pocos metros       (1-10m).         Conecta dispositivos personales (relojes, audífonos).    Bajo consumo de energía (Bluetooth) | Cobertura en un solo edificio u oficina. Conexión por cable de alta velocidad (Ethernet). Administración y propiedad 100% privada. | Mismo alcance que una LAN, pero sin cables (Wi-Fi).    Permite movilidad dentro de la zona de cobertura. Susceptible a interferencias y muros. | Interconecta varias LAN en un mismo complejo. Abarca múltiples edificios contiguos (universidad). Infraestructura privada de fibra o cableado. | Cobertura geográfica masiva (ciudades, países.       Utiliza infraestructura pública o alquilada (ISPs). Mayor latencia por las grandes distancias\| |
| **EJEMPLOS**        | Conexion entre un celular y audifonos o entre una computadora y un celular                                                                         | Conexion de una casa o un salon de clases.                                                                                         | Conexion Inalambrica de un Modem a un celular o a una computadora.                                                                             | Conexion de un Campus de una universidad o un complejo industrial.                                                                             | Conexionesde internet entre continentes o paises.                                                                                                    |


### Clase Dia Martes 29 de Septiembre 2026

#### Actividad 2.2

| Estándar     | Año  | Frecuencia                        | Velocidad Máxima    | Definición                                                                                                                                                                                                                                                    |
| :----------- | :--- | :-------------------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **802.11a**  | 1999 | 5 GHz                             | 54 Mbps             | Estándar pionero que introdujo la modulación OFDM. Ofrecía altas velocidades y menos interferencias al usar la banda de 5 GHz, pero con un alcance físico menor frente a obstáculos.                                                                          |
| **802.11b**  | 1999 | 2.4 GHz                           | 11 Mbps             | Conocido retroactivamente como **Wi-Fi 1**. Fue el primer estándar adoptado masivamente a nivel comercial. Su banda de 2.4 GHz le daba excelente alcance, pero sufría interferencias de electrodomésticos y teléfonos inalámbricos.                           |
| **802.11g**  | 2003 | 2.4 GHz                           | 54 Mbps             | Conocido como **Wi-Fi 3**. Evolución directa del 802.11b que logró igualar la velocidad del estándar "a" (54 Mbps) manteniendo el amplio alcance y compatibilidad de la banda de 2.4 GHz.                                                                     |
| **802.11n**  | 2009 | 2.4 GHz y 5 GHz                   | 600 Mbps            | Conocido como **Wi-Fi 4**. Revolucionó la conectividad al introducir la tecnología **MIMO** (uso de múltiples antenas para transmisión y recepción) y soporte de doble banda, multiplicando drásticamente la capacidad y la distancia de la señal.            |
| **802.11ac** | 2013 | 5 GHz                             | 433 Mbps a 6.9 Gbps | Conocido como **Wi-Fi 5**. Diseñado exclusivamente para la banda de 5 GHz. Introdujo **MU-MIMO** y canales mucho más amplios para permitir transmisiones ultrarrápidas simultáneas a múltiples dispositivos en entornos densos.                               |
| **802.11ax** | 2019 | 2.4 GHz, 5 GHz y 6 GHz (Wi-Fi 6E) | 9.6 Gbps            | Conocido como **Wi-Fi 6** (y **Wi-Fi 6E**). Orientado a la alta eficiencia en entornos saturados de dispositivos. Incorpora **OFDMA** para gestionar múltiples usuarios a la vez con menor latencia y reduce el consumo de batería de los equipos conectados. |

##### Que es el internet ?
Son millones de redes LAN y WLAN conectadas entre si, ninguna empresa ni gobierno administra internet como un todo, cada red que la compone es administrada de forma independiente y se conecta a las demas por acuerdo mutuo.
- Que la hace funcionar?
TCP/IP (Protocolo).
- Como se conectan entre si ?
A traves de proveedores de servicios de internet (ISP), organizados en niveles : los ISP locales se conectan a otros mas grandes, y estos entre si, hasta formar la red global. Los puntos de intercambio (IXP) son sitios fisicos donde distintos ISP conectan su trafico directamente entre si, en lugar de enviarlo por una ruta mas larga. En resumen reducen latencia y costo de trafico.



