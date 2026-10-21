1. Objetivo do Projeto
O objetivo principal deste projeto é desenvolver, treinar e avaliar um modelo preditivo de aprendizado de máquina (Machine Learning) capaz de classificar o risco de diabetes em pacientes com base em variáveis clínicas, demográficas e de estilo de vida.
Além disso, busca-se analisar quais fatores estão mais fortemente associados a diferentes níveis de risco (Baixo, Moderado ou Alto)


2. Pergunta de Pesquisa
É possível prever com precisão o nível de risco de diabetes de um paciente (Baixo, Moderado ou Alto) utilizando dados demográficos, hábitos de vida e exames laboratoriais básicos e qual é o desempenho de um modelo de Regressão Logística nessa tarefa?


3. Metodologia

A execução do projeto segue um fluxo padrão de ciência de dados estruturado nas seguintes etapas:

3.1 Aquisição e Carregamento dos Dados: Os dados foram obtidos através do Kaggle (mansiaggarwal88/diabetes-risk-prediction), totalizando um conjunto de 15.000 registros e 19 colunas (entre variáveis numéricas e categóricas).

3.2 Análise Exploratória e Tratamento de Dados (EDA & Pré-processamento): Identificação e tratamento de valores ausentes (missing values) nas colunas smoking_status, alcohol_consumption e income_bracket.
Análise descritiva das distribuições estatísticas das variáveis numéricas e categóricas.
Mapeamento da variável alvo diabetes_risk em três categorias ordinais: Low (Baixo - 60%), Moderate (Moderado - 25%) e High (Alto - 15%).

3.3 Engenharia de Atributos (Feature Engineering): Exclusão de colunas irrelevantes para o aprendizado (como o identificador patient_id).
Codificação de variáveis categóricas através de One-Hot Encoding.
Padronização (Standard Scaling) das variáveis numéricas para otimizar o desempenho do algoritmo.

3.4 Modelagem Preditiva: Divisão dos dados em conjuntos de treino (80% / 12.000 amostras) e teste (20% / 3.000 amostras), com estratificação para manter a proporção das classes.
Treinamento de um classificador base utilizando o algoritmo de Regressão Logística (configurado com a estratégia One-vs-Rest).

3.5 Avaliação de Desempenho: Utilização de métricas como Acurácia, Matriz de Confusão, Relatório de Classificação (Precisão, Recall e F1-Score) por classe.
Validação cruzada de 5 pastas (5-fold cross-validation) para garantir a robustez e estabilidade da acurácia média do modelo (alcançando cerca de 77.5% de acurácia).
