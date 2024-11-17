**Grupo**:  
- [Henrique Bouwman](https://github.com/henriquebouwman)  
- [Manuel Galvão](https://github.com/manuelfgalvao)  
- [Lucas Ferreira](https://github.com/lukitas20-beep)
- [João Rietra](https://github.com/jhlr)

**Disciplina**: Programação Imperativa e Funcional  
**Instituição**: CESAR School  

# i-C-mines

## Como Jogar
1. Iniciar o Jogo: O jogo começa com um campo de 10x10 células, onde 10 minas estão escondidas aleatoriamente. Cada célula pode conter uma mina ou um número indicando quantas minas estão ao seu redor.

2. Explorar Células:
- Abrir uma célula: Escolha uma posição para abrir. Se uma mina estiver presente, o jogo termina, e você perde.
- Número de minas vizinhas: Se a célula não contém uma mina, ela mostrará um número indicando quantas minas existem nas células adjacentes.
- Propagar células vazias: Se a célula for “0” (sem minas ao redor), ela abrirá automaticamente as células próximas até encontrar células com números.

3. Marcar uma célula:
- Caso desconfie de uma mina, marque a célula. Você pode marcar quantas quiser, mas cuidado com marcações desnecessárias!
- Para vencer, é preciso abrir todas as células livres de minas sem explodir nenhuma mina!

4. Terminar o Jogo:
- O jogo termina se todas as células sem mina forem abertas, ou se você acidentalmente abrir uma mina.
- Dica: Use os números como pistas para identificar áreas seguras.

## Descrição
Bem-vindo ao i-C-mines, onde enxergar ou não enxergar uma mina faz toda a diferença! Neste desafio explosivo, você terá que abrir caminho por um campo repleto de minas ocultas, confiando em sua lógica e instintos para sair vitorioso. Afinal, i-C-mines, do you see?

O campo de jogo é um tabuleiro 10x10, e, espalhadas por ele, estão várias minas à espera do próximo movimento. Seu objetivo? Desvendar todas as células seguras e marcar as minas suspeitas sem cair em uma armadilha. Cada célula aberta revelará pistas, números que mostram quantas minas estão por perto – use esses números para traçar seu caminho e evitar o perigo.

Marque as células que suspeita serem minas e continue explorando com cuidado. Se abrir uma célula com uma mina, o jogo termina, e a vitória escapa de suas mãos! Mas se conseguir limpar o campo, poderá dizer com orgulho: “i-C-mines, and I conquered!”

Então, está preparado? Abra o olho, tome cada decisão com cuidado e tente ver as minas antes que elas vejam você. Boa sorte!

## Implementação da mecânica do jogo
A implementação da mecânica do jogo i-C-mines pode ser feita em C para combinar simplicidade e controle direto sobre os dados.

1. Estrutura do Projeto
   
1.1 Arquivos principais:
-main.c: Contém o loop principal e chama as funções do jogo.
-game_logic.c e game_logic.h: Implementam e declaram funções para a lógica do jogo.
-board.c e board.h: Implementam e declaram funções para criar e manipular o tabuleiro.
1.2 Estruturas de Dados:
-Uma matriz de tamanho fixo (10x10) para o tabuleiro.
-Cada célula será representada por uma estrutura
-O tabuleiro será uma matriz de Cell

2. Etapas da Implementação
2.1 Inicializar o Tabuleiro
-Crie uma função para inicializar o tabuleiro:
-Coloque minas aleatoriamente.
-Calcule o número de minas ao redor para cada célula.

2.2 Exibir o Tabuleiro
-Crie uma função para exibir o tabuleiro
-Mostre o estado atual (aberto, marcado, ou oculto)

2.3 Abrir uma Célula
-Crie uma função para abrir uma célula. Se a célula for "0", propague a abertura para as células adjacentes.

2.4 Marcar uma Célula
-Permita que o jogador marque células suspeitas.

2.5 Loop Principal
-Implemente o loop principal para:
2.5.1 Exibir o tabuleiro.
2.5.2 Aceitar entradas do jogador.
2.5.3 Checar condições de vitória/derrota.
