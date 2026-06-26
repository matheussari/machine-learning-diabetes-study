# Machine Learning Diabetes Study

Estudo prático de Machine Learning desenvolvido durante um curso de Inteligência Artificial e Ciência de Dados, utilizando Python, Pandas e Scikit-Learn para classificação de casos de diabetes.

# Projeto de Classificação de Diabetes com Machine Learning

## Sobre o projeto

Este projeto foi desenvolvido como parte de um estudo prático durante um curso de Inteligência Artificial e Ciência de Dados.

O objetivo foi compreender as principais etapas de um projeto de Machine Learning, desde a análise exploratória dos dados até o treinamento, ajuste e avaliação de diferentes modelos de classificação.

## Ferramentas utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

## Etapas realizadas

* Importação e exploração dos dados
* Estatísticas descritivas
* Visualização das distribuições
* Separação entre conjuntos de treino e teste
* Padronização dos dados quando necessário
* Treinamento de diferentes modelos de Machine Learning
* Geração de previsões
* Avaliação dos modelos utilizando matriz de confusão e acurácia

# Resultados - KNN

* Após ajustes nos hiperparâmetros do modelo KNN, a acurácia aumentou de **76% para 78%**.
* Durante o desenvolvimento do projeto foi analisada a limitação da acurácia como métrica única de avaliação, especialmente em bases de dados médicas.
* Apesar da melhoria na acurácia, o modelo apresentou desempenho inferior na identificação de verdadeiros positivos quando comparado a outros algoritmos testados.

# Resultados - Naive Bayes

* O modelo Naive Bayes obteve **76% de acurácia**.
* Embora tenha apresentado uma acurácia inferior ao KNN e ao SVM, foi o algoritmo que identificou a maior quantidade de verdadeiros positivos entre os modelos avaliados.
* Esse comportamento pode ser interessante em aplicações médicas, onde reduzir a quantidade de falsos negativos costuma ser um fator importante.

# Resultados - Support Vector Machine (SVM)

* O modelo SVM apresentou inicialmente **78% de acurácia**.
* Foi utilizado o kernel padrão **RBF**, realizando posteriormente o ajuste do parâmetro **C** para **0.3**.
* Após esse ajuste, a acurácia aumentou para **79%**, tornando-se o melhor resultado geral entre os modelos testados.
* Entretanto, o aumento da acurácia ocorreu acompanhado de uma redução na quantidade de verdadeiros positivos.

# Comparação dos modelos

| Modelo      | Acurácia | Observações                                       |
| ----------- | -------: | ------------------------------------------------- |
| KNN         |      78% | Melhor desempenho após ajuste de hiperparâmetros. |
| Naive Bayes |      76% | Maior quantidade de verdadeiros positivos.        |
| SVM         |  **79%** | Maior acurácia geral após ajuste do parâmetro C.  |

# Conclusões

* O modelo KNN apresentou potencial para novos ajustes de hiperparâmetros, indicando possibilidade de melhoria futura.
* O SVM alcançou a maior acurácia entre os modelos avaliados, porém apresentou redução na quantidade de verdadeiros positivos.
* O Naive Bayes demonstrou um desempenho bastante interessante ao identificar corretamente um maior número de pacientes com diabetes, mesmo apresentando menor acurácia geral.
* Este projeto reforçou a importância de avaliar diferentes métricas de desempenho, mostrando que a escolha do melhor modelo depende do objetivo da aplicação e não apenas da acurácia.

# Objetivo de aprendizado

Este projeto teve como foco o aprendizado dos conceitos fundamentais de Machine Learning e do fluxo completo de desenvolvimento de modelos preditivos utilizando a biblioteca Scikit-Learn.

# Observação

*Este projeto foi desenvolvido como parte de um estudo guiado durante um curso de Ciência de Dados e Inteligência Artificial, com o objetivo de praticar análise de dados, pré-processamento, treinamento e avaliação de modelos de classificação utilizando Scikit-Learn.*

