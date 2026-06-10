---
layout: default
title: Ejercicio con estructura secuencial
---

# Ejercicio con estructura secuencial

## Planteamiento del problema

Desarrollar un programa en lenguaje C que permita ingresar la base y la altura de un rectángulo, y calcule su área.

## Análisis del problema

| Elemento | Descripción |
|---|---|
| Datos de entrada | Base (`b`) y altura (`h`) |
| Proceso | Área = base × altura |
| Salida | Área del rectángulo |

## Diseño del algoritmo

### Pseudocódigo

<figure class="figure">
  <img src="{{ '/assets/images/pseudocodigo-area-rectangulo.png' | relative_url }}" alt="Pseudocódigo del algoritmo área de rectángulo">
  <figcaption>Pseudocódigo del algoritmo Área_Rectangulo.</figcaption>
</figure>

### Diagrama de flujo

<figure class="figure">
  <img src="{{ '/assets/images/diagrama-area-rectangulo.png' | relative_url }}" alt="Diagrama de flujo para calcular el área de un rectángulo">
  <figcaption>Diagrama de flujo para calcular el área de un rectángulo.</figcaption>
</figure>

## Codificación en C

```c
#include <stdio.h>

int main() {
    float base, altura, area;

    printf("Ingrese la base: ");
    scanf("%f", &base);

    printf("Ingrese la altura: ");
    scanf("%f", &altura);

    area = base * altura;

    printf("El area del rectangulo es: %.2f\n", area);

    return 0;
}
```


## Validación: prueba de escritorio

| Base | Altura | Cálculo | Área |
|---:|---:|---|---:|
| 5 | 3 | 5 × 3 | 15 |
| 2.5 | 4 | 2.5 × 4 | 10 |

## Principales dificultades de los contenidos

Durante el desarrollo de este ejercicio en C, una de las principales dificultades fue comprender cómo funcionan las variables, ya que cada variable almacena un tipo de dato específico y debe ser declarada correctamente antes de usarse.

También se presentó cierta dificultad al utilizar la función `scanf`, especialmente en el uso del símbolo `&`, que es obligatorio para indicar la dirección de memoria donde se guardará el valor ingresado por el usuario.

Finalmente, otro aspecto importante fue diferenciar entre los tipos de datos como `int` y `float`, ya que elegir el tipo correcto es clave para evitar errores en los cálculos, sobre todo cuando se trabaja con números decimales.

## Reflexión crítica en la aplicación

La estructura secuencial es considerada la más sencilla dentro de la programación porque las instrucciones se ejecutan una tras otra en un orden establecido, sin tomar decisiones ni repetir procesos. Este tipo de ejercicios es muy útil para desarrollar la lógica básica de programación, ya que permite enfocarse en la correcta comprensión de las variables, operaciones y entrada/salida de datos.

Además, sirve como base fundamental antes de avanzar hacia estructuras más complejas, como las condicionales y los ciclos, que requieren un mayor nivel de razonamiento y control del flujo del programa.

## Conclusión

El desarrollo de este ejercicio con estructura secuencial en lenguaje C permitió comprender de manera clara cómo se ejecutan las instrucciones de forma ordenada, desde la entrada de datos hasta la obtención de un resultado final. A través de este proceso se reforzaron conceptos básicos como el uso de variables, la entrada y salida de datos con `scanf` y `printf`, y la importancia de seleccionar correctamente los tipos de datos.

Este tipo de ejercicios ayuda a fortalecer la lógica de programación, ya que constituye la base para resolver problemas más complejos en etapas posteriores, como los que incluyen decisiones o repeticiones.
