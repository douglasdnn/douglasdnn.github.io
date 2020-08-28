---
layout: post
title:  "Descobrindo nacionalidades no Scikit-Learn, Parte 1"
categories: machine learning
image: "https://mediastorage.cnnbrasil.com.br/IMAGES/00/00/01/11256_1CF540E9ECDD54CB.jpg"
published: false
---
Texto
	

## Primeiro passo: construindo uma lista de pessoas

Primeiro, 

Vamos importar duas bibliotecas

    import numpy as np
    import matplotlib.pyplot as plt

Além disso, vamos importar a função *randint()* do pacote *random* do python, que não vem carregada por padrão:

    from random import randint

media, desvio = 5, 1 # média e desvio padrão
s = np.random.normal(media, desvio, 500)
count, bins, ignored = plt.hist(s, 500, density=True)

Vamos exibir estes resultados no matplotlib:

    plt.plot(bins, 1/(desvio * np.sqrt(2 * np.pi)) * np.exp( - (bins - media)**2 / (2 * desvio**2) ), linewidth=2, color='r')
    plt.show()
  
  Vejamos que a distribuição corresponde ao que queremos

> Written with [StackEdit](https://stackedit.io/).


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTkxMTQ4ODYwMl19
-->