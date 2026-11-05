# 🚀 Sistema de Automatización y Gestión en Bash

Conjunto de scripts modulares desarrollados en Bash orientados al monitoreo del sistema, la administración segura de archivos, el análisis de rendimiento de servidores y la programación automatizada de tareas mediante `cron`.

---

## 📁 Estructura del Repositorio

El proyecto se compone de 4 módulos principales:

* **`modulo01.sh` (Reporte del Sistema):** Recopila y muestra información clave del equipo (usuario actual, fecha/hora, distribución de Linux, porcentaje de uso de CPU, memoria RAM total/usada y espacio del disco duro), guardando un registro limpio en `Reporte_Sistema.txt`.
* **`modulo02.sh` (Gestor de Archivos):** Menú interactivo con funciones avanzadas para **crear**, **copiar** (con validación de nombres duplicados), **cambiar permisos** (mediante cálculo octal interactivo de permisos `rwx` para usuario, grupo y otros) y **eliminar** archivos con doble confirmación de seguridad.
* **`modulo03.sh` (Gestión y Auditoría de Servidores):** Lee un archivo de origen (`servidores.txt`), filtra aquellos con uso de disco $\ge 70\%$, asigna etiquetas de riesgo dinámicas (`Crítico`, `Alto`, `Moderado`), y permite simular operaciones de mantenimiento reduciendo métricas y actualizando estados operativos (`Atendido`, `Estable`, `En Espera`) en un informe secundario.
* **`modulo04.sh` (Gestor de Tareas Automáticas - Cron):** Automatiza la ejecución de scripts en el sistema operativo. Permite listar las tareas activas de `crontab`, programar nuevas tareas de forma interactiva (ejecución única o diaria a una hora específica) y eliminar tareas existentes de manera guiada.

---

## ⚙️ Requisitos Previos

* Sistema operativo basado en Linux / UNIX o entorno compatible (como WSL en Windows).
* Intérprete **Bash** instalado.
* Permisos de ejecución en los scripts.
* Para el **Módulo 04**, el servicio de cron (`cron` / `crond`) debe estar activo en el sistema.

---

## 🚀 Instalación y Uso

1. Clona este repositorio o descarga los archivos en tu equipo:
   ```bash
   git clone [https://github.com/tu-usuario/tu-repositorio.git](https://github.com/tu-usuario/tu-repositorio.git)
   cd tu-repositorio
