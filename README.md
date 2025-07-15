# CardioVascularDetect
Previsão de Risco de Doença Cardíaca Utilizando Aprendizado de Máquina

Este repositório contém um projeto abrangente focado na previsão do risco de doenças cardiovasculares utilizando técnicas de Aprendizado de Máquina (Machine Learning). O objetivo é desenvolver e avaliar modelos preditivos que possam auxiliar profissionais da saúde no diagnóstico precoce e na identificação de pacientes em alto risco.

🎯 Objetivo do Projeto
As doenças cardiovasculares são uma das principais causas de mortalidade global. A prevenção e o diagnóstico precoce são ferramentas essenciais para a saúde pública. Este projeto visa aplicar algoritmos de Machine Learning para analisar dados clínicos e prever se um paciente tem alto risco de desenvolver uma doença cardíaca, oferecendo uma ferramenta de apoio robusta para decisões clínicas.

📊 Dataset
O estudo utiliza o dataset "Cardiovascular Disease dataset" (link: https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset) disponível no Kaggle. Este conjunto de dados contém:

+70.000 registros de pacientes.

11 variáveis clínicas (idade, peso, pressão arterial, colesterol, glicose, gênero, fumante, consumo de álcool, atividade física, etc.).

Uma variável-alvo binária (cardio) indicando a presença (1) ou ausência (0) de doença cardiovascular.

📈 Resultados
O modelo Random Forest alcançou uma acurácia geral de 73% no conjunto de teste.

Matriz de Confusão:

[[8387 2364]
 [3201 7048]]
Verdadeiros Negativos (TN): 8387 (pacientes sem doença cardíaca corretamente classificados)

Falsos Positivos (FP): 2364 (pacientes sem doença cardíaca classificados incorretamente como tendo)

Falsos Negativos (FN): 3201 (pacientes com doença cardíaca classificados incorretamente como não tendo)

Verdadeiros Positivos (TP): 7048 (pacientes com doença cardíaca corretamente classificados)

Relatório de Classificação:

Classe 0 (Sem Doença Cardíaca):

Precisão: 0.72

Recall: 0.78

F1-Score: 0.75

Classe 1 (Com Doença Cardíaca):

Precisão: 0.75

Recall: 0.69

F1-Score: 0.72

O modelo demonstra um bom desempenho geral. É importante notar a presença de Falsos Negativos (3201 casos), que representam pacientes com doença cardíaca não detectada, um ponto crítico em diagnósticos médicos. No entanto, a performance é satisfatória para uma aplicação inicial e tem potencial como ferramenta auxiliar no diagnóstico precoce.

💡 Conclusões e Próximos Passos
Este estudo demonstra a viabilidade do uso de aprendizado de máquina para prever o risco de doenças cardíacas. Um ponto crucial que emergiu da análise exploratória foi a necessidade crítica de dados de alta qualidade. Inconsistências em variáveis como 'Pressão sanguínea' ressaltam que a limpeza e validação de dados são pré-requisitos indispensáveis para a construção de modelos preditivos confiáveis na área da saúde.

Próximos passos podem incluir:

Tratamento de Outliers e Inconsistências: Implementar métodos mais robustos para lidar com valores anômalos, especialmente nas variáveis de pressão arterial.

Engenharia de Features: Criar novas features a partir das existentes que possam melhorar o poder preditivo do modelo (ex: BMI = peso / (altura em m)^2).

Otimização de Hiperparâmetros: Ajustar os hiperparâmetros do modelo Random Forest (ou de outros modelos como XGBoost e Redes Neurais, que foram mencionados na introdução mas não detalhados no código fornecido) para maximizar a performance.

Exploração de Outros Modelos: Aprofundar a análise com os outros modelos mencionados (Regressão Logística, SVM, XGBoost, Rede Neural Artificial) e comparar seus resultados de forma mais exaustiva.

Interpretabilidade do Modelo: Utilizar técnicas como SHAP ou LIME para entender quais features são mais importantes nas predições do modelo.

