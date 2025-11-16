## 🩸 README reescrito — Blood Donation Prediction Project
## 🩸 Blood Donation Prediction — Machine Learning for Donor Engagement

Um sistema preditivo para identificar doadores com maior probabilidade de comparecer em campanhas de doação de sangue.

# 📌 Visão Geral

Este projeto utiliza Machine Learning para prever se um doador retornará em futuras campanhas, permitindo que hemocentros planejem ações de forma mais eficiente, reduzam desperdícios e evitem estoques críticos.

A solução foi construída como parte de um estudo de caso de Aprendizado de Máquina, utilizando Support Vector Machine (SVM) para classificação binária.

# 🎯 Objetivo do Projeto

Auxiliar hemocentros a antecipar a demanda e disponibilidade de doadores.

Identificar padrões de comportamento baseados no histórico de doações.

Criar um modelo simples, interpretável e facilmente aplicável em sistemas reais.

# 📊 Dataset

O dataset doacao.csv contém 748 registros, com as seguintes variáveis:

Variável	Descrição
Recência	Meses desde a última doação
Frequência	Número total de doações
Quantidade	Volume total doado (cm³)
Tempo	Meses desde a primeira doação
Doou	Variável alvo (1 = doou, 0 = não doou)

O dataset apresenta desbalanceamento moderado, o que exigiu técnicas de ajuste.

# 🛠️ Metodologia
1. Pré-processamento

Carregamento e inspeção do dataset

Remoção de inconsistências

Balanceamento com undersampling para compensar a classe minoritária

Divisão treino/teste em 90% / 10%

2. Engenharia de Features

Padronização dos dados usando StandardScaler

Preparação do conjunto para modelos baseados em distância (como SVM)

3. Modelagem

Implementação do algoritmo SVC (Support Vector Classifier)

Treinamento com dados balanceados

Avaliação com matriz de confusão e métricas clássicas

# 📈 Resultados
## ➡️ Métricas do Modelo

Acurácia: 80,5%

Precisão (classe positiva): 82,4%

Recall (classe positiva): 77,8%

Esses resultados indicam que o modelo possui bom equilíbrio entre identificar corretamente os doadores que retornarão e evitar falsos positivos.

## ➡️ Interpretação

O modelo funciona bem para campanhas de previsão simples.

A sensibilidade (recall) é especialmente importante em hemocentros — o modelo atingiu um bom valor inicial.

Há potencial de melhoria com modelos como Random Forest ou Gradient Boosting.
