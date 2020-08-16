# Docs

Se le pide que configure y administre los dispositivos de una infraestructura de red para una empresa que está comenzando a crecer y desea implementar una red, un arquitecto de red les proporciona el **[diseño de la topología](#Topología) ** que serán utilizados por dicha empresa, pero deberán configurarlo para brindar comunicación de acuerdo a las necesidades indicadas.

Debe configurar y administrar el equipo de una infraestructura de red para una empresa que tiene **[4 hosts](#Hosts) ** que están conectados a 2 switches diferentes y estos están conectados entre sí a través de un **[router](#Router) ** que será el principal centro de comunicaciones.

- [Topología](#Topología)
- [Descripción](#Descripción)
- [Routers](#Routers)
- [Switches](#Switches)
- [VPCS](#VPCS)
- [VMS](#VMS)
- [Configuración](#Configuración)
- [Vocabulario](#Vocabulario)
- [Downloads](./downloads)



## Topología

<img src="./img/topology.PNG" alt="Topology" style="zoom: 100%;" />

## Descripción

Para la configuración de la topología solicitada, se proporcionan las siguientes tablas, con las direcciones IP y configuraciones de router necesarias para su correcta implementación.

### Router

| Interfaz | Dirección de Red | Dirección IP   |
| -------- | ---------------- | -------------- |
| f0/0     | 192.168.1X.0/24  | 192.168.1X.254 |
| f0/1     | 192.168.1Y.0/24  | 192.168.1Y.254 |

**donde x = 8 y y = 5*



### Hosts

| Tipo      | Nombre | Conectado a | Dirección IP  |
| --------- | ------ | ----------- | ------------- |
| TinyLinux | tiny-1 | Switch1     | 192.168.1X.30 |
| VPCS      | PC2    | Switch1     | 192.168.1X.15 |
| VPCS      | PC3    | Switch2     | 192.168.1Y.15 |
| VPCS      | PC4    | Switch2     | 192.168.1Y.30 |

**donde x = 8 y y = 5*



## Dispositivos

### Routers



### Switches



### VPCS



### VMS



## Configuración





## Vocabulario

#### **Router**

Un **rúter**,[1](https://es.wikipedia.org/wiki/Router#cite_note-1) **enrutador**,[2](https://es.wikipedia.org/wiki/Router#cite_note-2) (del inglés ***router***) o **encaminador**,[3](https://es.wikipedia.org/wiki/Router#cite_note-3) es un dispositivo que permite interconectar computadoras que funcionan en el marco de una red. Su función: se encarga de establecer la ruta que destinará a cada paquete de datos dentro de una red informática.

El funcionamiento básico de un enrutador o encaminador, como se deduce de su nombre, consiste en enviar los paquetes de red por el camino o ruta más adecuada en cada momento. Para ello almacena los paquetes recibidos y procesa la información de origen y destino que poseen. Con arreglo a esta información reenvía los paquetes a otro encaminador o bien al [anfitrión](https://es.wikipedia.org/wiki/Host) final, en una actividad que se denomina 'encaminamiento'. Cada encaminador se encarga de decidir el siguiente salto en función de su tabla de reenvío o [tabla de encaminamiento](https://es.wikipedia.org/wiki/Tabla_de_enrutamiento), la cual se genera mediante protocolos que deciden cuál es el camino más adecuado o corto, como protocolos basado en el [algoritmo de Dijkstra](https://es.wikipedia.org/wiki/Algoritmo_de_Dijkstra).

*[Wikipedia](https://es.wikipedia.org/wiki/Router)*

#### Host

El término ***host*** o **anfitrión** se usa en informática para referirse a las [computadoras](https://es.wikipedia.org/wiki/Computadora) u otros [dispositivos](https://es.wikipedia.org/wiki/Periférico_(informática)) ([tabletas](https://es.wikipedia.org/wiki/Tableta_(computadora)), [móviles](https://es.wikipedia.org/wiki/Teléfono_inteligente), [portátiles](https://es.wikipedia.org/wiki/Computadora_portátil)) conectados a una [red](https://es.wikipedia.org/wiki/Red_de_computadoras) que proveen y utilizan servicios de ella. Los servidores deben utilizar anfitriones para tener acceso a la red y pueden, a su vez, pedir los mismos servicios a otras máquinas conectadas a la red. Los anfitriones son, por tanto, [dispositivos](https://es.wikipedia.org/wiki/Periférico_(informática)) monousuario o multiusuario que ofrecen servicios de [transferencia de archivos](https://es.wikipedia.org/wiki/Transferencia_de_archivos), conexión remota, servidores de [base de datos](https://es.wikipedia.org/wiki/Base_de_datos), [servidores web](https://es.wikipedia.org/wiki/Servidor_web), etc.

De forma genérica, podemos decir que un anfitrión es todo equipo informático que posee una [dirección IP](https://es.wikipedia.org/wiki/Dirección_IP) y que se encuentra interconectado con uno o más equipos y que funciona como el punto de inicio y final de las transferencias de datos.[1](https://es.wikipedia.org/wiki/Host#cite_note-rfc871-1)

También es descrito como el lugar donde reside un sitio web, un anfitrión de Internet tiene por lo general una dirección de Internet única llamada "dirección IP" y un nombre de dominio único o nombre de anfitrión (*host name*).

[*Wikipedia*](https://es.wikipedia.org/wiki/Host)