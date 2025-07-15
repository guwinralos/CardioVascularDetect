CardioVascularDetect: Previsão de Risco de Doença Cardíaca com Machine Learning
Este repositório contém um projeto focado em utilizar Aprendizado de Máquina (Machine Learning) para prever o risco de doenças cardiovasculares. Nosso objetivo é desenvolver e avaliar modelos preditivos que possam auxiliar profissionais da saúde no diagnóstico precoce e na identificação de pacientes em alto risco.

🎯 Objetivo do Projeto
As doenças cardiovasculares são uma das principais causas de mortalidade global. A prevenção e o diagnóstico precoce são ferramentas essenciais para a saúde pública. Este projeto visa aplicar algoritmos de Machine Learning para analisar dados clínicos e prever se um paciente tem um alto risco de desenvolver uma doença cardíaca, oferecendo assim uma ferramenta de apoio robusta para decisões clínicas.

📊 Dataset
O estudo utiliza o "Cardiovascular Disease dataset" disponível no Kaggle: https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset.

Este conjunto de dados contém:

Mais de 70.000 registros de pacientes.

11 variáveis clínicas relevantes, como idade, peso, pressão arterial, níveis de colesterol e glicose, gênero, histórico de tabagismo e consumo de álcool, e nível de atividade física.

Uma variável-alvo binária (cardio) que indica a presença (1) ou ausência (0) de doença cardiovascular.

📈 Resultados Iniciais
Para a previsão, um modelo Random Forest foi treinado e avaliado. Alcançamos uma acurácia geral de 73% no conjunto de teste.

Aqui estão os detalhes da performance:

Matriz de Confusão
[[8387 2364]
 [3201 7048]]
Verdadeiros Negativos (TN): 8387 (pacientes sem doença cardíaca corretamente classificados).

Falsos Positivos (FP): 2364 (pacientes sem doença cardíaca classificados incorretamente como tendo a doença).

Falsos Negativos (FN): 3201 (pacientes com doença cardíaca classificados incorretamente como não tendo a doença).

Verdadeiros Positivos (TP): 7048 (pacientes com doença cardíaca corretamente classificados).

Relatório de Classificação
Classe

Precisão

Recall

F1-Score

0 (Sem Doença)

0.72

0.78

0.75

1 (Com Doença)

0.75

0.69

0.72


Exportar para as Planilhas
O modelo demonstra um bom desempenho geral. Contudo, a presença de 3201 Falsos Negativos (pacientes com doença cardíaca não detectada) é um ponto crítico em diagnósticos médicos. Apesar disso, a performance é satisfatória para uma aplicação inicial e mostra grande potencial como ferramenta auxiliar no diagnóstico precoce.

💡 Conclusões e Próximos Passos
Este estudo inicial valida a aplicação do aprendizado de máquina para prever o risco de doenças cardíacas. Um ponto crucial que aprendemos é a necessidade crítica de dados de alta qualidade. Inconsistências observadas em variáveis como 'Pressão sanguínea' ressaltam que a limpeza e validação dos dados são pré-requisitos indispensáveis para construir modelos preditivos confiáveis na área da saúde.

Para aprimorar o projeto, os próximos passos incluem:

Tratamento de Outliers e Inconsistências: Implementar métodos mais robustos para lidar com valores anômalos, especialmente nas variáveis de pressão arterial.

Engenharia de Features: Criar novas características a partir das existentes (ex: Índice de Massa Corporal - IMC) para melhorar o poder preditivo do modelo.

Otimização de Hiperparâmetros: Ajustar os parâmetros do modelo Random Forest e explorar a otimização de outros modelos como XGBoost e Redes Neurais para maximizar a performance.

Exploração de Outros Modelos: Realizar uma análise mais aprofundada e comparativa com Regressão Logística, Support Vector Machine (SVM), XGBoost e Redes Neurais Artificiais.

Interpretabilidade do Modelo: Utilizar técnicas como SHAP ou LIME para entender quais características são mais importantes nas previsões do modelo, aumentando a confiança e a transparência.

