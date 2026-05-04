# Ejercicio con estructura secuencial

## 🧩 Planteamiento del problema
Desarrollar un programa que permita calcular la suma de dos números ingresados por el usuario.

---

## 🔍 Análisis del problema

- **Entrada:** Dos números
- **Proceso:** Sumar los dos valores
- **Salida:** Resultado de la suma

---

## 🧠 Diseño del algoritmo

### Pseudocódigo

```text
Inicio
Leer A
Leer B
Suma ← A + B
Escribir Suma
Fin


---

## 💻 Codificación (Lenguaje C)

```c
#include <stdio.h>

int main() {
    float A, B, suma;

    printf("Ingrese el primer número: ");
    scanf("%f", &A);

    printf("Ingrese el segundo número: ");
    scanf("%f", &B);

    suma = A + B;

    printf("La suma es: %.2f", suma);

    return 0;
}


