# Memoria caché L1, L2 y L3

## 1. ¿Por qué hace falta?

La CPU puede ejecutar instrucciones muy deprisa, pero la RAM no siempre entrega datos al mismo ritmo. Si el procesador tuviera que esperar por cada dato, perdería tiempo. La **memoria caché** guarda copias de datos e instrucciones que probablemente volverán a utilizarse pronto.

Una analogía: la RAM es una estantería de libros y la caché es la pequeña selección que dejas sobre la mesa porque la consultas continuamente.

## 2. Dónde está y de qué está hecha

La caché del procesador suele estar integrada en el chip y utiliza normalmente **SRAM**, rápida y costosa, que no necesita refresco periódico mientras recibe alimentación. Por su precio, tiene menos capacidad que la RAM.

La caché no sustituye a la RAM ni guarda permanentemente tus documentos: acelera el acceso durante el procesamiento.

## 3. Los niveles

### L1

Es el nivel más cercano al núcleo y suele ser el más rápido y pequeño. En muchos diseños se divide en caché de instrucciones y caché de datos.

### L2

Normalmente es mayor que L1, pero tiene algo más de latencia. Conserva información que puede no encontrarse en L1. Según el diseño, puede estar dedicada a un núcleo o tener otra organización.

### L3

Suele ser mayor que L2 y más lenta que L1 y L2. En muchos procesadores modernos se comparte entre varios núcleos y ayuda a reducir accesos a la RAM.

La organización exacta depende del modelo de CPU; estas son reglas generales, no una descripción idéntica de todos los procesadores.

## 4. Aciertos y fallos de caché

1. La CPU busca el dato en un nivel de caché.
2. Si lo encuentra, ocurre un **acierto** (_cache hit_) y puede continuar con poca espera.
3. Si no está, ocurre un **fallo** (_cache miss_) y debe buscarlo en un nivel inferior o en RAM.
4. El dato recuperado puede guardarse en caché para acelerar accesos posteriores.

La caché funciona especialmente bien cuando los programas reutilizan datos o instrucciones.

## 5. Caché y memoria virtual no son lo mismo

* **Caché de CPU:** memoria rápida que reduce la latencia de acceso.
* **Memoria virtual o swap:** utiliza almacenamiento como respaldo cuando no basta la RAM. Linux puede usar partición o archivo swap; Windows usa un archivo de paginación.

El almacenamiento es mucho más lento que la RAM, por lo que depender intensamente de memoria virtual puede reducir el rendimiento.

## Ideas clave

* L1: normalmente más rápida y pequeña.
* L2: intermedia.
* L3: normalmente mayor y a menudo compartida.
* Caché acelera accesos; swap amplía la capacidad virtual a costa de velocidad.

## Preguntas

1. ¿Qué problema resuelve la caché?
2. ¿Qué es un acierto de caché?
3. ¿Cómo se comparan L1, L2 y L3?
4. ¿En qué se diferencia la caché de swap?

**Respuestas:** reduce esperas de la CPU; el dato ya está en caché; L1 suele ser rápida y pequeña, L2 intermedia y L3 mayor; swap utiliza almacenamiento como respaldo de la RAM.
