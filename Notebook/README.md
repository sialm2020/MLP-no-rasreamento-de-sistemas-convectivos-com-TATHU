
Esta pasta contém os notebooks utilizados para treinar, avaliar e visualizar os resultados da rede neural MLP.

O notebook principal é:

```text
trainMLP_TATHU_colab.ipynb

O notebook utiliza o arquivo processado disponível na pasta data/. Assim, não é necessário executar novamente a etapa de detecção e rastreamento dos sistemas convectivos com o TATHU para reproduzir o treinamento da MLP.

Esse notebook realiza as seguintes etapas:

leitura do dataset processado;
separação temporal dos dados em treino, validação e teste;
normalização das variáveis de entrada e saída;
definição da arquitetura da MLP;
treinamento com early stopping;
avaliação no conjunto de teste;
comparação com o baseline de persistência;
geração de gráficos e tabelas de desempenho.
