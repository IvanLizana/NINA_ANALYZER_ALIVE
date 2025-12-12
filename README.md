<div align="center">
  <img src="https://img.shields.io/badge/ASTROREMOTO-Precision_Software-blue?style=for-the-badge" alt="Astroremoto" />
  <br>
  <p>
    <strong>
      <a href="#-español-documentación-oficial">🇪🇸 ESPAÑOL (LEER PRIMERO)</a>
      &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
      <a href="#-english-official-documentation">🇬🇧 ENGLISH (READ BELOW)</a>
    </strong>
  </p>
</div>

---

<a name="-español-documentación-oficial"></a>
# 🔭 N.I.N.A. Analyzer - Precision Suite (v25)

![Versión](https://img.shields.io/badge/Versión-v25.0_Black_Box-gold)
![Plataforma](https://img.shields.io/badge/Plataforma-Windows_Portable-blue)
![Motor](https://img.shields.io/badge/Motor-Metrology_Engine_v2-cyan)
![Licencia](https://img.shields.io/badge/Licencia-Freeware-green)

<div align="center">
  <h3>Herramienta de Metrología Forense para Astrofotografía</h3>
  <p><em>Transforme gigabytes de logs de sesión en Inteligencia Operativa.</em></p>
  
  <a href="https://github.com/IvanLizana/NINA_ANALYZER_ALIVE/releases/latest">
    <img src="https://img.shields.io/badge/DESCARGAR_EXE_v25-Clic_Aquí-success?style=for-the-badge&logo=windows&logoColor=white" alt="Descargar Ahora" />
  </a>
</div>

## 📄 Descripción General

**N.I.N.A. Analyzer** es una suite de diagnóstico post-sesión diseñada para astrofotógrafos que utilizan *Nighttime Imaging 'N' Astronomy*. A diferencia de los visores de logs tradicionales, este software no solo muestra datos; aplica **heurística avanzada** para determinar la salud de su tren óptico, la calidad del cielo y la seguridad de su equipo.

El software se distribuye bajo la filosofía **"Portable & Standalone"**: Un único archivo ejecutable que lleva todo incluido (motor gráfico, librerías de cálculo y manuales), sin necesidad de instalar Python ni dependencias externas.

---

## ⚡ Novedades en v25: Arquitectura "Black Box"

Esta versión introduce módulos de auditoría profunda para detectar ineficiencias y eventos que antes pasaban desapercibidos.

### 1. Módulo Experimental: Caja Negra (Black Box) 👽
N.I.N.A. evoluciona constantemente. La v25 incluye un **Colector de Eventos No Mapeados**.
* **¿Qué hace?** Captura todas las líneas del log que el motor no reconoce (ej. nuevos drivers de rotadores, techos o scripts personalizados).
* **Análisis de Frecuencia:** Le muestra una tabla separando el "ruido" (avisos repetidos 5000 veces) de los eventos únicos críticos.
* **Colaboración:** Genera un reporte de texto automático para que pueda enviarlo al desarrollador y ayudar a mejorar el soporte de hardware.

### 2. Análisis de Distribución de Tiempo ⏳
Nuevo gráfico de torta (Pie Chart) para visualizar el **Balance de la Noche**.
* Responde a la pregunta: *"¿Cuánto tiempo estuve capturando fotones vs. cuánto tiempo perdí resolviendo problemas?"*.
* Vital para optimizar tiempos de dithering y enfoque.

### 3. Inspector de Tareas Detallado 🔍
Hemos desglosado el análisis en gráficos de barras independientes para:
* **Captura:** Verificación de tiempos de exposición reales.
* **Enfoque (AF):** Auditoría de duración de rutinas HFR (detecta backlashes lentos).
* **Errores:** Cronología visual de fallos y alertas del sistema.

### 4. Física de Precisión (F-Ratio & CFZ) 🔭
El motor matemático ha sido actualizado. Ahora permite ingresar la **Relación Focal (f/)** real de su telescopio.
* Esto permite un cálculo exacto de la **Zona Crítica de Enfoque (CFZ)** en micras.
* El software le dirá si sus re-enfoques fueron necesarios o si su óptica es limitada por difracción.

---

## 🔬 Funcionalidades Core (Heredadas de v24)

* **Cine Forense (Event Replay):** Reproducción animada de la estrella guía utilizando algoritmos de *Max-Pooling* para detectar golpes de viento que los promedios matemáticos esconden.
* **Gantt Interactivo:** Línea de tiempo con semáforo de calidad (Verde/Amarillo/Rojo) basado en su tolerancia de píxeles.
* **System DNA:** Auditoría de hardware (RAM y Disco) para prevenir fallos por saturación.
* **Manual Integrado:** Documentación técnica completa disponible dentro de la aplicación.

---

## 📥 Instrucciones de Instalación y Uso

Este programa es **100% Portable**. No ensucia su registro de Windows ni requiere permisos de administrador.

1.  **Descargar:** Vaya a la sección de **[Releases (Lanzamientos)](../../releases)** y baje el archivo `NINA_Analyzer_Alive_v25.exe`.
2.  **Ubicación:** Guarde el archivo donde quiera (Escritorio, Documentos, USB).
3.  **Ejecutar:** Abra el archivo.
    * *Aparecerá una consola negra (CMD) por unos segundos. **NO LA CIERRE**, es el motor del programa.*
    * *Si es la primera vez, puede pedir un correo. Presione ENTER para omitir.*
    * *Luego se abrirá la interfaz en su navegador predeterminado.*
4.  **Cargar Datos:** Use el botón "Explorar PC" para seleccionar un log en `%localappdata%\NINA\Logs`.

> **⚠️ Nota sobre Windows Defender:**
> Al ser software gratuito desarrollado por un **astrofotógrafo aficionado**, Windows puede mostrar una advertencia de "Editor Desconocido".
> * Esto es normal. Haga clic en **"Más información"** y luego en **"Ejecutar de todas formas"**.

---
---

<a name="-english-official-documentation"></a>
# 🔭 N.I.N.A. Analyzer - Precision Suite (v25)

![Version](https://img.shields.io/badge/Version-v25.0_Black_Box-gold)
![Platform](https://img.shields.io/badge/Platform-Windows_Portable-blue)
![Engine](https://img.shields.io/badge/Engine-Metrology_Engine_v2-cyan)

<div align="center">
  <h3>Forensic Metrology Tool for Astrophotography</h3>
  <p><em>Transform gigabytes of session logs into Operational Intelligence.</em></p>
  
  <a href="https://github.com/IvanLizana/NINA_ANALYZER_ALIVE/releases/latest">
    <img src="https://img.shields.io/badge/DOWNLOAD_v25_EXE-Click_Here-success?style=for-the-badge&logo=windows&logoColor=white" alt="Download Now" />
  </a>
</div>

## 📄 Overview

**N.I.N.A. Analyzer** is a post-session diagnostic suite tailored for astrophotographers using *Nighttime Imaging 'N' Astronomy*. Unlike traditional log viewers, this software doesn't just display data; it applies **advanced heuristics** to determine the health of your optical train, sky quality, and equipment safety.

The software follows a **"Portable & Standalone"** philosophy: A single executable file containing everything (graphics engine, math libraries, and manuals), with no need to install Python or external dependencies.

---

## ⚡ What's New in v25: "Black Box" Architecture

This version introduces deep audit modules to detect inefficiencies and events that previously went unnoticed.

### 1. Experimental Module: Black Box 👽
N.I.N.A. is constantly evolving. v25 includes an **Unmapped Event Collector**.
* **What does it do?** It captures all log lines the engine doesn't recognize (e.g., new rotator drivers, roofs, or custom scripts).
* **Frequency Analysis:** Displays a table separating "noise" (warnings repeated 5000 times) from critical unique events.
* **Collaboration:** Generates an automatic text report so you can send it to the developer and help improve hardware support.

### 2. Time Distribution Analysis ⏳
New Pie Chart visualization for **Night Balance**.
* Answers the question: *"How much time was I capturing photons vs. how much time did I waste solving problems?"*.
* Vital for optimizing dithering and focus times.

### 3. Detailed Task Inspector 🔍
We have broken down the analysis into independent bar charts for:
* **Imaging:** Verification of actual exposure times.
* **Autofocus (AF):** Audit of HFR routine duration (detects slow backlash).
* **Errors:** Visual timeline of system failures and alerts.

### 4. Precision Physics (F-Ratio & CFZ) 🔭
The math engine has been updated. It now allows inputting the real **Focal Ratio (f/)** of your telescope.
* This allows for an exact calculation of the **Critical Focus Zone (CFZ)** in microns.
* The software will tell you if your re-focusing was necessary or if your optics are diffraction-limited.

---

## 🔬 Core Features (Inherited from v24)

* **Forensic Cinema (Event Replay):** Animated playback of the guide star using *Max-Pooling* algorithms to detect wind gusts hidden by mathematical averages.
* **Interactive Gantt:** Timeline with a quality traffic light system (Green/Yellow/Red) based on your pixel tolerance.
* **System DNA:** Hardware audit (RAM and Disk) to prevent saturation failures.
* **Integrated Manual:** Full technical documentation available within the app.

---

## 📥 Installation & Usage Instructions

This program is **100% Portable**. It does not clutter your Windows Registry nor require admin rights.

1.  **Download:** Go to the **[Releases](../../releases)** section and download `NINA_Analyzer_Alive_v25.exe`.
2.  **Location:** Save the file anywhere (Desktop, Documents, USB drive).
3.  **Run:** Open the file.
    * *A black console window (CMD) will appear for a few seconds. **DO NOT CLOSE IT**, it is the program engine.*
    * *If it's the first time, it might ask for an email. Press ENTER to skip.*
    * *Then, the interface will launch in your default web browser.*
4.  **Load Data:** Use the "Browse PC" button to select a log in `%localappdata%\NINA\Logs`.

> **⚠️ Note on Windows Defender:**
> Since this is free software developed by an **amateur astrophotographer** (and not a corporation), Windows might show an "Unknown Publisher" warning.
> * This is normal. Click **"More Info"** and then **"Run Anyway"**.

---

## 🤝 Credits / Créditos
* **Developer:** Iván Lizana (ASTROREMOTO).
* **Tech Stack:** Python 3.14 + Streamlit + Plotly + Pandas.
* **Support:** veckoff@gmail.com
* Special thanks to **ACHAYA** for the theoretical foundations.
