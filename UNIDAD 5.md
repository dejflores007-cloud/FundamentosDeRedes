## Actividades
### Actividad 5.1

|        | Que es ? | Para que sirve ? |
| ------ | -------- | ---------------- |
| Capa 2 |          |                  |
| Capa 3 |          |                  |
| Capa 4 |          |                  |


## Clases
### Clase Dia Martes 17 de Noviembre 2026

#### Red y HOST
Las direcciones publicas son únicas en todo Internet y las asigna el proveedor de servicio (ISP).
Un equipo con dirección pública es alcanzable desde internet; las privadas, no.

- 192.168.1.1
- 192.168.1.2
- 192.168.1.3
- 192.168.1.4

Esos se conectan a un router, y ese router tiene la IP pública 82.129.80.111, que es la que lo conecta a Internet.
#### Direcciones publicas 
Las direcciones publicas son unicas en todo internet y las asigna el proveedor de servicio.
Un equipo con direccion publica es alcanzable desde internet, las privadas no.

#### Direcciones privadas
Se usan solo dentro de una red y no se enrutan en Internet.
Para salir usan NAT.

**NAT** (_Network Address Translation_ o **Traducción de Direcciones de Red**) es un mecanismo utilizado por los routers para modificar la información de las direcciones IP en el encabezado de los paquetes de datos mientras transitan de una red a otra.

Su función principal es permitir que múltiples dispositivos dentro de una **red privada** (LAN) compartan una única **dirección IP pública** para conectarse a Internet.

#### Tipos principales de NAT

| **Tipo**               | **Descripción**                                                                                                                            | **Uso común**                                                                |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------- |
| **NAT Estático**       | Asigna una IP privada fija a una IP pública fija (relación 1 a 1).                                                                         | Servidores web o servicios internos que deben ser accesibles desde Internet. |
| **NAT Dinámico**       | Asigna una IP privada a una IP pública disponible dentro de un grupo (_pool_) de direcciones públicas.                                     | Redes empresariales con múltiples IP públicas contratadas.                   |
| **PAT / NAT Overload** | Permite que cientos de dispositivos privados compartan **una sola IP pública** diferenciando cada conexión mediante **números de puerto**. | Routers domésticos y redes de oficinas pequeñas (el estándar más usado).     |

#### Direcciones Especiales
127.0.0.1 es el lopback (El propio equipo) y el 169.254.0.0/17 es la asignacion automatica cuando falla el DHCP.

#### Direcciones IPv4
una dirección IPv4 tiene 32 bits escritos en 4 octetos decimales separados por puntos, como 192.169.1.10; una parte identifica la red y la otra el host.

### Clase Dia Jueves 19 de Noviembre 2026
#### DHCP

* **Definición:** El **DHCP** (*Protocolo de configuración dinámica de host*) es un servicio que asigna direcciones IP automáticamente a los equipos de la red.
* **Ventajas:** Evita configurar cada equipo a mano y previene conflictos por direcciones duplicadas.
* **Parámetros entregados:** El servidor entrega IP, máscara de subred, puerta de enlace y DNS.
* **Proceso DORA (4 pasos):**
  1. **Discover:** Primer mensaje enviado como *broadcast*.
  2. **Offer:** El servidor ofrece una configuración IP disponible.
  3. **Request:** El cliente solicita la dirección ofrecida.
  4. **Acknowledge:** El servidor confirma y asigna la concesión.

| Paso | Mensaje | Quién lo envía | Qué hace |
|---|---|---|---|
| 1 | Discover | Cliente (broadcast) | Busca un servidor DHCP en la red. |
| 2 | Offer | Servidor | Ofrece una dirección IP disponible. |
| 3 | Request | Cliente (broadcast) | Pide la dirección ofrecida. |
| 4 | Acknowledge | Servidor | Confirma y entrega la configuración. |
#### Tiempo de concesión

* **Préstamo temporal:** La dirección se entrega en **préstamo** por un **tiempo de concesión** (*lease*), no de forma permanente.
* **Renovación:** El cliente **renueva** a la mitad del tiempo.
* **Comandos en Windows:**
  * `ipconfig /release`: libera la dirección.
  * `ipconfig /renew`: pide otra.

#### El pool de direcciones

* **Funcionamiento:** El servidor reparte direcciones de un **pool** (rango) y entrega con ellas la **máscara**, la **puerta de enlace** y el **DNS**.
* **Exclusiones y reservas:** Las direcciones fijas de servidores, impresoras y routers se **excluyen** del pool, o se **reservan** por dirección MAC.
* **Ejemplo de configuración DHCP:**
  * **Pool Name:** `DHCP_P1`
  * **Gateway por Defecto:** `201.10.220.90`
  * **Servidor DNS:** `201.10.220.90`
  * **Inicio de la Dirección IP:** `201.10.248.0`
  * **Subnet Mask:** `255.255.252.0`

#### Puertos y relevo de DHCP

* **Puertos UDP:** DHCP utiliza **UDP**; el servidor escucha en el **puerto 67** y el cliente en el **68**.
* **Relevo (*relay*):** Como el *broadcast* no cruza *routers*, un *router* configurado con `ip helper-address` reenvía las solicitudes a un servidor DHCP ubicado en otra red.