# 🚀 Sistema de Automatización y Gestión en Bash

## Descripción breve
Conjunto de scripts modulares desarrollados en Bash orientados al monitoreo del estado del sistema, la administración interactiva de archivos, el análisis automatizado de rendimiento de servidores y la gestión de tareas programadas mediante `cron`.

---

## Requisitos
* Sistema operativo basado en Linux / UNIX o entorno compatible (como WSL en Windows).
* Intérprete **Bash** instalado.
* Permisos de ejecución en los scripts.
* Para el funcionamiento del **Módulo 04**, el servicio de cron (`cron` / `crond`) debe estar activo en el sistema.

---

## Instalación y Ejecución

1. Clona este repositorio o descarga los archivos en tu equipo local:
   ```bash
   git clone [https://github.com/tu-usuario/tu-repositorio.git](https://github.com/tu-usuario/tu-repositorio.git)
   cd tu-repositorio

## Otorga permisos de ejecución a los scripts:

Bash
chmod +x *.sh

## Ejecuta el módulo de tu preferencia:

Bash
./modulo01.sh

## Módulos
📌 Módulo 01: Reporte del Sistema
Funcionalidad: Recopila información clave del equipo de forma automatizada, incluyendo el usuario actual, fecha y hora del sistema, distribución de Linux, porcentaje actual de uso de CPU, estado de la memoria RAM (total y usada) y el espacio disponible/utilizado en el disco duro. Toda la información recopilada se muestra en pantalla y se almacena en un archivo de salida llamado Reporte_Sistema.txt.

📌 Módulo 02: Gestor de Archivos
Funcionalidad: Proporciona un menú interactivo en bucle para realizar operaciones comunes sobre archivos de manera segura:

Creación: Permite crear nuevos archivos validando previamente si ya existen en el directorio.

Copia: Duplica archivos existentes verificando que el nuevo nombre de copia no genere conflictos.

Permisos: Calcula de forma interactiva y segura los permisos numéricos (octales) del sistema (rwx) tanto para el propietario, el grupo y otros usuarios mediante una interfaz guiada por preguntas de tipo sí/no.

Eliminación: Borra archivos de forma segura requiriendo una doble confirmación por parte del usuario antes de ejecutar la instrucción.

📌 Módulo 03: Gestión y Auditoría de Servidores
Funcionalidad: Automatiza la lectura y análisis de un archivo de origen (servidores.txt):

Análisis: Filtra los servidores cuyo uso de disco sea superior o igual al 70%, asignando etiquetas de criticidad automáticas (Crítico, Alto, Moderado) y generando un informe detallado (informe_servidores.txt).

Modificación y Mantenimiento: Permite procesar una copia del informe para simular operaciones de optimización (reduciendo métricas de uso de disco en un 20%) y actualizando automáticamente las etiquetas de estado a un perfil operativo (Atendido, Estable, En Espera).

📌 Módulo 04: Gestor de Tareas Automáticas (Cron)
Funcionalidad: Administra la automatización de scripts mediante el programador de tareas del sistema operativo (crontab):

Visualización: Lista de forma limpia las tareas activas programadas en el sistema.

Programación: Permite configurar nuevas tareas de ejecución única (especificando hora y minuto para el día actual) o recurrente (diaria) de manera completamente validada.

Eliminación: Muestra un listado amigable de las tareas existentes para permitir seleccionar y eliminar de manera precisa una tarea específica sin alterar las demás configuraciones del sistema.

## Autores
Denegri Sairytupac, Brenda

Farfan Requejo, Steven
