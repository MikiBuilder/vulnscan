# ⚡ VulnScan — Escáner de Vulnerabilidades con IA

Herramienta de análisis estático de seguridad potenciada por Claude AI. Detecta vulnerabilidades línea a línea en cualquier lenguaje de programación, directamente en el navegador, sin instalación ni servidor.

**[→ Ver demo en vivo](https://mikibuilder.github.io/vulnscan)**

---

## ✨ Características

- 🔍 **Autodetección de lenguaje** — Identifica automáticamente Python, JavaScript, TypeScript, PHP, SQL, Java, Go, Ruby, Bash, C# y más
- 📌 **Análisis línea a línea** — Cada vulnerabilidad se anota directamente sobre el código con descripción y sugerencia de fix
- ⚡ **Powered by Claude AI** — Análisis semántico real, no solo patrones regex
- 🛡 **Múltiples categorías** — SQL Injection, XSS, Secretos expuestos, Dependencias inseguras y más según el lenguaje
- 🎯 **3 niveles de severidad** — Crítico, Alto, Medio con código de colores
- 💻 **Sin backend** — 100% frontend, desplegable en GitHub Pages sin coste
- 🖥 **Estética terminal** — Diseño inspirado en herramientas de seguridad reales

## 🕵️ Vulnerabilidades detectadas

| Categoría | Ejemplos |
|---|---|
| **SQL Injection** | Queries con concatenación de strings, sin parámetros |
| **XSS** | Output HTML con input de usuario sin sanitizar |
| **Secretos expuestos** | API keys, passwords, tokens hardcodeados |
| **Dependencias inseguras** | `pickle`, `eval`, `unserialize`, `innerHTML`, `system()` |
| **Command Injection** | Ejecución de comandos con input externo |
| **Path Traversal** | Acceso a ficheros sin validar la ruta |
| **Insecure Deserialization** | Deserialización de datos no confiables |

## 🌐 Lenguajes soportados

Python · JavaScript · TypeScript · PHP · SQL · Java · Go · Ruby · Bash · C# · y más

## 🚀 Uso rápido

```bash
git clone https://github.com/mikibuilder/vulnscan.git
cd vulnscan
open index.html
```

No necesita servidor ni instalación. Abre `index.html` directamente en el navegador.

### GitHub Pages

1. **Settings → Pages → Source:** `main / root`
2. Disponible en `https://mikibuilder.github.io/vulnscan`

## 🗂 Estructura

```
vulnscan/
├── index.html    # App completa (single file, sin dependencias)
└── README.md
```

## ⚙️ Cómo funciona

1. Pega tu código o carga uno de los ejemplos incluidos
2. VulnScan detecta el lenguaje automáticamente mientras escribes
3. Al pulsar **Iniciar escaneo**, Claude AI analiza el código semánticamente
4. El resultado se muestra como código anotado — haz clic en cualquier línea marcada para ver el detalle y el fix sugerido

## 🧩 Tecnologías

- **Vanilla JS** — Sin frameworks ni dependencias
- **Claude API** (`claude-sonnet-4-20250514`) — Análisis de vulnerabilidades
- **Google Fonts** — JetBrains Mono + Orbitron
- **CSS animations** — Scanline, progress bar, anotaciones interactivas

## ⚠️ Aviso legal

Esta herramienta es orientativa y educativa. Los resultados deben ser validados por un profesional de seguridad. No reemplaza una auditoría formal (SAST/DAST). El código analizado no se almacena en ningún servidor.

## 📄 Licencia

MIT — Úsalo, fórkalo, mejóralo.
