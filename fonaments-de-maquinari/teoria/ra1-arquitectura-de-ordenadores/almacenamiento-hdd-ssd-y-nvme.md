# Almacenamiento HDD, SSD y NVMe

## 1. ¿Qué es el almacenamiento?

El almacenamiento conserva sistema operativo, aplicaciones y archivos aunque se apague el ordenador. A diferencia de la RAM, está pensado para mantener datos a largo plazo. Los materiales tratan HDD, SSD, NVMe, interfaces y medios ópticos o extraíbles.

## 2. HDD: disco duro mecánico

Un **HDD** (_Hard Disk Drive_) contiene platos que giran y almacenan información mediante magnetización. Los cabezales se desplazan por la superficie para leer y escribir.

Características principales:

* **Capacidad:** datos que puede almacenar, habitualmente en GB o TB.
* **Buffer/caché:** memoria intermedia que ayuda a gestionar datos.
* **Tiempo de acceso:** espera para localizar la información; depende del movimiento del cabezal y la rotación.
* **Velocidad de giro:** se mide en rpm; influye en la espera rotacional.
* **Interfaz:** determina cómo se conecta al equipo.

Como tiene piezas móviles, es sensible a golpes, especialmente mientras funciona.

## 3. SSD: unidad de estado sólido

Un **SSD** (_Solid-State Drive_) usa memoria flash y no tiene platos giratorios ni cabezales mecánicos. Normalmente ofrece menor latencia y acceso más rápido que un HDD.

La **controladora** gestiona las operaciones y la comunicación con la memoria. Algunos SSD incorporan caché y protección frente a pérdida de alimentación, pero sus características dependen del modelo.

## 4. SATA y NVMe

**SATA** es una interfaz común en HDD y SSD. En un SSD SATA, el límite de la interfaz restringe la velocidad máxima frente a unidades PCIe más rápidas.

**NVMe** es un protocolo diseñado para almacenamiento conectado mediante **PCI Express (PCIe)**. Puede ofrecer mayor rendimiento y paralelismo que SATA, dependiendo de la generación y del modelo.

Recuerda la diferencia:

* **HDD/SSD** describe la tecnología de la unidad.
* **SATA/NVMe** describe la interfaz o protocolo de comunicación.
* Un SSD puede ser SATA o NVMe; no todo SSD es NVMe.

## 5. Formato M.2

**M.2** es un formato físico de tarjeta y conector, no una garantía de que la unidad sea NVMe. Hay unidades M.2 SATA y M.2 PCIe/NVMe.

En **M.2 2280**, 22 indica 22 mm de ancho y 80 indica 80 mm de largo. Antes de instalar una unidad, comprueba compatibilidad SATA/PCIe, longitud, ranura, líneas disponibles y si requiere refrigeración. Algunas unidades NVMe de alto rendimiento pueden calentarse y reducir temporalmente su velocidad para protegerse.

## 6. Comparación general

| Característica       | HDD                         | SSD SATA               | SSD NVMe/PCIe                          |
| -------------------- | --------------------------- | ---------------------- | -------------------------------------- |
| Tecnología           | Platos magnéticos           | Memoria flash          | Memoria flash                          |
| Piezas móviles       | Sí                          | No                     | No                                     |
| Latencia             | Más alta normalmente        | Baja                   | Puede ser muy baja                     |
| Velocidad secuencial | Menor                       | Limitada por SATA      | Puede ser muy alta, según modelo       |
| Uso habitual         | Gran capacidad a bajo coste | Uso general y arranque | Tareas que aprovechan alto rendimiento |

Las cifras exactas dependen del modelo, la generación y la carga de trabajo; los valores de las diapositivas deben tomarse como referencias orientativas.

## 7. Otros medios e interfaces

Los materiales también mencionan CD-ROM, DVD, Blu-ray, memorias USB y disquetes históricos. Los discos ópticos utilizan láser para leer información; los pendrives utilizan memoria flash. IDE/ATA paralelo es antiguo; SATA es muy extendido; SCSI y SAS aparecen en entornos profesionales y servidores; PCIe se utiliza con SSD NVMe y otros dispositivos de alto rendimiento.

## Para memorizar

* HDD: magnético y mecánico.
* SSD: memoria flash sin piezas móviles.
* SATA: interfaz extendida.
* NVMe: protocolo para almacenamiento sobre PCIe.
* M.2: formato físico; comprueba el protocolo y la compatibilidad.

## Preguntas de repaso

1. ¿Cómo almacena datos un HDD y cómo un SSD?
2. ¿Qué diferencia hay entre SATA y NVMe?
3. ¿Qué significa M.2 2280?
4. ¿Por qué un HDD es sensible a golpes?
5. ¿Qué hay que comprobar antes de comprar un SSD M.2?

**Respuestas:** platos magnéticos frente a memoria flash; NVMe usa PCIe y SATA es otra interfaz; 22 × 80 mm; tiene partes móviles; protocolo, tamaño y compatibilidad con placa base.
