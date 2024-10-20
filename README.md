# Previsão de Churn de Clientes

Este projeto tem como objetivo prever se um cliente irá ser churn (cancelar o serviço) ou não, utilizando modelos de classificação. O foco é melhorar a retenção de clientes por meio da identificação antecipada de potenciais churn. As técnicas utilizadas incluem balanceamento de classes, busca de hiperparâmetros e visualização dos resultados.

## Estrutura do Projeto

- **`pandas` e `numpy`**: Utilizados para manipulação e análise dos dados.
- **`scikit-learn`**: Principal biblioteca para construção dos modelos, avaliação de métricas e pré-processamento de dados.
- **`imbalanced-learn`**: Utilizado para balanceamento de dados com a técnica de SMOTE.
- **`matplotlib` e `seaborn`**: Para visualização dos dados e das métricas dos modelos.

## Modelos Utilizados

1. **RandomForestClassifier**: Modelo de árvore de decisão baseado em múltiplas árvores (ensemble) para melhorar a precisão e reduzir o risco de overfitting.
2. **LogisticRegression**: Modelo linear que estima a probabilidade de um cliente churnar, sendo adequado para interpretação dos coeficientes.

## Técnicas de Pré-processamento

- **LabelEncoder** e **OneHotEncoder**: Para transformar variáveis categóricas em um formato numérico adequado para os modelos.
- **SMOTE (Synthetic Minority Over-sampling Technique)**: Usado para balancear a quantidade de amostras entre classes de clientes que churnam e não churnam. Isso ajuda a melhorar o desempenho do modelo ao lidar com conjuntos de dados desbalanceados.

## Otimização de Hiperparâmetros

- **GridSearchCV**: Utilizado para encontrar a melhor combinação de hiperparâmetros para os modelos, melhorando sua performance.

## Métricas de Avaliação

- **accuracy_score**: Avalia a proporção de previsões corretas.
- **confusion_matrix**: Fornece uma matriz de confusão para analisar a taxa de falsos positivos e falsos negativos.
- **classification_report**: Gera um relatório detalhado com precisão, recall e F1-score.
- **mean_absolute_error** e **root_mean_squared_error**: Utilizados para análise complementar dos erros, apesar do foco ser em classificação.

## Visualizações

- **Gráficos de Confusion Matrix**: Utilizados para visualizar a performance dos modelos em termos de previsões corretas e incorretas.
- **Histogramas e Scatter Plots**: Para análise exploratória dos dados antes do treinamento dos modelos.
