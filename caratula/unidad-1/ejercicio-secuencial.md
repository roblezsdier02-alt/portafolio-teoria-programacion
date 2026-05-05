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
<img width="571" height="922" alt="Diagrama de flujo" src="https://github.com/user-attachments/assets/28b4f4a3-2a98-4950-bbd8-321bb40a59e0" />


### Pseudocódigo (PSeInt)
<img width="615" height="503" alt="Pseudocodigo" src="https://github.com/user-attachments/assets/e2e01ac2-233a-464a-aac2-0dd089c021ed" />



### 📷 Pseudocódigo (evidencia)
<img width="605" height="360" alt="Pseudocódigo (evidencia)" src="https://github.com/user-attachments/assets/6f53067a-d700-4f66-ac88-857c930d857a" />




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

