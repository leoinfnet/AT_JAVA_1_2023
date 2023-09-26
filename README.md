# Projeto de Conclusão de disciplina.
### Fundamentos de Desenvolvimento JAVA.

- Sua tarefa será desenvolver um jogo chamado Medieval Battle.

-- O jogo é baseado em turnos e consiste em simular batalhas entre personagens hérois e monstros.


-- Seu jogo consiste em 2 programas.

-- O primeiro é o principal onde toda a simulação de batalhas ocorrerá.
-- O segundo servirá para ler os logs e informar a pontuação.


## Programa Principal
- Seu programa deve inciar perguntando o nickname do jogador e qual classe de herói ele deseja escolher.
- O programa irá simular uma batalha entre o jogador e um monstro que será escolhido aleatoriamente 
     
-- Ver a tabela de classes. [a relative link](other_file.md)


### Simulação da batalha:
#### O primeiro passo é o cálculo da iniciativa.

-- Esse cálculo é dado pela seguinte fómula: Rola-se um dado de 10 faces + fator de agilidade.

-- O Maior valor entre monstro e herói inicia o ataque.

-- Caso o valor seja igual, repete-se o teste até que alguem ganhe.

#### O segundo passo é o ataque.

-- Calcula-se o fator de ataque que é dado por: dado de 10 faces (1d10) + agilidade + força.

-- Calcula-se o fator de defesa que é dado por: dado de 10 faces (1d10) + fator de agilidade + fator de defesa.

-- Se o fator de ataque for maior que o fator de defesa calcula-se o dano,senão nada acontece.

#### Cálculo de Dano.

-- Rola-se o dado com o fator de dano do personagem(monstro ou heroi) + pontos de força. 

-- O resultado é subtraído dos pontos de vida do atacado.

### Finalização da batalha.

- A batalha se encerra quando os pontos de vida de algum personagem chegue a zero ou menos

### Gravação de LOG:
- Você pode escrever o que quiser na tela do console que te ajude a depurar o programa. Esse passo é opcional.
- Ao final da execução da batalha você DEVE: 
     -- Gravar um arquivo texto numa pasta chamad "temp" no mesmo diretório do seu programa.

     -- O nome desse arquivo deve seguir o padrão: nicknameDoJogador.csv ex: leogloria.csv 

     -- Cada linha desse arquivo representa uma batalha relacionada áquele jogador. 

     -- Cada linha deve seguir o formato:

          --- Data Da partida;heroi escolhido;PERDEU[ou]GANHOU;monstro enfrentado;quantidadeDeRodadas;

               ---- ex: 14/11/2023;Guerreiro;GANHOU;Morto Vivo;12

## Programa De Relatórios
- Esse programa será responsável por gerar relatórios de um jogador.

- Ele deverá iniciar perguntando o nickname do jogador.

- Após ele deverá procurar o arquivo com o nome nickname.csv na pasta "temp".

- Crie uma classe para representar cada linha do arquivo e adicione-as a uma estrutura de dados. ArrayList, Linkedlist, etc.

- Imprima na tela dados como:
     Heroi mais jogado.
     Monstro mais enfrentado.
     Quantiadade total de Pontos. Sendo que a cada batalha a quantidade de pontos é dada por 100 - quantiadeDeRodadas.
     Pode imprimir quais dados achar relevate.


## Importante!!!!
- Você deve utilizar:

     -- Polimorfismo (Pode utilizar Classes abstratas ou Interfaces)

     -- Exceptions (Dica: utilize exceptions quando estiver lendo dados 
     do teclado).

     -- Api de Stream do Java 8.







