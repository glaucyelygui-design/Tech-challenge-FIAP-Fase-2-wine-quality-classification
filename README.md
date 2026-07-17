# Tech-challenge-FIAP-Fase-2-
Classificação da Qualidade de Vinhos com Machine Learning

## Sobre o projeto

Este projeto foi desenvolvido como parte do **Tech Challenge - Fase 2** da Pós-Tech em Data Analytics da FIAP.

O objetivo consiste em desenvolver um modelo de Machine Learning capaz de prever a qualidade de um vinho utilizando apenas suas características físico-químicas, a partir de dados já coletados anteriormente.

Tradicionalmente, a qualidade dos vinhos é determinada por especialistas através de análises sensoriais. Entretanto, esse processo pode ser subjetivo e depender da experiência do avaliador. Neste trabalho, busquei investigar se as técnicas de Ciência de Dados seriam capazes de auxiliar esse processo por meio da construção de modelos preditivos.



# Objetivo

Construir uma pipeline completa de Ciência de Dados capaz de:

- Compreender o problema de negócio;
- Realizar análise exploratória dos dados (EDA);
- Preparar os dados para Machine Learning;
- Treinar modelos de classificação;
- Comparar o desempenho dos modelos;
- Interpretar os resultados obtidos.

A variável **quality** foi transformada em uma classificação binária para facilitar a execução e avaliação das problemáticas:

- Alta Qualidade: qualidade ≥ 7;
- Baixa/Média Qualidade: qualidade < 7.



# Dataset

Foi utilizado o **Wine Quality Dataset**, disponibilizado publicamente no Kaggle.

O conjunto de dados contém informações físico-químicas dos vinhos, incluindo:

- Fixed Acidity;
- Volatile Acidity;
- Citric Acid;
- Residual Sugar;
- Chlorides;
- Free Sulfur Dioxide;
- Total Sulfur Dioxide;
- Density;
- pH;
- Sulphates;
- Alcohol;
- Quality.



# Tecnologias utilizadas

- Python
- Google Colab

## Bibliotecas

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn


# Metodologia

O projeto foi desenvolvido seguindo as etapas propostas pelo Tech Challenge.

## 1. Compreensão do problema

Foi realizada a contextualização do problema de negócios, identificando a necessidade de prever a qualidade dos vinhos por meio de suas características físico-químicas.

## 2. Análise Exploratória dos Dados (EDA)

Durante a análise exploratória foram realizadas as seguintes etapas:

- inspeção da estrutura da base de dados;
- estatísticas descritivas;
- identificação de valores nulos;
- verificação de registros duplicados;
- análise da distribuição das variáveis;
- avaliação do balanceamento das classes;
- estudo das correlações entre as variáveis;
- identificação de possíveis outliers.

Os principais insights encontrados foram:

- o dataset não apresenta valores nulos;
- não existem registros duplicados;
- o teor alcoólico apresentou correlação positiva com a qualidade;
- a acidez volátil apresentou correlação negativa com a qualidade;
- os outliers identificados representam características reais dos vinhos e foram mantidos na análise
- os vinhos de boa qualidade possuem menos indícios de outliers.

## 3. Pré-processamento

Nesta etapa foram realizadas:

- identidicação da variável alvo;
- transformação da variável de qualidade em classificação binária;
- divisão dos dados em conjuntos de treino e teste;
- normalização das variáveis utilizando MinMaxScaler.

## 4. Desenvolvimento dos Modelos

Foram treinados dois modelos de classificação:

### Regressão Logística

Utilizada como modelo base para problemas de classificação binária.

### Random Forest

Modelo baseado em árvores de decisão, capaz de identificar relações não lineares e interações entre as variáveis.


# Avaliação dos Modelos

Os modelos foram avaliados utilizando as seguintes métricas:

- Accuracy;
- Precision;
- Recall;
- F1-score;
- ROC-AUC.

Também foram analisados:

- matrizes de confusão;
- relatórios de classificação;
- comparação entre os modelos.


# Resultados

A comparação entre os modelos demonstrou que a **Random Forest apresentou desempenho superior em todas as métricas avaliadas**, especialmente na identificação dos vinhos classificados como de alta qualidade.

O modelo apresentou melhor equilíbrio entre precisão e sensibilidade, tornando-se a alternativa mais adequada para o problema proposto.


# Principais Insights

- O teor alcoólico apresentou relação positiva com a qualidade do vinho.
- A acidez volátil apresentou relação negativa com a qualidade.
- A qualidade do vinho depende da interação entre diversas características físico-químicas.
- O modelo baseado em árvores de decisão apresentou desempenho superior para o problema apresentado.


# Conclusão

Os resultados demonstraram que técnicas de Machine Learning podem ser utilizadas como ferramenta de apoio à tomada de decisão na classificação de qualidade dos vinhos.

Embora não substituam a avaliação realizada por especialistas, os modelos desenvolvidos permitem prever, com boa precisão, a qualidade dos vinhos a partir de suas características físico-químicas, auxiliando produtores no controle de qualidade e na padronização da produção.

Entre os modelos avaliados, a **Random Forest apresentou o melhor desempenho**, sendo considerada a solução mais adequada ao modelo de negócio.


# Autora

**Glaucyely**

Pós-Tech em Data Analytics

FIAP


# Referências

- Wine Quality Dataset (Kaggle)
- Scikit-Learn
- Numpy
- Pandas 
- Matplotlib 
- Seaborn 
