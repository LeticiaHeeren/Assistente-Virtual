# Assistente Virtual

Este projeto é uma assistente virtual desenvolvida no Google Colab que recebe comandos de áudio em português e, ao transcrever a fala, abre links relacionados a comandos como "abrir YouTube", "acessar Wikipedia", entre outros. Utiliza reconhecimento de fala para interpretar comandos e gerar links clicáveis de maneira interativa.

# Como Funciona

O projeto funciona através de upload de arquivos de áudio que contêm comandos gravados em português (pt-BR). Após o envio do áudio, o sistema transcreve a fala para texto e interpreta o comando, gerando um link correspondente que o usuário pode clicar diretamente no notebook.

# Como executar

* **Upload do Áudio:** O usuário faz o upload de um arquivo de áudio (em formatos como .wav, .mp3, .ogg, etc.) utilizando a interface do Google Colab.

* **Transcrição do Áudio:** O áudio é transcrito em tempo real para texto usando a API do Google Speech-to-Text.

* **Interpretação do Comando:** O comando transcrito é analisado e comparado com um conjunto de palavras-chave predefinidas (ex: "youtube", "google", "wikipedia").

* **Geração de Link:** Dependendo do comando identificado, um link correspondente é gerado e apresentado de forma clicável.
  Por exemplo: "Abra o YouTube" gera um link para o YouTube.  "Acesse o Wikipedia" gera um link para a página principal da Wikipedia em português.

# Requisitos

Este projeto utiliza as seguintes bibliotecas:

* **speech_recognition** — Para transcrever o áudio para texto.

* **ipywidgets** — Para interface interativa no Google Colab.

* **pydub** — Para manipulação de arquivos de áudio (conversão para WAV, se necessário).

* **re** — Para realizar buscas de palavras-chave no comando transcrito.
