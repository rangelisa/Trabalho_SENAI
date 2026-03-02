# 🚢 Projeto de Machine Learning - Titanic (SENAI)

Projeto desenvolvido para aplicar conceitos de **Machine Learning** utilizando o dataset do Titanic, com o objetivo de prever a sobrevivência dos passageiros.

---

## 🎯 Objetivo

Construir um modelo de classificação capaz de prever se um passageiro sobreviveu ou não ao naufrágio do Titanic, utilizando o algoritmo **Decision Tree (Árvore de Decisão)**.

---

## 📊 Dataset

O conjunto de dados utilizado foi o **Titanic Dataset**, contendo informações como:

- Classe do passageiro (Pclass)
- Sexo (Sex)
- Idade (Age)
- Número de irmãos/cônjuges a bordo (SibSp)
- Número de pais/filhos a bordo (Parch)
- Tarifa paga (Fare)
- Sobrevivência (variável alvo)

---

## 🛠️ Tecnologias Utilizadas

- Python
- Google Colab
- Pandas
- Scikit-learn
- Pickle

---

## 🔎 Etapas do Projeto

### 1️⃣ Importação dos dados
Os dados foram carregados a partir de um arquivo `.xlsx` armazenado no Google Drive.

### 2️⃣ Tratamento dos dados
- Remoção de colunas irrelevantes (`Name`, `PassengerId`, `index`)
- Transformação da variável `Sex` em variável numérica:
  - male → 0
  - female → 1

### 3️⃣ Separação das variáveis
- Variáveis independentes (X):
  - `Pclass`
  - `Sex`
  - `Age`
  - `SibSp`
  - `Parch`
  - `Fare`

- Variável dependente (y):
  - `Survived_y`

### 4️⃣ Divisão dos dados
Os dados foram divididos em:
- 90% para treino
- 10% para teste

Utilizando `train_test_split`.

### 5️⃣ Treinamento do modelo
Foi utilizado o algoritmo:

```
DecisionTreeClassifier(max_depth=1)
```

### 6️⃣ Avaliação
O modelo foi avaliado utilizando a métrica **Accuracy (Acurácia)**.

Exemplo de saída:

```
Acurácia: 0.xx
```

---

## 📈 Resultado

O modelo apresentou uma acurácia baseada no conjunto de teste, indicando a porcentagem de previsões corretas realizadas.

---
