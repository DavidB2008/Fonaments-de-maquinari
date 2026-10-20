# Microprocesadores

## 1. ¿Qué es una CPU?

El microprocesador o CPU es un circuito integrado que ejecuta instrucciones y procesa datos. Está formado por muchísimos **transistores**, dispositivos semiconductores que controlan señales eléctricas y forman los circuitos lógicos del chip.

## 2. Fabricación, paso a paso

Se parte de silicio de gran pureza, que se corta en discos finos llamados **obleas** (_wafers_). Mediante fotolitografía se define el circuito; después se realizan procesos como el dopado y la formación de distintas capas. La oblea se corta en chips individuales (_dies_) y cada chip se encapsula con contactos eléctricos y una solución para ayudar a disipar el calor.

## 3. Componentes y conceptos

* **Núcleo:** unidad física capaz de ejecutar ciclos de instrucciones. Varios núcleos pueden trabajar en paralelo si la tarea lo permite.
* **Hilo (thread):** flujo lógico de ejecución. Tecnologías como Hyper-Threading de Intel y SMT de AMD permiten que un núcleo gestione varios hilos, pero los hilos no equivalen a núcleos físicos.
* **Registros:** memoria interna muy rápida y de poca capacidad.
* **Contador de instrucciones:** conserva la dirección de la siguiente instrucción.
* **Decodificador:** interpreta qué operación representa la instrucción.
* **Unidad de control y ALU:** coordinan y ejecutan las operaciones.

## 4. Frecuencia y rendimiento

La frecuencia de reloj, expresada en GHz, indica ciclos de reloj por segundo. **No basta para comparar procesadores**: también influyen la arquitectura, las instrucciones ejecutadas por ciclo, los núcleos, la caché, el consumo y la temperatura. Una aplicación que no aprovecha varios núcleos no siempre mejora mucho al añadirlos.

## 5. Socket y contactos

El **socket** es la conexión física entre CPU y placa base. Deben ser compatibles el socket, la placa, el firmware y la memoria admitida.

* **LGA:** contactos en el socket y superficies de contacto en la CPU.
* **PGA:** pines en el procesador y orificios en el socket.
* **BGA:** chip soldado directamente a la placa.

## 6. x86, RISC y CISC

x86 es una familia de arquitecturas de instrucciones que evolucionó desde Intel 8086. Los 32 y 64 bits se relacionan con el modo en que CPU, sistema operativo y software manejan datos y direcciones.

* **CISC:** conjunto de instrucciones amplio, con operaciones complejas; históricamente se asocia con x86.
* **RISC:** conjunto de instrucciones más reducido y regular; ARM es un ejemplo conocido.

No significa que una familia sea siempre más rápida: depende del diseño completo y de la tarea.

## 7. Temperatura y frecuencia

La CPU genera calor y necesita refrigeración. Si se calienta demasiado, puede reducir automáticamente la frecuencia para protegerse. El **overclocking** aumenta la frecuencia por encima de ciertos valores de referencia y puede mejorar el rendimiento, pero también aumenta consumo, calor e inestabilidad. El _underclocking_ reduce frecuencia para priorizar consumo o temperatura.

## Repaso

1. Diferencia entre núcleo e hilo.
2. ¿Por qué no basta con mirar los GHz?
3. ¿Qué significan LGA, PGA y BGA?
4. ¿Qué riesgos tiene el overclocking?

**Respuestas:** núcleo físico e hilo lógico; también importan arquitectura, caché y carga; varía dónde están los contactos; puede elevar calor, consumo e inestabilidad.
