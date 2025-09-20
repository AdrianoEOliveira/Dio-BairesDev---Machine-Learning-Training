# Projeto YOLO Transfer Learning

Este projeto demonstra como realizar Transfer Learning utilizando o modelo YOLOv8 em um subconjunto do dataset COCO 2017. O objetivo é treinar o modelo para detectar as classes `person` e `car` com um número limitado de imagens, seguindo as etapas descritas abaixo.

## Etapas do Projeto

1. **Atualização de Bibliotecas**  
    Garantimos que as bibliotecas `Ultralytics` e `Weights & Biases (W&B)` estão atualizadas.

2. **Desativação do W&B**  
    Configuramos o ambiente para que o treinamento ocorra localmente, sem envio de métricas para o W&B.

3. **Importação de Bibliotecas**  
    Utilizamos bibliotecas como `ultralytics`, `torch`, `matplotlib`, `pandas`, entre outras.

4. **Configuração Inicial**  
    Definimos as classes alvo (`person` e `car`) e o número máximo de imagens por classe.

5. **Download do COCO 2017**  
    Baixamos as anotações e imagens necessárias para o treinamento.

6. **Conversão COCO → YOLO**  
    Convertendo as anotações do formato COCO JSON para o formato YOLO TXT.

7. **Divisão do Dataset**  
    Dividimos os dados em 70% treino, 15% validação e 15% teste.

8. **Organização do Dataset**  
    Estruturamos as pastas para imagens e labels conforme o padrão YOLO.

9. **Criação do `dataset.yaml`**  
    Geramos o arquivo de configuração necessário para o treinamento do YOLO.

10. **Transfer Learning com YOLO Pré-treinado**  
     Realizamos o fine-tuning do modelo `yolo11n.pt` no dataset preparado.

11. **Avaliação no Conjunto de Teste**  
     Avaliamos o modelo treinado no split de teste, analisando métricas como `box_loss`, `cls_loss` e `precision`.

12. **Visualização das Métricas**  
     Plotamos as curvas de perda e métricas de precisão utilizando os logs gerados.

13. **Predições em Imagens de Teste**  
     Geramos predições em imagens do conjunto de teste e exibimos os resultados.

## Link para o Google Colaboratory

Você pode acessar e executar o notebook diretamente no Google Colaboratory através do link abaixo:

[Notebook no Google Colab](https://colab.research.google.com/drive/1gE4dacXmezB1Ziu_t6DCeeRcJzD2S_dd?usp=sharing)
