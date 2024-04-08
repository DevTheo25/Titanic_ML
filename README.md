# Projeto Machine Learning: Titanic
Este repositório contém o código e os recursos utilizados para a participação na [competição do Titanic no Kaggle.](https://www.kaggle.com/competitions/titanic)

## Resultados das Análises
![image](https://github.com/DevTheo25/Titanic_ML/assets/122491960/2acf553e-8cde-4f22-9b63-520e3c8b985d)



## [Primeira Análise:](https://github.com/DevTheo25/Titanic_ML/blob/main/Primeira_analise.ipynb)

Nesta primeira análise, utilizamos as colunas **Sex** e **Age** como características-chave para o treinamento dos modelos de Machine Learning. Isso se baseia na conhecida política de priorização de mulheres e crianças durante o naufrágio do Titanic.
- Fizemos a conversão da coluna **Sex** para binário, onde **female** recebeu o valor 1 e **male** recebeu o valor 0.
- Fizemos o tratamento de dados nulos na coluna **Age**, substituindo os valores nulos pela média da coluna.
- Utilizamos 3 modelos de Machine Leaning que são **RandomForest**, **KNeighborsClassifer** e **LogisticRegression**.
### Resultados da acurácia dos modelos em dados de Treino e Validação.
- **RandomForest**: 0.6502242152466368
- **KNeighborsClassifer**: 0.6860986547085202
- **LogisticRegression**: 0.6591928251121076

### Resultado final com o modelo **KNeighborsClassifer**:
- O score público retornado pelo kaggle foi de: **0.69377**
---
## [Segunda Análise:](https://github.com/DevTheo25/Titanic_ML/blob/main/Segunda_analise.ipynb)
Nesta análise, utilizamos a maioria das colunas do conjunto de dados para treinar os modelos, excluindo apenas aquelas com alta cardinalidade, como Name, Ticket e Cabin. Identificamos padrões nas demais colunas e aplicamos os tratamentos necessários.
- Fizemos os mesmos tratamentos para as colunas **Sex** e **Age** feito na [primeira análise.](https://github.com/DevTheo25/Titanic_ML/blob/main/Primeira_analise.ipynb)
- Fizemos o tratamento de valores nulos da coluna **Fare**, substituindo pela média da coluna.
- Fizemos o tratamento da coluna de texto **Embarked** utlizando **One-hot encoding**.
- Utilizamos 3 modelos de Machine Leaning que são **RandomForest**, **KNeighborsClassifer** e **LogisticRegression**.
### Resultados da acurácia dos modelos em dados de Treino e Validação.
- **RandomForest**: 0.7757847533632287
- **KNeighborsClassifer**: 0.7309417040358744
- **LogisticRegression**: 0.7937219730941704

### Resultado final com o modelo **LogisticRegression**:
- O score público retornado pelo kaggle foi de: **0.77033**
---
## [Terceira Análise:](https://github.com/DevTheo25/Titanic_ML/blob/main/Terceira_analise.ipynb)
