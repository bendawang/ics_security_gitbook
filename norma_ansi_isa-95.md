# Norma ANSI/ISA-95

## ¿Qué es ANSI/ISA-95?
 ISA-95 as it is more commonly referred, is an international standard from the International Society of Automation for developing an automated interface between enterprise and control systems. This standard has been developed for global manufacturers. It was developed to be applied in all industries, and in all sorts of processes, like batch processes, continuous and repetitive processes.

The objectives of ISA-95 are to provide consistent terminology that is a foundation for supplier and manufacturer communications, provide consistent information models, and to provide consistent operations models which is a foundation for clarifying application functionality and how information is to be used.

Para presentar mejor todos estos elementos se va a utilizar la clasificación realizada por la
“International Society of Automation” (ISA), organismo que agrupa a más de 30 mil miembros con el objetivo de delimitar los principales estándares industriales, en su norma ISA-95 que regula la automatización industrial.

### Clasificación de niveles ISA-95

La ISA-95 define 5 niveles de operaciones en la automatización industrial:
* **Nivel 0:** el propio proceso productivo.
* **Nivel 1:** los propios dispositivos que procesan y manipulan el producto en sí (robots,
actuadores, instrumentación). Normalmente los dispositivos PLCs y DCS se incluyen en
este nivel aunque, dependiendo del grado de automatización de una organización, también
es frecuente que se ubiquen en el siguiente nivel. Los DCS se ubican en este nivel, ya que
combinan tecnologías de control (los propios controladores) con el software de supervisión
ligado a dichos controladores de proceso.
* **Nivel 2:** los dispositivos que monitorizan y controlan el proceso productivo (HMI, SCADAs).
* **Nivel 3:** los dispositivos que controlan el work flow y las recetas del proceso productivo y que almacenan toda la información sobre el mismo (MES, Batch, Historian, LIMS.
* **Nivel 4:** el nivel que contiene la infraestructura de logística, inventario, ERP 8 o planificación.

### Descripción de los niveles

#### Nivel 0
---
Engloba el propio proceso productivo.

#### Nivel 1
---
En este nivel se encuentran los elementos que adquieren los datos de planta y los que actúan
sobre la cadena. Dependiendo de su complejidad, pueden disponer de una sencilla conexión a la
entrada de un **PLC**; como por ejemplo, un simple pulsador, o necesitar de una compleja parametrización vía un bus de campo, como un sensor de presión avanzado. Dentro del apartado
de sensórica se pueden encontrar dispositivos para la medida de cualquier unidad: niveles de
líquido en un tanque, temperaturas del producto en un reactor, presión del aire en el circuito,
luminosidad, caudal, presencia de impurezas. El coste de la instrumentación utilizada en una
instalación industrial, como en el caso de una planta química, puede ser muy superior al de los
dispositivos de control.

A este nivel también pertenecen los PLCs y DCS que mediante programas de control procesan los
datos de entrada. Mientras que los PLCs son dispositivos compactos, los DCS suelen disponer de
una arquitectura distribuida con diferentes CPUs de control.
Los dispositivos de este nivel requieren de una programación específica. En su diseño prima la
robustez contra las duras condiciones ambientales de la industria.

También se incluyen en este nivel las RTUs que permiten la adquisición remota de datos para
traspasarlos a los elementos de Nivel 2.

#### Nivel 2
---
Aunque ya se ha citado que se pueden encontrar PLCs en este nivel, habitualmente el nivel 2 se
identifica con la capa de supervisión y control de proceso, bien localmente (es decir, desde los interfaces de operador que incluyen las máquinas) como centralizadamente (a través de centros de control que se construyen sobre lo que se llama soluciones SCADA).

Cuando se realiza una supervisión y control local, se utilizan normalmente las pantallas HMI.
Aparatos compactos para la visualización de procesos.

Cuando se realiza una supervisión centralizada, se utilizan los programas SCADA, con base en
ordenadores, que además de la simple visualización del proceso de los HMI pueden incorporar
funcionalidades avanzadas como Data Logging, control de alarmas, gestión de usuarios o
comunicación con los sistemas del siguiente nivel.

#### Nivel 3
---
Desde este nivel se controla el flujo de la producción, recetas y cantidades. También el
almacenamiento de la información de producción como lotes, trazabilidad, productividad, calidad…
Se sitúan en este nivel los controladores Batch, que realizan parte del control del proceso de
recetas, principalmente en industrias químicas y farmacéuticas.

#### Nivel 4
---
Este nivel corresponde al nivel más alto de la gestión, controlando la programación de la
producción de una o varias plantas de una empresa, el uso de materiales, inventario y logística.
Desde este nivel, la dirección ejecutiva obtiene una visión general del funcionamiento de las
mismas a todos los niveles (eficiencia, económicos, logísticos) de forma que puede tomar las
decisiones oportunas sobre su funcionamiento.