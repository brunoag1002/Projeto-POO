DESENVOLVIMENTO PROJETO DE SOFTWARE

Integrantes do Grupo:

BRUNO AMARAL GONZALEZ - bruno.amaral@unisantos.br 

EMANUEL RODRIGUES SOARES - emanuel.soares@unisantos.br

ENZO LIUTKUS GOING - enzogoing@unisantos.br 


# Sistema de Batalha em Python

Este projeto implementa um simulador simples de batalha entre duas
bases, onde cada base pode recrutar tropas e atacar o inimigo até que
uma delas seja destruída.

## Descrição

O programa cria duas bases e permite, a cada rodada, que o jogador
adicione tropas e execute ataques. As tropas podem atacar outras tropas
inimigas ou diretamente a base adversária, caso não haja tropas
disponíveis.

## Funcionalidades

-   Criação de duas bases (Base 1 e Base 2)\
-   Recrutamento de tropas:
    -   **Soldado** --- vida 3, dano 1\
    -   **Tanque** --- vida 8, dano 3\
-   Ataques entre tropas ou diretamente à base inimiga\
-   Remoção automática de tropas derrotadas\
-   Exibição do estado atual do campo de batalha\
-   Fim do jogo quando uma das bases chega a 0 de vida

## Como executar

1.  Salve o código em um arquivo, por exemplo:

    main.py

2.  Execute no terminal:

``` bash
python main.py
```

3.  Siga as instruções exibidas no console.

## Estrutura do Código

-   **Base**: representa uma base, com vida e nome.\
-   **Tropas (classe abstrata)**: classe base para qualquer tropa.\
-   **Soldado**: tropa leve com baixo dano e pouca vida.\
-   **Tanque**: tropa pesada com alto dano e mais vida.\
-   **Campo_de_batalha**: gerencia tropas, ataques e andamento da
    batalha.

## Exemplo de uso

Durante a execução, o programa solicitará:

-   Se deseja adicionar tropas\
-   O tipo de tropa\
-   O alvo do ataque

Exemplo:

    ===== RODADA 1 =====
    Base 1 quer adicionar tropas? (s/n)
