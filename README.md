# Titanic

Case do Kaggle com o objetivo de gerar previsão de quem sobreviveu ou não.

<p align='justify'>Primeiro fiz a parte de análise de dados e entender melhor o meu dataset, minhas variáveis e como as variáveis se relacionam com o variável alvo. Também procurei trabalhar algumas variáveis, criando caregórias, preenchendo linhas vazias etc. Como o dataset não é muito grande - não há nem 1000 linhas, evitei dropar linhas problemáticas, ao invés disso, procurei tratá-las.

<p align='justify'>Depois, verifiquei as variáveis que tiveram alguma correlação com a variável alvo atavés da correlação de Pearson. Essas variáveis foram utilizadas na modelagem. Para modelagem, utilizei os seguintes modelos:
- Logistic Regression
- SVC
- K Neighbors Classifier
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier

<p align='justify'>Em um primeiro momento, rodei os modelos sem paramêtros afim de pré-selecionar os três melhores (a métrica utilizada aqui foi accuracy), que nesse caso foram: Gradient Boosting Classifier, SVC e Logistic Regression. A partir desses três selecionados, fiz um GridSearchCV para dar uma melhor robustez e escolher os melhores parâmetros. A partir daí, fiz o predict no dataset de test para comparar melhor os modelos e junto deles, cada matriz de confusão. O modelo escolhido, foi o Gradient Boosting Classifier. Mas vale ressaltar que os resultados foram bem semelhantes entre as métricas e os modelos.</p>

Todas essas informações, funções e gráficos estão bem detalhadas no notebook. =)
