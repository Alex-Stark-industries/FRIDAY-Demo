# FRIDAY Demo — un chatbot y agente de voz gratuito, todo en local

🌐 [English](README.md) · [Italiano](README.it.md) · **Español** · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [हिन्दी](README.hi.md)

[![Descargar](https://img.shields.io/badge/Descargar-%C3%9Altima%20versi%C3%B3n-e91e63?logo=github)](../../releases/latest)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-2ea44f)](LICENSE)
[![Plataforma](https://img.shields.io/badge/Windows-10%20%2F%2011-0078D6?logo=windows)](../../releases/latest)

**Un chatbot y asistente de voz con IA, gratuito, que se ejecuta por completo en
tu propio ordenador.** Escribe o habla — Friday responde por texto y también en
voz alta, con una voz que eliges tú — **sin cuenta, sin clave de API, sin
suscripción, sin nube y sin telemetría.** Nada de lo que dices se envía a ningún
servidor: el modelo se ejecuta en local con [Ollama](https://ollama.com), y la
voz funciona en el dispositivo.

> **Local. Privado. Gratis.** Descarga el instalador, ejecútalo y empieza a
> hablar. Friday responde en **inglés**.

Esto es una muestra gratuita del asistente de escritorio **Friday**, más
completo. Conserva solo dos cosas — el **chat** y el **modo de voz avanzado** — y
nada más.

---

### Lo esencial

- 💬 **Chat** — un modelo de lenguaje local mediante [Ollama](https://ollama.com), con la respuesta apareciendo palabra por palabra.
- 🎙️ **Modo de voz avanzado** — una esfera de partículas a pantalla completa, con manos libres y detección neuronal del turno de habla. Mantén pulsado **Espacio** o toca el micrófono; ella escucha, piensa y te responde en voz alta.
- 🔊 **Seis voces en el dispositivo** — elige la que prefieras en la cabecera. El audio nunca sale de tu máquina.
- 💾 **Sesiones guardadas** — tus conversaciones anteriores se guardan en local y se pueden recargar.
- 🌐 **Voz totalmente sin conexión** — el motor de voz (Kokoro) y el entorno de ejecución vienen incluidos; solo la descarga única de los modelos de voz y tus mensajes hacia tu propio Ollama pasan por la red.
- 🇬🇧 **Siempre en inglés** — escribas o digas lo que escribas, Friday responde en inglés.

---

### Capturas

<table>
<tr>
<td width="50%">

**Chat** — el núcleo neuronal, los diagnósticos en vivo y una conversación en streaming con el modelo local.
<img src="docs/screenshots/chat.png" alt="Interfaz de chat de Friday Demo" width="100%">

</td>
<td width="50%">

**Modo de voz avanzado** — una esfera reactiva a pantalla completa con detección neuronal del micrófono; mantén pulsado Espacio o toca para hablar.
<img src="docs/screenshots/voice.png" alt="Modo de voz avanzado de Friday Demo" width="100%">

</td>
</tr>
</table>

---

### Descarga e instalación

1. Abre la página de [**Releases**](../../releases/latest) y descarga
   `Friday-Voice-Agent-Setup-<versión>.exe`.
2. Ejecútalo. El instalador es **por usuario** — **no requiere permisos de
   administrador**.
3. Inicia **Friday Voice Agent** desde el menú Inicio (o el acceso directo del
   escritorio, si lo solicitaste).

> **Primer inicio:** el instalador no está firmado digitalmente, así que Windows
> SmartScreen puede mostrar *"Windows protegió su PC"*. Haz clic en **Más
> información → Ejecutar de todas formas**. Es normal en las apps gratuitas e
> independientes.

¿Es tu primera vez? La [**Guía de bienvenida e instalación**](WELCOME.es.md) te
acompaña paso a paso sin dar nada por sentado.

### Configuración inicial (obligatoria)

El "cerebro" de Friday se ejecuta en local mediante **Ollama**, un motor de IA
local y gratuito:

1. Instala [Ollama](https://ollama.com).
2. Descarga el modelo una vez, en una terminal:
   ```
   ollama pull qwen2.5:3b
   ```
3. Asegúrate de que Ollama esté en ejecución y luego inicia Friday.

La primera vez que abras la voz, se descargan una sola vez los modelos de voz
(unos cientos de MB); después funciona para siempre sin conexión.

---

### Documentación

| Documento | De qué trata |
|---|---|
| [Bienvenida e instalación](WELCOME.es.md) | Para principiantes, paso a paso: instalar, iniciar, primer chat, primera voz |
| [Changelog](CHANGELOG.md) | Qué cambió en cada versión (en inglés) |
| [Licencia](LICENSE) | MIT — uso libre |

---

### Requisitos del sistema

Friday ejecuta el modelo de IA y la voz **en tu propia máquina**, así que el
resultado depende de tu PC. Estos son los mínimos realistas para el modelo
incluido `qwen2.5:3b`.

| | Mínimo | Recomendado |
|---|---|---|
| **Sistema operativo** | Windows 10 / 11, 64 bits | Windows 11, 64 bits |
| **CPU** | Cualquier procesador moderno de 64 bits (x64) | CPU multinúcleo reciente |
| **RAM** | 8 GB | 16 GB |
| **Espacio libre** | ~4 GB (app ≈0,5 GB · modelo ≈2 GB · modelos de voz ≈0,5 GB) | 6 GB+ |
| **GPU** | Ninguna — se ejecuta en CPU (voz más lenta) | Una GPU con soporte **WebGPU** (NVIDIA / AMD / Intel recientes) para una voz ágil |
| **Internet** | Solo para la configuración inicial (Ollama, modelo, primera descarga de voz) | — |

- **[Ollama](https://ollama.com)** debe estar en ejecución en local con
  `qwen2.5:3b` descargado (`ollama pull qwen2.5:3b`).
- Todo lo demás — chat y voz — funciona sin conexión una vez configurado.
- Con menos RAM o sin GPU, Friday sigue funcionando; las respuestas y la voz solo
  tardan más.

---

### Privacidad de un vistazo

- **Sin cuentas, sin claves de API, sin telemetría, sin analíticas, sin
  actualizaciones automáticas.**
- El modelo de lenguaje se ejecuta **en tu propia máquina** mediante Ollama.
- La voz (reconocimiento y síntesis de voz) se ejecuta **en el dispositivo**.
- El único uso de la red es la descarga única de los modelos de voz y tus propios
  mensajes yendo a Ollama en tu propio ordenador.

---

### Licencia

MIT — uso libre. Consulta [LICENSE](LICENSE). El producto **Friday** completo del
que esto es una vista previa es una aplicación separada y propietaria.
