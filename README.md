# Organización de los Sistemas de Cómputo (ODSC)

Repositorio general del curso Organización de los Sistemas de Cómputo (ISIS ODSC-101), que agrupa —mediante submódulos de git— los laboratorios y proyectos del curso.

Cada submódulo es un repositorio independiente con su propio historial de commits y README. Para clonar este repositorio junto con todo su contenido, ver [Cómo clonar](#cómo-clonar).

## Estructura del proyecto

```
Organizaci-n-de-los-Sistemas-de-C-mputo/
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

## Cómo clonar

```bash
git clone --recurse-submodules https://github.com/JuanGuayazanC/Organizaci-n-de-los-Sistemas-de-C-mputo.git
```

Si ya clonaste el repositorio sin submódulos:

```bash
git submodule update --init --recursive
```
