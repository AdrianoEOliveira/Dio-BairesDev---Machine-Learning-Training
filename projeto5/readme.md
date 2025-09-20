# Sistema de Reconhecimento Facial  

Este projeto implementa um sistema de reconhecimento facial utilizando o framework YOLOv8 e redes neurais com TensorFlow. O objetivo é detectar e classificar rostos em imagens, utilizando o dataset **LFW (Labeled Faces in the Wild)**, considerando apenas indivíduos com 10 ou mais imagens de referência, garantindo maior consistência nos resultados.  

## Etapas do Projeto  

### 1. Atualização e Instalação de Dependências  
As bibliotecas necessárias para o projeto incluem:  
- `ultralytics`: Framework YOLOv8 para detecção de objetos.  
- `tensorflow`: Suporte para redes neurais.  
- `opencv-python-headless`: Manipulação de imagens.  
- `matplotlib`: Visualização de gráficos.  
- `tqdm`: Barra de progresso.  

### 2. Download do Dataset  
O dataset **LFW** é baixado utilizando o `tensorflow_datasets`. As imagens são organizadas em pastas por nome da pessoa, facilitando o processamento.  

### 3. Detecção e Recorte de Faces  
Utilizamos o modelo YOLOv8 pré-treinado para detectar rostos nas imagens. As faces detectadas são recortadas e redimensionadas para 160×160 pixels, sendo salvas em uma nova pasta organizada por pessoa.  

### 4. Treinamento do Modelo  
O modelo de reconhecimento facial é treinado utilizando as imagens processadas. O dataset é dividido em 70% para treino e 30% para validação.  

### 5. Avaliação  
A acurácia do modelo é avaliada no conjunto de validação, e os resultados são apresentados em gráficos de perda e precisão.  

## Como Executar  
1. Certifique-se de ter o Python 3.8+ instalado.  
2. Clone este repositório.  
3. Instale as dependências listadas no notebook.  
4. Execute o notebook no Google Colaboratory ou localmente.  

## Link para o Google Colaboratory  

Você pode acessar e executar o notebook diretamente no Google Colaboratory através do link abaixo:

[Notebook no Google Colab](https://colab.research.google.com/drive/1HnS5c9hkWDJyj-8HiK8bETEzS_R-S90x?usp=sharing)  