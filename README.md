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
# 🔭 N.I.N.A. Analyzer - Precision Suite (v24)

![Versión](https://img.shields.io/badge/Versión-v24.0_Gold-gold)
![Plataforma](https://img.shields.io/badge/Plataforma-Windows_Portable-blue)
![Motor](https://img.shields.io/badge/Motor-Deep_Freeze-cyan)
![Licencia](https://img.shields.io/badge/Licencia-Freeware-green)

<div align="center">
  <h3>Herramienta de Metrología Forense para Astrofotografía</h3>
  <p><em>Transforme gigabytes de logs de sesión en Inteligencia Operativa.</em></p>
  
  <a href="https://github.com/IvanLizana/NINA_ANALYZER_ALIVE/releases/latest">
    <img src="https://img.shields.io/badge/DESCARGAR_EXE_v24-Clic_Aquí-success?style=for-the-badge&logo=windows&logoColor=white" alt="Descargar Ahora" />
  </a>
</div>

## 📄 Descripción General

**N.I.N.A. Analyzer** es una suite de diagnóstico post-sesión diseñada para astrofotógrafos que utilizan *Nighttime Imaging 'N' Astronomy*. A diferencia de los visores de logs tradicionales, este software no solo muestra datos; aplica **heurística avanzada** para determinar la salud de su tren óptico, la calidad del cielo y la seguridad de su equipo.

El software se distribuye bajo la filosofía **"Portable & Standalone"**: Un único archivo ejecutable que lleva todo incluido (motor gráfico, librerías de cálculo y manuales), sin necesidad de instalar Python ni dependencias externas.

---

## ⚡ Tecnología v24: El Motor "Deep Freeze"

La versión 24 introduce un cambio radical en la arquitectura del software para manejar sesiones masivas (miles de subs) sin latencia.

* **Persistencia de Memoria:** Los gráficos vectoriales complejos (Cronologías, Análisis de Deriva) se calculan una sola vez y se "congelan" en la memoria RAM.
* **Navegación Instantánea:** Puede saltar entre el *Inspector de Enfoque*, el *Análisis de Ciclos* y el *Reporte de Seguridad* sin tiempos de carga ni parpadeos de pantalla.
* **Interfaz Nativa:** Hemos reemplazado los cargadores web lentos por integración directa con **Windows API**. Ahora puede abrir carpetas de logs de cualquier tamaño usando el explorador de archivos nativo del sistema.

---

## 🔬 Metrología y Ciencia (Lo Nuevo)

Esta versión va más allá de mostrar gráficos bonitos. Aplica fórmulas ópticas para decirle **por qué** falló una subexposición.

### 1. El Analizador de Ciclos (Heurística Ambiental)
El software segmenta la noche basándose en los eventos de Auto-Enfoque y clasifica automáticamente qué está ocurriendo con su equipo:

* 🟢 **Estabilidad Térmica:** Detecta cuando el HFR se mantiene plano (pendiente $\approx$ 0). Su equipo está en equilibrio.
* ❄️ **Deriva Térmica (Thermal Drift):** Identifica una pendiente lineal positiva en el HFR. Diagnóstico: Su tubo óptico se está contrayendo por el frío.
* ☁️ **Detección de Nubes:** Si el conteo de estrellas cae por debajo del **Percentil 15 (P15)** histórico de la sesión, marca el ciclo como "Interferencia Atmosférica".
* 🌊 **Turbulencia (Seeing):** Si el promedio de HFR es estable pero la desviación estándar ($\sigma$) es alta, diagnostica mal *seeing* local.

### 2. Zona Crítica de Enfoque (CFZ)
El software lee la distancia focal y la relación focal de su telescopio para calcular su **Límite de Difracción Teórico**.
> *¿Realmente necesitaba reenfocar o fue solo una ráfaga de viento?*
La línea de CFZ en los gráficos le dará la respuesta definitiva.

### 3. Auditoría de Seguridad
Un nuevo panel forense al final del reporte verifica cómo terminó la sesión:
* ¿Confirmó la montura el estado "Parked"?
* ¿Se enviaron los comandos de cierre de cúpula/obturador?
* ¿Se calentó la cámara antes de desconectar?

---

## 📥 Instrucciones de Instalación y Uso

Este programa es **100% Portable**. No ensucia su registro de Windows ni requiere permisos de administrador.

1.  **Descargar:** Vaya a la sección de **[Releases (Lanzamientos)](../../releases)** y baje el archivo `NINA_Analyzer_Alive_v24.exe`.
2.  **Ubicación:** Guarde el archivo donde quiera (Escritorio, Documentos, USB).
3.  **Ejecutar:** Abra el archivo.
    * *Aparecerá una consola negra por unos segundos (es el motor Deep Freeze cargando).*
    * *Luego se abrirá la interfaz en su navegador predeterminado.*
4.  **Cargar Datos:** Use el botón "Browse Folder" para seleccionar su carpeta de Logs de N.I.N.A.

> **⚠️ Nota sobre Windows Defender:**
> Al ser un software gratuito desarrollado por un **astrofotógrafo aficionado** (y no por una corporación), Windows puede mostrar una pantalla azul indicando "Editor Desconocido".
> * Esto es normal. Haga clic en **"Más información"** y luego en **"Ejecutar de todas formas"**.

---

## 📚 Documentación Integrada
No necesita descargar PDFs aparte. El **Manual de Referencia Técnica v24** está digitalizado e incrustado dentro de la propia aplicación. Puede consultarlo en la pestaña "Manual" mientras analiza sus datos.

---
---

<a name="-english-official-documentation"></a>
# 🔭 N.I.N.A. Analyzer - Precision Suite (v24)

![Version](https://img.shields.io/badge/Version-v24.0_Gold-gold)
![Platform](https://img.shields.io/badge/Platform-Windows_Portable-blue)
![Engine](https://img.shields.io/badge/Engine-Deep_Freeze-cyan)

<div align="center">
  <h3>Forensic Metrology Tool for Astrophotography</h3>
  <p><em>Transform gigabytes of session logs into Operational Intelligence.</em></p>
  
  <a href="https://github.com/IvanLizana/NINA_ANALYZER_ALIVE/releases/latest">
    <img src="https://img.shields.io/badge/DOWNLOAD_v24_EXE-Click_Here-success?style=for-the-badge&logo=windows&logoColor=white" alt="Download Now" />
  </a>
</div>

## 📄 Overview

**N.I.N.A. Analyzer** is a post-session diagnostic suite tailored for astrophotographers using *Nighttime Imaging 'N' Astronomy*. Unlike traditional log viewers, this software doesn't just display data; it applies **advanced heuristics** to determine the health of your optical train, sky quality, and equipment safety.

The software follows a **"Portable & Standalone"** philosophy: A single executable file containing everything (graphics engine, math libraries, and manuals), with no need to install Python or external dependencies.

---

## ⚡ v24 Technology: The "Deep Freeze" Engine

Version 24 introduces a radical architecture change to handle massive sessions (thousands of subs) with zero latency.

* **Memory Persistence:** Complex vector charts (Timelines, Drift Analysis) are calculated once and "frozen" in RAM.
* **Instant Navigation:** Jump between the *Focus Inspector*, *Cycle Analysis*, and *Security Report* with no loading times or screen flickering.
* **Native Integration:** We replaced slow web uploaders with direct **Windows API** integration. You can now open log folders of any size using the system's native file explorer.

---

## 🔬 Metrology & Science (New Features)

This version goes beyond pretty charts. It uses optical formulas to tell you **why** a sub-exposure failed.

### 1. The Cycle Analyzer (Environmental Heuristics)
The software segments the night based on Auto-Focus events and automatically classifies what is happening with your gear:

* 🟢 **Thermal Stability:** Detects when HFR remains flat (slope $\approx$ 0). Your rig is in equilibrium.
* ❄️ **Thermal Drift:** Identifies a positive linear slope in HFR. Diagnosis: Your optical tube is contracting due to cold.
* ☁️ **Cloud Detection:** If the Star Count drops below the historical **15th Percentile (P15)** of the session, the cycle is flagged as "Atmospheric Interference".
* 🌊 **Turbulence (Seeing):** If the average HFR is stable but the Standard Deviation ($\sigma$) is high, it diagnoses poor local seeing.

### 2. Critical Focus Zone (CFZ)
The software reads your telescope's focal length and focal ratio to calculate its **Theoretical Diffraction Limit**.
> *Did you really need to refocus, or was it just a wind gust?*
The CFZ line on the charts will give you the definitive answer.

### 3. Security Audit
A new forensic panel at the end of the report verifies how the session ended:
* Did the mount confirm the "Parked" status?
* Were the dome/shutter close commands sent?
* Did the camera warm up before disconnecting?

---

## 📥 Installation & Usage Instructions

This program is **100% Portable**. It does not clutter your Windows Registry nor require admin rights.

1.  **Download:** Go to the **[Releases](../../releases)** section and download `NINA_Analyzer_Alive_v24.exe`.
2.  **Location:** Save the file anywhere (Desktop, Documents, USB drive).
3.  **Run:** Open the file.
    * *A black console window will appear for a few seconds (this is the Deep Freeze engine loading).*
    * *Then, the interface will launch in your default web browser.*
4.  **Load Data:** Use the "Browse Folder" button to select your N.I.N.A. Logs folder.

> **⚠️ Note on Windows Defender:**
> Since this is free software developed by an **amateur astrophotographer** (and not a corporation), Windows might show a blue screen saying "Unknown Publisher".
> * This is normal. Click **"More Info"** and then **"Run Anyway"**.

---

## 🤝 Credits / Créditos
* **Developer:** Iván Lizana (ASTROREMOTO).
* **Tech Stack:** Python 3.13 + Streamlit + Plotly + Pandas.
* Special thanks to **ACHAYA** for the theoretical foundations.
