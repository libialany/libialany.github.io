## Parte 6 - Aplicaciones y contenedores

### Descripción

En este ejercicio se explorará la ejecución de aplicaciones en TrueNAS mediante contenedores. Se aprenderá a desplegar servicios adicionales, configurar almacenamiento persistente y administrar aplicaciones dentro del entorno TrueNAS SCALE.

### Apps

![app](part3/1.png)

### Descripcion de la aplicacion

![app](part3/2.png)

### Seleccionar Pool

![app](part3/3.png)

### Panel de aplicaciones

![app](part3/4.png)

### Probar la Aplicacion de LDAP

![app](part3/5.png)

## Ejercicio

Instala la aplicacion Photo prism.

**Puntos importantes.** 

Storage Configuration:

Storage: seleccionar Host Path y apuntar al dataset del Ejercicio 1 (/mnt/tank/rh-<tu_nombre>), o crear una subcarpeta photos dentro de él

Storage Path (config/db de la app) → puede ir en un dataset separado o subcarpeta photoprism-config dentro del mismo dataset

Admin Password: definir una

Networking: dejar el puerto por defecto o el que asigne el wizard

Apps → Discover Apps (o Available Applications según versión) → buscar PhotoPrism.

**Referencias:**

1. Documentación de aplicaciones en TrueNAS SCALE:
   [https://www.truenas.com/docs/scale/scaletutorials/apps/](https://www.truenas.com/docs/scale/scaletutorials/apps/)

2. Documentación oficial de contenedores Docker:
   [https://docs.docker.com/get-started/](https://docs.docker.com/get-started/)
