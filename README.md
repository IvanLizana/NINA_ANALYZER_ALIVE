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
# 🔭 N.I.N.A. Analyzer - Precision Suite (v27)

![Versión](https://img.shields.io/badge/Versión-v27.0_Metrology_Engine-gold)
![Plataforma](https://img.shields.io/badge/Plataforma-Windows_Portable-blue)
![Motor](https://img.shields.io/badge/Motor-Metrology_Engine_v3-cyan)
![Licencia](https://img.shields.io/badge/Licencia-Freeware-green)

<div align="center">
  <h3>Herramienta de Metrología Forense para Astrofotografía</h3>
  <p><em>Transforme gigabytes de logs de sesión en Inteligencia Operativa.</em></p>
  
  <a href="https://github.com/IvanLizana/NINA_ANALYZER_ALIVE/releases/latest">
    <img src="https://img.shields.io/badge/DESCARGAR_EXE_v27-Clic_Aquí-success?style=for-the-badge&logo=windows&logoColor=white" alt="Descargar Ahora" />
  </a>
</div>

> # ⚠️ REQUISITO CRÍTICO DE USO
> **PARA QUE ESTE SOFTWARE FUNCIONE CORRECTAMENTE:**
> 1.  **Motor:** Debe usar el **SECUENCIADOR AVANZADO** (Advanced Sequencer).
> 2.  **Configuración:** El nivel de log en N.I.N.A. debe estar en **"DEBUG"** o **"TRACE"**.
>     * *(Opciones > General > Nivel de Log)*
>     * *Los logs estándar ("Info") no contienen la telemetría granular necesaria.*

---

## 📄 Descripción General

**N.I.N.A. Analyzer** es una suite de diagnóstico post-sesión diseñada para astrofotógrafos que utilizan *Nighttime Imaging 'N' Astronomy*. A diferencia de los visores de logs tradicionales, este software no solo muestra datos; aplica **heurística avanzada** para determinar la salud de su tren óptico, la calidad del cielo y la seguridad de su equipo.

El software se distribuye bajo la filosofía **"Portable & Standalone"**: Un único archivo ejecutable que lleva todo incluido (motor gráfico, librerías de cálculo y manuales), sin necesidad de instalar Python ni dependencias externas.

---

## ⚡ Novedades en v27: "The Metrology Engine"

Esta actualización transforma el software de una herramienta de visualización a una plataforma de **Auditoría Forense Estricta**.

### 1. Motor de Metrología Fijo (Física Real) 📐
Se acabaron las opiniones subjetivas. El sistema ahora calcula matemáticamente si su foto es válida basándose en la física de su equipo.
* **Semáforo de 5 Niveles:** Verde (Excelencia), Amarillo (Advertencia), Naranja (Elongación), Rojo (Fallo Mecánico) y Gris (Sin Datos).
* **Cálculo:** Compara la resolución de su cámara principal ($"/px$) contra la precisión de su guiado, definiendo un umbral de tolerancia personalizado.

### 2. Cine Forense & `st.fragment` 🎬
Hemos reescrito el motor gráfico para permitir reproducción de video fluida.
* **Tecnología de Fragmentos:** Al usar el deslizador de tiempo (*Frame Scrubber*), la página ya no se recarga completa. Solo se actualiza el recuadro de la estrella.
* **Smart Downsampling:** El reproductor selecciona inteligentemente 60 cuadros clave para mostrar la evolución de eventos largos (viento, nubes) sin saturar la memoria RAM.

### 3. KPI Industrial: "Overhead" (Tiempo Muerto) ⏱️
Nueva métrica que audita la eficiencia de su hardware (USB/Disco).
* Mide el tiempo perdido entre el cierre del obturador y la escritura final en disco.
* Detecta cuellos de botella en cables USB lentos o discos duros fragmentados (> 15s).

### 4. Interfaz "Surgical Dark" 🌑
Rediseño completo de la UI con alto contraste (Texto Cian/Negro) optimizado para pantallas de observatorio nocturno, garantizando legibilidad total sin deslumbrar.

---

## 📜 Historial de Versiones

### [v25] - Arquitectura "Black Box"
Esta versión introdujo módulos de auditoría profunda para detectar ineficiencias y eventos no mapeados.

* **Módulo Experimental: Caja Negra (Black Box) 👽:**
    * Captura todas las líneas del log que el motor no reconoce (ej. nuevos drivers de rotadores).
    * Genera reportes para enviar al desarrollador.
* **Análisis de Distribución de Tiempo ⏳:**
    * Gráfico de torta (Pie Chart) para visualizar el Balance de la Noche (Imaging vs Overhead).
* **Inspector de Tareas Detallado 🔍:**
    * Gráficos independientes para Captura, Enfoque y Errores.
* **Física de Precisión (CFZ) 🔭:**
    * Cálculo exacto de la Zona Crítica de Enfoque basado en el F-Ratio del usuario.

---

## 🔬 Funcionalidades Core (Heredadas)

* **Cine Forense (Event Replay):** Reproducción animada de la estrella guía utilizando algoritmos de *Max-Pooling*.
* **Gantt Interactivo:** Línea de tiempo para navegación rápida.
* **System DNA:** Auditoría de hardware (RAM y Disco).
* **Manual Integrado:** Documentación técnica completa disponible dentro de la aplicación.

---

## 📥 Instrucciones de Instalación y Uso

Este programa es **100% Portable**. No ensucia su registro de Windows ni requiere permisos de administrador.

1.  **Descargar:** Vaya a la sección de **[Releases (Lanzamientos)](../../releases)** y baje el archivo `NINA_Analyzer_Alive_v27.exe`.
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
# 🔭 N.I.N.A. Analyzer - Precision Suite (v27)

![Version](https://img.shields.io/badge/Version-v27.0_Metrology_Engine-gold)
![Platform](https://img.shields.io/badge/Platform-Windows_Portable-blue)
![Engine](https://img.shields.io/badge/Engine-Metrology_Engine_v3-cyan)

<div align="center">
  <h3>Forensic Metrology Tool for Astrophotography</h3>
  <p><em>Transform gigabytes of session logs into Operational Intelligence.</em></p>
  
  <a href="https://github.com/IvanLizana/NINA_ANALYZER_ALIVE/releases/latest">
    <img src="https://img.shields.io/badge/DOWNLOAD_v27_EXE-Click_Here-success?style=for-the-badge&logo=windows&logoColor=white" alt="Download Now" />
  </a>
</div>

> # ⚠️ CRITICAL REQUIREMENT
> **FOR THIS SOFTWARE TO WORK CORRECTLY:**
> 1.  **Engine:** You must use the N.I.N.A. **ADVANCED SEQUENCER**.
> 2.  **Settings:** Log Level must be set to **"DEBUG"** or **"TRACE"**.
>     * *(Options > General > Log Level)*
>     * *Standard ("Info") logs lack the necessary granular telemetry.*

---

## 📄 Overview

**N.I.N.A. Analyzer** is a post-session diagnostic suite tailored for astrophotographers using *Nighttime Imaging 'N' Astronomy*. Unlike traditional log viewers, this software doesn't just display data; it applies **advanced heuristics** to determine the health of your optical train, sky quality, and equipment safety.

The software follows a **"Portable & Standalone"** philosophy: A single executable file containing everything (graphics engine, math libraries, and manuals), with no need to install Python or external dependencies.

---

## ⚡ What's New in v27: "The Metrology Engine"

This update transforms the software from a visualization tool into a **Strict Forensic Audit** platform.

### 1. Fixed Metrology Engine (Real Physics) 📐
Subjective opinions are gone. The system now mathematically calculates if your photo is valid based on your equipment's physics.
* **5-Level Traffic Light:** Green (Excellence), Yellow (Warning), Orange (Elongation), Red (Failure), and Gray (No Data).
* **Calculation:** Compares your main camera resolution ($"/px$) against your guiding precision, defining a personalized tolerance threshold.

### 2. Forensic Cinema & `st.fragment` 🎬
We rewrote the graphics engine to allow fluid video playback.
* **Fragment Technology:** Using the time slider (*Frame Scrubber*) no longer reloads the entire page. Only the star box updates.
* **Smart Downsampling:** The player intelligently selects 60 keyframes to show the evolution of long events (wind, clouds) without saturating RAM.

### 3. Industrial KPI: "Overhead" (Dead Time) ⏱️
New metric auditing your hardware efficiency (USB/Disk).
* Measures wasted time between shutter close and final disk write.
* Detects bottlenecks in slow USB cables or fragmented hard drives (> 15s).

### 4. "Surgical Dark" Interface 🌑
Complete UI redesign with high contrast (Cyan/Black text) optimized for night observatory screens, ensuring readability without dazzling.

---

## 📜 Version History

### [v25] - "Black Box" Architecture
This version introduced deep audit modules to detect inefficiencies and unmapped events.

* **Experimental Module: Black Box 👽:**
    * Captures all log lines the engine doesn't recognize.
    * Generates reports to send to the developer.
* **Time Distribution Analysis ⏳:**
    * Pie Chart to visualize Night Balance (Imaging vs Overhead).
* **Detailed Task Inspector 🔍:**
    * Independent bar charts for Imaging, Autofocus, and Errors.
* **Precision Physics (CFZ) 🔭:**
    * Exact Critical Focus Zone calculation based on F-Ratio.

---

## 🔬 Core Features (Inherited)

* **Forensic Cinema (Event Replay):** Animated playback of the guide star using *Max-Pooling* algorithms.
* **Interactive Gantt:** Timeline with quality traffic lights.
* **System DNA:** Hardware audit (RAM and Disk).
* **Integrated Manual:** Full technical documentation available within the app.

---

## 📥 Installation & Usage Instructions

This program is **100% Portable**. It does not clutter your Windows Registry nor require admin rights.

1.  **Download:** Go to the **[Releases](../../releases)** section and download `NINA_Analyzer_Alive_v27.exe`.
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
* Special thanks to **WWW.ACHAYA.CL** for the theoretical foundations.
