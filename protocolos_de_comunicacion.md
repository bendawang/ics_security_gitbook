# Protocolos de comunicación

Existen multitud de protocolos con propósitos muy similares o incluso idénticos. De hecho, a diferencia de lo que ocurre en el ámbito de las tecnologías de información en el entorno corporativo, donde organizaciones como IETF y la ISCO, a través de sus RFC, estandarizan la práctica totalidad de los protocolos, en el ámbito industrial cada fabricante define el suyo propio.

En este sentido cada fabricante establece normalmente un protocolo diferente, e incluso a veces un mismo fabricante define distintos protocolos según la serie del dispositivo y el propósito de la comunicación. Solo existen algunos intentos de estandarización como puede ser el protocolo Modbus adoptado, aparte del propietario actual de la marca Modicon (Schneider) en algunos de sus dispositivos, por fabricantes de dispositivos auxiliares como pudieran ser variadores de frecuencia, medidores de potencia o instrumentación, y también como segunda opción en muchos dispositivos de control como PLCs.

| MARCA | SERIE | PROTOCOLO |
| -- | -- | -- |
| SIEMENS | S7 1200/300/400 | S7 MESSAGING |
| OMRON | CJ/CS | FINS |
| HITACHI | H SERIES | HI-PROTOCOL |
| ROCKWELL | LOGIX | RS-LOGIX |
| B&R | X20 | INA |
| SCHNEIDER | TSX | UNITELWAY |
| HONEYWELL | UDC 3000 | UDC |
| MITSUBISHI | FX | FX PROTOCOL |

## Profibus
---

## Profinet
---
Profinet es el mismo protocolo de Profibus pero en el medio físico de Ethernet.

## Modbus
---
El protocolo basado en comunicación continua más extendido dentro de la industria es Modbus.

El protocolo Modbus se formuló a finales de los 70 por los creadores del primer PLC (Modicon) y
aún persiste, con unas pocas variaciones, en los PLCs de dicha marca (en la actualidad propiedad de Schneider Electric).

Al pasar el protocolo a libre uso, ha sido incorporado en infinidad de dispositivos (generalmente de un rango inferior a un PLC) como variadores de frecuencia, RTUs, IEDs y, como segunda opción, en algunos PLCs a través de módulos de comunicación (software y/o hardware adicional).

Las especificaciones del protocolo también soportan el encapsulamiento de las tramas serie dentro de tramas TCP, lo que permite como ya hemos comentado, la comunicación a través de
dispositivos Ethernet con dispositivos serie RS-232 o RS-485 con la pasarela adecuada.

Las especificaciones del protocolo son bastante sencillas, con unos pocos comandos de lectura y
escritura, y unos tipos de datos muy reducidos.

Los tipos de datos a leer y escribir se reducen a 4 tipos:
* Bobinas (salidas digitales)
* Contactos (bits de programa)
* Entradas analógicas (registros de 16 bits)
* Holding Registers (registros de programa de 16 bits).

En cuanto al tamaño de los datos (registros de 16 bits, enteros de 32 bits con signo o sin signo, floats) el protocolo no contempla distinciones, sino que la conversión se realiza a nivel de aplicación. Por ejemplo, la lectura de un registro de 32 bits con signo correspondería a la lectura de dos registros de 16 bits, y será el driver de comunicaciones quien compusiese el dato final a través de los datos proporcionados por el dispositivo.