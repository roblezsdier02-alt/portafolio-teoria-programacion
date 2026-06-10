# Unidad 2: Estructuras de Control de Flujo

## 📝 Introducción
En el desarrollo de software, la secuencialidad lineal de las instrucciones no siempre es suficiente para resolver problemas del mundo real. Para construir algoritmos verdaderamente inteligentes y dinámicos, es indispensable alterar el orden de ejecución en función de los datos. 

Esta unidad abarca el estudio y aplicación de las **Estructuras de Control de Flujo**, las cuales representan los pilares fundamentales de la lógica de programación. Se profundiza en el análisis de las estructuras **condicionales** (que permiten tomar decisiones lógicas en base a evaluaciones booleanas) y las estructuras **repetitivas** (que optimizan la ejecución de tareas mediante ciclos controlados por condiciones). [cite_start]A través de estas herramientas, un estudiante de Computación adquiere la capacidad de abstraer problemas complejos, diseñar soluciones algorítmicas eficientes en diagramas de flujo y pseudocódigo, y traducirlas con precisión a un lenguaje de programación de alto nivel.

---

## 🗂️ ¿Qué contiene esta unidad?

[cite_start]Este apartado del portafolio funciona como un registro de aprendizaje práctico y teórico, organizado bajo las siguientes secciones requeridas por el plan de la asignatura:

1. **Estructuras Condicionales:** Marco teórico sobre los tipos de condicionales (simples, dobles y múltiples), detallando su respectiva representación en pseudocódigo y esquemas gráficos mediante diagramas de flujo.
2. **Estructuras Repetitivas:** Análisis detallado de los bucles lógicos más utilizados (ciclos condicionados y ciclos por contador), junto con su modelado gráfico y estructural.
3. **Evidencia de Aplicación Práctica:** Desarrollo paso a paso de un ejercicio integrador basado en el lenguaje de programación analizado en el aula, desglosado en:
    * Planteamiento formal del problema.
    * Análisis exhaustivo de requerimientos (Entradas, Procesos y Salidas).
    * Diseño lógico a través de un Diagrama de Flujo.
    * Codificación en limpio del código fuente.
    * Validación de resultados por medio de una Prueba de Escritorio.
4. **Reflexión Crítica y Dificultades:** Autoevaluación del proceso formativo, identificando los retos conceptuales y técnicos superados durante el aprendizaje de estos contenidos.

---

## 1. Estructuras Condicionales

Las estructuras condicionales permiten bifurcar el flujo de ejecución de un programa basándose en la evaluación de una condición lógica (booleana). [cite_start]Dependiendo de si la condición es verdadera o falsa, el algoritmo tomará un camino u otro.

### 🔹 Tipos de Estructuras Condicionales:
1. **Simples (Si-Entonces / If):** Evalúan una condición y ejecutan un bloque de instrucciones únicamente si el resultado es verdadero. Si es falso, el programa continúa de forma lineal.
2. **Dobles (Si-Entonces-Sino / If-Else):** Ofrecen dos caminos alternativos. Si la condición se cumple, se ejecuta un bloque de código; si no se cumple, se ejecuta un bloque secundario.
3. **Múltiples o Anidadas (Según / Switch / If-Else If):** Permiten evaluar múltiples condiciones en cascada o seleccionar una opción entre varios casos posibles de manera eficiente.

### 📐 Estructura General en Pseudocódigo y Diagramas de Flujo

#### Estructura Condicional Doble:
* **Pseudocódigo:**
    ```text
    Si (condicion_logica) Entonces
        // Bloque de instrucciones si la condición es Verdadera
    Sino
        // Bloque de instrucciones si la condición es Falsa
    FinSi
    ```
* **Esquema en Diagrama de Flujo:**
    Para asegurar una correcta representación visual del flujo lógico y la bifurcación, se anexa el siguiente diagrama estándar:
<img width="1024" height="932" alt="image" src="https://github.com/user-attachments/assets/836e445c-1e7c-4068-82df-ed370dd2694e" />


---

## 2. Estructuras Repetitivas

Las estructuras repetitivas, comúnmente denominadas ciclos o bucles, permiten ejecutar un bloque de instrucciones de forma cíclica e iterativa. [cite_start]La ejecución se repite mientras una condición lógica permanezca como verdadera o hasta que se alcance un límite definido.

### 🔹 Tipos de Estructuras Repetitivas:
1. **Ciclo Mientras (While):** Evalúa la condición antes de ingresar al bucle. Si la condición es falsa desde el inicio, las instrucciones internas nunca se ejecutan (bucle condicionado por entrada).
2. **Ciclo Repetir / Hacer-Mientras (Do-While):** Ejecuta el bloque de código al menos una vez y evalúa la condición al final. Si la condición se cumple, vuelve a iterar (bucle condicionado por salida).
3. **Ciclo Para (For):** Se utiliza cuando se conoce de antemano el número exacto de iteraciones que se deben realizar. Utiliza una variable contadora integrada, un límite y un valor de incremento.

### 📐 Estructura General en Pseudocódigo y Diagramas de Flujo

#### Estructura Repetitiva (Mientras):
* **Pseudocódigo:**
    ```text
    Mientras (condicion_logica) Hacer
        // Bloque de instrucciones que se repiten en cada iteración
        // (Modificación de la variable de control)
    FinMientras
    ```
* **Esquema en Diagrama de Flujo:**
    A continuación, se detaria la representación gráfica del ciclo iterativo, ilustrando cómo el flujo regresa al punto de evaluación de la condición:
    <img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/f02092cb-1ebe-4b6c-865d-655f92c80e7e" />

---

## 3. Ejercicio Integrador (Condicional Múltiple + Estructuras Repetitivas)

[cite_start]A continuación, se detalla el desarrollo práctico de la actividad integradora de la unidad, aplicando las estructuras de decisión y los ciclos estudiados en la asignatura.

### 📝 Planteamiento del Problema
Desarrollar un programa en lenguaje C que genere y muestre los términos de la sucesión de Fibonacci hasta una posición de término $n$ ingresada por el usuario. El programa debe validar de forma iterativa que el número ingresado no sea negativo. [cite_start]Si el término solicitado es 0 o 1, el sistema debe imprimir directamente los valores base (0 y 1 respectivamente); para términos mayores, debe calcular la serie sumando los dos valores antecesores correspondientes.

### 🔍 Análisis del Problema
**Datos de entrada:** Variable entera `n` (posición del término deseado).
* [cite_start]**Proceso:** 1. Utilizar un ciclo repetitivo `do-while` para forzar la lectura del número hasta que `n` sea un valor mayor o igual a 0.
    2. [cite_start]Evaluar el valor de `n` mediante una estructura condicional múltiple (`if - else if - else`) para discriminar los casos base.
    3. [cite_start]Si `n > 1`, emplear un ciclo iterativo `for` controlado por la variable `cont` (que arranca en 2 hasta llegar a `n`) para calcular y actualizar dinámicamente los términos antecesores (`anta` y `antb`) y sumarlos.
* [cite_start]**Datos de salida:** Impresión en consola de los términos de la serie calculados de forma secuencial.

### 📐 Diseño del Algoritmo (Diagrama de Flujo)
[cite_start]Este es el diseño gráfico del algoritmo, el cual se renderiza directamente a continuación:
<img width="1024" height="1536" alt="ejercicio_integrador" src="https://github.com/user-attachments/assets/401558ce-d9a5-439e-b000-ef492d6be256" />


### 💻 Codificación (Código Fuente)
[cite_start]Implementación limpia y corregida en lenguaje C para el cálculo de la serie:

```c
#include <stdio.h>

int main() {
    int n, anta = 0, antb = 1, cont, suma;

    // Estructura Repetitiva 1 (Do-While): Validación de datos de entrada
    do {
        printf("Ingrese un numero:\n");
        scanf("%i", &n);
    } while (n < 0);

    // Estructura Condicional Múltiple: Casos base y generales
    if (n == 0) {
        printf("%i\n", 0);
    } 
    else if (n == 1) {
        printf("%i\n", 1);
    } 
    else {
        // Estructura Repetitiva 2 (For): Cálculo dinámico de términos iterativos
        for (cont = 2; cont <= n; cont++) {
            suma = anta + antb;
            printf("%i\n", suma);
            anta = antb;
            antb = suma;
        }
    }

    return 0;
}
