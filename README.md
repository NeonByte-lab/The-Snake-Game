# 🐍 Snake Arcade — Jogo da Cobrinha

Um jogo clássico de cobrinha com visual moderno, desenvolvido com **HTML5, CSS3 e JavaScript puro (Vanilla JavaScript)**. O objetivo é simples: coma as frutas, aumente seu tamanho, acumule pontos e tente superar seu recorde!

🎮 **Estilo:** Arcade clássico  
🌐 **Plataforma:** Navegadores web  
💻 **Execução:** Local, sem servidor ou instalação  
📄 **Estrutura:** Arquivo HTML único

---

## 📖 Sobre o projeto

O **Snake Arcade** é uma versão moderna do tradicional jogo da cobrinha, combinando mecânicas clássicas com uma interface intuitiva, responsiva e visualmente agradável.

O jogador controla uma cobrinha em um tabuleiro dividido em células. A cada fruta consumida, a cobrinha cresce e a pontuação aumenta. Entretanto, o desafio também cresce: a velocidade aumenta progressivamente, exigindo reflexos rápidos, atenção e planejamento dos movimentos.

O projeto foi desenvolvido com foco em simplicidade, acessibilidade e facilidade de execução, sem depender de frameworks, bibliotecas externas, APIs ou conexão com a internet.

## ✨ Funcionalidades

- 🐍 **Movimentação da cobrinha:** controle em quatro direções.
- 🍎 **Sistema de alimentos:** frutas aparecem aleatoriamente em posições livres do tabuleiro.
- 📈 **Pontuação dinâmica:** cada fruta consumida vale 10 pontos.
- 🏆 **Sistema de recordes:** o melhor resultado fica salvo no navegador.
- ⚡ **Dificuldade progressiva:** a velocidade aumenta a cada 50 pontos, até atingir o limite máximo de velocidade.
- 💥 **Sistema de colisões:** a partida termina quando a cobrinha bate nas paredes ou no próprio corpo.
- ⏸️ **Pausa e retomada:** interrompa e continue a partida quando quiser.
- 🔄 **Reinício de partida:** comece novamente para tentar melhorar sua pontuação.
- 🏅 **Condição de vitória:** ocupe todas as células disponíveis do tabuleiro.
- 📱 **Controles para dispositivos móveis:** botões direcionais e gestos de deslizar.
- 🎨 **Interface moderna:** tema escuro, detalhes em verde, elementos arredondados e efeitos visuais suaves.
- ♿ **Acessibilidade básica:** rótulos para elementos interativos, foco visível nos botões e suporte à preferência por movimento reduzido.

## 🛠️ Tecnologias utilizadas

### 🌐 HTML5

Responsável pela estrutura e organização dos elementos da interface.

Principais recursos utilizados:
- Estrutura semântica com elementos como `header`, `main`, `section` e `footer`.
- Elementos `button` para os controles do jogo.
- Elemento `canvas` para a renderização do tabuleiro.
- Atributos de acessibilidade, como `aria-label`.
- Meta tags para configuração da codificação, responsividade e cor do tema do navegador.

### 🎨 CSS3

Responsável pelo visual, pela organização dos elementos e pela adaptação da interface a diferentes tamanhos de tela.

Principais recursos utilizados:
- **CSS Grid e Flexbox:** organização dos painéis e controles.
- **Variáveis CSS:** centralização das cores e de outros valores visuais.
- **Gradientes e transparências:** criação de profundidade na interface.
- **Bordas arredondadas e sombras:** acabamento visual dos componentes.
- **Media queries:** adaptação para telas pequenas.
- **Transições:** feedback visual durante as interações.
- **`prefers-reduced-motion`:** redução das transições para usuários que preferem menos movimento.

### ⚙️ JavaScript (Vanilla JavaScript)

Responsável por toda a lógica e pelo funcionamento do jogo, sem utilização de frameworks ou bibliotecas externas.

Principais recursos utilizados:
- Manipulação do DOM para atualizar a interface.
- Gerenciamento do estado da partida.
- Controle de teclado e eventos de ponteiro.
- Movimentação da cobrinha e detecção de colisões.
- Geração aleatória de alimentos.
- Cálculo de pontuação e progressão de velocidade.
- Temporizador com `setTimeout` e cancelamento com `clearTimeout`.
- Persistência do recorde com `localStorage`.
- Funções organizadas para inicialização, pausa, retomada, desenho e encerramento da partida.

### 🖌️ Canvas API

A Canvas API é utilizada por meio do elemento HTML `<canvas>` e do contexto de renderização 2D.

Ela permite desenhar diretamente no tabuleiro:
- A grade de células.
- A cabeça e o corpo da cobrinha.
- Os olhos da cobrinha, orientados conforme a direção do movimento.
- As frutas com efeito de brilho.

### 💾 LocalStorage

A API `localStorage` armazena o recorde no navegador, permitindo recuperá-lo em partidas futuras.

O jogo também trata possíveis falhas de acesso ao armazenamento, mantendo a partida funcional mesmo quando o recurso não está disponível.

## 🎮 Como jogar

### 1. Iniciando uma partida

1. Abra o arquivo `index.html` em um navegador moderno.
2. Clique em **Iniciar jogo** ou pressione uma tecla direcional para começar.
3. Controle a cobrinha e procure alcançar as frutas espalhadas pelo tabuleiro.

### 2. Controles

| Ação | Teclas ou comandos |
|---|---|
| Mover para cima | `↑` ou `W` |
| Mover para baixo | `↓` ou `S` |
| Mover para a esquerda | `←` ou `A` |
| Mover para a direita | `→` ou `D` |
| Pausar a partida | `Espaço` ou botão **Pausar** |
| Retomar a partida | `Espaço` ou botão **Continuar** |
| Reiniciar | Botão **Reiniciar** |

📱 **No celular:** utilize os botões direcionais exibidos abaixo do tabuleiro ou deslize o dedo na direção desejada.

### 3. Pontuação

- 🍎 Cada fruta consumida concede **10 pontos**.
- 📊 A pontuação atual é exibida no painel superior.
- 🏆 O recorde registra a melhor pontuação armazenada no navegador.
- ⚡ A cada 50 pontos, a velocidade aumenta, tornando a partida mais desafiadora.

### 4. Como perder ou vencer

**💥 Fim de jogo:** a partida termina quando a cabeça da cobrinha colide com uma parede ou com o próprio corpo.

**🏆 Vitória:** se a cobrinha ocupar todas as células disponíveis do tabuleiro, o jogo reconhece a vitória.

**🔄 Tente novamente:** após o encerramento, inicie uma nova partida e tente superar sua pontuação anterior.

## 🕹️ Estilo de gameplay

O Snake Arcade segue o estilo **Arcade**, com partidas rápidas, regras simples e dificuldade crescente.

Sua jogabilidade combina três elementos principais:

- **🎯 Precisão:** escolha a direção correta e evite colisões.
- **🧠 Estratégia:** planeje seus movimentos considerando o crescimento contínuo da cobrinha e o espaço disponível.
- **⚡ Reflexos:** reaja rapidamente conforme a velocidade aumenta.

A experiência começa de maneira acessível, permitindo que o jogador compreenda as mecânicas nos primeiros movimentos. Conforme a pontuação cresce, a cobrinha fica mais rápida e ocupa uma área maior do tabuleiro, exigindo decisões cada vez mais cuidadosas.

O desafio não depende de inimigos ou combate, mas da administração do espaço, da antecipação dos movimentos e da capacidade de permanecer em segurança enquanto se busca uma pontuação maior.

## 📁 Estrutura do projeto

O projeto utiliza um único arquivo HTML, reunindo toda a estrutura, a estilização e a lógica do jogo.

```text
snake-arcade/
└── index.html
    ├── HTML5      → Estrutura da interface
    ├── CSS3       → Estilização e responsividade
    └── JavaScript → Regras e lógica do jogo
```

Essa organização simplifica a distribuição, a execução e o estudo do código, sendo especialmente útil para projetos educacionais e experimentos de desenvolvimento web.

## 🚀 Como executar

Não é necessário instalar dependências, configurar um servidor ou utilizar ferramentas de compilação.

1. Salve o arquivo do jogo com o nome `index.html`.
2. Localize o arquivo no computador.
3. Dê dois cliques nele ou utilize a opção **Abrir com** e selecione seu navegador.
4. Clique em **Iniciar jogo** e divirta-se! 🎉

**Requisitos:** um navegador moderno com suporte a HTML5 Canvas, JavaScript e CSS3.

## 🎓 Objetivos de aprendizagem

Este projeto também pode servir como material de estudo para quem está aprendendo desenvolvimento web.

Ao explorar o código, é possível praticar:

- Estruturação de páginas com HTML5.
- Criação de interfaces responsivas com CSS3.
- Manipulação de elementos HTML com JavaScript.
- Uso de eventos de teclado e ponteiro.
- Aplicação de lógica condicional e estruturas de repetição.
- Manipulação de arrays e objetos.
- Detecção de colisões em jogos.
- Controle de estados e temporizadores.
- Desenho gráfico com Canvas API.
- Armazenamento local com `localStorage`.
- Organização do código em funções reutilizáveis.

## 🔮 Possíveis melhorias futuras

O projeto pode evoluir com novas funcionalidades, como:

- 🍓 Diferentes tipos de frutas com pontuações variadas.
- 🧱 Obstáculos distribuídos pelo tabuleiro.
- 👾 Inimigos com comportamentos próprios.
- ✨ Habilidades especiais e efeitos temporários.
- 🗺️ Fases com diferentes mapas e desafios.
- 🎵 Efeitos sonoros e música de fundo.
- 🎨 Temas visuais desbloqueáveis.
- 📊 Estatísticas de partidas e histórico de recordes.
- 🎚️ Seleção de dificuldade antes de começar.

Essas melhorias permitiriam transformar o arcade clássico em uma experiência mais variada, com elementos de progressão e inspiração em jogos roguelike.

## 📌 Considerações finais

O **Snake Arcade** demonstra como HTML5, CSS3 e JavaScript puro podem ser combinados para criar um jogo funcional, responsivo e visualmente agradável diretamente no navegador.

Com código concentrado em um único arquivo, mecânicas clássicas e controles acessíveis, o projeto é uma base interessante tanto para jogar casualmente quanto para estudar os fundamentos da programação de jogos para a web.

🐍 **Coma, cresça, desvie e bata seu recorde!** 🏆
