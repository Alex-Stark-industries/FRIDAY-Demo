# Bem-vindo à Friday 👋

🌐 [English](WELCOME.md) · [Italiano](WELCOME.it.md) · [Español](WELCOME.es.md) · [Français](WELCOME.fr.md) · [Deutsch](WELCOME.de.md) · **Português** · [हिन्दी](WELCOME.hi.md)

Este guia leva você do zero até conversar com a Friday, sem pressupor **nada**. Se
você sabe baixar um arquivo, sabe iniciar a Friday.

A Friday é um assistente de IA gratuito que roda no **seu próprio computador**.
Você pode **escrever** para ela ou **falar** com ela, e ela responde — por texto e
em voz alta. Não precisa de conta, cadastro nem assinatura paga. A Friday responde
em **inglês**.

---

## O que você precisa

- Um PC com **Windows 10 ou 11** (64 bits).
- **8 GB de RAM** ou mais (16 GB é confortável). A Friday executa a IA na sua
  própria máquina, então a memória importa.
- Cerca de **4 GB de espaço livre** no total: o app em si (~0,5 GB), o modelo de
  IA que você baixa uma vez (~2 GB) e os modelos de voz baixados no primeiro uso
  da voz (~0,5 GB).
- Uma conexão de internet **apenas para a configuração** — depois de configurado,
  o chat e a voz funcionam offline.

Uma placa de vídeo (GPU) com suporte a **WebGPU** (qualquer GPU NVIDIA, AMD ou
Intel recente) deixa a voz rápida — mas a Friday funciona sem ela também, só mais
devagar. Em um PC mais simples tudo funciona mesmo assim; as respostas e a voz
apenas levam um pouco mais de tempo.

> Não sabe as especificações do seu PC? Pressione a **tecla Windows**, digite
> **"Sobre o seu PC"** e abra — ele mostra a versão do Windows, o processador e a
> RAM instalada.

---

## Passo 1 — Instale o Ollama (o cérebro da Friday)

A Friday pensa usando um motor de IA local e gratuito chamado **Ollama**. Você o
instala uma única vez.

1. Acesse **https://ollama.com** e clique em **Download**.
2. Execute o instalador que você baixou e siga as instruções. Pronto — o Ollama
   agora roda discretamente em segundo plano.
3. Abra um terminal (pressione a **tecla Windows**, digite **`cmd`**, pressione
   **Enter**) e cole esta linha, depois pressione **Enter**:

   ```
   ollama pull qwen2.5:3b
   ```

   Isso baixa o modelo de IA que a Friday usa (cerca de 2 GB). Espere terminar —
   você só faz isso uma vez.

> **Como sei se o Ollama está rodando?** Depois de instalar, procure o ícone do
> Ollama perto do relógio na barra de tarefas. Se não o vir, abra o menu Iniciar e
> inicie o **Ollama**.

---

## Passo 2 — Baixe a Friday

1. Acesse a página de [**Releases**](../../releases/latest).
2. Na versão mais recente, baixe o arquivo chamado
   **`Friday-Voice-Agent-Setup-<versão>.exe`**.

---

## Passo 3 — Instale e inicie a Friday

1. Abra o arquivo que você acabou de baixar (geralmente na pasta **Downloads**).

   **Na primeira vez**, o Windows pode mostrar uma caixa azul dizendo *"O Windows
   protegeu seu computador"*. Isso acontece com todos os apps gratuitos sem
   assinatura paga. Basta clicar em:

   - **Mais informações**
   - depois **Executar assim mesmo**

2. O instalador abre. Ele instala **só para você** e **não precisa de senha de
   administrador**. Clique em **Avançar → Instalar → Concluir**. (Você pode marcar
   "Criar um ícone na área de trabalho" no caminho, se quiser.)
3. Inicie o **Friday Voice Agent** — pelo **menu Iniciar**, pelo **ícone na área
   de trabalho**, ou deixando marcada a opção "Iniciar Friday Voice Agent" na
   última tela do instalador.

A Friday abre. Se o Ollama estiver rodando, no topo da janela aparece **ALL
SYSTEMS ONLINE (LOCAL)**.

> **Para desinstalar depois:** abra **Configurações → Aplicativos** do Windows,
> encontre *Friday Voice Agent* e clique em **Desinstalar**.

---

## Passo 4 — Seu primeiro chat

Na parte inferior da janela há uma caixa que diz **"Message Friday…"**.

- Clique nela, digite algo como *"Hi Friday! What can you do?"* e pressione
  **Enter**.
- A Friday responde no painel, palavra por palavra. Se o som estiver ligado, ela
  também lê a resposta em voz alta. Clique em **LISTEN** abaixo de qualquer
  resposta para ouvi-la de novo.

---

## Passo 5 — Fale com a Friday (modo de voz)

1. Clique no botão de **microfone** (canto inferior esquerdo da caixa de
   mensagens), ou no controle **Voice mode**, para abrir a esfera luminosa em tela
   cheia.
2. **Segure a barra de espaço** enquanto fala e depois solte — ou toque no
   microfone na tela.
3. A Friday transcreve o que você disse, pensa e **responde em voz alta**.
4. Prefere outra voz? Use o controle de vozes no cabeçalho (canto superior
   direito) para escolher entre **seis vozes**.
5. Clique em **✕ EXIT** (canto superior direito) para voltar ao chat.

> **No primeiro uso da voz**, os modelos de voz são baixados uma vez (algumas
> centenas de MB). Depois disso, a voz funciona totalmente offline.

---

## Dicas e solução de problemas

- **A Friday diz que os sistemas estão offline / o chat não responde.** O Ollama
  não está rodando, ou o modelo não foi baixado. Verifique se o Ollama está aberto
  e se você executou `ollama pull qwen2.5:3b` (Passo 1).
- **A voz escolheu o microfone errado.** Use o botão **MIC** no cabeçalho para
  escolher outra entrada.
- **A primeira inicialização parece lenta.** A Friday aquece o motor de voz ao
  iniciar e baixa os modelos de voz no primeiro uso da voz. As próximas
  inicializações são mais rápidas.
- **Nada é enviado para a nuvem.** Suas conversas e sua voz ficam na sua máquina. O
  único uso de rede são os downloads únicos e suas mensagens indo para o Ollama no
  seu próprio PC.

---

Aproveite a Friday — e se você gostar desta amostra gratuita, ela é uma pequena
fatia do assistente de desktop **Friday** completo.
