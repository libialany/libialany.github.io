## Descripción

En este nivel se aprenderá los fundamentos de la herramienta y los principales servicios que ofrece TrueNAS. Los participantes conoceran los casos de uso de truenas.

## Temas

- [Requisitos](./parte1.md)
- [Conceptos Base](./parte2.md)
- [Control de Usuarios](./parte3.md)

## Introduccion - Los datos digitales 

Estos datos se almacenan en tres tipos de medios:

* **Magnéticos:** Los discos magnéticos incluyen el disco duro de tu computadora portátil, discos duros externos, entornos de red y servidores, y cintas magnéticas (de carrete a carrete y de cartucho).
* **Ópticos:** Los medios ópticos incluyen discos compactos (CD, CD-ROM, CD-R, CD-RW), discos versátiles digitales (DVD, DVD+R, DVD-R, DVD-RAM, DVD+RW, DVD-RW), discos de una sola escritura y múltiples lecturas (WORM), discos DVD de alta definición (Blu-ray y HD-DVD), tarjetas inteligentes y cintas ópticas.
* **De estado sólido:** Tarjetas de memoria flash, unidades USB Flash y discos duros de estado sólido (SSD).

### Buenas prácticas al guardar

Estos son los primeros pasos:

* Localiza todos los archivos de datos que deseas almacenar.
* Decide qué necesitas conservar.
* Crea un directorio que identifique tus archivos de datos por **nombre, formato, tamaño y ubicación**. ¡Mantenlo actualizado!
* Etiqueta los contenedores de datos y los medios que se encuentran dentro de ellos. ¿Qué sucedería si se separaran?
* Localiza y/o crea documentación complementaria (**metadatos**) para cada archivo de datos. Incluye nombres de variables, descripciones, unidades, estándares, calibraciones de instrumentos, códigos, algoritmos utilizados para transformar los datos y software utilizado (incluida la versión y el sistema operativo). ¿Qué necesitarías para poder utilizar este archivo de datos si no recordaras todos estos detalles?
* Organiza los archivos. Documenta tu metodología de organización y utilízala de manera consistente.

### El almacenamiento de datos

El almacenamiento de datos puede parecer bastante sencillo. Simplemente almacena los datos en tu disco duro o en la nube, ¿verdad?
Antes de comenzar a tomar decisiones sobre el almacenamiento, deberías hacerte algunas preguntas sobre los datos:

* ¿Qué tan importantes son los datos?
* ¿Necesito conservar estos datos? ¿Los datos pueden reproducirse o son únicos?
* ¿Durante cuánto tiempo quiero o necesito conservar los datos?
* ¿Con qué rapidez necesito acceder a los datos?
* ¿Qué nivel de seguridad necesitan los datos?
* ¿Necesitan otras personas acceder a los datos?
* ¿Qué requisitos institucionales o de los financiadores deben cumplirse?

### Buenas prácticas: regla 3-2-1 y zonas de riesgo

Las copias de seguridad (**backups**) de los datos son muy importantes. Sigue la **regla 3-2-1**:

* Mantén **tres copias** de cualquier archivo de datos importante: una copia principal y dos copias de seguridad.
* Mantén **dos copias en medios digitales diferentes**, por ejemplo, un disco duro (HDD) y una unidad Flash.
* Mantén **una copia fuera del sitio** (*offsite*) o, al menos, **sin conexión** (*offline*).

A esto a veces se le denomina **Aquí-Cerca-Lejos (Here-Near-Far)**:

* Copia de trabajo: **Aquí**
* Copia de seguridad principal: **Cerca**
* Segunda copia de seguridad: **Lejos**

### ¿Qué es una zona de riesgo (*threat zone*)?

Una **zona de riesgo** es una ubicación geográfica diferente de aquella en la que estás trabajando.

Por ejemplo, si ocurriera un desastre natural en Virginia y todos tus archivos de datos estuvieran allí, probablemente lo perderías todo. Coloca tu copia principal o tu copia de seguridad principal en un medio seguro y envíala a un amigo o colega que se encuentre en otro estado para mantenerla a salvo.

**¿Se puede considerar la nube como una zona geográfica diferente?**

![datos](https://us1.discourse-cdn.com/spiceworks/original/4X/d/4/f/d4f28c328662057a7605c93d6211089561b5eb94.jpeg)

Sí, siempre que los servidores no se encuentren en la misma zona geográfica en la que estás. Algunos proveedores de almacenamiento en la nube permiten especificar dónde se almacenan físicamente tus datos.
