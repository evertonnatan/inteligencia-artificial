# Introdução à Inteligência Artificial

## Conceito

Inteligência Artificial (IA) pode ser definida como sendo o ramo da ciência da computação que se ocupa da automação do comportamento inteligente.

## Áreas de pesquisa em IA
* Machine learning em larga escala
* Deep learning
* Aprendizado por reforço
* Robótica
* Visão computacional
* Processamento de linguagem natural
* Sistemas colaborativos
* Internet das Coisas (IoT)
* Teoria dos Jogos e computação social

### Modelos de IA
* algoritmos genéticos
* programação evolutiva
* lógica fuzzy
* sistemas baseados em conhecimento
* raciocício baseado em casos
* programação genética
* redes neurais

## Áreas de aplicação da IA
* transporte
* healthcare
* educação
* social (segurança pública, prevenção de doenças, etc)
* trabalho
* entretenimento

## Sistemas inteligentes
A Linha de Pesquisa Sistemas Inteligentes visa ao estudo, desenvolvimento e aplicação de sistemas computacionais capazes de solucionar problemas que exigem inteligência para serem resolvidos. Tem como objetivo aplicar os conceitos, técnicas e ferramentas da Inteligência Artificial no auxilio da resolução de problemas conceituais e práticos da computação e das demais áreas do conhecimento, além de estudar e desenvolver o estado-da-arte da inteligência artificial objetivando seu uso prático em processos industriais e agroindustriais. Integram esta linha, sistemas que evoluem e se adaptam (Sistemas Evolutivos), sistemas de inteligência distribuída (Sistemas Multiagentes) e sistemas que são capazes de aprender com a experiência (Aprendizado de Máquina).

### Características de Sistemas Inteligentes:
* aprendizagem e descoberta
* capacidade de adaptação
* resistência a erros e falhas
* capacidade de gerar

### Tecnologias de Sistemas Inteligentes:

![image](https://user-images.githubusercontent.com/37844708/146837002-7fc6bd4a-e725-4907-9d1b-870d9fb4c548.png)

## Chatbots
São serviços baseados em regras e, às vezes, em IA. Veja o [Chatbot do Facebook](https://developers.facebook.com/docs/messenger-platform/) e o do [Google](https://cloud.google.com/dialogflow/es/docs/integrations/dialogflow-messenger)


## Teste de Turing
Russell e Norvig no clássico livro sobre Inteligência Artificial de 1995 observaram que programar um sistema de computador para passar no Teste de Turing é uma tarefa muito difícil. Tal sistema precisaria ter pelo menos as seguintes capacidades:

* Processamento de linguagem natural para se comunicar com o usuário;
* Representação de conhecimento para armazenar o que sabe ou aprende;
* Raciocínio automatizado para usar o conhecimento armazenado com a finalidade de responder perguntas ou tirar novas conclusões;
* Aprendizado de máquina para se adaptar a novas circunstâncias, detectar e extrapolar padrões, a fim de atualizar o seu conhecimento armazenado.

## Sala Chinesa
A sala chinesa é um argumento construído por **John Searle** em 1980, um filósofo norte-americano que pretendia contrapor os pesquisadores da área da Inteligência Artificial. A ideia possui certa relação com o Teste de Turing, que objetiva verificar se uma máquina pode ou não ser considerada inteligente. O ponto chave do argumento de Searle é baseado no fato de que os computadores podem entender somente a **sintaxe** mas não a **semântica** das linguagens processadas. 

## Agentes Inteligentes
São entidades autônomas, dotadas de uma base de conhecimento e capazes de interagir com o meio em que estão, tomando, assim, decisões que irão auxiliar ou até mesmo substituir o trabalho de um humano.Pode ser um software desenvolvido para automatizar e executar uma tarefa em uma rede para o usuário. Possui 3 características principais: inteligência, interatividade e autonomia.

![image](https://user-images.githubusercontent.com/37844708/147291159-a62bbc39-17a5-4b7c-92be-4bda8b9e7c72.png)


### Tipos de agentes inteligentes:

* agentes reativos simples (aspirador de pó)
* agentes reativos baseados em modelos
* agentes baseados em objetivos
* agentes baseados na utilidade
* agentes com aprendizagem
    * crítico
    * elemento de aprendizagem
    * elemento de desempenho
    * gerador de problemas
* agentes de resolução de problemas

## Componentes de um problema:
* estado inicial (espaço de estados do problema)
* ações (espaço de estados do problema)
* modelo de transição (espaço de estados do problema)
* teste de objetivo
* custo do caminho

### Problema do caxeiro viajante
O Problema do [Caixeiro Viajante](https://pt.wikipedia.org/wiki/Problema_do_caixeiro-viajante) (PCV) é um problema que tenta determinar a menor rota para percorrer uma série de cidades (visitando uma única vez cada uma delas), retornando à cidade de origem. Ele é um problema de otimização [NP-difícil](https://pt.wikipedia.org/wiki/NP-dif%C3%ADcil) inspirado na necessidade dos vendedores em realizar entregas em diversos locais (as cidades) percorrendo o menor caminho possível, reduzindo o tempo necessário para a viagem e os possíveis custos com transporte e combustível.


## Estratégias de busca sem informação:
1. Busca em largura - breadth-first search (BFS)
2. Busca em profundidade - depth-first search (DFS)
3. Busca em profundidade limitada - depth-limited search (DLS)
4. Busca de aprofundamento iterativo - iterative-deepening search (IDS)
5. Busca de custo uniforme - uniform-cost search (UCS)

## Estratégias de busca informada
1. Busca gulosa de melhor escolha (Greedy Best-First Search)
2. Busca A* (A* Search)

### Busca de subida de encosta (Hill Climbing)
Como o próprio nome indica, o algoritmo avalia e escolhe os melhores estados a partir da expansão do estado atual, utilizando uma função heurística. Russell e Norvig (2004,
p.111) assim explicam: _“O algoritmo termina quando alcança um ‘pico’ em que nenhum vizinho tem valor mais alto”_. No entanto, o algoritmo pode ficar preso em máximos locais.A esse respeito, Luger (2013, p.106) afirma: _“Se elas alcançarem um estado que tenha uma avaliação melhor que qualquer um dos filhos, o algoritmo fracassa”_.Para contornar esse
problema, foram propostas variações do algoritmo utilizando reinicio estocástico.

### Têmpera Simulada
Têmpera simulada (simulated annealing)- Consiste em uma metáfora com atividades metalúrgicas, o algoritmo que usa a têmpera simulada, em vez de escolher o melhor estado no caso da subida de encosta, executa uma escolha estocástica (aleatória).Tal algoritmo sempre aceitará o próximo estado se for este o melhor. Caso não se trate do melhor estado, haverá uma probabilidade de ser aceito ou não. Essa probabilidade tende a diminuir de modo exponencial durante a execução do algoritmo, monitorada por uma variável que simula a temperatura _T_ do sistema. Desse modo, podem ser escolhidos movimentos ruins, porém essa possibilidade diminui ao longo das iterações. A vantagem de tal procedimento da têmpera simulada é evitar que o algoritmo fique preso em mínimos locais'. No caso de _T_ diminuir a uma velocidade adequada, _“o algoritmo encontrará um valor ótimo global com probabilidade próxima de 1”_ (Russell; Norvig, 2004, p.114).



 



























