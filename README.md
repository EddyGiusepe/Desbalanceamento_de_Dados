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

Podemos vizualizar, também, num gráfico de Dispersão, assim:

![image](https://user-images.githubusercontent.com/69597971/152691943-011530c3-3349-4b0b-87bc-40fff1bca437.png)

Nesse caso, por ser apresentado ao número muito maior de amostras que não são spam, seu modelo irá ter uma facilidade maior de identificar o que não é um spam. Pelo mesmo motivo, seu modelo terá muito mais dificuldades em identificar o que é um spam, ou mesmo irá ignorar esses casos, o que pode acontecer quando temos uma diferença muito expressiva no número de amostras.

Note o quão grave pode ser esse problema, especialmente, porque em uma aplicação desse tipo, você deve estar mais interessado na classe com o menor número de amostras (_classe minoritária_), e não naquele com mais amostras (_classe majoritária_). A pergunta, então, é: "O que podemos fazer para solucionar esse tipo de problema?". É o que veremos na próxima seção. 

O gráfico a seguir mostra as técnicas empregadas para solucionar esses desbalanceamento. Ver o seguinte site para ver estás técnicas: [Undersampling e Oversampling](https://medium.com/data-hackers/como-lidar-com-dados-desbalanceados-em-problemas-de-classifica%C3%A7%C3%A3o-17c4d4357ef9)

![image](https://user-images.githubusercontent.com/69597971/152692275-b4873e13-d7e4-43b5-b640-f850626359f3.png)

## Técnicas para lidar com o Viés por Desbalanceamento de Amostras

Como foi comentado acima, existem, à princípio, duas técnicas para lidar com esse problema, sobre as quais iremos nos aprofundar nesse artigo:

### Undersampling

De forma simples, essa técnica visa _remover_ as amostras da classe majoritária, até que esta se iguale, em número, às amostras da classe minoritária. Os dois tipos principais de ``undersampling`` são:

* **Random Undersampling:** A escolha dos dados da classe majoritária é feita de forma aleatória.

* **NearMiss:** Elimina-se as amostras "mais próximas" (ou que menos diferem) entre si, de modo a maximizar a variabilidade entre as classes e, também, entre os dados que compõem a própria classe (majoritária). Esse processo é ilustrado pela figura abaixo (para mais detalhes [click aqui](https://dev.to/charfaouiyounes/resampling-to-properly-handle-imbalanced-datasets-in-machine-learning-4anb)).

![image](https://user-images.githubusercontent.com/69597971/152694643-e4fc798e-21be-4265-8bdc-987137d275ee.png)






















Links de estudo e DataSet:

* [Dados Desbalanceados](https://sigmoidal.ai/como-lidar-com-dados-desbalanceados/)

* [Problemas de Viés e Desbalanceamento de Amostras na Ciência de Dados](https://letscode-academy.com/blog/problemas-de-vies-e-desbalanceamento-de-amostras-na-ciencia-de-dados)

* [Dataset: bank.zip](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

* [DataSet: creditcard.csv](https://www.dropbox.com/s/b44o3t3ehmnx2b7/creditcard.csv?dl=1)



Thanks God!





