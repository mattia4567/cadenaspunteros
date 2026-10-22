
## Institución

**Institución:** E.E.S.T. N.º 1 “Eduardo Ader” — Vicente López  
**Curso:** 5.º año  
**Materia:** Laboratorio de Programación (LPR)  
**Actividad:** Actividad 4 — Manipulación de Cadenas y Punteros en C/C++  
**Ciclo lectivo:** 2026

---

## Descripción del Proyecto

CADENASPUNTEROS es un proyecto académico desarrollado en C++ para estudiar el funcionamiento de los punteros y la manipulación de datos en la memoria RAM.

El programa implementa un sistema básico de control de acceso por edad. Para ello, utiliza un puntero que almacena la dirección de memoria de una variable entera, permitiendo ingresar, consultar y evaluar la edad mediante el operador de desreferenciación.

El proyecto tiene como finalidad aplicar conceptos fundamentales de programación en C++, comprender la relación entre las variables, los punteros y las direcciones de memoria, y utilizar estructuras condicionales para validar los datos ingresados.

## Integrantes

- **Federico Mattia** — Desarrollo del programa, implementación de punteros y documentación técnica.

## Requisitos e Instalación

Para compilar y ejecutar el proyecto, se necesitan las siguientes herramientas:

- **Compilador:** GCC (`g++`).
- **Lenguaje:** C++.
- **Editor recomendado:** Visual Studio Code.
- **Control de versiones:** Git.
- **Sistema operativo:** Windows, con un entorno de compilación compatible con GCC, como MinGW o MSYS2.

### Instalación

1. Instalar un compilador de C++ compatible con GCC y configurar su acceso desde la terminal.
2. Instalar Git y Visual Studio Code, si todavía no están instalados.
3. Clonar el repositorio:

   ```bash
   git clone URL_DEL_REPOSITORIO
   ```

4. Ingresar en la carpeta del proyecto:

   ```bash
   cd CADENASPUNTEROS
   ```

**Nota:** reemplazar `URL_DEL_REPOSITORIO` por la dirección real del repositorio de GitHub.

## Ejecución

Desde la terminal de Visual Studio Code, ubicada en la carpeta raíz del proyecto, seguir estos pasos.

### 1. Compilar

```bash
g++ src/main.cpp -o src/cadenaspunteros.exe
```

### 2. Ejecutar

En PowerShell, utilizar:

```powershell
.\src\cadenaspunteros.exe
```

Si no se dispone de un entorno de compilación local, se puede utilizar un compilador en línea, como OnlineGDB.

## Funcionamiento del Programa

El programa realiza las siguientes operaciones:

1. Declara la variable entera `edad` y la inicializa en cero.
2. Declara el puntero `p` y almacena en él la dirección de memoria de `edad`.
3. Solicita al usuario que ingrese su edad.
4. Utiliza `cin >> *p` para guardar el valor ingresado en la variable apuntada.
5. Evalúa la edad mediante una estructura condicional.
6. Muestra un mensaje de acceso aprobado si la edad es igual o superior a 18 años, o de acceso rechazado si es menor.
7. Imprime la edad registrada y la dirección de memoria representada en formato hexadecimal.

## Conceptos Fundamentales

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

**Importante:** la dirección que muestra el programa corresponde a una dirección de memoria virtual utilizada por el proceso, no necesariamente a una dirección física real de la RAM.

## Estructura del Repositorio

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

## Ejemplo de Ejecución

```text
=====================================================
   CONTROL DE ACCESO RAM - ESTUDIANTE: Federico Mattia
=====================================================
=> Ingrese su edad: 20

--- ANALIZANDO ACCESO SEGURO EN MEMORIA ---
[ACCESO APROBADO] El usuario es mayor de edad.
Edad registrada: 20 anos.
Direccion de memoria Hexadecimal: 0x...
=====================================================
```

**Nota:** la dirección `0x...` es ilustrativa. La dirección real cambia según la ejecución y el entorno.

## Documentación y Evidencias

La carpeta `docs/` contiene el informe del proyecto en formato PDF, elaborado según las normas APA 7.

La carpeta `capturas/` contiene las evidencias de ejecución del programa y el esquema de memoria utilizado para explicar el funcionamiento de los punteros.

## Objetivos del Proyecto

- Comprender el funcionamiento de los punteros en C++.
- Diferenciar una dirección de memoria de su contenido.
- Aplicar los operadores de dirección (`&`) y desreferenciación (`*`).
- Analizar la representación hexadecimal de las direcciones de memoria.
- Implementar una estructura condicional para validar la edad ingresada.
- Compilar, ejecutar y documentar un programa en C++.

## Autor

**Federico Mattia**

Proyecto realizado para la asignatura Laboratorio de Programación (LPR) durante el ciclo lectivo 2026, en el marco de la Actividad 4: Manipulación de Cadenas y Punteros en C/C++.

## Licencia

Este proyecto se distribuye bajo la licencia MIT. Para consultar las condiciones de uso, modificación y distribución, revisar el archivo `LICENSE` incluido en el repositorio.
