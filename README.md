# ASSIO-ESA

Repositorio de entregables de la práctica **88020_P2_ESA**, de Administración y Servicios de Sistemas Operativos. La memoria trata acceso e identificación, estructura de directorios, usuarios/grupos, permisos DAC, SGID y listas de control de acceso en un entorno Linux de laboratorio.

## Contenido y uso

| Archivo | Uso |
| --- | --- |
| `88020_P2_ESA.pdf` | Memoria con pasos, capturas, decisiones y validaciones del laboratorio |
| `88020_P2_ESA.pptx` | Presentación editable de la práctica |

Abre el PDF con un lector o la presentación con una aplicación compatible. En la rama `main` auditada no hay código fuente ejecutable, scripts de configuración, manifiesto de dependencias ni VM; no hay instalación, arranque de aplicación o comando de tests que ejecutar desde ella.

## Material en otras ramas

También se inspeccionó el inventario de las otras tres ramas existentes. No se fusionan ni se cambian sus archivos:

| Rama | Material localizado |
| --- | --- |
| `I001---Código---ESA` | [Código/Comandos .pdf](https://github.com/EduardoManzanoAlcaraz/ASSIO-ESA/blob/bf68d3dcbcf82cfdf311f40204357acd2c2d3364/C%C3%B3digo/Comandos%20.pdf), inventario comprobado; contenido no auditado en esta revisión |
| `I001---Documentacion---ESA` | [Documentación de P1](https://github.com/EduardoManzanoAlcaraz/ASSIO-ESA/tree/ac6b263a313ed7e74aa5fd9c684df3974677978a/Documentaci%C3%B3n), dos PDF localizados; contenido no auditado aquí |
| `I002---Sistema-de-archivos,-comandos,-usuarios-y-permisos-(Codigo)` | [Código (P2)/88020_P2_ESA.txt](https://github.com/EduardoManzanoAlcaraz/ASSIO-ESA/blob/8695bfb5d381e34528f90c6471e77b4d23fef6a5/C%C3%B3digo%20%28P2%29/88020_P2_ESA.txt), texto de comandos leído completo |

El TXT de P2 contiene secuencias manuales para crear directorios/usuarios/grupos y configurar/probar propietarios, permisos y ACL con herramientas Linux (`setfacl`/`getfacl`, entre otras). Incluye encabezados y sesiones interactivas `su`: **no es un script idempotente ejecutable de principio a fin**. Necesita VM Linux de laboratorio, estado previo y privilegios definidos; no se ejecutó. Los enlaces fijan los commits inspeccionados y evitan confundir ese material con el contenido de `main`.

## Estado y siguientes pasos

Revisión del 2026-11-19 sobre `1ea390309b1a148e643415a1edad770989c7aa26`. Las observaciones del código se distinguen de las pruebas ejecutadas y de los informes históricos. Esta revisión solo modifica documentación.

Se verificó el inventario y se extrajo el texto de la memoria para identificar su alcance. Eso no reproduce el laboratorio ni verifica hoy los permisos mostrados en las capturas; tampoco acredita el renderizado completo del PPTX. No se crearon usuarios ni se cambiaron permisos del equipo.

Para reproducir la práctica hará falta una VM Linux de laboratorio y reconstruir sus pasos, usando el TXT de P2 como referencia revisada, no como automatización ya probada; no aplicar los comandos administrativos al ordenador habitual. Como mejora futura, convertir esa referencia en scripts idempotentes y comprobaciones de acceso por rol, si se desarrollan y verifican expresamente.

[Instrucciones para agentes](AGENTS.md).
