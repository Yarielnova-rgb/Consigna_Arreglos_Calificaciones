# Consigna_Arreglos_Calificaciones
# Registro de Calificaciones Estudiantiles

## Descripción del proyecto

Programa en C++ que permite registrar las calificaciones finales de un grupo de
estudiantes de la asignatura de Cálculo Diferencial. Utiliza arreglos
unidimensionales paralelos para almacenar los nombres y sus notas
correspondientes, permitiendo mostrar el listado completo, identificar la nota
más alta y la más baja, calcular el promedio general del grupo, y determinar
cuántos estudiantes aprobaron y cuántos reprobaron.

Este proyecto fue desarrollado como actividad práctica para la asignatura de
Lógica de Programación, con el objetivo de aplicar arreglos unidimensionales
paralelos en C++.

## Integrantes del grupo

| Nombre completo | Matrícula |
|---|---|
| [Yariel Israel Nova Moreta] | [2025-0306] |
| [camilo salas jimenez] | [2025-2431] |

## Instrucciones de compilación y ejecución

### Requisitos
- Tener instalado un compilador de C++ (g++, o Visual Studio con soporte C++).

### Compilar y ejecutar desde terminal (g++)
```bash
g++ -o calificaciones calificaciones.cpp
./calificaciones
```

### Ejecutar desde Visual Studio
1. Abrir el archivo `calificaciones.cpp` en Visual Studio.
2. Presionar `Ctrl+F5` para compilar y ejecutar sin depuración.

## Capturas de pantalla

### Entrada de datos
[Insertar aquí captura mostrando el programa pidiendo nombre y calificación]

### Resultados (tabla, promedio, máximo, mínimo, aprobados/reprobados)
[Insertar aquí captura mostrando los resultados finales del programa]

## Explicación de los arreglos utilizados

El programa utiliza dos arreglos unidimensionales **paralelos**:

- `string nombres[]`: almacena el nombre de cada estudiante.
- `float notas[]`: almacena la calificación correspondiente a cada estudiante.

Ambos arreglos se relacionan por medio del **índice**: la posición `i` en
`nombres[]` corresponde siempre al mismo estudiante que la posición `i` en
`notas[]`. Por ejemplo, `nombres[2]` y `notas[2]` pertenecen al mismo
estudiante. Esta técnica se conoce como **paralelismo de índices** y permite
recorrer ambos arreglos con un mismo ciclo `for`, manteniendo la relación entre
el nombre y su nota sin necesidad de estructuras más complejas.
