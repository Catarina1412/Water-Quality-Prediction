# Water Quality Prediction
 
 **EN**
_In this repository, you will find various files related to a completed project. Included are a detailed project report, the dataset used, and the Python code implementing the project._

Files:
* [Water Potability.ipynb](<Water Potability.ipynb>): contains the Jupyter notebook with the project code
* [water_potability.xls](water_potability.xls): contains the data used in the project
* [Water Quality Prediction Report.pdf](<Water Quality Prediction Report.pdf>): project report in English
* [Relatório da Previsão da Qualidade da Água.pdf](<Relatório da Previsão da Qualidade da Água.pdf>): project report in Portuguese

**Objective:**

This project aimed to analyze the "Drinking Water Probability" dataset with the goal of predicting whether a water sample is potable or not (1 or 0).

**Dataset Description:**

Accessibility to clean drinkable water is essential for health and a fundamental human right, playing a crucial role in health and development at national, regional, and local levels. In some regions, it has been demonstrated that investments in water supply and sanitation can yield economic benefits, as the reductions in adverse health effects and health costs outweigh the costs of implementing interventions.
The file water_potability.csv contains information on 9 metrics related to water quality for 3276 distinct water samples: pH value, Hardness, Total Dissolved Solids (TDS), Chloramines, Sulfate, Conductivity, Organic Carbon, Trihalomethanes and Turbidity.

**Project Description:**

The project followed several stages, including:

_Data Exploration:_ Statistical analysis of features, representation of water distribution (potable/non-potable) through a pie chart from the plotly.express library, and studying water distribution in each column using the kdeplot method from the seaborn library. A correlation analysis of the data was also conducted.

_Pre-processing:_ Identification of missing values and outliers, with illustrations to easy visualization. Missing values were treated using the KNN Imputer method from the scikit-learn library, with k=10. Regarding outliers, after analysis, it was decided not to treat them as they were considered plausible values.

_Models:_ The data were split into X_train, X_test, y_train, and y_test sets, reserving 30% of the data for testing. The need to scale the data was identified. Subsequently, three models were used: SVC, MLP Classifier, and Random Forest, with GridSearchCV and Cross-validation.

_Results:_ Among the evaluated models, Random Forest achieved the best results, with an accuracy of 0.678.




**PT**
_Neste repositório, encontrar-se-ão diversos ficheiros relacionados com um projeto concluído. Incluem-se um relatório detalhado do projeto, o conjunto de dados utilizado e o código em Python da implementação do projeto._

Ficheiros:
* [Water Potability.ipynb](<Water Potability.ipynb>): contém o jupyter notebook com o código do projeto
* [water_potability.xls](water_potability.xls): contém os dados usados no projeto
* [Water Quality Prediction Report.pdf](<Water Quality Prediction Report.pdf>): relatório do projeto em inglês
* [Relatório da Previsão da Qualidade da Água.pdf](<Relatório da Previsão da Qualidade da Água.pdf>): relatório do projeto em português

**Objetivo:**

Este projeto teve como propósito a análise do conjunto de dados "Drinking Water Probability" com o intuito de prever se uma amostra de água é potável ou não (1 ou 0).

**Descrição do Dataset:**

A acessibilidade à água potável é essencial para a saúde e um direito humano básico, sendo muito importante como uma questão de saúde e desenvolvimento a nível nacional, regional e local. Em algumas regiões, foi demonstrado que os investimentos em abastecimentos de água e saneamento podem gerar um benefício económico, visto que as reduções nos efeitos adversos à saúde e nos custos de saúde superam os custos de realização das intervenções.
O ficheiro water_potability.csv contém informações sobre 9 métricas relacionadas à qualidade da água, referentes a 3276 amostras de água distintas: Valor de pH, Dureza, Sólidos (Total de sólidos dissolvidos - TDS), Cloraminas, Sulfato, Condutividade, Carbono Orgânico, Trihalometanos e Turbidez.

**Descrição do Projeto:**

O projeto seguiu várias etapas, incluindo:

_Exploração de dados:_ Análise estatística das features , representação da distribuição de água (potável/não potável) através de um pie chart da biblioteca plotly.express e estudo da distribuição da água em cada coluna usando o método kdeplot da biblioteca seaborn. Também foi realizada uma análise da correlação dos dados.

_Pré-processamento:_ Identificação de valores em falta e outliers, com ilustrações para facilitar a visualização. Os valores em falta foram tratados utilizando o método KNN Imputer da biblioteca scikit-learn, com k=10. Quanto aos outliers, após análise, optei por não os tratar, pois eram considerados valores plausíveis.

_Modelos:_ Os dados foram divididos em conjuntos X_train, X_test, y_train e y_test, reservando 30% dos dados para teste. Verificou-se a necessidade de escalar os dados. Posteriormente, foram utilizados três modelos: SVC, MLP Classifier e Random Forest, com GridSearchCV e Cross-validation.

_Resultados:_ Entre os modelos avaliados, o Random Forest obteve os melhores resultados, alcançando uma accuracy de 0.678.
