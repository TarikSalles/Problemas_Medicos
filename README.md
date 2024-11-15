
- **Câncer de Mama (Previsão)**:
    - Junta um trio de modelos (Random Forest, Rede Neural Profunda, Regressão Logistica) para prever, por meio de dados em um dataset .csv, o câncer de mama em pacientes, fazendo também uma limpeza de dados e uma augmentação de dados para a melhor previsão em casos de pacientes do gênero masculino, considerando a raridade da doença para homens.


- **Melanoma Detecção**: 
     - Utiliza de uma rede neural profunda de convolução DenseNet121 com pesos treinados da imagenet para detectar se manchas na pele são melanoma ou não.

- **Preenchimento de Dados de Colesterol Faltante**:
     - Utiliza diversas técnicas para preencher dados faltantes, desde utilizar a técnica de K-nearest neighbors até treinar uma random forest para os preencher, garantindo resultados  com propriedades similares ao esperado.

- **Probabilidade de Sobrevivência Câncer de Mama**: 
     - Utiliza de equações de probabilidade de sobrevivência para analisar a sobrevivência de pacientes ao passar dos anos após o último tratamento ou cirurgia, utiliza técnicas de limpeza de dados e augmentação considerando o tamanho pequeno do dataset original.

- **Risco de Ataque Cardíaco(Prognóstico)**:
     - Analisa resultados de um modelo de regressão logistica com dados de um csv com n variáveis diferentes com base em suas significâncias para o prognóstico, o melhor modelo então é decidido pelos resultados da curva ROC, e verificando também as matrizes de confusão.

- **Segmentação(Átrio Esquerdo)**: 
     - Utiliza do modelo de segmentação popular U-NET com uma profundidade de 3/4 para gerar como resultado n imagens com os possíveis locais do átrio esquerdo com base em diversos dados separados por n segmentos de um coração (cada segmento é uma imagem, e o modelo gera imagens representando cada segmento). É necessário diversos processos para treinar a rede e utilizar os segmentos de forma apropriada, optando-se por somente utilizar uma "fatia" contendo n segmentos dos totais e utilizando somente uma parcela do tamanho original dos segmentos, isso facilita o treino do modelo e ao  mesmo tempo o mostra dados mais variados considerando que essas fatias são randomicamente selecionadas (isso sendo feito com uma porcentagem mínima de píxeis do átrio esquerdo por fatia, Ex: pegar uma fatia com 5 segmentos de tamanho 100x100 de um conjunto de 20 segmentos cada um 500x500, esse segmento possui uma porcentagem de pixeis que são classificados como átrio esquerdo maior ou igual à requisitada e por isso é escolhido). Por fim o modelo é treinado de forma que gere um conjunto de segmentos com as mesmas dimensões do original mostrando as possíveis posições do átrio esquerdo (diferindo com o fundo de cor diferente).


Todos os exemplos são melhor explicados e detalhados em seus respectivos arquivos .ipynb, contendo, além disso, a fonte original dos dados utilizados. 
