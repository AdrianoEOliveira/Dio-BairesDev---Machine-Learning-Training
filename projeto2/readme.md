# Redução de Dimensionalidade em Imagens para Redes Neurais

Este projeto demonstra técnicas de processamento de imagens para reduzir a dimensionalidade e preparar os dados para uso em redes neurais. O notebook realiza as seguintes etapas:

## Etapas do Projeto

### 1. **Download da Imagem**
- A imagem é baixada do Wikimedia Commons utilizando a biblioteca `requests` com um cabeçalho `User-Agent` para evitar erros de requisição.

### 2. **Processamento da Imagem**
- **Conversão para Tons de Cinza**:
    - Cada pixel da imagem original é convertido de RGB para escala de cinza utilizando a fórmula ponderada:
        \[
        \text{cinza} = 0.299 \cdot R + 0.587 \cdot G + 0.114 \cdot B
        \]
- **Conversão para Imagem Binária**:
    - Um limiar (threshold) é aplicado para gerar uma imagem binária:
        - Pixels com valor >= 128 são convertidos para branco (255).
        - Pixels com valor < 128 são convertidos para preto (0).

### 3. **Salvamento e Exibição**
- As imagens processadas são salvas como:
    - `Cidade_Maravilhosa_cinza.jpg`
    - `Cidade_Maravilhosa_binaria.jpg`
- As imagens geradas são exibidas diretamente no ambiente do Google Colab.

## Tecnologias Utilizadas
- Python 3
- Bibliotecas:
    - `requests`
    - `Pillow`
    - `IPython.display`

## Como Executar
1. Clone este repositório.
2. Abra o notebook no Google Colaboratory.
3. Execute as células sequencialmente para realizar o processamento da imagem.

## Link para o Google Colaboratory

Você pode acessar e executar o notebook diretamente no Google Colaboratory através do link abaixo:

[Notebook no Google Colab](https://colab.research.google.com/drive/1Pe7a-ircb6pOEp0ry1f3EHtVP6kyzoFj?usp=sharing)
