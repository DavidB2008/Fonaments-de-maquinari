# Introducción y arquitectura de Von Neumann

## 1. ¿Qué es la arquitectura de un ordenador?

La arquitectura de ordenadores estudia cómo se organizan los componentes de un equipo y cómo colaboran para ejecutar programas. Un ordenador realiza cuatro funciones básicas: **recibir entradas**, **procesar información**, **producir salidas** y **almacenar datos**.

Los tres bloques funcionales básicos son:

* **CPU:** interpreta y ejecuta instrucciones y coordina el procesamiento.
* **Memoria principal (RAM):** guarda temporalmente programas, instrucciones y datos en uso.
* **Entrada/salida (E/S):** permite comunicarse con el exterior mediante teclado, ratón, pantalla, impresora y otros dispositivos.

Los **buses** conectan estos bloques y transportan datos, direcciones y señales de control.

## 2. Arquitectura de Von Neumann

La arquitectura de **Von Neumann** se basa en el concepto de programa almacenado: las instrucciones y los datos comparten una misma memoria de lectura y escritura. Cada posición se localiza mediante una dirección y las instrucciones suelen ejecutarse en secuencia, excepto cuando una instrucción de salto o una condición cambia el flujo.

Sus ideas clave son la memoria compartida para datos e instrucciones, el acceso mediante direcciones y la representación binaria. Los materiales también mencionan la arquitectura Harvard como alternativa, pero presentan Von Neumann como base conceptual de la mayoría de ordenadores de propósito general.

## 3. Partes principales de la CPU

* **Unidad de control (UC):** obtiene instrucciones, coordina señales y dirige su ejecución. El contador de instrucciones mantiene la dirección de la próxima instrucción.
* **Unidad aritmético-lógica (ALU/UAL):** realiza operaciones aritméticas, como sumas y restas, y lógicas, como AND, OR y NOT.
* **Registros:** pequeñas memorias internas muy rápidas que guardan datos, direcciones y resultados temporales.
* **Reloj:** genera impulsos que sincronizan las operaciones; la frecuencia suele expresarse en GHz.
* **FPU:** unidad especializada en operaciones de coma flotante.

## 4. Ejemplo: sumar 7 + 5

El programa y los valores se encuentran en memoria. La CPU obtiene la instrucción, la unidad de control coordina la operación, la ALU calcula 12 y el resultado se guarda en un registro o en memoria. Si hace falta, se envía después a la pantalla u otro dispositivo de salida. Es una simplificación didáctica, pero muestra cómo colaboran CPU, memoria y buses.

## Para memorizar

* CPU procesa; RAM mantiene datos e instrucciones de trabajo; E/S comunica con el exterior.
* Von Neumann comparte memoria para instrucciones y datos.
* UC coordina, ALU calcula y registros guardan información temporal.

## Preguntas de repaso

1. ¿Cuáles son las cuatro funciones básicas de un ordenador?
2. ¿Qué tres bloques forman el modelo básico?
3. ¿Qué caracteriza a Von Neumann?
4. ¿Qué diferencia hay entre la UC y la ALU?

**Respuestas:** recibir, procesar, producir salidas y almacenar; CPU, memoria y E/S; comparte memoria para datos e instrucciones; la UC coordina y la ALU calcula.
