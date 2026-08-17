## Parte 1 - Instalación y configuración inicial

### Descripción

En este ejercicio se aprenderá el proceso de instalación y configuración inicial de TrueNAS, incluyendo los requisitos mínimos del sistema, la preparación del medio de instalación y los pasos necesarios para realizar una instalación limpia. También se configurarán los parámetros básicos del sistema como red, almacenamiento y servicios esenciales.

### Requisitos del sistema

Requisitos de hardware para montar un servidor TrueNAS

- 2 discos duros de al menos 950 GiB cada uno, destinados al almacenamiento de datos.
- Una PC de gama media, preferiblemente con procesador de 64 bits y suficiente memoria RAM para ejecutar TrueNAS de forma estable.
- Una memoria USB para crear el medio de instalación y realizar el arranque de TrueNAS.
- Conexión de red Ethernet, preferiblemente Gigabit (1 GbE) o superior, para aprovechar adecuadamente el almacenamiento en red.

Recomendaciones

Se recomienda contar con al menos 8 GiB de RAM para una instalación básica de TrueNAS.

### Instalación

![Instalación](part1/2.jpg)

### Configuración inicial

![Configuración](part1/3.jpg)

![Requisitos](part1/1.jpg)

### Interfaz web

![Interfaz web](part1/4.jpg)

---

# ZFS

**ZFS (Zettabyte File System)** es un tipo especial de sistema de archivos que se usa para almacenar y gestionar datos en computadoras y servidores. 

## ¿Qué puede hacer ZFS?

1. Protege tus datos (checksums)
2. Autorreparación (self-healing) 
3. Snapshots (instantáneas)
4. Compresión
5. Fácil de expandir 
6. Combina discos inteligentemente

## Componentes Principales de ZFS

### 1. ZFS Pool (zpool)
El **pool** formado de varios discos. En vez de formatear cada disco por separado, pones todos los discos dentro de un pool, y ZFS gestiona todo el conjunto como una sola unidad. Tus archivos y carpetas se crean dentro de este pool.

### 2. Vdev (Dispositivo Virtual)
Un pool no está hecho directamente de discos está hecho de **vdevs** (dispositivos virtuales). Un vdev es un grupo de uno o más discos físicos que se comportan como una sola unidad dentro del pool.

Tipos de vdev

#### Vdev de disco único (Single Disk)
- Es solo **un disco**, usado solo. 100% del espacio del disco.
- Sin protección: si ese disco falla, **pierdes los datos** que contenía.

#### Vdev en espejo (Mirror)
- Usa dos o más discos que guardan la misma copia exacta de los datos. ZFS puede "autorrepararse" usando la copia buena
- Si un disco falla, el otro sigue teniendo todos los datos seguros.

## Quiz

1. ¿Cuál es el propósito principal de un **ZFS pool**?
2. Nombra **dos características especiales** que ofrece ZFS y que un sistema de archivos normal usualmente no tiene.
3. Si tienes dos discos de 500GB en un **vdev en espejo (mirror)**, ¿cuánto espacio de almacenamiento útil tendrás realmente? ¿Por qué?


**Referencias:**

1. Guía de instalación de TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/install/](https://www.truenas.com/docs/scale/scaletutorials/install/)

2. Requisitos del sistema TrueNAS:
   [https://www.truenas.com/docs/scale/gettingstarted/sysreqs/](https://www.truenas.com/docs/scale/gettingstarted/sysreqs/)
