# Memorias

## 1. ¿Por qué existen distintos tipos?

El ordenador necesita memorias con diferentes velocidades, capacidades y costes. Las memorias más rápidas suelen ser caras y pequeñas; el almacenamiento masivo conserva más datos a largo plazo, pero normalmente es más lento.

Podemos distinguir entre registros y caché dentro o cerca de la CPU, **RAM** para datos de trabajo y almacenamiento como HDD o SSD para guardar programas y archivos de forma persistente.

## 2. Características para describir una memoria

* Tecnología utilizada.
* Localización: dentro de la CPU, memoria principal o medio externo.
* Duración de la información.
* Forma de acceso.
* Capacidad.
* Velocidad y latencia.

**Volátil** significa que la información no se conserva sin alimentación; la RAM es el ejemplo típico. Una memoria **no volátil**, como flash, mantiene los datos apagada. Algunas memorias necesitan **refresco** periódico mientras reciben corriente.

En el acceso **aleatorio** se selecciona directamente una dirección; en el **secuencial** puede ser necesario recorrer información anterior antes de llegar a la deseada.

## 3. ROM y memorias reprogramables

La **ROM** (_Read-Only Memory_) se ha utilizado para guardar firmware. En los equipos actuales el firmware suele almacenarse en memorias flash reprogramables.

* **PROM:** se programa una sola vez.
* **EPROM:** se puede borrar mediante un procedimiento específico y volver a programar.
* **EEPROM:** se borra y reprograma eléctricamente.
* **Flash:** memoria no volátil que permite borrar y escribir bloques; se usa en SSD, USB y firmware.

## 4. RAM: la mesa de trabajo

La **RAM** (_Random Access Memory_) mantiene los datos e instrucciones que utilizan los programas activos. Imagínala como una mesa: si tiene espacio suficiente, puedes trabajar con varios documentos a mano. Si falta RAM, el sistema puede recurrir a memoria virtual respaldada por almacenamiento, que es mucho más lenta.

La RAM es volátil, así que hay que guardar los documentos en un medio persistente para conservarlos al apagar el equipo.

### DRAM y SRAM

* **DRAM:** necesita refresco periódico y se utiliza habitualmente como memoria principal por su capacidad y coste.
* **SRAM:** no necesita refresco periódico mientras recibe alimentación y suele ser más rápida y cara por bit; se usa habitualmente en caché.

## 5. DDR y formatos

DDR significa _Double Data Rate_: transfiere datos en ambos flancos del ciclo de reloj. Existen generaciones como DDR, DDR2, DDR3, DDR4 y DDR5; tienen diferencias eléctricas y físicas y no son intercambiables libremente.

**DIMM** es habitual en sobremesa y **SO-DIMM** en muchos portátiles. Antes de ampliar RAM, comprueba generación, formato, capacidad admitida y compatibilidad con placa base y CPU.

La capacidad suele expresarse en GB. La frecuencia o tasa de transferencia no explica por sí sola todo el rendimiento: también importan latencia, canales y controlador de memoria.

## Resumen

* RAM: temporal, volátil y para programas activos.
* Flash: no volátil y utilizada en almacenamiento y firmware.
* DRAM: memoria principal habitual; requiere refresco.
* SRAM: rápida y costosa; habitual en caché.
* DDR: generaciones distintas que requieren compatibilidad.

## Preguntas de repaso

1. Diferencia entre RAM y almacenamiento.
2. ¿Qué significa volátil?
3. Diferencia entre DRAM y SRAM.
4. ¿Qué significan DIMM y SO-DIMM?
5. ¿Por qué no puedes cambiar DDR4 por DDR5 sin comprobar compatibilidad?

**Respuestas:** RAM para datos en uso y almacenamiento para conservar archivos; volátil pierde contenido sin corriente; DRAM necesita refresco y SRAM no; son formatos de módulo; las generaciones tienen características físicas y eléctricas diferentes.
