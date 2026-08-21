## Parte 4 - Uso compartido SMB/NFS

### Descripción

En este ejercicio se configurarán servicios de compartición de archivos utilizando los protocolos **SMB (Windows)** y **NFS (Linux/Unix)**. Los participantes aprenderán a crear recursos compartidos, aplicar permisos y conectar clientes externos al almacenamiento TrueNAS.
Todo esto lo encuentras en la seccion:

**System → Services → NFS**

Este es la imagen del resultado.

<img width="919" height="220" alt="image" src="https://github.com/user-attachments/assets/6643bdc5-9990-480b-8927-596b15278319" />

Ahora empecemos....

### Configuracion de accesos(users, grupos, dataset)

<img width="818" height="467" alt="image" src="https://github.com/user-attachments/assets/fb48fa4b-a57d-4b9a-b145-8c2038037481" />

### Panel para compartir

![configuracion_1](part1/11.png)

### Configurar la carpeta a compartir

![configuracion_2](part1/12.png)

### Estatus

![configuracion_3](part1/13.png)

### Permitir a usuario 

![configuracion_4](part1/14.png)

### Ejercicio

Objetivo: Exponer el dataset del Ejercicio 1 vía NFS.

Pasos:

Paso 1.

Path: /mnt/tank/rh-<tu_nombre>
Description: opcional
Maproot User/Group: dejar vacío para empezar
Networks/Hosts: si quieren restringir, agregar la subred del laboratorio (ej. 192.168.1.0/24); si no, dejar abierto para el ejercicio

Paso 2.

```
   sudo mkdir -p /mnt/prueba
   sudo mount -t nfs <ip_truenas>:/mnt/tank/workshop-<tu_nombre> /mnt/prueba
```


**Referencias:**

1. Configuración de recursos compartidos SMB en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/shares/smb/](https://www.truenas.com/docs/scale/scaletutorials/shares/smb/)

2. Configuración de recursos compartidos NFS en TrueNAS:
   [https://www.truenas.com/docs/scale/scaletutorials/shares/nfs/](https://www.truenas.com/docs/scale/scaletutorials/shares/nfs/)
