# Departamento de Relações Publicas

>   Contratar e reter funcionários são tarefas extremamente complexas que exigem capital, tempo e habilidades.
>   Pequenos empresários gastam em torno de 40% das horas de trabalho em tarefas que não geram receitas, como a contratação.
>   “Pequenos empresários gastam em torno de 40% das horas de trabalho em tarefas que não geram receitas, como a contratação”.
>   “Empresas gastam de 15% a 20% do salário dos funcionários para recrutar um novo candidato”
>   “Uma empresa média perde entre 1% e 2.5% de sua receita total no tempo que leva para treinar um novo funcionário”
>   A contratação de um novo funcionário custa em média $7645 (em uma empresa com aproximadamente 500 funcionários)
>   Demora mais ou menos 52 dias para um funcionário ocupar de fato sua nova posição   

-   **Você trabalha como cientista de dados para uma empresa**

-   **O departamento de RH coletou dados dos funcionários e gostaria que você
    fizesse a previsão de quais são mais propensos para sair do emprego**

-   **Alguns exemplos de dados:**

    -   **Envolvimento com o trabalho**

    -   **Escolaridade**

    -   **Satisfação com o trabalho**

    -   **Métricas de desempenho**

    -   **Relacionamento**

    -   **Equilíbrio entre atividades pessoais e profissionais.**

Fonte: <https://toggl.com/blog/cost-of-hiring-an-employee>

Fonte dos dados:
https://**[www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset](http://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset)**

1.  **REGRESSÃO LOGÍSTICA**

-   **Regressão linear** é usada para prever números

    -   Exemplo: previsão de lucros baseado na temperatura

-   **Regressão logística** é usada para prever saídas binárias

    -   Uma das duas classes: aprovado/reprovado, ganhar/perder, saudável/doente
    
![Regressão Logística](https://github.com/callacius/Data_Science_RH/blob/main/images/01.png?raw=true)

-   Primeiro, utiliza uma equação linear
-   Converte o valor em uma probabilidade (valores entre 0 e 1)

![Regressão Logística](https://github.com/callacius/Data_Science_RH/blob/main/images/02.png?raw=true)

-   Conversão para probabilidade
![Regressão Logística](https://github.com/callacius/Data_Science_RH/blob/main/images/03.png?raw=true)

2.  **RANDOM FOREST**

-   Classificar se uma pessoa pode se aposentar baseado nas economias e idade
-   Random Forest é considerado com conjunto de algoritmos (ensemble)
-   Cria um conjunto de árvores de decisão baseados em atributos randômicos
-   Combina os votos de diferentes árvores de decisão
![Random Forest](https://github.com/callacius/Data_Science_RH/blob/main/images/04.png?raw=true)

3.  **REDES NEURAIS ARTIFICIAIS**

![Redes Neurais Artificiais](https://github.com/callacius/Data_Science_RH/blob/main/images/05.png?raw=true)

**MATRIZ DE CONFUSÃO**
![Redes Neurais Artificiais](https://github.com/callacius/Data_Science_RH/blob/main/images/06.png?raw=true)

KPIs (KEY PERFORMANCE INDICATORS)
    -   True positives (TP): quando o classificador previu TRUE (tem a doença), e  a classe correta era TRUE (tem a doença)
    -   True negatives (TN): quando o modelo previu FALSE (não tem a doença), e a classe correta era FALSE (não tem a doença)
    -   False positives (FP) (Type I error): classificador previu TRUE, mas a classe  correta era FALSE (não tem a doença) 
    -   False negatives (FN) (Type II error): classiﬁcador previu FALSE (não tem a doença), mas na verdade o paciente tem a doença
    -   Classiﬁcation Accuracy = (TP+TN) / (TP + TN + FP + FN)
    -   Precision = TP/Total TRUE Predictions = TP/ (TP+FP) - quando o modelo  previu TRUE, o quanto a previsão estava correta?
    -   Recall = TP/ Actual TRUE = TP/ (TP+FN) (quando a classe era TRUE, o quanto o classificador estava correto?)
 
**PRECISION VS. RECALL**

![Redes Neurais Artificiais](https://github.com/callacius/Data_Science_RH/blob/main/images/08.png?raw=true)
![Redes Neurais Artificiais](https://github.com/callacius/Data_Science_RH/blob/main/images/07.png?raw=true)
    -   Classiﬁcation Accuracy = (TP+TN) / (TP + TN + FP + FN) = 91%
    -   Precision = TP/Total TRUE Predictions = TP/ (TP+FP) = ½=50% (quando o  modelo prevê a doença, ele está correto em 50% dos casos)
    -   Recall = TP/ Actual TRUE = TP/ (TP+FN) = 1/9 = 11% (o modelo identifica corretamente 11% dos pacientes doentes)
    
**F1-SCORE**

-   F1 Score combina precision e recall
-   Média harmônica de precision e recall
-   Em dados desbalanceados, se tivermos um grande número  de verdadeiros negativos (true negatives – pacientes  saudáveis), o accuracy será enganador. Nesse caso, F1 é uma  métrica melhor por prover um “balanceamento” entre  precision e recall

![Redes Neurais Artificiais](https://github.com/callacius/Data_Science_RH/blob/main/images/09.png?raw=true)

Fonte: ![Curso Udemy](**https://www.udemy.com/course/ciencia-de-dados-para-empresas-e-negocios**?raw=true)
