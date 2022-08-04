# Classificação de Drogas

Neste projeto, será utilizado modelos de machine learning para prever qual é o tipo de droga está presente no paciente, assim será usado este dataset obtido no kaggle (que pode ser obtido clicando [aqui](https://www.kaggle.com/datasets/prathamtripathi/drug-classification)).

Assim, será feito a análise exploratória, o pré-processamento, a modelagem e comparação das métrica para verificar qual modelo teve a melhor perfomace.

## Análise Exploratória

O dataset é formado pelas variaveis abixo mais a target mostrando o tipo de droga.

![image](https://user-images.githubusercontent.com/39843884/182940387-5a68e1be-12dc-4ce3-8caf-a58e5b6bd035.png)

o dataset tem 200 linhas e 6 colunas, indicando que a separação em teste e treino não seria a melhor opção será utilizar *cross validation*.

Podemos ver que em se tratadon do target podemos ver que temos mais drogas y, como podemos ver:

![image](https://user-images.githubusercontent.com/39843884/182941142-373dd8c3-3d5b-4fff-9390-0ba1453b9950.png)

Vendo por este gráfico de dispersão vale ver que, com a razão do sódio co potássio acima de 15, temos só drugy, comparado em relação aos demais

![image](https://user-images.githubusercontent.com/39843884/182941291-6a5d2b3c-bfa8-4ec7-b42b-13a7112f3ffd.png)

Em relação a idade, podemos ver a droga b aparece a partir dos 50 anos e a droga a aparece dos 50 para baixo

![image](https://user-images.githubusercontent.com/39843884/182941725-ad6e341f-a47b-4d2f-b178-f4460595eadf.png)

Com relação ao colesterol, verifica-se que a droga x aparace mais em que tem colesterol normal.

![image](https://user-images.githubusercontent.com/39843884/182942059-16e5d1c8-7e39-407f-ac0f-81005e81090b.png)

## Modelagem

Feito o pré-processamento, foi aplicado *cross-validation*, por temos pouca linhas no dataset, assim foi dividido em 5 folds, e dentre os resultados os que tiveram a melhor performace foi a árvore de decisão e o random forest, no qual foi escolhido arvore de decisão por conta do processamento no qual teve as seguintes métrica (no caso a média).

![image](https://user-images.githubusercontent.com/39843884/182943067-cb120295-85af-4e98-96b2-523fdd606858.png)

## Conclusão

Temos então que o modelo teve uma boa perfomace, indicando que o modelo tem um bom potencial para classificar o tipo de droga, mas devemos nos atentar ao
fato de que como temo poucos dados seria necssário colher mais dados para verificar termo uma dimensão maior de como ocorre a sua distribuição.





