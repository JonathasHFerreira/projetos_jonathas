1. Objetivo do Projeto
O objetivo principal deste projeto é desenvolver, avaliar e comparar modelos de aprendizado de máquina voltados para a classificação e identificação preditiva de transações fraudulentas, visando mitigar riscos operacionais, otimizar a acurácia na tomada de decisão e reduzir a carga cognitiva ou erros em sistemas automatizados de detecção de anomalias financeiras.

2. Pergunta de Pesquisa
Como modelos supervisionados e não supervisionados de aprendizado de máquina podem ser otimizados e comparados para maximizar a detecção de fraudes financeiras, mantendo taxas aceitáveis de falsos positivos em cenários de alta desproporção de classes (dados desbalanceados)?

3. Metodologia
A metodologia do projeto é estruturada em etapas sequenciais de ciência de dados e engenharia analítica:

Coleta e Pré-processamento de Dados:
Importação e inspeção inicial do conjunto de dados transacionais.
Tratamento de valores ausentes, remoção de duplicatas, codificação de variáveis categóricas e normalização ou padronização de atributos numéricos.

Análise Exploratória de Dados (AED):
Investigação da distribuição das variáveis e identificação do grau de desbalanceamento das classes (fraude versus transações legítimas).
Mapeamento de correlações e análise de multicolinearidade para seleção dos atributos mais relevantes (feature engineering).

Tratamento de Desbalanceamento:
Aplicação de técnicas de amostragem — como subamostragem (undersampling), sobreamostragem (oversampling, ex: SMOTE) ou ajustes de pesos nas classes — para evitar o viés dos algoritmos em direção à classe majoritária.

Modelagem Preditiva (Treinamento e Validação):
Divisão do conjunto de dados em subconjuntos de treino, validação e teste.
Implementação de algoritmos de classificação (como Regressão Logística, Árvores de Decisão, Random Forest, XGBoost ou modelos equivalentes adequados ao problema).
Validação cruzada (cross-validation) para garantir a robustez e a generalização dos modelos.

Avaliação de Desempenho:
Utilização de métricas adequadas a problemas altamente desbalanceados, com foco especial na Área sob a Curva ROC (ROC-AUC), Precisão, Revocação (Recall), F1-Score e na análise da matriz de confusão para minimizar impactos de falsos alarmes.
