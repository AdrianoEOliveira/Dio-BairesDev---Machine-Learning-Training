# Sistema de Geração de Testes Unitários com Google Gemini

Este projeto apresenta um sistema automatizado para geração de testes unitários utilizando o modelo **Google Gemini 1.5 Flash**. O objetivo é facilitar a criação de testes para funções Python, garantindo cobertura básica e acelerando o processo de validação de código.

## Funcionalidades

1. **Instalação de Dependências**: Instalação das bibliotecas necessárias, como `google-generativeai` e `pytest`.
2. **Configuração da API**: Integração com a API do Google Gemini utilizando os **Secrets do Google Colab**.
3. **Geração Automática de Testes**: Criação de testes unitários com base no comportamento real das funções fornecidas.
4. **Execução de Testes**: Salvamento dos testes gerados e execução automática utilizando `pytest`.
5. **Exemplos Práticos**: Geração e execução de testes para funções simples, como soma e divisão.

## Como Funciona

1. **Entrada**: Código Python e nome do arquivo.
2. **Processamento**: O modelo Google Gemini analisa o código e gera testes unitários seguindo boas práticas.
3. **Saída**: Arquivo de testes gerado e resultados da execução dos testes.

## Requisitos

- Python 3.12 ou superior.
- Conta no Google Colab com acesso à API do Google Gemini.
- Bibliotecas: `google-generativeai`, `pytest`.

## Como Executar

1. Clone este repositório.
2. Abra o notebook no Google Colab.
3. Siga as instruções do notebook para instalar dependências, configurar a API e gerar testes.
4. Execute os testes gerados para validar o comportamento das funções.

## Observações

- Revise os testes gerados antes de utilizá-los em produção.
- Certifique-se de configurar corretamente a chave da API no Google Colab.

## Link para o Google Colab

[Notebook no Google Colaboratory](https://colab.research.google.com/drive/1k3Bd4m0ChQmbT31IzUfImoIdUQKM-1be)  