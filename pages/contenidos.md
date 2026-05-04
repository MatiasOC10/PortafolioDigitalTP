---
layout: default
title: Contenidos
---

# Contenidos

## Algoritmo

Un algoritmo es un conjunto ordenado, finito y definido de instrucciones o reglas paso a paso que permiten solucionar un problema, realizar un cómputo o procesar datos. Funciona recibiendo datos de entrada (*input*), procesándolos mediante reglas lógicas y produciendo un resultado final (*output*). Son la base de la programación y la tecnología moderna.

En clase se realizó un algoritmo llamado **calculodegalones**. Su propósito es convertir la producción diaria ingresada en litros a su equivalente en galones y, a partir de ello, calcular el monto total a cobrar según un precio por galón. Primero se definen las variables necesarias para almacenar los datos de entrada y los resultados. Luego se solicita al usuario que ingrese la cantidad de litros producidos y el precio por galón. Posteriormente, en el proceso, se realiza la conversión de litros a galones utilizando el factor 3.785 y se calcula el total a pagar multiplicando los galones obtenidos por el precio ingresado. Finalmente, el algoritmo muestra en pantalla la cantidad equivalente en galones y el total a cobrar.

## Pseudocódigo

El pseudocódigo es una forma de representar algoritmos y la lógica de programación utilizando una mezcla de lenguaje natural y estructuras de código, sin las reglas sintácticas estrictas de un lenguaje real. Sirve como borrador para planificar programas, enfocándose en el flujo lógico antes de la codificación.

En este caso, se presenta el algoritmo **calculodegalones**:

<figure class="figure">
  <img src="{{ '/assets/images/pseudocodigo-calculodegalones.png' | relative_url }}" alt="Pseudocódigo del algoritmo calculodegalones">
  <figcaption>Pseudocódigo del algoritmo calculodegalones.</figcaption>
</figure>

## Diagrama de flujo

Un diagrama de flujo, también llamado flujograma, es una representación gráfica de un proceso, algoritmo o sistema. Utiliza símbolos estandarizados conectados por flechas para secuenciar pasos. Permite visualizar de forma clara y ordenada acciones, decisiones y el flujo de información desde el inicio hasta el final de una tarea.

<figure class="figure">
  <img src="{{ '/assets/images/diagrama-calculodegalones.png' | relative_url }}" alt="Diagrama de flujo del algoritmo calculodegalones">
  <figcaption>Diagrama de flujo del algoritmo calculodegalones.</figcaption>
</figure>

## Prueba de escritorio

Una prueba de escritorio es la simulación manual y paso a paso de un algoritmo, pseudocódigo o código, utilizando papel y lápiz o una tabla para rastrear los valores de las variables y verificar la lógica sin ejecutarlo en la computadora. Es fundamental para detectar errores tempranos, validar la funcionalidad y entender el flujo del programa.

En el programa de cálculo de galones, la prueba de escritorio sería:

### Caso 1

| Paso | litros | precioPorGalon | galones | totalaCobrar |
|---|---:|---:|---:|---:|
| Entrada | 15 | 5 |  |  |
| Conversión | 15 | 5 | 3.96 |  |
| Cálculo | 15 | 5 | 3.96 | 19.80 |

### Caso 2

| Paso | litros | precioPorGalon | galones | totalaCobrar |
|---|---:|---:|---:|---:|
| Entrada | 50 | 3.2 |  |  |
| Conversión | 50 | 3.2 | 13.21 |  |
| Cálculo | 50 | 3.2 | 13.21 | 42.27 |

## Lenguajes de programación

Los lenguajes de programación son sistemas formales utilizados para dar instrucciones a las computadoras. Se dividen principalmente en lenguajes de alto nivel, cercanos al lenguaje humano, y lenguajes de bajo nivel, cercanos al hardware. Entre los más populares se encuentran Python, JavaScript, Java, C# y C/C++.

En clase se utilizó el lenguaje C en Visual Studio porque permite entender bases fundamentales de la programación, como el manejo de memoria, las estructuras de control y la lógica computacional de forma clara y directa. C es un lenguaje de bajo nivel comparado con otros, por lo que obliga a comprender cómo funciona realmente el computador. Además, Visual Studio ofrece herramientas como depuración paso a paso y autocompletado, que facilitan el aprendizaje y ayudan a detectar errores.

Mi pseudocódigo transformado en lenguaje C:

```c
#include <stdio.h>

int main() {
    float litros, precioPorGalon;
    float galones, totalACobrar;

    // Entrada
    printf("Ingrese la produccion del dia (en litros): ");
    scanf("%f", &litros);

    printf("Ingrese el precio por galon ($): ");
    scanf("%f", &precioPorGalon);

    // Proceso
    galones = litros / 3.785;
    totalACobrar = galones * precioPorGalon;

    // Salida
    printf("\n--- Resultados ---\n");
    printf("Equivalente en galones: %.2f\n", galones);
    printf("Total a cobrar: $ %.2f\n", totalACobrar);

    return 0;
}
```

<figure class="figure">
  <img src="{{ '/assets/images/codigo-c-calculodegalones.png' | relative_url }}" alt="Código C del algoritmo calculodegalones en Visual Studio">
  <figcaption>Código C del algoritmo calculodegalones.</figcaption>
</figure>

## Programación por bloques

La programación por bloques es un método visual para crear software arrastrando y encajando piezas gráficas que representan comandos, eliminando la necesidad de escribir sintaxis compleja. Es ideal para principiantes porque permite aprender lógica de programación secuencial de forma intuitiva y sin errores de escritura.
