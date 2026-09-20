# Bienvenido a Friday 👋

🌐 [English](../WELCOME.md) · [Italiano](WELCOME.it.md) · **Español** · [Français](WELCOME.fr.md) · [Deutsch](WELCOME.de.md) · [Português](WELCOME.pt.md) · [हिन्दी](WELCOME.hi.md)

Esta guía te lleva de cero a hablar con Friday, sin dar **nada** por sentado. Si
sabes descargar un archivo, sabes iniciar Friday.

Friday es un asistente de IA gratuito que se ejecuta en **tu propio ordenador**.
Puedes **escribirle** o **hablarle**, y responde — por texto y en voz alta. No
necesita cuenta, ni registro, ni suscripción de pago. Friday responde en
**inglés**.

---

## Qué necesitas

- Un PC con **Windows 10 u 11** (64 bits).
- **8 GB de RAM** o más (16 GB van cómodos). Friday ejecuta la IA en tu propia
  máquina, así que la memoria importa.
- Alrededor de **4 GB de espacio libre** en disco en total: la app en sí
  (~0,5 GB), el modelo de IA que descargas una vez (~2 GB) y los modelos de voz
  descargados en el primer uso de la voz (~0,5 GB).
- Una conexión a internet **solo para la configuración** — una vez configurado, el
  chat y la voz funcionan sin conexión.

Una tarjeta gráfica (GPU) con soporte **WebGPU** (cualquier GPU NVIDIA, AMD o
Intel reciente) hace que la voz sea rápida — pero Friday también funciona sin
ella, solo más lento. En un PC de gama baja todo sigue funcionando; las
respuestas y la voz simplemente tardan un poco más.

> ¿No conoces las características de tu PC? Pulsa la **tecla Windows**, escribe
> **"Acerca de tu PC"** y ábrelo — muestra la versión de Windows, el procesador y
> la RAM instalada.

---

## Paso 1 — Instala Ollama (el cerebro de Friday)

Friday piensa usando un motor de IA local y gratuito llamado **Ollama**. Se
instala una sola vez.

1. Ve a **https://ollama.com** y haz clic en **Download**.
2. Ejecuta el instalador que descargaste y sigue las indicaciones. Listo — ahora
   Ollama se ejecuta discretamente en segundo plano.
3. Abre una terminal (pulsa la **tecla Windows**, escribe **`cmd`**, pulsa
   **Enter**) y pega esta línea, luego pulsa **Enter**:

   ```
   ollama pull qwen2.5:3b
   ```

   Esto descarga el modelo de IA que usa Friday (unos 2 GB). Espera a que
   termine — solo lo haces una vez.

> **¿Cómo sé si Ollama está en ejecución?** Tras instalarlo, busca el icono de
> Ollama cerca del reloj en la barra de tareas. Si no lo ves, abre el menú Inicio
> e inicia **Ollama**.

---

## Paso 2 — Descarga Friday

1. Ve a la página de [**Releases**](https://github.com/Alex-Stark-industries/FRIDAY-Demo/releases/latest).
2. Bajo la última versión, descarga el archivo llamado
   **`Friday-Voice-Agent-Setup-<versión>.exe`**.

---

## Paso 3 — Instala e inicia Friday

1. Abre el archivo que acabas de descargar (normalmente en la carpeta
   **Descargas**).

   **La primera vez**, Windows puede mostrar un recuadro azul que dice *"Windows
   protegió su PC"*. Ocurre con todas las apps gratuitas sin firma de pago.
   Simplemente haz clic en:

   - **Más información**
   - luego **Ejecutar de todas formas**

2. Se abre el instalador. Instala **solo para ti** y **no necesita contraseña de
   administrador**. Haz clic en **Siguiente → Instalar → Finalizar**. (Si quieres,
   puedes marcar "Crear un icono en el escritorio" por el camino.)
3. Inicia **Friday Voice Agent** — desde el **menú Inicio**, el **icono del
   escritorio**, o dejando marcado "Iniciar Friday Voice Agent" en la última
   pantalla del instalador.

Friday se abre. Si Ollama está en ejecución, en la parte superior de la ventana
aparece **ALL SYSTEMS ONLINE (LOCAL)**.

> **Para desinstalar más adelante:** abre **Configuración → Aplicaciones** de
> Windows, busca *Friday Voice Agent* y haz clic en **Desinstalar**.

---

## Paso 4 — Tu primer chat

En la parte inferior de la ventana hay una casilla que dice **"Message Friday…"**.

- Haz clic en ella, escribe algo como *"Hi Friday! What can you do?"* y pulsa
  **Enter**.
- Friday responde en el panel, palabra por palabra. Si el altavoz está activado,
  también lee la respuesta en voz alta. Haz clic en **LISTEN** bajo cualquier
  respuesta para volver a escucharla.

---

## Paso 5 — Habla con Friday (modo de voz)

1. Haz clic en el botón del **micrófono** (abajo a la izquierda de la casilla de
   mensajes), o en el control **Voice mode**, para abrir la esfera luminosa a
   pantalla completa.
2. **Mantén pulsada la barra espaciadora** mientras hablas, y luego suéltala — o
   toca el micrófono en pantalla.
3. Friday transcribe lo que dijiste, piensa y **te responde en voz alta**.
4. ¿Prefieres otra voz? Usa el control de voces en la cabecera (arriba a la
   derecha) para elegir entre **seis voces**.
5. Haz clic en **✕ EXIT** (arriba a la derecha) para volver al chat.

> **El primer uso de la voz** descarga una vez los modelos de voz (unos cientos de
> MB). Después, la voz funciona totalmente sin conexión.

---

## Consejos y solución de problemas

- **Friday dice que los sistemas están offline / el chat no responde.** Ollama no
  está en ejecución, o el modelo no se ha descargado. Asegúrate de que Ollama esté
  abierto y de haber ejecutado `ollama pull qwen2.5:3b` (Paso 1).
- **La voz eligió el micrófono equivocado.** Usa el botón **MIC** en la cabecera
  para elegir otra entrada.
- **El primer inicio parece lento.** Friday calienta su motor de voz al arrancar y
  descarga los modelos de voz en el primer uso de la voz. Los inicios posteriores
  son más rápidos.
- **Nada se envía a la nube.** Tus conversaciones y tu voz permanecen en tu
  máquina. El único uso de la red es la descarga única y tus mensajes yendo a
  Ollama en tu propio PC.

---

Disfruta de Friday — y si te gusta esta muestra gratuita, es una pequeña porción
del asistente de escritorio **Friday** completo.
