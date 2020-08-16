# Docs

Se le pide que configure y administre los dispositivos de una infraestructura de red para una empresa que está comenzando a crecer y desea implementar una red, un arquitecto de red les proporciona el **[diseño de la topología](#Topología)** que serán utilizados por dicha empresa, pero deberán configurarlo para brindar comunicación de acuerdo a las necesidades indicadas.

Debe configurar y administrar el equipo de una infraestructura de red para una empresa que tiene **[4 hosts](#Hosts)** que están conectados a 2 switches diferentes y estos están conectados entre sí a través de un **[router](#Router)** que será el principal centro de comunicaciones.

- [Topología](#Topología)
- [Descripción](#Descripción)
- [Routers](#Routers)
- [Switches](#Switches)
- [VPCS](#VPCS)
- [VMS](#VMS)
- [Configuración](#Configuración)
- [Vocabulario](#Vocabulario)
- [Downloads](./downloads.md)



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

#### VPCS

Virtual PC Simulator es un programa escrito por Paul Meng, que le permite simular una PC liviana que admite DHCP y ping. Consume solo 2 MB de RAM por instancia y no requiere una imagen adicional.

[*GNS3* docs](https://docs.gns3.com/docs/emulators/vpcs/#:~:text=Virtual%20PC%20Simulator%20is%20a,not%20require%20an%20additional%20image.)

#### Switch

**Conmutador** (***switch***) es el dispositivo digital lógico de interconexión de equipos que opera en la [capa de enlace de datos](https://es.wikipedia.org/wiki/Capa_de_enlace_de_datos) del [modelo OSI](https://es.wikipedia.org/wiki/Modelo_OSI). Su función es interconectar dos o más host de manera similar a los [puentes de red](https://es.wikipedia.org/wiki/Puente_de_red), pasando datos de un segmento a otro de acuerdo con la [dirección MAC](https://es.wikipedia.org/wiki/Dirección_MAC) de destino de las [tramas](https://es.wikipedia.org/wiki/Trama_de_red) en la red y eliminando la conexión una vez finalizada esta.[1](https://es.wikipedia.org/wiki/Conmutador_(dispositivo_de_red)#cite_note-1)

Los conmutadores se utilizan cuando se desea conectar múltiples tramos de una red, fusionándolos en una sola red. Al igual que los puentes, dado que funcionan como un filtro en la red y solo retransmiten la información hacia los tramos en los que hay el destinatario de la trama de red, mejoran el rendimiento y la seguridad de las [redes de área local](https://es.wikipedia.org/wiki/Red_de_área_local) ([LAN](https://es.wikipedia.org/wiki/Local_Area_Network))

[*Wikipedia*](https://es.wikipedia.org/wiki/Conmutador_(dispositivo_de_red))

#### Dirección IP

La **dirección IP** es un conjunto de números que identifica, de manera lógica y jerárquica, a una [Interfaz](https://es.wikipedia.org/wiki/Interfaz) en la red (elemento de comunicación/conexión) de un dispositivo ([computadora](https://es.wikipedia.org/wiki/Computadora), [laptop](https://es.wikipedia.org/wiki/Laptop), [teléfono inteligente](https://es.wikipedia.org/wiki/Teléfono_inteligente)) que utilice el [protocolo](https://es.wikipedia.org/wiki/Internet_Protocol) o (*Internet Protocol*), que corresponde al nivel de red del [modelo TCP/IP](https://es.wikipedia.org/wiki/Modelo_TCP/IP).[1](https://es.wikipedia.org/wiki/Dirección_IP#cite_note-:2-1) La dirección IP no debe confundirse con la [dirección MAC](https://es.wikipedia.org/wiki/Dirección_MAC), que es un identificador de 48 bits expresado en código hexadecimal, para identificar de forma única la [tarjeta de red](https://es.wikipedia.org/wiki/Tarjeta_de_red) y no depende del protocolo de conexión utilizado en la red.

La dirección IP puede cambiar a menudo debido a cambios en la red, o porque el dispositivo encargado dentro de la red de asignar las direcciones IP, decida asignar otra IP (por ejemplo, con el protocolo [DHCP](https://es.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol)). A esta forma de asignación de dirección IP se le denomina también *dirección IP dinámica* (normalmente abreviado como *IP dinámica*).[1](https://es.wikipedia.org/wiki/Dirección_IP#cite_note-:2-1)Los sitios de Internet que por su naturaleza necesitan estar permanentemente conectados, generalmente tienen la necesidad de una *dirección IP fija* (comúnmente, *IP fija* o *IP estática*). Esta no cambia con el tiempo. Los servidores de correo, DNS, FTP públicos y servidores de páginas web necesariamente deben contar con una dirección IP fija o estática, ya que de esta forma se permite su localización en la red.[1](https://es.wikipedia.org/wiki/Dirección_IP#cite_note-:2-1)

Los dispositivos se conectan entre sí mediante sus respectivas direcciones IP. Sin embargo, para las personas es más fácil recordar un [nombre de dominio](https://es.wikipedia.org/wiki/Dominio_de_Internet) que los números de la dirección IP. Los servidores de nombres de dominio [DNS](https://es.wikipedia.org/wiki/Domain_Name_System), "traducen" el nombre de dominio en una dirección IP. Si la dirección IP dinámica cambia, es suficiente actualizar la información en el servidor DNS. El resto de las personas seguirán accediendo al dispositivo por el nombre de dominio.[2](https://es.wikipedia.org/wiki/Dirección_IP#cite_note-:0-2)

[*Wikipedia*](https://es.wikipedia.org/wiki/Direcci%C3%B3n_IP)

#### Topología

La **topología** (del [griego](https://es.wikipedia.org/wiki/Idioma_griego) τόπος, 'lugar', y λόγος, 'estudio') es la rama de las [matemáticas](https://es.wikipedia.org/wiki/Matemáticas) dedicada al estudio de aquellas propiedades de los cuerpos geométricos que permanecen inalteradas por transformaciones continuas.[1](https://es.wikipedia.org/wiki/Topología#cite_note-1) Es una disciplina que estudia las propiedades de los [espacios topológicos](https://es.wikipedia.org/wiki/Espacio_topológico) y las [funciones continuas](https://es.wikipedia.org/wiki/Función_continua). La topología se interesa por conceptos como *proximidad*, *número de agujeros*, el tipo de *consistencia* (o *textura*) que presenta un objeto, comparar objetos y clasificar múltiples atributos donde destacan [conectividad](https://es.wikipedia.org/wiki/Conjunto_conexo), [compacidad](https://es.wikipedia.org/wiki/Espacio_compacto), [metricidad o metrizabilidad](https://es.wikipedia.org/wiki/Espacio_métrico), entre otros.

[*Wikipedia*](https://es.wikipedia.org/wiki/Topolog%C3%ADa)

#### Interfaz

Una **interfaz** (**interfaces**, en plural) se utiliza en [informática](https://es.wikipedia.org/wiki/Informática) para nombrar a la conexión funcional entre dos sistemas, programas, dispositivos o componentes de cualquier tipo, que proporciona una comunicación de distintos niveles, permitiendo el intercambio de información. Esto es un ejemplo de la realidad virtual. [1](https://es.wikipedia.org/wiki/Interfaz#cite_note-1)

[*Wikipedia*](https://es.wikipedia.org/wiki/Interfaz)

#### Red de Computadoras

Una **red de computadoras** (también llamada **red de ordenadores** o **red informática**) es un conjunto de [equipos nodos](https://es.wikipedia.org/wiki/Hardware_de_red) y [software](https://es.wikipedia.org/wiki/Software) conectados entre sí por medio de [dispositivos físicos](https://es.wikipedia.org/wiki/Hardware_de_red) o inalámbricos que envían y reciben [impulsos eléctricos](https://es.wikipedia.org/wiki/Corriente_eléctrica), [ondas electromagnéticas](https://es.wikipedia.org/wiki/Radiación_electromagnética) o cualquier otro medio para el transporte de [datos](https://es.wikipedia.org/wiki/Dato), con la finalidad de compartir información, recursos y ofrecer [servicios](https://es.wikipedia.org/wiki/Servicio_de_red).[1](https://es.wikipedia.org/wiki/Red_de_computadoras#cite_note-FOOTNOTETanenbaum20033-1)

[*Wikipedia*](https://es.wikipedia.org/wiki/Red_de_computadoras)

#### Dominio de Broadcast

Un **dominio de difusión** (***broadcast domain***) es el área lógica en una [red de computadoras](https://es.wikipedia.org/wiki/Red_de_computadoras) en la que cualquier [computadora](https://es.wikipedia.org/wiki/Computadora) conectada a la red puede transmitir directamente a cualquier otra computadora en el dominio sin precisar ningún dispositivo de encaminamiento, dado que comparten la misma subred, dirección de [puerta de enlace](https://es.wikipedia.org/wiki/Puerta_de_enlace) y están en la misma [red de área local](https://es.wikipedia.org/wiki/Red_de_área_local) ([LAN](https://es.wikipedia.org/wiki/Local_Area_Network)) o [VLAN](https://es.wikipedia.org/wiki/VLAN) (predeterminada o instalada).

[*Wikipedia*](https://es.wikipedia.org/wiki/Dominio_de_difusi%C3%B3n)

#### Dominio de Colisión

Un **dominio de colisión** es un segmento físico de una [red de computadores](https://es.wikipedia.org/wiki/Red_de_computadores) donde es posible que las tramas puedan "colisionar" (interferir) con otros. Estas colisiones se dan particularmente en el protocolo de red [Ethernet](https://es.wikipedia.org/wiki/Ethernet).

A medida que aumenta el número de nodos que pueden transmitir en un segmento de red, aumentan las posibilidades de que dos de ellos transmitan a la vez. Esta transmisión simultánea ocasiona una interferencia entre las señales de ambos nodo, que se conoce como *colisión*. Conforme aumenta el número de colisiones disminuye el [rendimiento de la red](https://es.wikipedia.org/wiki/Rendimiento_de_red).

[*Wikipedia*](https://es.wikipedia.org/wiki/Dominio_de_colisi%C3%B3n)