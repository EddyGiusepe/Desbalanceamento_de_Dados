# Problemas de Viés e Desbalanceamento de Amostras na Ciência de Dados

O problema de viés é amplamente discutido na área de Ciência de Dados, visto que esse problema pode estar presente em todas as etapas da análise de dados:

* **Na geração dos dados:** nesse caso, o viés já é adicionado desde o processo de obtenção dos Dados, ou seleção das amostras.

* **Na implementação dos modelos:** ao implementar um modelo de _Machine Learning_ com um desbalanceamento nas amostras de treinamento, o nosso modelo poderá ficar enviesado.

* **Na interpretação dos dados:** trata-se do viés humano; ou seja, é possível que, de acordo com a nossa tendência de enxergar aquela análise de uma forma específica, chegamos a conclusões enviesadas na interpretação dos nossos resultados.


Tendo em vista a amplitude do assunto, esse artigo visa dar ênfase apenas no segundo tipo de viés, ou seja, aquele que pode estar presente no momento da criação do nosso modelo de Machine Learning (ML).

## Entendendo o desbalaceamento de Amostras

Como apresentado anteriormente, o viés contido na implementação de modelos está associado ao desbalanceamento das amostras dos Dados durante o processo de treinamento do modelo. 

### Mas o que seria essa tal "desbalanceamento"?

Imagine que você deseja criar um modelo de ML capaz de identificar, por meio de um conjunto de informações de e-mails, se um e-mail específico se caracteriza como um spam ou não. É bem provável que no seu conjunto de dados de treinamento haja um número muito maior de amostras de e-mails que não são spam, do que amostras que representam em um spam. A figura abaixo representa esse cenário por meio de um gráfico com a contagem das amostras de cada classe.

![image](https://user-images.githubusercontent.com/69597971/152691515-abf571a8-c10d-4b5a-b47d-31612a0a73b2.png)












Links de estudo e DataSet:

* [Dados Desbalanceados](https://sigmoidal.ai/como-lidar-com-dados-desbalanceados/)

* [Problemas de Viés e Desbalanceamento de Amostras na Ciência de Dados](https://letscode-academy.com/blog/problemas-de-vies-e-desbalanceamento-de-amostras-na-ciencia-de-dados)

* [Dataset: bank.zip](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

* [DataSet: creditcard.csv](https://www.dropbox.com/s/b44o3t3ehmnx2b7/creditcard.csv?dl=1)



Thanks God!





