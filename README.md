# Projeto de Tratamento e Análise de Dados de Imóveis

Este repositório contém um conjunto de scripts em Python para realizar web scraping, tratamento, análise e modelagem de dados relacionados a preços de imóveis. O projeto abrange diversas funcionalidades para extrair dados de imóveis disponíveis para venda ou aluguel em várias cidades brasileiras, realizar análises exploratórias, pré-processamento desses dados e compará-los com uma base de dados disponível no Kaggle.

## Funcionalidades

### Web Scraping e Pré-processamento

- Utilizamos a biblioteca `requests` para realizar requisições HTTP e `json` para manipulação de dados JSON.
- Para manipulação e análise de dados, empregamos as bibliotecas `pandas` e `numpy`.
- Realizamos tratamento de valores ausentes com `SimpleImputer` e codificação de variáveis categóricas com `LabelEncoder` e `OneHotEncoder`.
- Normalizamos dados numéricos com `StandardScaler` e `MinMaxScaler`.
- Dividimos o conjunto de dados em conjuntos de treino e teste com `train_test_split` e avaliamos modelos usando `cross_val_score` e `GridSearchCV`.
- Os modelos de regressão incluem `LinearRegression`, `KNeighborsRegressor`, `DecisionTreeRegressor` e `RandomForestRegressor`.
- Para classificação, empregamos `LogisticRegression`, `DecisionTreeClassifier` e `GaussianNB`.
- Avaliamos os modelos usando métricas como `classification_report`, `accuracy_score`, `precision_score`, `recall_score`, `f1_score` e `confusion_matrix`.

### Visualização e Comparação de Modelos

- Utilizamos `matplotlib` e `seaborn` para criação de gráficos e visualização de dados estatísticos.
- Comparamos diferentes algoritmos de regressão quanto ao seu desempenho usando métricas como R² score e MSE.

## Utilização

Para utilizar este projeto, siga os seguintes passos:

1. Clone este repositório em sua máquina local.
2. Instale todas as bibliotecas necessárias listadas no arquivo `requirements.txt`.
3. Execute o script `Imóveis_(DATA_CLEANING)` para extrair os dados de imóveis de várias cidades brasileiras.
4. Execute o script `Imóveis_(TRAINING_MODELS)` para comparar os dados extraídos com a base de dados disponível no Kaggle.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir um pull request ou uma issue para propor melhorias, correções ou novas funcionalidades.

## Licença

Este projeto é licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT).
