# Jogo da Velha (Implementação em Pseudocódigo) Tic-Tac-Toe Logic

![Logic](https://img.shields.io/badge/Language-Pseudocode-blue.svg)

Este repositório contém a implementação da lógica completa para um clássico Jogo da Velha, escrito em uma linguagem estruturada de pseudocódigo (similar ao Portugol). O projeto foi desenvolvido para focar puramente na lógica de programação, sendo uma excelente base de estudos para algoritmos de jogos.

---

## 🎲 Lógica e Funcionalidades

O código está estruturado em funções e tipos de dados que controlam todo o fluxo do jogo, desde o início até a sua conclusão.

### Estrutura de Dados
-   **`tabuleiro`**: Uma matriz 3x3 que representa o estado atual do jogo.
-   **`jogador`**: Uma estrutura que armazena o nome e o símbolo ('X' ou 'O') de cada jogador.
-   **`jogada`**: Armazena as coordenadas (linha e coluna) da jogada de um jogador.

### Fluxo do Jogo
1.  **Inicialização**: O tabuleiro é zerado (preenchido com espaços vazios) e os dois jogadores ('A' com 'X' e 'B' com 'O') são criados.
2.  **Loop Principal**: O jogo continua em um loop `enquanto` o tabuleiro não estiver cheio e não houver um vencedor.
3.  **Alternância de Turnos**: O controle de turno alterna entre o jogador 0 e o jogador 1 a cada jogada válida.
4.  **Validação da Jogada**: O código verifica se a posição escolhida pelo jogador já está ocupada. Se estiver, informa que a jogada é inválida e solicita uma nova.
5.  **Verificação de Vitória**: Após cada jogada, a função `jogo_acabou` verifica todas as possíveis condições de vitória:
    -   As 3 linhas.
    -   As 3 colunas.
    -   As 2 diagonais.
6.  **Verificação de Empate**: Se o loop terminar porque o tabuleiro está cheio (`tabuleiro_cheio`) e não houve vencedor, o jogo termina em empate.
7.  **Fim de Jogo**: Ao final, o programa anuncia o jogador vencedor ou declara que houve um empate.

---

## 🔧 Como o Código Funciona

O projeto é totalmente procedural e modularizado. As principais funções são:

-   `zerar(t)`: Limpa o tabuleiro para o início de uma nova partida.
-   `imprimir(t)`: Exibe o estado atual do tabuleiro no console.
-   `aguardar_jogada(jogador)`: Pede e captura as coordenadas da jogada do jogador atual.
-   `realizar_jogada(t, jogada, jogador)`: Tenta aplicar a jogada no tabuleiro e retorna se foi bem-sucedida.
-   `jogo_acabou(t)`: Retorna `verdadeiro` se alguma condição de vitória for atingida.
-   `tabuleiro_cheio(t)`: Retorna `verdadeiro` se não houver mais espaços vazios.

Este código é um excelente material de estudo para quem está aprendendo lógica de programação e desenvolvimento de algoritmos.
