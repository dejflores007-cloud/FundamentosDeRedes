## <mark style="background:#ff4d4f">  NOTAS  </mark>
Una red computacional es un sistema complejo de intercambio de informacion, requiriendo una combinacion de infraestructura fisica y reglas logicas para una comunicacion efectiva.


## Actividadades Unidad 1

#### Actividad 1.1

Que esperan aprender de esta materia ?
Mi expectativa para la materia es poder manejar bien las redes basicas, configuraciones, etc.

#### Actividad 1.2

Para mi las redes informaticas en este tiempo es lo de las cosas mas importantes, porque por ejemplo todo es con redes y si son vulnerables es peligroso, un ejemplo son los negocios ya que si se llega a caer la red que usan tienen perdidas monetarias, en un aeropuerto puede incluso haber perdidas humanas


### Clase Dia Martes 08 de Septiembre 2026
#### Actividad 1.1

Que esperan aprender de esta materia ?
Mi expectativa para la materia es poder manejar bien las redes basicas, configuraciones, etc.

### Clase Dia Jueves 10 de Septiembre 2026
#### Actividad 1.2

Para mi las redes informaticas en este tiempo es lo de las cosas mas importantes, porque por ejemplo todo es con redes y si son vulnerables es peligroso, un ejemplo son los negocios ya que si se llega a caer la red que usan tienen perdidas monetarias, en un aeropuerto puede incluso haber perdidas humanas
###### Que es una red computacional?

es un sistema complejo de intecambio de informacion, requeriendo una combinacion de infraestructura fisica y reglas logicas para una combinacion efectiva.

Nodos: Origen y destino

Enlaces: Camino fisico 

Direcciones: Identidad digital

Protocolos: El lenguaje comun

Enrutamiento: Gestion de rutas

Nodo 1 ─────Ethernet (10 Gbps)─────► Nodo 2
              (enlace más rápido)      (hub central)
                                          │
                                    Fibra Óptica
                                    (200 Mbps)
                                          │
                                       Nodo 3 ◄──── 5G (5 MHz – 35 Gbps)
                                    (servidor                  Nodo 4
                                     central)              (edge/outdoor)

###### Componentes por Nodo

#### **Nodo 1** (Entrada Local)

- **Función:** Captar datos del entorno cercano
- **Equipos:**
    - Computadora (servidor local)
    - Auditor (medición/control)
    - Lavadora inteligente (IoT)
    - Servidor (respaldo)

#### **Nodo 2** (Distribución/Mesh)

- **Función:** Repetidor, agregador, fallback
- **Equipos:**
    - Modem WiFi mesh (amplifica señal)
    - Satélite (contingencia cuando falla fibra)

#### **Nodo 3** (Centro de Control)

- **Función:** Procesar, almacenar, rutear todo
- **Equipos:**
    - Servidor principal (base de datos)
    - Switch (distribuye tráfico)
    - Antenas (conexión Nodo 4)
    - UFI y Bluetooth (acceso próximo)

#### **Nodo 4** (Remoto/5G)

- **Función:** Edge computing, acceso móvil
- **Equipos:**
    - Servidor edge (procesa localmente)
    - Computadora
    - Lavadora inteligente (IoT remoto)
    - 5G (última conexión)

- **IP** = "¿Dónde está?"
- **TCP/UDP** = "¿Cómo lo envío?"
- **MAC** = "¿Quién es en mi red?"

#### Usa TCP si:

- Los datos **no pueden perderse** (correos, dinero, archivos)
- **Orden importa** (video-conferencia con audio-video sincronizado)
- Puedes esperar un poco

#### Usa UDP si:

- **Velocidad es crítica** (juegos, streaming)
- Perder un paquete no mata la experiencia
- Muchos clientes se conectan a la vez

### Clase Dia Martes 15 de Septiembre 2026

 **Calidad de servicio (QoS):** define la calidad de servicio o por sus siglas en ingles QoS que son el conjunto de mecanismos que decide que trafico se atiende primero cuando la red no tiene capacidad suficiente para todo al mismo tiempo

**Seguridad:** se refiere a proteger la red y la informacion que circula por ella contra accesos, modificaciones o interrupciones no autorizadas

**Suplantacion de la MAC** (spoofing)

**Ataque de intrmediario** (man-in-the-middle)

**Denegacion de servicios** (DoS / DDoS)

Acceso no autorizado a un punto de acceso inalambrico

**Pishing** o ingenieria social 

### Clase Dia Jueves 17 de Septiembre 2026 

**Arquitectura de red :** Es el conjunto de reglas y decisciones de diseno que definen como se organiza una red para que la comunicacion funcione; que funcion cumple cada parte, en que orden se procesan los datos y quien tiene cl control sobre que.

**Modelo OSI**
Modelo de refencia de siete capas :
1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application
Encapsulamiento :
Al bajar por las capas, cada una envuelve el dato con su propio encabezado; al llegar al destino, el proceso se invierte y cada capa retira el encabezado que le corresponda.
