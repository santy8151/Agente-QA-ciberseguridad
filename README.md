# 🛡️ CyberQA Agent — Plataforma de Seguridad Informática

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-00ff88?style=for-the-badge)

> Página web de análisis de vulnerabilidades, análisis forense digital y aprendizaje en ciberseguridad.  
> Desarrollada como proyecto integrador para las materias de **Introducción a la Seguridad Informática** y **Pruebas y Calidad del Software** — CUN Bogotá 2025.

---

## 📋 Tabla de Contenidos

- [Descripción](#-descripción)
- [Demo](#-demo)
- [Características](#-características)
- [Tecnologías](#-tecnologías)
- [Estructura del proyecto](#-estructura-del-proyecto)
- [Instalación y uso](#-instalación-y-uso)
- [Secciones de la aplicación](#-secciones-de-la-aplicación)
- [Herramientas integradas](#-herramientas-integradas)
- [Cursos y recursos](#-cursos-y-recursos)
- [Autor](#-autor)

---

## 📌 Descripción

**CyberQA Agent** es una plataforma web estática de una sola página (`index.html`) que centraliza herramientas, recursos y conocimiento de ciberseguridad para estudiantes y profesionales. Su propósito es funcionar como panel de control de seguridad informática con accesos rápidos a las herramientas más importantes del sector.

El proyecto nació de la idea de combinar dos materias:

- 🔐 **Introducción a la Seguridad Informática** → análisis de vulnerabilidades OWASP, escaneo de red, herramientas forenses
- 🧪 **Pruebas y Calidad del Software (QA)** → testing de aplicaciones web, análisis de vulnerabilidades como proceso de QA

---

## 🌐 Demo

```
Abre el archivo cyberqa_final.html directamente en tu navegador.
No requiere servidor ni instalación.
```

> Para publicarlo online: arrastra el archivo a **[Netlify Drop](https://app.netlify.com/drop)** y obtienes una URL pública en segundos.

---

## ✨ Características

| Característica | Descripción |
|---|---|
| 🦠 Escaneo de virus | Acceso directo a VirusTotal (70+ motores antivirus) |
| 🌐 Recrear red | Herramienta online Draw.io para diagramar topología de red |
| ⚡ Acceso Cisco | Links directos a Cisco.com, NetAcad, Learning y Advisories |
| 🔍 Escaneo OWASP | Análisis de vulnerabilidades con HostedScan |
| 🌍 Shodan | Motor de búsqueda para dispositivos IoT expuestos |
| 🔓 HaveIBeenPwned | Verificación de filtraciones de datos |
| 🌐 Monitor de red | Detección de IP pública, subred, broadcast y rango de hosts |
| 🛡️ OWASP Top 10 | Tabla completa de vulnerabilidades web más críticas 2021 |
| 🔬 Herramientas forenses | 8 herramientas profesionales con descripción y enlaces |
| 🎓 Centro de cursos | 4 cursos con video: Kali Linux, GPG, Cisco NetAcad, TryHackMe |
| 🔐 Banner de criptografía | Recurso destacado con link a video tutorial |
| 🖥️ Terminal animado | Muestra resultados de detección de red en tiempo real |

---

## 🛠️ Tecnologías

- **HTML5** — estructura semántica
- **CSS3** — estilos con variables CSS, animaciones y diseño responsivo
- **JavaScript (Vanilla)** — lógica de detección de red, reloj en tiempo real, terminal
- **Google Fonts** — tipografías `Share Tech Mono`, `Rajdhani`, `Orbitron`
- **ipapi.co API** — detección de IP pública e información de red (gratuita, sin key)
- **Sin frameworks, sin dependencias externas** — funciona offline excepto fuentes e IP

---

## 📁 Estructura del proyecto

```
cyberqa-agent/
│
├── cyberqa_final.html      # Aplicación completa (archivo único)
├── README.md               # Este archivo
└── LICENSE                 # Licencia MIT
```

> El proyecto es un **single-file app** — toda la lógica, estilos y estructura están en un solo archivo HTML. Ideal para despliegue estático sin configuración.

---

## 🚀 Instalación y uso

### Opción 1 — Abrir localmente

```bash
# Clona el repositorio
git clone https://github.com/tu-usuario/cyberqa-agent.git

# Entra al directorio
cd cyberqa-agent

# Abre en el navegador (doble clic o desde terminal)
open cyberqa_final.html         # macOS
start cyberqa_final.html        # Windows
xdg-open cyberqa_final.html     # Linux
```

### Opción 2 — Servidor local (recomendado para IP real)

```bash
# Con Python
python -m http.server 8080

# Con Node.js
npx serve .

# Luego abre: http://localhost:8080/cyberqa_final.html
```

### Opción 3 — Netlify (publicación en la nube)

1. Ve a [app.netlify.com/drop](https://app.netlify.com/drop)
2. Arrastra el archivo `cyberqa_final.html`
3. ¡Obtienes una URL pública en menos de 30 segundos!

---

## 📂 Secciones de la aplicación

### 1️⃣ Hero / Inicio
Presentación del proyecto con botones de acción rápida hacia las secciones principales.

### 2️⃣ 🔐 Banner de Criptografía
Recurso destacado con botón directo a tutorial de cifrado de archivos y contraseñas con GPG y VeraCrypt.

### 3️⃣ ⚡ Centro de Acciones Rápidas
Seis tarjetas con acceso directo a:
- **VirusTotal** — escaneo de virus y malware
- **Draw.io** — recrear topología de red online
- **Cisco.com** — portal oficial
- **HostedScan OWASP** — análisis de vulnerabilidades web
- **Shodan** — búsqueda de dispositivos IoT
- **HaveIBeenPwned** — verificar filtraciones

### 4️⃣ 🌐 Monitor de Red en Vivo
Detecta automáticamente:
- IP pública del usuario
- ISP / Proveedor de internet
- País y ciudad
- Subred calculada (`x.x.x.0/24`)
- Dirección broadcast
- Rango de hosts disponibles
- Terminal animado con resultados en tiempo real

### 5️⃣ ⚡ Panel de Acceso Cisco
Botones directos a Cisco.com, Cisco Learning, NetAcad, y el escáner OWASP, más links a recursos técnicos de Cisco.

### 6️⃣ 🛡️ OWASP Top 10
Tabla completa con las 10 vulnerabilidades web más críticas según el estándar OWASP 2021, con nivel de riesgo (ALTO / MEDIO / BAJO), descripción y vector de ataque.

### 7️⃣ 🔬 Herramientas de Análisis Forense
8 herramientas profesionales con descripción, categoría y enlace de descarga:

| Herramienta | Tipo | Uso |
|---|---|---|
| Autopsy | Forense | Análisis de discos y archivos |
| Wireshark | Red | Captura de tráfico |
| Nmap | Red | Escaneo de puertos |
| Burp Suite | Web | Pentesting de aplicaciones |
| Metasploit | Pentesting | Framework de exploits |
| Volatility | Forense | Análisis de memoria RAM |
| Hashcat | Contraseñas | Auditoría de hashes |
| The Sleuth Kit | Forense | Análisis de sistemas de archivos |

### 8️⃣ 🎓 Centro de Aprendizaje
4 recursos educativos seleccionados:

| Curso | Plataforma | Nivel |
|---|---|---|
| Instalar Kali Linux | YouTube | Principiante |
| GPG y VeraCrypt (criptografía) | YouTube | Intermedio |
| Fundamentos de Redes Cisco | NetAcad | Principiante |
| TryHackMe — Práctica CTF | TryHackMe.com | Todos los niveles |

---

## 🔗 Herramientas integradas

```
VirusTotal          → https://www.virustotal.com
Draw.io             → https://app.diagrams.net
Cisco               → https://www.cisco.com
NetAcad             → https://www.netacad.com
HostedScan OWASP    → https://hostedscan.com/owasp-vulnerability-scan
Shodan              → https://www.shodan.io
HaveIBeenPwned      → https://haveibeenpwned.com
Nmap                → https://nmap.org
Wireshark           → https://www.wireshark.org
Autopsy             → https://www.autopsy.com
Burp Suite          → https://portswigger.net/burp
Metasploit          → https://www.metasploit.com
TryHackMe           → https://tryhackme.com
```

---

## 📡 API utilizada

| API | URL | Uso | Key requerida |
|---|---|---|---|
| ipapi.co | `https://ipapi.co/json/` | Detección de IP, país, ISP | ❌ No |

---

## 🎯 Relación con las materias

### Introducción a la Seguridad Informática
- Implementación del OWASP Top 10
- Uso de herramientas de análisis forense (Autopsy, Wireshark, Volatility)
- Escaneo de vulnerabilidades con HostedScan
- Monitoreo de red y análisis de subred

### Pruebas y Calidad del Software (QA)
- La plataforma en sí es un **artefacto QA** — centraliza herramientas de testing de seguridad
- Cada herramienta integrada representa un tipo de prueba: análisis estático, dinámico, de red, forense
- El escaneo OWASP es un proceso de **QA de seguridad** aplicado a aplicaciones web

---

## 📄 Licencia

Este proyecto está bajo la licencia **MIT** — puedes usarlo, modificarlo y distribuirlo libremente dando crédito al autor.

```
MIT License — Copyright (c) 2025 Santiago — ITM
```

---

<div align="center">

**🛡️ CyberQA Agent** 

</div>
