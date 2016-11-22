# Aproximación a la protección de los sistemas de control y automatización


La protección a nivel lógico de los sistemas de control y automatización frente a eventos de
seguridad intencionados o accidentales viene limitada por un conjunto de restricciones que
condicionan las técnicas y estrategias de protección a aplicar, debiendo ser éstas, a veces,
distintas de las elegidas en la protección de los sistemas de información que se encuentran en el entorno corporativo o de oficina. Particularmente, su propia idiosincrasia les confiere características únicas con las que no cuentan los sistemas corporativos, aun a pesar de ser también sistemas informáticos. Adicionalmente, la naturaleza del proceso o actividad que controlan, o la del propio personal que los diseña y mantiene, impone también limitaciones relevantes a la hora de abordar su protección.

En cualquier caso, las medidas de protección que se van a aplicar en los sistemas de control y
automatización van a aprovechar las herramientas, procesos y tecnologías de seguridad existente
en el ámbito de TI, pero teniendo en cuanta que su aplicación a estos sistemas no puede ser
directa por las características especificas que tienen estos entornos.

Una de las soluciones de seguridad que más se está integrando en los sistemas de control y
automatización son los cortafuegos. Esta medida de seguridad se está utilizando tanto como
solución de seguridad perimetral como en redes internas. Sin embargo, el uso de cortafuegos
tradicionales viene limitado por su capacidad a la hora de interpretar los numerosos protocolos de telecontrol o telemedida, que son radicalmente distintos a los de los sistemas de TI habituales. Últimamente, ya están surgiendo soluciones de cortafuegos específicos para sistemas de control y automatización, que son capaces de comprender los protocolos industriales y, por tanto, ayudan a controlar mejor los flujos de comunicaciones.

Medidas complementarias a los cortafuegos, como IDS/IPS, también se están utilizando en los
sistemas de control y automatización. La limitación de estas soluciones es similar al de los
cortafuegos, ya que no comprenden muchos protocolos industriales. Además, el tiempo de análisis
del tráfico, sobre todo en configuraciones in-line, puede incurrir en latencias no compatibles con la naturaleza de tiempo real de ciertos procesos industriales.
Siguiendo con la protección en las redes y las comunicaciones están las VPN de tipo Host-Host
para asegurar las comunicaciones entre pares de dispositivos. La limitación en el uso de esta
tecnología viene determinada por la cantidad de recursos computacionales que son necesarios en
los procesos criptográficos, y que las hacen prácticamente inviables en la mayor parte de los
dispositivos de automatización y control empotrados.

Las soluciones antivirus de los entornos de TI también son válidas en los sistemas de control y
automatización, pero su uso se restringe a los sistemas, ya que los controladores y otros
dispositivos empotrados no suelen utilizar sistemas operativos y aplicaciones comerciales que sean soportados por los antivirus. A esto se suman posibles sobrecargas durante el proceso de
actualización de firmas y análisis de binarios, que pueden afectar al cumplimento con los
parámetros de tiempo real. En relación con el proceso de actualización de firmas, la centralización del mismo también puede ser incompatible con ciertas buenas prácticas de filtrado, que impidan que las redes de control tengan acceso hasta consola central corporativa.

La última medida de protección de esta introducción son las auditorias técnicas de seguridad. Las auditorías técnicas de seguridad permiten conocer el estado de seguridad de un sistema, pero también suelen ser muy agresivas, llevándolos a veces a estados no controlados (p. ej.
indisponibilidad). Estas consecuencias son inaceptables en un entorno de automatización y control, donde estos sistemas juegan un papel fundamental en el “core” del negocio. Es por ello que hay que buscar metodologías y técnicas de auditoría alternativas de riesgo nulo para los sistemas en producción