<div align="center">
  <p>
    <strong>
      <a href="#-english-version">🇬🇧 READ IN ENGLISH</a>
      &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
      <a href="#-versión-en-español">🇪🇸 LEER EN ESPAÑOL</a>
    </strong>
  </p>
</div>

---

<a name="-english-version"></a>
# 🔭 N.I.N.A. Analyzer (Precision Edition)

**Powered by ASTROREMOTO**

![Platform](https://img.shields.io/badge/Platform-Windows-blue)
![License](https://img.shields.io/badge/License-Freeware-green)
![Status](https://img.shields.io/badge/Version-20.0_Gold-gold)

**Precision metrology tool for N.I.N.A. astrophotography logs.**

This application analyzes your session logs to calculate the **True RMS (Root Mean Square)** guiding error, performs forensic diagnosis of your guide star (using PHD2 data), and displays real-time efficiency metrics. Designed with a "Deep Dark" interface to preserve your night vision inside the observatory.

> **Note:** This is a standalone portable application. No installation or Python knowledge is required.

## 🚀 Key Features

### 1. Precision Metrology (RMS)
Calculates the **True RMS** error for every single exposure based on raw guiding pulses. Features an **Auto-Centering Statistical Engine** to show the true mechanical performance of your mount, eliminating calibration bias.

### 2. The "PHD2 Doctor" (Star Diagnosis)
Performs data mining on the logs to reconstruct what the guide camera saw:
* **Bullseye:** Animated playback of guide star deviation with crosshair reference.
* **Heatmap:** Analysis of star morphology (roundness/elongation).
* **Scatter Cloud:** Total session drift analysis.

### 3. Smart Gantt Timeline
A detailed timeline with a **Dual-Track System**:
* **Top Track:** Visual Quality (Star roundness/elongation).
* **Bottom Track:** Mechanical Precision (RMS value).

### 4. Real-Time Monitoring (Live Mode)
* **Auto-detects** the active log file in the N.I.N.A directory.
* **Auto-refresh** (configurable interval) to act as a secondary monitor.

---

## ⚠️ Important Prerequisite

To unlock the advanced metrology and star diagnosis features, **N.I.N.A. must be configured to save detailed logs.**

1.  Go to **N.I.N.A. > Options > General**.
2.  Set **Log Level** to **`DEBUG`**.

> *Without `DEBUG` level, the app will only show basic timing KPIs, but star reconstruction and RMS calculations will be unavailable.*

---

## 📥 Download & Usage

This software is distributed as a **single portable executable** (`.exe`).

1.  **Download** the latest release (`.zip`) from the **[Releases](../../releases)** section (on the right sidebar).
2.  **Unzip** the folder to a location of your choice.
3.  **Run** `nina_analyzer_alive_v20.exe`.

*The application includes an integrated **Reference Manual** accessible via the sidebar.*

### Note on Windows Security
Since this application is not digitally signed with a corporate certificate, Windows Defender or SmartScreen might display a warning ("Unknown Publisher"). This is normal for independent open-source software. You can safely click **"More Info" -> "Run Anyway"**.

---

## 📸 Screenshots

### Dashboard & KPIs
*(Place your screenshot here)*

### Precision Timeline (Smart Gantt)
*(Place your screenshot here)*

---

## 🤝 Acknowledgments

* Developed by **Ivan Lizana (ASTROREMOTO)**.
* Special thanks to **ACHAYA** (Chilean Association of Astronomy and Astronautics) for the knowledge and support.
* Dedicated to the astrophotography community.

**Clear Skies!** 🔭

<br>
<br>
<br>
<div align="center">--- 🇪🇸 ---</div>
<br>
<br>

<a name="-versión-en-español"></a>
# 🔭 Versión en Español

**Desarrollado por ASTROREMOTO**

![Plataforma](https://img.shields.io/badge/Plataforma-Windows-blue)
![Licencia](https://img.shields.io/badge/Licencia-Freeware-green)
![Estado](https://img.shields.io/badge/Versión-20.0_Gold-gold)

**Herramienta de metrología de precisión para logs de astrofotografía de N.I.N.A.**

Esta aplicación analiza los registros de tu sesión para calcular el error de guiado **RMS Real (Root Mean Square)**, realiza un diagnóstico forense de tu estrella guía (utilizando datos de PHD2) y muestra métricas de eficiencia en tiempo real. Diseñada con una interfaz "Deep Dark" para preservar tu visión nocturna dentro del observatorio.

> **Nota:** Es una aplicación portátil independiente. No requiere instalación ni conocimientos de Python.

---

## 🚀 Características Principales

### 1. Metrología de Precisión (RMS)
Calcula el error **RMS Real** para cada exposición basándose en los pulsos de guiado crudos. Cuenta con un **Motor Estadístico de Auto-Centrado** para mostrar el verdadero rendimiento mecánico de tu montura, eliminando el sesgo de calibración.

### 2. El "Doctor PHD2" (Diagnóstico Estelar)
Realiza minería de datos en los logs para reconstruir lo que vio la cámara guía:
* **Diana (Bullseye):** Reproducción animada de la desviación de la estrella con retícula central.
* **Mapa de Calor:** Análisis de la morfología de la estrella (redondez/elongación).
* **Nube de Dispersión:** Análisis de la deriva total de la sesión.

### 3. Cronología Inteligente (Smart Gantt)
Una línea de tiempo detallada con un **Sistema de Doble Pista**:
* **Pista Superior:** Calidad Visual (Redondez/Elongación de la estrella).
* **Pista Inferior:** Precisión Mecánica (Valor RMS numérico).

### 4. Monitoreo en Tiempo Real (Modo Live)
* **Auto-detecta** el archivo de log activo en el directorio de N.I.N.A.
* **Auto-refresco** (intervalo configurable) para actuar como un monitor secundario dentro del observatorio.

---

## ⚠️ Prerrequisito Importante

Para desbloquear la metrología avanzada y el diagnóstico estelar, **N.I.N.A. debe estar configurado para guardar logs detallados.**

1.  Ve a **N.I.N.A. > Opciones > General**.
2.  Configura el **Nivel de Registro (Log Level)** en **`DEBUG`**.

> *Sin el nivel `DEBUG`, la aplicación solo mostrará KPIs básicos de tiempo, pero la reconstrucción de estrellas y los cálculos RMS no estarán disponibles.*

---

## 📥 Descarga y Uso

Este software se distribuye como un **ejecutable portátil único** (`.exe`).

1.  **Descarga** la última versión (`.zip`) desde la sección **[Releases](../../releases)** (en la barra lateral derecha).
2.  **Descomprime** la carpeta en la ubicación que prefieras.
3.  **Ejecuta** `nina_analyzer_alive_v20.exe`.

*La aplicación incluye un **Manual de Referencia** integrado accesible desde la barra lateral.*

### Nota sobre Seguridad de Windows
Dado que esta aplicación no está firmada digitalmente con un certificado corporativo costoso, Windows Defender o SmartScreen pueden mostrar una advertencia ("Editor Desconocido"). Esto es normal para software de código abierto independiente. Puedes hacer clic con seguridad en **"Más información" -> "Ejecutar de todos modos"**.

---

## 📸 Capturas de Pantalla

### Panel de Control y KPIs
*(Inserta tu captura aquí)*

### Cronología de Precisión
*(Inserta tu captura aquí)*

---

## 🤝 Agradecimientos

* Desarrollado por **Iván Lizana (ASTROREMOTO)**.
* Agradecimientos especiales a **ACHAYA** (Asociación Chilena de Astronomía y Astronáutica) por el conocimiento y apoyo.
* Dedicado a la comunidad de astrofotografía.

**¡Cielos Despejados!** 🔭
