# Algoritmo de Otimização por Enxame de Partículas
Trabalho 2 referente a disciplina de Inteligência Artificial.

### Alunos: 
Gabriel Pontes Marchezi e Gabriel Viggiano Fonseca

# Explicação Teórica
A otimização de enxame de partículas (PSO) é uma técnica de otimização estocástica de base populacional desenvolvida pelo Dr. Eberhart e Dr. Kennedy   em 1995, inspirada no comportamento social do bando de pássaros ou na educação de peixes. 

O PSO compartilha muitas semelhanças com técnicas de computação evolutiva, como algoritmos genéticos (GA). O sistema é inicializado com uma população de soluções aleatórias e procura por ótimos, atualizando gerações.

Como afirmado anteriormente, o PSO simula os comportamentos de pássaros reunidos. Suponha o seguinte cenário: um grupo de pássaros está pesquisando aleatoriamente comida em uma área. Há apenas um pedaço de comida na área sendo pesquisada. Todos os pássaros não sabem onde está a comida. Mas eles sabem até que ponto a comida está em cada iteração. Então, qual é a melhor estratégia para encontrar a comida? O eficaz é seguir o pássaro mais próximo da comida.

O PSO aprendeu com o cenário e o usou para resolver os problemas de otimização. No PSO, cada solução é um "pássaro" no espaço de pesquisa. Nós chamamos de "partícula". Todas as partículas têm valores de aptidão que são avaliados pela função de aptidão a ser otimizada e possuem velocidades que direcionam o vôo das partículas. As partículas voam pelo espaço do problema seguindo as partículas ideais atuais.

O PSO é inicializado com um grupo de partículas aleatórias (soluções) e, em seguida, procura por ótimos, atualizando gerações. Em cada iteração, cada partícula é atualizada seguindo dois "melhores" valores. A primeira é a melhor solução (fitness) alcançada até o momento. (O valor de condicionamento físico também é armazenado.) Esse valor é chamado de pbest.

# Problema Proposto
O problema sugerido envolve utilizar algum algoritmo PSO para minimizar a função <i><b> Eggholder Function </b></i> descrita pela equação:<br>
![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/egg2.png?raw=true "funcao egg")<br>


# Implementação
Para a implementação do algoritmo de otimização, foi utilizada a linguagem de programação Python, essa que vem ganhando bastante popularidade na área de de Inteligência Artificial, por ser uma linguagem de fácil aprendizado e com alto nível de produtividade.

### Trechos mais Importantes
1. Função que cria as particulas, a partir do número recebido pelo usuário. E assim, é gerado uma lista com a quantidade de particulas. Vale ressaltar que os valores de posição das particulas são geradas randomicamente dentro do escopo do domínio pré estipulado.

![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/criaparticulas.png?raw=true "criaParticulas")<br>

2. Função que calcula a Fitness (eggholder function)

![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/calculoEGG.png?raw=true "calculoEGG")<br>

3. Função que atualiza as velocidades X1 e X2, de acordo com a fórmula passada na especificação do trabalho.
![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/atualizarVelocidade.png?raw=true "attVEL")<br>

4. Função getGbests: Com o numero de iterações definido pelo usuário, é gerado uma lista de partículas, se é utilizado a função eggholder em cada partícula para atualizar sua aptidão e seu pbest e mapeando o melhor de todos. Além disso, ela retorna uma lista de Gbests a partir de uma lista de pbests anteriormente gerada.

![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/getGBEST.png?raw=true "getGbest")<br>

5. Funções de atualizações: Posição, Aptidão e Pbest

![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/atualizacoes.png?raw=true "getGbest")<br>

# Resultados e Análise
![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/Figure_1.png?raw=true "1")<br>

![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/Figure_2.png?raw=true "2")<br>

![Alt text](https://github.com/gabrielviggiano/Trab02_IA_PSO/blob/master/Figure_3.png?raw=true "3")<br>

# Bibliografia

http://www.swarmintelligence.org/tutorials.php

