# Ejercicio con estructura secuencial
---

## 📚 Desarrollo de actividades

## 🧩 Planteamiento del problema
Desarrollar un programa que permita calcular la suma de dos números ingresados por el usuario.

---

## 🔍 Análisis del problema

- **Entrada:** Dos números
- **Proceso:** Sumar los dos valores
- **Salida:** Resultado de la suma

---

## 🧠 Diseño del algoritmo

### 📊 Diagrama de flujo
<img width="571" height="922" alt="Captura de pantalla 2026-05-04 010640" src="https://github.com/user-attachments/assets/bb23f67f-3d71-42d2-b34a-693d2315a815" />


### Pseudocódigo (PSeInt)

### 📷 Pseudocódigo (evidencia)

<p align="center">
  <img src="../recursos/imagenes/pseudocodigo.jpg" width="400">
</p>

| A | B | Resultado |
|---|---|----------|
| 4 | 3 | 7 |


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

