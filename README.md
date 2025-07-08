# Search Algorithm Visualizer

Este projeto simula um agente que coleta comida em um ambiente 2D, navegando por terrenos com diferentes custos e desviando de obstáculos. A ideia é visualizar como diferentes algoritmos de busca se comportam em situações variadas.

## Sobre o Projeto

A simulação acontece em uma grade (grid) gerada aleatoriamente. Em cada rodada, o agente precisa encontrar o caminho até a comida utilizando um dos algoritmos disponíveis. O ambiente inclui terrenos com custos diferentes, que afetam a movimentação do agente, e a execução da busca é mostrada de forma animada, passo a passo.

Após coletar a comida, uma nova posição é sorteada e o processo se repete automaticamente.

## Algoritmos de Busca

- Busca em Largura (BFS)
- Busca em Profundidade (DFS)
- Custo Uniforme (UCS)
- Gulosa
- A* (A-estrela)

## Tipos de Terreno

Cada célula da grade pode conter:

- Obstáculo (não atravessável)
- Areia (custo baixo)
- Atoleiro (custo médio)
- Água (custo alto)

## Estrutura do Projeto

```

Search-Algorithm-Visualizer/
├── index.html              # Página principal
├── style.css               # Estilo visual da interface
├── README.md               # Documentação
├── src/                    # Código-fonte da simulação
│   ├── config.js           # Parâmetros globais
│   ├── drawing.js          # Renderização gráfica
│   ├── map_generator.js    # Geração do mapa aleatório
│   ├── search_logic.js     # Implementação dos algoritmos e animação da busca
│   ├── sketch.js           # Controle geral da simulação
│   └── ui.js               # Interface e interações com o usuário

````

## Como Executar

### Acesso Online (Recomendado)

O projeto pode ser acessado diretamente pelo navegador através do link abaixo!

**[Clique aqui para abrir o projeto](https://andreywid.github.io/Search-Algorithm-Visualizer/)**


### Execução Local

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/Search-Algorithm-Visualizer.git
cd Search-Algorithm-Visualizer
````

2. Abra a pasta no Visual Studio Code.

3. Com a extensão **Live Server** instalada, clique com o botão direito no arquivo `index.html` e escolha **"Open with Live Server"**.

4. O projeto será carregado automaticamente no navegador.

## Tecnologias

* HTML, CSS e JavaScript
* [p5.js](https://editor.p5js.org/ayls/sketches/ZOPH2OKem) (para animação)
* Nenhuma dependência externa ou instalação adicional

## Funcionalidades

* Geração automática de ambientes com diferentes terrenos
* Interface para escolher o algoritmo de busca
* Animação da execução da busca (visitados, fronteira, caminho final)
* Velocidade do agente varia com o tipo de terreno
* Nova comida aparece automaticamente após cada coleta

## Equipe

Projeto desenvolvido para a disciplina de Sistemas Inteligentes (UFPE):

* **Andreywid Yago Lima de Souza** — Integração geral dos algoritmos e testes
* **Artur Vinícius Pereira Fernandes** — Integração geral dos algoritmos e testes
* **Felipe Mateus Falcão Barreto** — Geração do ambiente e controle de acessibilidade
* **João Pedro Mafaldo de Paula** — Lógica de movimentação e coleta da comida
* **Matheus Ayres dos Santos** — Animação da busca e interface visual
