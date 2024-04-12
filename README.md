# Segmentação de imagens
## Abaixo serão apresentados o passo a passo para a segmentação e classificação da imagem
### Imagem original:
![imagem](https://github.com/PauloHenriqueRod/processamento-de-imagens/assets/96426671/b9459047-07d8-4ae8-ab48-55f286ceb5cd)
## Passo 1:
### Aplicação do filtro gaussiano na etapa de pré processamento da imagem.
![gaussiano](https://github.com/PauloHenriqueRod/processamento-de-imagens/assets/96426671/ae266576-c2da-4c14-8e4d-01985fd79d1b)
## Passo 2:
### Aplicação do algoritmo de canny para detecção de bordas da imagem.
![canny](https://github.com/PauloHenriqueRod/processamento-de-imagens/assets/96426671/83dd0f9d-908a-407f-acd3-317181535fcb)
## Passo 3:
### Função para detecção de objetos circulares da imagem, utilizando a transformada de Hough, fatores como o size-error-margin, e minDIst, param1, param2, minRadius, maxRadius foram escolhidos de forma empírica para que apenas os objetos circulares fossem obtidos, e para que as moedas iguais tivesse a mesma cor. Essa forma de detecção de objetos é semelhante a técnica utilizada em maquinas para diferenciar as moedas que são inseridas.
![objetos_circulares](https://github.com/PauloHenriqueRod/processamento-de-imagens/assets/96426671/e2d7e75d-a2cd-48a0-81e9-e2ba4cdc568b)
## Passo 4:
### Função para que os objetos circulares sejam removidos da imagem
![objetos_nao_circulares](https://github.com/PauloHenriqueRod/processamento-de-imagens/assets/96426671/667e5c37-5455-4421-905a-ef60e69f459c)
## Passo 5:
### Utilizando a diferença de momentos para diferenciação de objetos na imagem. A diferença de momentos foi escolhida, pois é um fator que não se altera mesmo que o objeto esteja rotacionado ou em uma posição diferente.
![momentos](https://github.com/PauloHenriqueRod/processamento-de-imagens/assets/96426671/8d9729d5-e6f6-4ca5-88ae-cbb5f4ae82dc)
