## Parte 5 - Instantáneas y replicación

### Descripción

En este ejercicio se implementará una estrategia de protección de datos utilizando **snapshots** y replicación. Se aprenderá cómo crear puntos de recuperación, programar instantáneas automáticas y replicar información hacia otro sistema TrueNAS para recuperación ante desastres.

Secciones a revisar:

Storage → Snapshots

System → Services →  SSH

### Configurar Replicacion

<img width="484" height="515" alt="image" src="https://github.com/user-attachments/assets/770e9c66-d57b-4be2-ba9f-543ab75cfdee" />

<img width="508" height="512" alt="image" src="https://github.com/user-attachments/assets/e795b4c2-4880-485b-a659-f75395be06ca" />


### Ejercicio

Objetivo: Crear una snapshot y replicarla hacia otro TrueNAS.

**Master TrueNAS**

1. Crear a Snapshot de un dataset.

2. Data Protection → Replication Tasks → Add (el asistente crea automáticamente la SSH connection si no existe):
   
   Source: dataset del Ejercicio 1
   
   Destination: sistema remoto + dataset destino
   
   Transport: SSH (dejar que el wizard genere/instale la clave SSH automáticamente)
   
   Schedule: "Run Once" para el ejercicio (o cada 5 min si quieren verlo en vivo)
   
   Ejecutar la tarea manualmente (Run Now).

**Slave TrueNAS**

1. Crear un pool/dataset destino vacío para recibir la réplica.

2. revisar Storage → Pools y confirmar que el dataset replicado apareció con los datos.



**Referencias:**

1. Documentación de snapshots en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/dataprotection/](https://www.truenas.com/docs/scale/scaletutorials/dataprotection/)

2. Documentación de replicación ZFS en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/dataprotection/replication/](https://www.truenas.com/docs/scale/scaletutorials/dataprotection/replication/)
