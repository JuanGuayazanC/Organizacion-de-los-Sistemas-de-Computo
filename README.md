# Organización de los Sistemas de Cómputo (ODSC)

Repositorio general del curso. Para saber cómo aprovecharlo, ver [Cómo usar este repositorio](#cómo-usar-este-repositorio).

## Estructura del proyecto

```
Organizacion-de-los-Sistemas-de-Computo/
├── Laboratorios/
│   ├── Arquitectura-del-computador-ODSC/
│   ├── MARIE-Assembler-Language-ODSC/
│   └── ARM-Assembler-Language-ODSC/
└── Proyectos/
    ├── Division-entera-Complemento-9-ODSC/
    ├── Secuencia-de-Collatz-ODSC/
    ├── Sistemas-Operativos-ODSC/
    └── SSEM-48-ODSC/
```

## Temas del curso

El curso recorre la organización interna de un computador, desde la arquitectura del conjunto de instrucciones hasta la construcción de circuitos digitales y la instalación de sistemas operativos:

- **Arquitectura del computador**: organización de la CPU, registros, ciclo de instrucción.
- **Conjunto de instrucciones y ensamblador**: programación en lenguaje ensamblador sobre arquitecturas didácticas (MARIE) y reales (ARM).
- **Aritmética computacional**: representación y operaciones sobre números de precisión arbitraria (división mediante complemento a 9).
- **Circuitos digitales (HDL)**: diseño de memoria y unidades aritméticas a nivel de compuertas lógicas (proyecto SSEM-48), en línea con el enfoque de construcción de un computador desde cero (Nand2Tetris).
- **Sistemas operativos**: instalación y configuración de distintas plataformas (Linux Slackware, Solaris, Windows Server) sobre máquina virtual, incluyendo particionamiento de disco, gestión de paquetes, configuración de red y administración de permisos.

## Cosas a tener en cuenta

- `MARIE-Assembler-Language-ODSC` y `ARM-Assembler-Language-ODSC` provienen del mismo repositorio original (`Conjunto-de-instrucciones-y-arquitectura-ODSC`), separados aquí porque cada uno corresponde a una arquitectura y una entrega distintas. En ambos, los archivos de ejercicio del laboratorio quedaron vacíos en el repositorio original (nunca se subió el código); se conservan así, junto con el simulador/ejemplo real que sí se subió.

## Herramientas

- Simuladores de arquitectura (MARIE Simulator)
- Ensambladores ARM (GNU `as`)
- VMware Workstation Pro, VirtualBox
- HDL (Hardware Description Language) / Nand2Tetris

## Profesor

Gerardo Ospina Hernández.

## Cómo usar este repositorio

Este repositorio no contiene código directamente: es una colección de repositorios independientes (laboratorios y proyectos), organizados por carpetas. Cada carpeta es un submódulo de git que apunta al repositorio real de esa actividad.

- **Para consultar una actividad puntual**: entra directamente a su carpeta en GitHub (o navega el submódulo) y revisa su propio README.
- **Para tener todo el contenido en tu máquina**:

```bash
git clone --recurse-submodules https://github.com/JuanGuayazanC/Organizacion-de-los-Sistemas-de-Computo.git
```

Si ya clonaste el repositorio sin submódulos:

```bash
git submodule update --init --recursive
```
