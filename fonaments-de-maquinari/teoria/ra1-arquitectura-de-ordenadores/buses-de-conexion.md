# Buses de conexión

## 1. ¿Qué es un bus?

Un **bus** es un sistema de comunicación que transfiere datos, direcciones y señales de control entre componentes. Incluye conexiones físicas y reglas o protocolos de comunicación. Imagínalo como una vía por la que circula la información: si es limitada o lenta, puede convertirse en un cuello de botella.

## 2. Características principales

* **Ancho:** número de bits que se pueden transferir en paralelo.
* **Frecuencia:** ritmo de funcionamiento, habitualmente expresado en MHz o GHz.
* **Tasa de transferencia:** cantidad de datos por unidad de tiempo, por ejemplo MB/s o Gbit/s.

Las tasas reales dependen también del protocolo, las transferencias por ciclo y la codificación. Atención a las unidades: **MB/s** son megabytes por segundo y **Mb/s** son megabits por segundo; un byte equivale a ocho bits.

## 3. Los tres buses del sistema

* **Bus de datos:** transporta datos e instrucciones; suele ser bidireccional.
* **Bus de direcciones:** indica la posición de memoria o el destino del acceso. En el modelo clásico va desde el solicitante hacia el destino.
* **Bus de control:** comunica qué operación se realiza —lectura o escritura, por ejemplo— y ayuda a sincronizarla.

Los tres se estudian conjuntamente como parte del bus del sistema.

## 4. FSB, BSB y bus de memoria

El **FSB** (_Front Side Bus_) comunicaba la CPU con el puente norte en arquitecturas antiguas. En muchos sistemas modernos, el controlador de memoria está integrado en el procesador, por lo que ese esquema ha cambiado. El **BSB** (_Back Side Bus_) aparece en diseños históricos para conectar niveles de caché. El bus de memoria conecta el controlador con la RAM.

## 5. Buses de expansión

* **ISA:** estándar paralelo antiguo para tarjetas de ampliación.
* **EISA:** evolución de ISA a 32 bits.
* **PCI:** estándar paralelo que mejoró la expansión y configuración.
* **AGP:** conexión dedicada históricamente a tarjetas gráficas.
* **PCI Express (PCIe):** estándar moderno, serie, punto a punto y organizado en carriles (_lanes_).

PCIe se ofrece en tamaños como x1, x4, x8 y x16. Más carriles permiten mayor ancho de banda potencial. El tamaño físico de la ranura no garantiza que estén conectados todos los carriles, así que conviene revisar el manual de la placa base.

## Para memorizar

* Datos = qué información se mueve.
* Direcciones = dónde se accede.
* Control = qué operación se realiza.
* PCIe = expansión moderna organizada por carriles.

## Preguntas

1. ¿Qué es un bus?
2. Diferencia entre datos, direcciones y control.
3. ¿Qué significa PCIe x16?
4. ¿Qué bus desplazó a AGP?

**Respuestas:** sistema de comunicación; transportan contenido, indican destino y coordinan operaciones; 16 carriles; PCI Express.
