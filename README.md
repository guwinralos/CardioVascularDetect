# 🫀 CardioVascularDetect: Previsão de Risco de Doença Cardíaca com Machine Learning

Este repositório contém um projeto voltado para o uso de **Machine Learning** na previsão de **riscos de doenças cardiovasculares**. O objetivo é desenvolver modelos preditivos que auxiliem profissionais da saúde na **identificação precoce de pacientes com alto risco**, reforçando ações preventivas e diagnósticos mais assertivos.

---

## 🎯 Objetivo do Projeto

As doenças cardiovasculares estão entre as principais causas de morte no mundo. A detecção precoce e a prevenção são fundamentais para reduzir esse impacto. Este projeto propõe a aplicação de algoritmos de Aprendizado de Máquina para:

- Analisar dados clínicos estruturados
- Prever a probabilidade de ocorrência de doenças cardíacas
- Suportar decisões médicas com uma ferramenta inteligente e acessível

---

## 📊 Dataset Utilizado

O modelo foi treinado com o [Cardiovascular Disease Dataset do Kaggle](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset), que contém:

- ✅ 70.000+ registros de pacientes
- ✅ 11 variáveis clínicas (idade, peso, colesterol, glicose, pressão arterial, etc.)
- ✅ 1 variável-alvo binária (`cardio`: 0 - sem doença, 1 - com doença)

---

## ⚙️ Modelagem e Resultados

Foi utilizado o algoritmo **Random Forest**, que obteve **73% de acurácia** no conjunto de testes.

### 🔢 Matriz de Confusão
[[8387 2364] [3201 7048]]


| Métrica              | Valor |
|----------------------|-------|
| Verdadeiros Negativos (TN) | 8387 |
| Falsos Positivos (FP)      | 2364 |
| Falsos Negativos (FN)      | 3201 |
| Verdadeiros Positivos (TP) | 7048 |

### 📊 Relatório de Classificação

| Classe | Precisão | Recall | F1-Score |
|--------|----------|--------|----------|
| 0 (Sem Doença) | 0.72 | 0.78 | 0.75 |
| 1 (Com Doença) | 0.75 | 0.69 | 0.72 |

> 💡 Observação: Os 3201 falsos negativos representam um desafio crítico em aplicações médicas, reforçando a importância de ajustes futuros no modelo.

---

## 🛠️ Próximos Passos

Para aprimorar a performance e confiabilidade do modelo, serão exploradas as seguintes melhorias:

- 🔍 **Tratamento de Outliers e Inconsistências**
- 🧠 **Engenharia de Features** (ex: cálculo de IMC)
- ⚙️ **Otimização de Hiperparâmetros**
- 🔄 **Comparação com Outros Algoritmos** (SVM, XGBoost, Redes Neurais)
- 🌐 **Explicabilidade do Modelo** com ferramentas como SHAP ou LIME

---

## 📌 Conclusão

Este projeto demonstra o potencial do uso de Machine Learning como ferramenta auxiliar na área da saúde. Apesar das limitações iniciais, como a alta taxa de falsos negativos, os resultados indicam um caminho promissor rumo à **inovação em diagnóstico médico**. Contribuições e melhorias são bem-vindas!

---

## 📬 Contato

Para dúvidas, sugestões ou colaboração, entre em contato com [Seu Nome ou Equipe].

---
