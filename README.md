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
     
-- Ver a tabela de classes.
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












-- Obs. O projeto pode ser o mais simples possível, um CRUD, um conversor de medidas , etc.

- Criar testes unitários para métodos utilizando 
     - JUNIT 
    -  MOCKITO0 .
    - TESTContainers (Opcional)

- Expor o health check do seu projeto com o Actuator.
- Exportar métricas do seu projeto para o formato do Prometheus utilizando o micrometer. 
- Exportar LOGs do seu projeto para alguma ferramenta de logs. (Ex. Papertrail)  
- Exportar dados do seu projeto para o Zipkin. 
- Criar Script no terraform em qualquer provedor que crie apenas uma máquina virtual de qualquer formato. Esse script deve possuir 1 arquivo main, um arquivo de variáveis e um arquivo de outputs. 

- Criar um pipeline de build do seu projeto no Gitlab. 
# Grupos.
- Podem ser feitos em grupos de até 5 participantes.
# Regras de entrega.

- Projeto deve estar versionado em alguma ferramenta de versionamento.(Github, bitbuck,etc.). 
- Projeto deve estar público.
- Deve ser entregue o link para o projeto.
- Na raiz do projeto deve ter arquivos de imagem com printscreens do zipking rodando.
- Todos devem postar o link para o projeto no Moodle. Aqueles que fizerem em grupo colocar no README do projeto o nome do grupo.
