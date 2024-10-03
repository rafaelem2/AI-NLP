# AI-NLP

# Classificação de Tweets de Desastres no Dataset Kaggle

Este projeto tem como objetivo classificar tweets relacionados a desastres usando técnicas de processamento de linguagem natural (NLP) e aprendizado de máquina. O dataset utilizado foi extraído da competição "Natural Language Processing with Disaster Tweets" do Kaggle.

## Estrutura do Projeto

O projeto está estruturado da seguinte forma:

- `project.ipynb`: Contém o código implementado em Python, incluindo a análise exploratória, pré-processamento dos dados e treinamento dos modelos de classificação.
- `train.csv`: Dataset utilizado para treinar os modelos de classificação.
- `test.csv`: Dataset utilizado para testar as previsões dos modelos treinados.
- `README.md`: Este arquivo, que fornece uma visão geral do projeto.
- `artigo.pdf`: Um relatório técnico em formato IEEE detalhando o pipeline de classificação, resultados e conclusões.

## Objetivo

O objetivo deste projeto é desenvolver um pipeline de classificação para identificar se um tweet está relacionado a desastres. Foram utilizados diferentes classificadores de aprendizado de máquina para comparar seus desempenhos:

- **Regressão Logística**
- **Máquina de Vetores de Suporte (SVM)**
- **Naive Bayes**

## Etapas do Projeto

1. **Pré-processamento dos Dados**:
   - Remoção de stopwords
   - Tokenização e stemming
   - Conversão dos textos em vetores usando TF-IDF

2. **Treinamento dos Modelos**:
   Foram treinados três classificadores: Regressão Logística, SVM e Naive Bayes.

3. **Avaliação dos Modelos**:
   O Naive Bayes apresentou o melhor desempenho geral.

4. **Análise do Tamanho do Dataset**:
   Foi realizada uma análise do impacto do tamanho do dataset no desempenho do modelo, observando-se melhorias até certo ponto de saturação de dados.

5. **Previsões Finais**:
   As previsões foram geradas no dataset de teste (**test.csv**) utilizando o modelo Naive Bayes.

## Como Executar o Projeto

### Requisitos

Certifique-se de que você tem os seguintes pacotes instalados:
- `numpy`
- `pandas`
- `scikit-learn`
- `nltk`
- `matplotlib`

Você pode instalar os requisitos com o seguinte comando:

```bash
pip install -r requirements.txt
