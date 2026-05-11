# Aplicação de MLP no rastreamento de sistemas convectivos com TATHU

Previsão do deslocamento de sistemas convectivos com TATHU e MLP usando imagens GOES-13.

Este repositório contém o dataset processado, notebooks e scripts utilizados no estudo de previsão do deslocamento de sistemas convectivos a partir da integração entre o software TATHU e uma rede neural do tipo Multilayer Perceptron (MLP).

## Objetivo

Avaliar se uma MLP é capaz de prever o deslocamento futuro de sistemas convectivos rastreados pelo TATHU em uma janela temporal de uma hora.

## Metodologia

A metodologia consiste em:

1. utilizar imagens do canal 4 do satélite GOES-13;
2. detectar sistemas convectivos com o TATHU;
3. rastrear os sistemas em imagens consecutivas;
4. extrair atributos físicos e espaciais;
5. construir um dataset supervisionado no formato `t-1 → t → t+1`;
6. treinar uma MLP para prever o deslocamento futuro do centroide;
7. comparar o desempenho da MLP com um baseline de persistência.
