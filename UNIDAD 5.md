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

### Tipos principales de NAT

| **Tipo**               | **Descripción**                                                                                                                            | **Uso común**                                                                |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------- |
| **NAT Estático**       | Asigna una IP privada fija a una IP pública fija (relación 1 a 1).                                                                         | Servidores web o servicios internos que deben ser accesibles desde Internet. |
| **NAT Dinámico**       | Asigna una IP privada a una IP pública disponible dentro de un grupo (_pool_) de direcciones públicas.                                     | Redes empresariales con múltiples IP públicas contratadas.                   |
| **PAT / NAT Overload** | Permite que cientos de dispositivos privados compartan **una sola IP pública** diferenciando cada conexión mediante **números de puerto**. | Routers domésticos y redes de oficinas pequeñas (el estándar más usado).     |

#### Direcciones Especiales
127.0.0.1 es el lopback (El propio equipo) y el 169.254.0.0/17 es la asignacion automatica cuando falla el DHCP.

#### Direcciones IPv4
una dirección IPv4 tiene 32 bits escritos en 4 octetos decimales separados por puntos, como 192.169.1.10; una parte identifica la red y la otra el host.
