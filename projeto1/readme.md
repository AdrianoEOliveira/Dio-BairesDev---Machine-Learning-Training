# Treinamento de Redes Neurais com Transfer Learning

Este projeto utiliza **Transfer Learning** com o modelo **MobileNetV2** para classificar imagens de gatos e cachorros. O objetivo é demonstrar como aproveitar modelos pré-treinados para resolver problemas de classificação de imagens com eficiência.

## Estrutura do Notebook

### 1. **Imports**
As bibliotecas necessárias são importadas:
- `TensorFlow` e `Keras` para construção e treinamento do modelo.
- `Matplotlib` para visualização de gráficos e imagens.
- `os`, `zipfile` e `pathlib` para manipulação de arquivos e diretórios.

### 2. **Download do Dataset**
- O dataset **Cats and Dogs** é baixado automaticamente, caso ainda não esteja presente.
- O arquivo ZIP é extraído para um diretório local.

### 3. **Configurações**
- Define o tamanho das imagens (`IMG_SIZE = 224`), tamanho do batch (`BATCH_SIZE = 32`) e uma seed para reprodutibilidade.

### 4. **Filtragem de Imagens Válidas**
- Verifica e filtra imagens corrompidas.
- Cria uma lista de labels:
    - `0` para gatos.
    - `1` para cachorros.

### 5. **Criação do Dataset TensorFlow**
- Converte as imagens e labels em um `tf.data.Dataset`.
- Aplica pré-processamento:
    - Redimensiona as imagens.
    - Normaliza os valores dos pixels para o intervalo `[0, 1]`.

### 6. **Divisão do Dataset**
- Divide o dataset em:
    - **Treino (70%)**
    - **Validação (15%)**
    - **Teste (15%)**

### 7. **Modelo com Transfer Learning**
- Utiliza o **MobileNetV2** pré-treinado como base.
- Adiciona camadas personalizadas:
    - `GlobalAveragePooling2D`
    - `Dense` com 128 neurônios e ativação ReLU.
    - `Dropout` com taxa de 0.3.
    - `Dense` com 1 neurônio e ativação Sigmoid.
- Compila o modelo com:
    - Otimizador Adam.
    - Função de perda binária.
    - Métrica de acurácia.

### 8. **Treinamento**
- O modelo é treinado por 5 épocas, utilizando o conjunto de treino e validação.

### 9. **Avaliação**
- Avalia o modelo no conjunto de teste.
- Exibe a acurácia final.

### 10. **Visualização de Predições**
- Exibe até 5 imagens do conjunto de teste com:
    - Label real (Gato/Cachorro).
    - Predição do modelo (Gato/Cachorro).

## Como Executar
1. Certifique-se de ter o Python 3.7+ instalado.
2. Instale as dependências:
     ```bash
     pip install tensorflow matplotlib
     ```
3. Execute o notebook em um ambiente como Jupyter Notebook ou Google Colab.

## Resultados Esperados
- O modelo deve alcançar uma boa acurácia no conjunto de teste, demonstrando a eficácia do Transfer Learning.
- Gráficos de acurácia e exemplos de predições são gerados para análise.

## Referências
- [Documentação do TensorFlow](https://www.tensorflow.org/)
- [Dataset Cats and Dogs](https://www.microsoft.com/en-us/download/details.aspx?id=54765)

## Executar no Google Colab

Você pode acessar e executar o notebook diretamente no Google Colaboratory através do link abaixo:

[Notebook no Google Colab](https://colab.research.google.com/drive/1vH_dN_dBwolKivtEhFUuvAM71z0IjYUo?usp=sharing)