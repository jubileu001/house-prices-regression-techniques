### Regressão Linear e métodos de regularização

A regularização é um método utilizado para reduzir a quantidade de variáveis (features) em um modelo de regressão. Uma vez que, queremos um modelo que seja muito simples a ponto de não conseguir performar nem mesmo nos dados de treino (underfitting), e que não aprenda a modelar todos os dados de treino e quando chegar um dados novo ele não consegue generalizar (overfitting).

Para isso podem ser utilizadas dois métodos de regularização:
- A Regularização Lasso — também referida como L1 — aplica uma penalização equivalente ao valor absoluto da magnitude dos coeficientes. Resumingo, vai aplicar uma restrição aos coeficientes menos importantes, levando-os a zero.
- Regularização Ridge — ou L2 — funciona de modo semelhando, porém aplicando uma penalização equivalente ao valor ao quadrado da magnitude dos coeficientes. Penalizando os coeficientes que assumem valores muito grandes, levando-os a tender a zero, mas não zerando-os.

A grande diferença aqui é que este tipo não chega a zerar o coeficiente, mas reduz os menos importantes a valores muito baixos e mantendo todos eles no modelo.

Dessa forma, esse projeto tem como objetivo aplicar esses dois tipos de regularização, juntamente com a Regressão Linear e análisar seus desempenhos.

O dataset usado para análise pode ser encontrado nesse link: https://www.kaggle.com/c/house-prices-advanced-regression-techniques