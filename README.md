# Machine Learning Diabetes Study

Estudo prático de Machine Learning Supervisionado desenvolvido durante um curso de Inteligência Artificial. O projeto compara diferentes algoritmos de classificação aplicados à predição de diabetes utilizando Python, Pandas, Matplotlib, Seaborn, Numpy, Scikit-Learn e XGBoost.

## Sobre o projeto

Este projeto foi desenvolvido como parte de um estudo prático durante um curso de Inteligência Artificial e Ciência de Dados.

O objetivo foi compreender as principais etapas de um projeto de Machine Learning, desde a análise exploratória dos dados até o treinamento, ajuste e avaliação de diferentes modelos de classificação.

Ao longo do projeto, foram testados diferentes algoritmos clássicos de Machine Learning, comparando seus desempenhos por meio de acurácia, matriz de confusão e análise dos verdadeiros positivos.

## Etapas realizadas

- Importação e exploração dos dados
- Estatísticas descritivas
- Visualização das distribuições
- Separação entre conjuntos de treino e teste
- Padronização dos dados quando necessário
- Treinamento de diferentes modelos de Machine Learning
- Ajustes de hiperparâmetros
- Geração de previsões
- Avaliação dos modelos utilizando matriz de confusão e acurácia
- Comparação entre diferentes algoritmos de classificação

## Tipo de problema

Todos os algoritmos implementados neste projeto pertencem à categoria de **Machine Learning Supervisionado para Classificação**.

O objetivo é prever se um paciente possui ou não diabetes, utilizando a variável alvo **Outcome**, caracterizando um problema de **classificação binária**, no qual existem apenas duas classes possíveis:

- **0** → Paciente sem diabetes
- **1** → Paciente com diabetes

Todos os modelos foram treinados utilizando a mesma base de dados e avaliados nas mesmas condições, permitindo uma comparação justa entre seus desempenhos.

## Modelos de Classificação Testados

- K-Nearest Neighbors (KNN)
- Naive Bayes
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- XGBoost

Cada modelo foi analisado considerando não apenas a **acurácia**, mas também a **matriz de confusão** e o comportamento na identificação de **verdadeiros positivos**, permitindo uma avaliação mais completa do desempenho de cada algoritmo.

## Resultados - KNN

* Após ajustes nos hiperparâmetros do modelo KNN, a acurácia aumentou de **76% para 78%**.
* Durante o desenvolvimento do projeto foi analisada a limitação da acurácia como métrica única de avaliação, especialmente em bases de dados médicas.
* Apesar da melhoria na acurácia, o modelo apresentou desempenho inferior na identificação de verdadeiros positivos quando comparado a outros algoritmos testados.

## Resultados - Naive Bayes

* O modelo Naive Bayes obteve **76% de acurácia**.
* Embora tenha apresentado uma acurácia inferior a outros modelos, foi um dos algoritmos com melhor desempenho na identificação de verdadeiros positivos.
* Esse comportamento pode ser interessante em aplicações médicas, onde reduzir a quantidade de falsos negativos costuma ser um fator importante.

## Resultados - Support Vector Machine (SVM)

* O modelo SVM apresentou inicialmente **78% de acurácia**.
* Foi utilizado o kernel padrão **RBF**, realizando posteriormente o ajuste do parâmetro **C** para **0.3**.
* Após esse ajuste, a acurácia aumentou para **79%**, tornando-se um dos melhores resultados gerais entre os modelos testados.
* Entretanto, o aumento da acurácia ocorreu acompanhado de uma redução na quantidade de verdadeiros positivos.

## Resultados - Decision Tree

* O modelo Decision Tree apresentou inicialmente **70% de acurácia**.
* Após ajustes no modelo, a acurácia aumentou para **77%**.
* A Árvore de Decisão se destacou pela interpretabilidade, permitindo compreender melhor como as variáveis influenciam a classificação.
* Apesar da melhoria, seu desempenho geral permaneceu abaixo dos modelos com melhor acurácia no projeto.

## Resultados - Random Forest

* O modelo Random Forest obteve **78% de acurácia**.
* O algoritmo utiliza múltiplas Árvores de Decisão, combinando suas previsões para gerar um resultado mais robusto.
* Apesar de não superar o SVM e o XGBoost em acurácia, apresentou desempenho estável e competitivo.

## Resultados - XGBoost

* O modelo XGBoost apresentou o melhor desempenho geral entre os modelos testados.
* A acurácia final foi de **80%**.
* O modelo também apresentou **57 verdadeiros positivos**, mostrando forte capacidade de identificar corretamente casos positivos de diabetes.
* Esse resultado foi especialmente relevante porque combinou a maior acurácia geral com bom desempenho na classificação da classe positiva.

## Comparação dos modelos

| Modelo        | Acurácia | Observações                                               |
| ------------- | -------: | --------------------------------------------------------- |
| KNN           |      78% | Melhor desempenho após ajuste de hiperparâmetros.         |
| Naive Bayes   |      76% | Bom desempenho na identificação de verdadeiros positivos. |
| SVM           |      79% | Alta acurácia após ajuste do parâmetro C.                 |
| Decision Tree |      77% | Evoluiu de 70% para 77% após ajustes.                     |
| Random Forest |      78% | Modelo estável baseado em múltiplas árvores de decisão.   |
| XGBoost       |  **80%** | Melhor acurácia geral e 57 verdadeiros positivos.         |

## Conclusões

* O projeto demonstrou que a acurácia, sozinha, não é suficiente para definir o melhor modelo em um problema de classificação médica.
* O Naive Bayes apresentou bom desempenho na identificação de verdadeiros positivos, mesmo com menor acurácia geral.
* O SVM obteve uma acurácia alta, mas sacrificou parte dos verdadeiros positivos.
* A Decision Tree teve uma evolução significativa após ajustes, aumentando sua acurácia de 70% para 77%.
* O Random Forest apresentou um resultado estável, empatando com o KNN em acurácia.
* O XGBoost foi o modelo com melhor desempenho geral, alcançando **80% de acurácia** e **57 verdadeiros positivos**.
* Para este tipo de problema, especialmente por envolver dados médicos, é importante considerar métricas além da acurácia, como verdadeiros positivos, falsos negativos, precision, recall e F1-score.

## Objetivo de aprendizado

Este projeto teve como foco o aprendizado dos conceitos fundamentais de Machine Learning e do fluxo completo de desenvolvimento de modelos preditivos utilizando bibliotecas como Scikit-Learn e XGBoost.

## Observação

*Este projeto foi desenvolvido como parte de um estudo guiado durante um curso de Inteligência Artificial, com o objetivo de praticar análise de dados, pré-processamento, treinamento, ajuste e avaliação de modelos de classificação.*
