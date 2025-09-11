## 🩸 Blood Donation Prediction Project
# 📋 Descrição do Projeto
Este projeto implementa um sistema de predição usando Machine Learning para identificar doadores de sangue que compareceram a uma campanha de doação. Desenvolvido como estudo de caso para a disciplina de Aprendizado de Máquina, o sistema utiliza uma Máquina de Vetores de Suporte (SVM) para classificar doadores com base em seu histórico de doações.

# 🎯 Objetivo
Monitorar estoques de sangue e prever a disponibilidade de doadores, permitindo que hemocentros planejem campanhas de forma mais eficiente e evitem faltas críticas de suprimentos.

# 📊 Base de Dados
O projeto utiliza o arquivo doacao.csv contendo 748 registros com as seguintes variáveis:

Recência: Meses desde a última doação

Frequência: Número total de doações

Quantidade: Volume total doado (em cm³)

Tempo: Meses desde a primeira doação

Doou: Variável alvo (1 = doou, 0 = não doou)

# ⚙️ Metodologia
1. Pré-processamento
Carregamento e limpeza dos dados

Balanceamento do dataset (undersampling para corrigir desbalanceamento de classes)

Divisão em conjuntos de treino e teste (90%/10%)

2. Engenharia de Features
Padronização dos dados (média zero e desvio padrão unitário)

Preparação para o algoritmo SVM

3. Modelagem
Implementação de Support Vector Classifier (SVC)

Treinamento com dados balanceados

Validação com matriz de confusão

# 📈 Resultados
O modelo alcançou os seguintes resultados na matriz de confusão:

Acurácia: 80.5%

Precisão: 82.4% (para classe positiva)

Recall: 77.8% (para classe positiva)
