# Refrigeración, almacenamiento, placa base

### 1. ❄️ REFRIGERACIÓN EN EQUIPOS MICROINFORMÁTICOS

Los sistemas de refrigeración son esenciales para disipar el calor generado por los componentes (especialmente CPU y GPU) y mantener la estabilidad del sistema.

### 1.1. Tipos de Refrigeración

1. Refrigeración Pasiva:

Mecanismo: Incrementa la superficie de contacto con el aire para maximizar el calor disipado por convección natural.

Estructura: Formada por disipadores con cientos de aletas delgadas (a más aletas y más delgadas, mayor eficiencia).

Ventaja: Silenciosa y sin consumo eléctrico.

2. Refrigeración por Ventilación (Activa de Aire):

Mecanismo: Fuerza el flujo de aire de entrada (frío) y salida (caliente) dentro del chasis.

Variantes:

* Ventiladores normales (velocidad fija).
* Ventiladores inteligentes (control de velocidad PWM según la temperatura).

3. Heatpipes (Tubos de Calor):

Mecanismo: Utilizan la convección por evaporación y condensación de un líquido en un circuito cerrado.

Proceso: El líquido se evapora en la zona caliente (base del procesador), asciende en forma de vapor hacia las aletas del disipador donde se condensa (se enfría) y vuelve a bajar en estado líquido.

4. Refrigeración Líquida:

Mecanismo: Extrae el calor fuera del chasis mediante un fluido refrigerante (generalmente mezcla de agua destilada y glicol).

Componentes principales:

Bloques fríos (Cold blocks): En contacto directo con el procesador/GPU.

Bomba: Impulsa el líquido por el circuito.

Depósito de líquido: Almacena el reservorio del fluido.

Radiador y Ventiladores: Disipan el calor del fluido hacia el exterior.

Tubos de conducción: Conectan el circuito cerrado.

### 1.2. Refrigeración en Portátiles

Sistemas integrados: Combinan un disipador plano, heatpipes, un ventilador tipo turbina (blower) y rejillas de ventilación pasiva.

Complementos externos:

Bases/Placas de ventilación: Soporte inferior con ventiladores adicionales.

Módulos/Extractores de aire nocturnos: Dispositivos de succión fijados a la salida de aire lateral/trasera.

### 2. 🖥️ PLACA BASE Y DISPOSITIVOS INTERNOS

La placa base (Motherboard) es el componente central que determina:

1. El rendimiento general.
2. La organización interna de los componentes.
3. La capacidad de actualización y expansión.

#### 2.1. Factores de Forma (Tamaños)

El factor de forma define las dimensiones físicas, distribución de componentes y compatibilidad con el chasis:

EATX (Extended ATX): Formato mayor orientado a servidores/entusiastas.

ATX: Formato estándar estándar para PCs de sobremesa.

micro-ATX: Formato compacto más económico, con menos ranuras PCIe.

mini-ITX: Formato ultracompacto para sistemas de pequeño tamaño.

#### 2.2. Componentes y Arquitectura de la Placa Base

| Componente                 | Función Principal                                                                      |
| -------------------------- | -------------------------------------------------------------------------------------- |
| Zócalo CPU (Socket)        | Conector donde se instala el procesador.                                               |
| VRM (MOSFETs)              | Módulo de regulación de voltaje que suministra energía estable a la CPU.               |
| Ranuras de Memoria (DIMM)  | Slots para instalar los módulos de RAM (ej. Dual Channel DDR4).                        |
| Ranuras PCIe / M.2         | Buses de expansión de alta velocidad para tarjetas gráficas y almacenamiento SSD NVMe. |
| Conectores SATA            | Interfaz para discos duros tradicionales y SSDs SATA.                                  |
| BIOS / UEFI / Flash ROM    | Firmware integrado encargada del arranque del sistema y la comprobación de hardware.   |
| Memoria CMOS               | Almacena la configuración de la BIOS y la hora (alimentada por pila de botón).         |
| Master Panel / Front Panel | Pines donde se conectan los botones de encendido, reset y LEDs de la caja.             |

#### 2.3. Estructura del Chipset Tradicional

El Chipset es el conjunto de circuitos integrados que gestiona las comunicaciones entre el procesador y los periféricos.

+-------------------+ | C P U | +---------+---------+ | Bus Frontal (FSB) v +-------------------+ | PUENTE NORTE | <---> Memoria RAM (Bus de Memoria) | (Northbridge) | <---> Tarjeta Gráfica (PCIe / AGP) +---------+---------+ | Bus Interno v +-------------------+ | PUENTE SUR | <---> Puertos SATA / IDE (Almacenamiento) | (Southbridge) | <---> Puertos USB / Ethernet / Audio +---------+---------+ <---> Ranuras PCI / Bus LPC | v +-------------------+ | Super I/O | <---> Teclado, Ratón, Puertos Serie/Paralelo, Floppy +-------------------+



1. Puente Norte (Northbridge / Concentrador Controlador de Memoria):

Gestiona los componentes de alta velocidad: CPU, Memoria RAM y la Tarjeta Gráfica (AGP/PCI Express).

2. Puente Sur (Southbridge / Concentrador Controlador de E/S):

Gestiona los componentes de menor velocidad: Discos duros (SATA/IDE), USB, Ethernet, Audio, BIOS y ranuras PCI.

3. Chip Super I/O:

Conectado al Puente Sur por el bus LPC, administra puertos heredados: teclado/ratón PS/2, puerto serie, puerto paralelo y disquetera.

### 3. 💾 UNIDADES DE ALMACENAMIENTO

Guardan la información de forma permanente (no volátil).

#### 3.1. Tipos de Discos y Unidades

1. HDD (Hard Disk Drive - Disco Duro Mecánico):

Utiliza platos magnéticos giratorios y cabezales mecánicos de lectura/escritura.

2. SSD (Solid State Drive - Unidad de Estado Sólido):

Utiliza memorias de tipo Flash NAND sin partes móviles. Alto rendimiento y mayor resistencia a golpes.

3. SSHD (Solid State Hybrid Drive):

Disco híbrido que combina la gran capacidad de un HDD con un pequeño caché de memoria flash SSD para acelerar los archivos más usados.

4. NVMe (Non-Volatile Memory Express):

Protocolo de comunicación diseñado específicamente para SSDs conectadas a través de bahías M.2 en buses PCIe, superando con creces las limitaciones de velocidad del protocolo SATA tradicional.

#### 3.2. Comparativa de Tiempos de Arranque / Velocidad

$$\text{Velocidad: } \mathbf{NVMe\ PCIe\ 4.0} \ > \ \mathbf{SSD\ SATA} \ > \ \mathbf{SSHD\ SATA} \ > \ \mathbf{HDD\ SATA}$$

#### 3.3. Estructura Física y Lógica del HDD (Disco Mecánico)

**Parámetros / Características Clave del HDD:**

* Capacidad: Volumen total de datos (en GB o TB).
* Velocidad de rotación: Revoluciones por minuto de los platos (RPM: ej. 5400 RPM, 7200 RPM).
* Tiempo medio de búsqueda/acceso: Tiempo que tarda el cabezal en situarse en la pista y sector deseado.
* Buffer: Memoria caché integrada en el disco para agilizar transferencias.

**Estructura Geométrica del Disco:**

* Pista (Track): Cada uno de los anillos concéntricos grabados en la superficie del plato.
* Sector: División de una pista. Es la unidad mínima de información accesible a nivel físico (habitualmente 512 bytes o 4 KB).
* Clúster: Grupo de sectores continuos que constituyen la unidad mínima de asignación del sistema de archivos.
* Sector Geométrico: Porción angular en forma de "quesito" que abarca las pistas desde el centro hasta el borde.

#### 📌 Preguntas Frecuentes para Repaso Rápido (Autoevaluación)

1. ¿Qué diferencia la refrigeración pasiva de la activa?

* _La pasiva no usa elementos móviles ni energía (solo un disipador de aletas), mientras que la activa añade ventiladores o bombas para forzar la disipación._

2. ¿Cómo funciona un Heatpipe?

* _Mediante convección: un líquido interno se evapora con el calor del componente, viaja al extremo frío donde se condensa y regresa a la base._

3. ¿De qué se encarga el Puente Norte (Northbridge)?

* _De comunicar la CPU con la memoria RAM y la tarjeta gráfica._

4. ¿Por qué un SSD NVMe es más rápido que un SSD SATA?

* _Porque NVMe utiliza el bus PCI Express directo, mientras que el SSD SATA está limitado por el ancho de banda del bus SATA._

5. ¿Qué es un Clúster en un disco duro?

* _Es la unidad mínima de asignación del sistema de archivos, compuesta por la agrupación de varios sectores._
