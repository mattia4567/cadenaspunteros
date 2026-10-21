# CADENASPUNTEROS

**Actividad 4 — Manipulación de Cadenas y Punteros en C/C++**  
**Materia:** Laboratorio de Programación (LPR)  
**Institución:** E.E.S.T. N.º 1 “Eduardo Ader” — Vicente López  
**Estudiante:** Federico Mattia  
**Año:** 2026

## Descripción

CADENASPUNTEROS es un proyecto académico desarrollado en C++ para estudiar el funcionamiento de los punteros y la manipulación de datos en la memoria RAM.

El programa implementa un sistema básico de control de acceso por edad. Para ello, utiliza un puntero que almacena la dirección de memoria de una variable entera, permitiendo ingresar, consultar y evaluar la edad mediante el operador de desreferenciación.

## Objetivos

- Comprender el funcionamiento de los punteros en C++.
- Diferenciar una dirección de memoria de su contenido.
- Aplicar los operadores de dirección (`&`) y desreferenciación (`*`).
- Analizar la representación hexadecimal de las direcciones de memoria.
- Implementar una estructura condicional para validar la edad ingresada.
- Compilar, ejecutar y documentar un programa en C++.

## Tecnologías utilizadas

- **Lenguaje:** C++.
- **Biblioteca estándar:** `iostream`.
- **Compilador:** GCC (`g++`).
- **Editor recomendado:** Visual Studio Code.
- **Control de versiones:** Git y GitHub.

## Funcionamiento del programa

El programa realiza las siguientes operaciones:

1. Declara la variable entera `edad` e inicializa su valor en cero.
2. Declara el puntero `p` y almacena en él la dirección de memoria de `edad`.
3. Solicita al usuario que ingrese su edad.
4. Utiliza `cin >> *p` para guardar el valor ingresado en la variable apuntada.
5. Evalúa la edad mediante una estructura condicional.
6. Muestra un mensaje de acceso aprobado si la edad es igual o superior a 18 años, o de acceso rechazado si es menor.
7. Imprime la edad registrada y la dirección de memoria representada en formato hexadecimal.

**Importante:** la dirección mostrada corresponde a una dirección de memoria virtual utilizada por el proceso, no necesariamente a una dirección física real de la RAM.

## Conceptos fundamentales

### Punteros

Un puntero es una variable que almacena la dirección de memoria de otro objeto. En este proyecto, `p` apunta a la variable `edad`.

```cpp
int edad = 0;
int* p = &edad;
```

### Operador de dirección (`&`)

Obtiene la dirección de memoria de una variable.

```cpp
p = &edad;
```

### Operador de desreferenciación (`*`)

Permite acceder al valor almacenado en la dirección a la que apunta un puntero.

```cpp
cin >> *p;
cout << *p;
```

### Dirección y contenido

- `p`: representa la dirección almacenada en el puntero.
- `*p`: representa el valor de la variable ubicada en esa dirección.

## Estructura del proyecto

```text
CADENASPUNTEROS/
├── .gitignore
├── LICENSE
├── README.md
├── docs/
│   └── InformeProyectoCADENASPUNTEROS.pdf
├── src/
│   └── main.cpp
└── capturas/
    ├── ejecucion_punteros.png
    └── esquema_ram.png
```

## Compilación y ejecución

Para compilar el programa en Windows, es necesario contar con un compilador de C++ compatible con GCC, como MinGW o MSYS2.

Desde la terminal de Visual Studio Code, ubicada en la carpeta raíz del proyecto, ejecutar:

### 1. Compilar

```powershell
g++ src/main.cpp -o src/cadenaspunteros.exe
```

### 2. Ejecutar

```powershell
.\src\cadenaspunteros.exe
```

Si no se dispone de un entorno de compilación local, se puede utilizar un compilador en línea como OnlineGDB.

## Ejemplo de ejecución

```text
=====================================================
   CONTROL DE ACCESO RAM - ESTUDIANTE: Federico Mattia
=====================================================
=> Ingrese su edad: 20

--- ANALIZANDO ACCESO SEGURO EN MEMORIA ---
[ACCESO APROBADO] El usuario es mayor de edad.
Edad registrada: 20 anos.
Direccion fisica en RAM Hexadecimal: 0x...
=====================================================
```

**Nota:** la dirección `0x...` es ilustrativa. La dirección real cambia según la ejecución y el entorno.

## Documentación y evidencias

La carpeta `docs/` contiene el informe del proyecto en formato PDF, elaborado según las normas APA 7.

La carpeta `capturas/` contiene las evidencias de ejecución del programa y el esquema de memoria utilizado para explicar el funcionamiento de los punteros.

## Autor

**Federico Mattia**

Proyecto realizado para la asignatura Laboratorio de Programación durante el ciclo lectivo 2026.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Para consultar las condiciones de uso, modificación y distribución, revisar el archivo `LICENSE`.
