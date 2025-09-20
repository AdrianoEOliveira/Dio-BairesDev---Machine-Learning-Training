# Projeto: Sistema de Assistência Virtual do Zero

Este projeto implementa um sistema de assistência virtual utilizando Python. O assistente é capaz de realizar tarefas como reconhecimento de voz, síntese de fala, pesquisa na Wikipédia, e geração de links para YouTube e Google Maps. O código foi desenvolvido em um ambiente Jupyter Notebook.

## Funcionalidades

1. **Reconhecimento de Voz**: Transcrição de áudio para texto utilizando a biblioteca `SpeechRecognition`.
2. **Síntese de Fala**: Conversão de texto para áudio com a biblioteca `gTTS`.
3. **Pesquisa na Wikipédia**: Busca e resumo de informações diretamente da Wikipédia.
4. **Geração de Links**:
    - Pesquisa no YouTube.
    - Localização de farmácias próximas via Google Maps.
5. **Interatividade**: O assistente responde aos comandos do usuário em áudio e texto.

## Observação Importante

O Google Colaboratory não permite o uso direto do microfone para captura de áudio devido a restrições de segurança. Por isso, o sistema utiliza arquivos de áudio pré-gravados ou entradas de texto para simular a interação.

## Como Executar

1. Clone este repositório para sua máquina local.
2. Certifique-se de ter o Python 3 instalado.
3. Instale as dependências necessárias:
    ```bash
    pip install SpeechRecognition pydub gTTS wikipedia
    ```
4. Execute o notebook em um ambiente compatível, como Jupyter Notebook ou Google Colaboratory.

## Link para o Google Colaboratory

Você pode acessar e executar o notebook diretamente no Google Colaboratory através do link abaixo:

[Notebook no Google Colaboratory](https://colab.research.google.com/drive/1HnS5c9hkWDJyj-8HiK8bETEzS_R-S90x?usp=sharing)
