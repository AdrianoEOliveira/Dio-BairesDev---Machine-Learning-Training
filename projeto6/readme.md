# Sistema de Recomendação por Imagens Digitais  

Este projeto implementa um **Sistema de Recomendação por Imagens Digitais** utilizando o dataset **Fashion-MNIST** como exemplo. O objetivo é criar um sistema eficiente que, dado uma imagem de consulta, retorna as imagens mais similares do dataset.  

## Motivação  
Para evitar problemas de falta de espaço e otimizar o uso de memória, o projeto utiliza uma versão leve da rede neural **MobileNetV2** com `alpha=0.35` e redimensiona as imagens para **96x96 pixels**. Além disso, o índice **FAISS** é utilizado para busca eficiente de similaridade entre os embeddings gerados.  

## Etapas do Projeto  
1. **Instalação e Imports**: Configuração do ambiente e bibliotecas necessárias.  
2. **Carregamento do Dataset**: Divisão do Fashion-MNIST em treino, validação e teste (70/15/15).  
3. **Pré-processamento**: Redimensionamento, conversão para RGB, normalização e criação de batches.  
4. **Modelo MobileNetV2**: Transfer Learning com uma versão leve da MobileNetV2 para gerar embeddings.  
5. **Treinamento**: Treinamento rápido (3 épocas) para extrair features representativas.  
6. **Modelo de Embeddings**: Criação de um modelo derivado para gerar embeddings de 128 dimensões.  
7. **Índice FAISS**: Criação de um índice FAISS para busca eficiente de imagens similares.  
8. **Recomendação**: Função que retorna as imagens mais similares à consulta.  

## Como Executar  
1. Clone este repositório.  
2. Certifique-se de ter o Python 3 e as bibliotecas listadas no notebook instaladas.  
3. Execute o notebook no Google Colaboratory ou em sua máquina local.  

## Link para o Google Colaboratory 

Você pode acessar e executar o notebook diretamente no Google Colaboratory através do link abaixo:

[Notebook no Google Colaboratory](https://colab.research.google.com/)  