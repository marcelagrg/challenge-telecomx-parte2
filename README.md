# 📊 Análise de Evasão de Clientes (Churn) – Telecom X (Parte 2)
Este projeto é a continuação da análise da evasão de clientes (churn) da empresa Telecom X.

O objetivo principal é identificar padrões e fatores associados ao cancelamento de clientes, fornecendo insights que possam apoiar estratégias de retenção e melhoria na experiência do cliente.

Além da Análise Exploratória de Dados foi também utilizado modelos de Machine Learning para prever a probabilidade de cancelamento de clientes com base em diferentes características do serviço e do perfil do cliente.

## 🔍 Preparação dos Dados

Antes da modelagem, foi realizado um processo de preparação dos dados para garantir maior qualidade nas análises.

As variáveis foram classificadas em dois grupos principais:
- Variáveis categóricas
- Variáveis numéricas

### Codificação das variáveis categóricas
As variáveis categóricas foram transformadas utilizando **One-Hot Encoding**, permitindo que os modelos de machine learning utilizem essas informações em formato numérico.

### Separação dos dados
O conjunto de dados foi dividido em:
- 80% para treino
- 20% para teste

Essa separação permite avaliar a capacidade dos modelos de generalizar para novos dados.

## 🤖 Modelos de Machine Learning utilizados
### Regressão Logítica
Modelo estatístico amplamente utilizado para problemas de classificação binária, capaz de estimar a probabilidade de cancelamento de clientes.

Foi utilizada uma versão balanceada do modelo, para lidar com possíveis desequilíbrios entre clientes que cancelaram e os que permaneceram.

### Random Forest
O Random Forest é um algoritmo baseado em múltiplas árvores de decisão, que combina diversas árvores para produzir previsões mais robustas.

Esse modelo também permite avaliar a importância das variáveis, indicando quais fatores mais influenciam a previsão de churn.

### Avaliação dos Modelos

Os modelos foram avaliados utilizando as seguintes métricas:

- Acurácia
- Precisão
- Recall
- F1-score

### Matriz de confusão

A matriz de confusão foi utilizada para visualizar o número de acertos e erros de cada modelo, permitindo identificar verdadeiros positivos (clientes corretamente identificados como churn), verdadeiros negativos, falsos positivos e falsos negativos

Essa análise permite compreender melhor como o modelo se comporta na identificação de clientes que cancelam o serviço.

## 📈 Principais Resultados
A análise indicou que o churn está principalmente associado a:
- Clientes nos primeiros meses de contrato;
- Contratos mensais;
- Ausência de serviços adicionais;
- Determinados métodos de pagamento (ex: cheque eletrônico).

## 🛠 Tecnologias Utilizadas
- Python 3
- Pandas - Manipulação e análise de dados
- NumPy - Operações numéricas e suporte a arrays
- Matplotlib - Visualização de dados
- Seaborn - Visualizações estatísticas
- Scikit-learn - Modelos de Machine Learning
- Jupyter Notebook / Google Colab - Ambiente de desenvolvimento

## 🚀 Como executar o projeto
  ### 1️⃣ Utilizando Google Colab
  Baixe o arquivo [Challenge_TelecomX.ipynb](https://github.com/marcelagrg/challenge-telecomx-parte2/blob/main/Challenge_TelecomX_Parte2.ipynb) e abra no Colab ou acesse diretamente pelo link 'Open in Colab'.

  ### 2️⃣ Localmente utilizando Jupyter Notebook
  #### Certifique-se de ter o Python 3 instalado.
  Clone o repositório
  ```
  git clone github.com/marcelagrg/challenge-telecomx-parte2
  cd challenge-telecomx
  ```
  Instale as dependências
  ```
  pip install -r requirements.txt
  ```
  Execute o Jupyter Notebook
  ```
  jupyter notebook
```
