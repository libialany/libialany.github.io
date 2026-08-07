Aquí tienes descripciones orientadas a un **taller práctico de administración de TrueNAS**, con dos referencias recomendadas para cada ejercicio.

---

## Parte 2 - Grupos de almacenamiento y ZFS

### Descripción

En este ejercicio se aprenderán los conceptos fundamentales del almacenamiento en TrueNAS mediante **ZFS**, incluyendo la creación de pools de almacenamiento, datasets, vdevs y la configuración de propiedades como compresión, cuotas y reservas. El objetivo es comprender cómo ZFS proporciona integridad de datos, protección contra fallos y administración flexible del almacenamiento.

**Referencias:**

1. Documentación oficial de TrueNAS sobre pools y ZFS:
   [https://www.truenas.com/docs/scale/scaletutorials/storage/](https://www.truenas.com/docs/scale/scaletutorials/storage/)

2. Documentación oficial de OpenZFS sobre conceptos de almacenamiento:
   [https://openzfs.org/wiki/Main_Page](https://openzfs.org/wiki/Main_Page)

---

## Parte 3 - Usuarios, grupos y permisos

### Descripción

En este ejercicio se configurará la administración de usuarios y grupos en TrueNAS. Se practicarán la creación de cuentas, asignación de grupos, permisos sobre datasets y control de acceso mediante ACL. El objetivo es aprender a implementar una estructura segura para usuarios y recursos compartidos.

**Referencias:**

1. Administración de usuarios y grupos en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/credentials/](https://www.truenas.com/docs/scale/scaletutorials/credentials/)

2. Guía de permisos y ACL en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/shares/](https://www.truenas.com/docs/scale/scaletutorials/shares/)

---

## Parte 4 - Uso compartido SMB/NFS

### Descripción

En este ejercicio se configurarán servicios de compartición de archivos utilizando los protocolos **SMB (Windows)** y **NFS (Linux/Unix)**. Los participantes aprenderán a crear recursos compartidos, aplicar permisos y conectar clientes externos al almacenamiento TrueNAS.

**Referencias:**

1. Configuración de recursos compartidos SMB en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/shares/smb/](https://www.truenas.com/docs/scale/scaletutorials/shares/smb/)

2. Configuración de recursos compartidos NFS en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/shares/nfs/](https://www.truenas.com/docs/scale/scaletutorials/shares/nfs/)

---

## Parte 5 - Instantáneas y replicación

### Descripción

En este ejercicio se implementará una estrategia de protección de datos utilizando **snapshots ZFS** y replicación. Se aprenderá cómo crear puntos de recuperación, programar instantáneas automáticas y replicar información hacia otro sistema TrueNAS para recuperación ante desastres.

**Referencias:**

1. Documentación de snapshots en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/dataprotection/](https://www.truenas.com/docs/scale/scaletutorials/dataprotection/)

2. Documentación de replicación ZFS en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/dataprotection/replication/](https://www.truenas.com/docs/scale/scaletutorials/dataprotection/replication/)

---

## Parte 6 - Aplicaciones y contenedores

### Descripción

En este ejercicio se explorará la ejecución de aplicaciones en TrueNAS mediante contenedores. Se aprenderá a desplegar servicios adicionales, configurar almacenamiento persistente y administrar aplicaciones dentro del entorno TrueNAS SCALE.

**Referencias:**

1. Documentación de aplicaciones en TrueNAS SCALE:
   [https://www.truenas.com/docs/scale/scaletutorials/apps/](https://www.truenas.com/docs/scale/scaletutorials/apps/)

2. Documentación oficial de contenedores Docker:
   [https://docs.docker.com/get-started/](https://docs.docker.com/get-started/)

---

## Parte 7 - Estrategia de copia de seguridad

### Descripción

En este ejercicio se diseñará una estrategia básica de copias de seguridad utilizando las herramientas disponibles en TrueNAS. Se trabajarán conceptos como copias locales, replicación remota, programación de tareas y recuperación de información para garantizar la disponibilidad de los datos.

**Referencias:**

1. Guía de protección de datos en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/dataprotection/](https://www.truenas.com/docs/scale/scaletutorials/dataprotection/)

2. Buenas prácticas de estrategia de backup (regla 3-2-1):
   [https://www.cisa.gov/news-events/news/data-backup-options](https://www.cisa.gov/news-events/news/data-backup-options)

---

Estas descripciones pueden integrarse directamente como páginas Markdown para un sitio Docsify de un **curso de administración TrueNAS**.
