# A evolução do algoritmo — Projeto para a Feira de Ciências

> Documento elaborado com o ChatGPT (via JarvisAssistenteWeb) em 28/09/2026 para o jogo
> **"Encontre o erro no algoritmo"**. O jogo em si está no arquivo [`index.html`](index.html),
> nesta mesma pasta.

| | |
|---|---|
| **Projeto** | A evolução do algoritmo |
| **Jogo interativo** | Encontre o erro no algoritmo |
| **Homenagem** | Ada Lovelace e o nascimento da programação |
| **Turma** | 903 — Feira de Ciências (Projeto Ciência Delas na Nicomedes) |

---

## A) Documento do projeto

### 1. Ideia central

O projeto apresenta a programação de um jeito visual e interativo.

O visitante recebe um pequeno problema e várias instruções representadas por blocos. Os blocos começam fora da ordem correta, e a tarefa é reorganizá-los para formar um algoritmo.

Enquanto os blocos são movimentados, três representações do mesmo programa aparecem ao mesmo tempo:

1. **Blocos**: a lógica visual criada pelo visitante;
2. **Código JavaScript**: o programa equivalente;
3. **Máquina**: a execução real daquele programa.

Quando o visitante toca em **Testar**, o computador executa exatamente as instruções que recebeu. Se estiverem certas, o objetivo é alcançado. Se estiverem erradas, a máquina não tenta "entender o que a pessoa quis dizer": ela simplesmente executa o algoritmo recebido.

Esse comportamento mostra uma das ideias fundamentais da programação:

> **Computadores executam instruções. Eles não conhecem nossa intenção.**

### 2. Objetivo geral

Demonstrar de maneira simples e interativa como algoritmos se transformam em programas de computador. O visitante deve compreender que programar envolve:

- organizar instruções;
- definir uma sequência lógica;
- trabalhar com dados e variáveis;
- criar decisões;
- repetir operações;
- testar;
- encontrar erros;
- corrigir algoritmos.

### 3. Conceitos demonstrados

**Sequência lógica.** A ordem das instruções pode mudar completamente o resultado.

```
número = 7
multiplicar por 2
somar 10
mostrar resultado
```

produz **24**, enquanto outra ordem pode produzir outro resultado ou até um erro.

**Instruções precisas.** O computador não interpreta intenções humanas. Se mandarmos:

```
colocar queijo
abrir pão
```

um robô literal tentaria colocar o queijo antes mesmo de abrir o pão. Isso mostra por que algoritmos precisam ser claros.

**Variáveis.** Variáveis são espaços onde o programa guarda informações:

```js
let nota1 = 8;
let nota2 = 6;
let media = (nota1 + nota2) / 2;
```

Durante a execução, o jogo mostra os valores dessas variáveis mudando em tempo real.

**Testes e depuração.** Um programa normalmente não nasce perfeito. O programador cria o algoritmo, executa, observa o resultado, identifica o problema, corrige e testa novamente. Esse processo se chama **depuração** (*debugging*), e o jogo transforma justamente esse processo em uma atividade.

**Algoritmo × programa.** Um algoritmo é uma sequência de passos para resolver um problema. Um programa é uma forma de escrever essas instruções numa linguagem que o computador consegue executar. No projeto, o bloco **Somar 10** vira `x = x + 10;`. Assim o visitante percebe que os blocos e o código representam a mesma lógica.

### 4. Relação com Ada Lovelace

Ada Lovelace trabalhou no século XIX estudando a **Máquina Analítica**, projetada por Charles Babbage. Em suas anotações sobre a máquina, especialmente a famosa **Nota G**, Ada descreveu um procedimento detalhado envolvendo os **números de Bernoulli**.

Sua contribuição é reconhecida como um marco histórico da programação porque ela descreveu uma sequência de operações destinada a ser executada por uma máquina. Nosso jogo reproduz a mesma ideia fundamental:

```
dados → instruções → operações intermediárias → resultado
```

A última fase é inspirada na Nota G e usa um cálculo simplificado envolvendo um número de Bernoulli.

> **Importante:** explicar ao visitante que a atividade é uma simplificação pedagógica, e não uma reprodução completa do algoritmo histórico de Ada Lovelace.

### 5. Público-alvo

O projeto foi pensado para crianças, adolescentes, adultos, pessoas que nunca programaram e pessoas que já conhecem programação. **Não é preciso saber JavaScript**: a interface visual permite entender a lógica antes mesmo de conhecer a linguagem.

### 6. Roteiro da apresentação (cerca de 2 minutos por visitante)

| Momento | Quem | Tempo | O que fazer / falar |
|---|---|---|---|
| Abertura | Aluna 1 | ~20 s | "Nosso projeto se chama *A evolução do algoritmo* e é uma homenagem a Ada Lovelace. Ela trabalhou com ideias para a Máquina Analítica de Charles Babbage e é reconhecida como uma das figuras fundamentais da história da programação." |
| Conceito | Aluna 2 | ~20 s | "Um algoritmo é basicamente uma sequência de instruções para resolver um problema. Mas tem uma coisa importante: o computador não sabe o que a gente queria fazer. Ele executa exatamente o que mandamos." |
| Convite | Aluna 3 | ~20 s | "Por isso criamos este jogo. Aqui existem vários blocos fora de ordem. Você precisa arrastar os blocos e montar o algoritmo que acha correto." → **entregar o celular/tablet ao visitante.** |
| Visitante joga | Equipe | 30–50 s | Enquanto ele move os blocos: "Olha o painel do meio. Cada bloco que você move muda automaticamente o código JavaScript." Depois: "Agora aperta **Testar**." |
| Execução | Equipe | ~20 s | "A máquina está executando uma instrução de cada vez." Apontar para a **linha destacada**, o **painel de variáveis**, a **saída** e o **resultado**. Se estiver errado: "Ela não corrigiu nosso algoritmo. Executou exatamente o que recebeu. Agora precisamos descobrir o erro. Isso é parecido com a depuração que os programadores fazem." |
| Encerramento | Equipe | ~15 s | "As primeiras fases trabalham com sequências simples. Depois aparecem variáveis, decisões, repetições e, na fase final, fazemos um pequeno cálculo inspirado no trabalho de Ada Lovelace com números de Bernoulli." |

### 7. Instruções de uso e instalação

O projeto usa apenas **HTML, CSS e JavaScript puro**, sem bibliotecas externas e sem servidor. É **um único arquivo**: `index.html`.

**No computador**

1. Copiar `index.html` para uma pasta.
2. Clicar duas vezes no arquivo.
3. Abrir no Chrome, Edge ou Firefox.

**No tablet ou celular**

- Copiar o arquivo para o aparelho e abri-lo num navegador que aceite arquivos HTML locais; ou
- rodar o arquivo num notebook e disponibilizá-lo pela rede local.

Como tudo está dentro do próprio HTML, depois de aberto ele **não depende de internet**.

**Modo de apresentação (recomendado)**

- tablet na horizontal, quando possível;
- navegador em tela cheia;
- zoom em 100%;
- impedir que o aparelho desligue a tela durante a exposição.

No celular, a interface muda sozinha para painéis empilhados.

---

## B) Modelo de interface

### 1. Conceito visual

A interface mistura laboratório, programação, jogo educativo e exposição científica. Ela deve parecer tecnológica sem ficar técnica demais. **A prioridade é a legibilidade.**

### 2. Layout desktop / tablet na horizontal (três painéis)

```
┌──────────────────────────────────────────────────────────────────────┐
│ A EVOLUÇÃO DO ALGORITMO       Fase 3         ★ 2/8 concluídas       │
├──────────────────────────────────────────────────────────────────────┤
│ Objetivo: calcular a média de duas notas                            │
└──────────────────────────────────────────────────────────────────────┘

┌───────────────────┬──────────────────────┬───────────────────────────┐
│ 1. BLOCOS         │ 2. CÓDIGO            │ 3. MÁQUINA                │
│                   │                      │                           │
│ ≡ nota1 = 8       │ let nota1 = 8;       │ Executando linha 1        │
│                   │                      │                           │
│ ≡ nota2 = 6       │ let nota2 = 6;       │ nota1 = 8                 │
│                   │                      │ nota2 = 6                 │
│ ≡ calcular média  │ let media = (...)    │ media = 7                 │
│                   │                      │                           │
│ ≡ mostrar média   │ console.log(media);  │ Saída: 7                  │
│                   │                      │                           │
│ ─ NÃO USAR ─      │                      │ ✅ Resultado correto      │
└───────────────────┴──────────────────────┴───────────────────────────┘

        [▶ TESTAR] [💡 DICA] [↺ REINICIAR]   Velocidade ━━━●━━
```

### 3. Layout celular (painéis empilhados)

```
┌───────────────────────────┐
│ Fase 1 — Dobro + 10       │
│ Objetivo...               │
└───────────────────────────┘
┌───────────────────────────┐
│ 1. BLOCOS                 │
│ ≡ Escolher número         │
│ ≡ Multiplicar             │
│ ≡ Somar                   │
│ ≡ Mostrar                 │
└───────────────────────────┘
┌───────────────────────────┐
│ 2. CÓDIGO                 │
│ let x = 7;                │
│ x = x * 2;                │
│ x = x + 10;               │
│ console.log(x);           │
└───────────────────────────┘
┌───────────────────────────┐
│ 3. MÁQUINA                │
│ x = 7                     │
│ x = 14                    │
│ x = 24                    │
│ saída = 24                │
└───────────────────────────┘
[ TESTAR ]
[ DICA ] [ REINICIAR ]
Velocidade ━━━●━━━━
```

### 4. Paleta de cores

| Uso | Cor | Observação |
|---|---|---|
| Fundo principal | `#F6F4FF` | quase branco com leve violeta |
| Roxo principal | `#5B5FC7` | botões, cabeçalhos, identificação principal |
| Roxo secundário | `#7C82F3` | |
| Azul-marinho | `#2F356B` | |
| Destaque amarelo/laranja | `#FFB454` | linha que está sendo executada |
| Sucesso | `#1F9D6A` | |
| Erro | `#D94F70` | |
| Fundo do código | `#191B2B` | |

### 5. Tipografia

Fontes nativas do aparelho, para funcionar totalmente offline.

- **Interface:** `system-ui, "Segoe UI", Arial, sans-serif`
- **Código:** `Consolas, Menlo, monospace`

### 6. Componentes

**Bloco de algoritmo.** O ícone ⋮⋮ indica que ele pode ser arrastado.

```
⋮⋮  1  Definir número = 5
       let x = 5;
```

**Área "Não usar".** Recebe instruções que não pertencem ao algoritmo.

```
┌─────────────────────────┐
│ NÃO USAR                │
│ ≡ Subtrair 100          │
└─────────────────────────┘
```

**Código.** Cada bloco gera uma linha equivalente, e a linha que está sendo executada recebe destaque visual.

**Painel de variáveis.** Os valores mudam durante a animação.

```
x = 5
nota1 = 8
nota2 = 6
media = 7
```

**Console.** Registra a execução:

```
> Programa iniciado
> Linha 1: Definir número
> x = 5
> Linha 2: Somar 3
> x = 8
> Linha 3: Multiplicar por 2
> x = 16
```

### 7. Estados da interface

| Estado | Aparência |
|---|---|
| **Normal** | blocos brancos |
| **Arrastando** | bloco levemente transparente e elevado, acompanhando o mouse ou o dedo; a área de destino fica destacada |
| **Testando** | botão Testar desabilitado; a linha executada aparece destacada (`▶  x = x * 2;`) |
| **Acertou** | painel verde: `✅ ACERTOU!  7 × 2 = 14 → 14 + 10 = 24` |
| **Errou** | painel rosa/vermelho: `🔎 AINDA HÁ UM BUG`, com a explicação do erro |

---

## C) Fases

Progressão pedagógica: **sequência → instruções precisas → variáveis → depuração → decisões → repetições → manipulação de memória → algoritmo matemático inspirado em Ada.** O visitante começa quase sem perceber que está programando e termina usando os principais conceitos da programação estruturada.

### Fase 1 — Dobro + 10

- **Objetivo:** escolher o número 7, calcular o dobro, somar 10 e mostrar o resultado (**24**).
- **Blocos iniciais:** Mostrar resultado · Somar 10 · Escolher número 7 · Multiplicar por 2
- **Ordem correta:** Escolher número 7 → Multiplicar por 2 → Somar 10 → Mostrar resultado

```js
let x = 7;
x = x * 2;
x = x + 10;
console.log(x);
```

- **Erro comum:** fazer uma operação antes de a variável existir.
- **Mensagem:** "Uma operação depende dos valores produzidos anteriormente. A máquina não sabe qual número você pretendia usar."

### Fase 2 — Robô faz um sanduíche

- **Objetivo:** dar instruções precisas para um robô preparar um sanduíche.
- **Blocos iniciais:** Servir sanduíche · Colocar queijo · Abrir pão · Fechar sanduíche
- **Ordem correta:** Abrir pão → Colocar queijo → Fechar sanduíche → Servir sanduíche

```js
robo.abrirPao();
robo.colocarQueijo();
robo.fecharSanduiche();
robo.servir();
```

- **Erro comum:** mandar colocar o recheio antes de abrir o pão.
- **Mensagem:** "O robô não completa sozinho as etapas que você esqueceu. Ele só executa as instruções recebidas."

### Fase 3 — Média de duas notas

- **Objetivo:** calcular a média de 8 e 6 (**7**).
- **Blocos iniciais:** Calcular média · Definir nota1 = 8 · Mostrar média · Definir nota2 = 6
- **Uma ordem correta:** Definir nota1 = 8 → Definir nota2 = 6 → Calcular média → Mostrar média

```js
let nota1 = 8;
let nota2 = 6;
let media = (nota1 + nota2) / 2;
console.log(media);
```

- Definir `nota2` antes de `nota1` **também é aceito**, porque as duas operações são independentes.
- **Erro comum:** calcular antes de ter as duas notas.
- **Mensagem:** "O cálculo usou informações que ainda não estavam disponíveis."

### Fase 4 — Bloco distrator

- **Objetivo:** fazer (5 + 3) × 2 e mostrar **16**. Um dos blocos não pertence ao programa.
- **Blocos iniciais:** Mostrar resultado · Subtrair 100 · Multiplicar por 2 · Definir número = 5 · Somar 3
- **Algoritmo:** Definir número = 5 → Somar 3 → Multiplicar por 2 → Mostrar resultado
- **Não usar:** Subtrair 100

```js
let x = 5;
x = x + 3;
x = x * 2;
console.log(x);
```

- **Erro comum:** achar que todos os blocos precisam entrar no programa.
- **Mensagem:** "Depurar também significa descobrir se existe uma instrução que não deveria estar no algoritmo."

### Fase 5 — Par ou ímpar (se/senão)

- **Objetivo:** com `n = 7`, mostrar "ímpar" usando uma decisão.
- **Blocos iniciais:** Mostrar "ímpar" · Fim do se · Definir n = 7 · Se n for par · Senão · Mostrar "par"
- **Ordem correta:**

```
Definir n = 7
Se n for par
    Mostrar "par"
Senão
    Mostrar "ímpar"
Fim
```

```js
let n = 7;
if (n % 2 === 0) {
    console.log("par");
} else {
    console.log("ímpar");
}
```

- **Resultado:** ímpar
- **Erro comum:** inverter os comandos dos dois caminhos.
- **Mensagem:** "A condição está correta, mas cada resultado precisa estar no ramo certo."

### Fase 6 — Repita 3 vezes

- **Objetivo:** começar em zero e somar 2 três vezes (**6**).
- **Blocos iniciais:** Mostrar total · Fim da repetição · Somar 2 ao total · Definir total = 0 · Repita 3 vezes
- **Ordem correta:**

```
Definir total = 0
Repita 3 vezes
    Somar 2
Fim da repetição
Mostrar total
```

```js
let total = 0;
for (let i = 0; i < 3; i++) {
    total = total + 2;
}
console.log(total);
```

- **Execução mostrada:** total = 0 → repetição 1: 2 → repetição 2: 4 → repetição 3: 6
- **Erro comum:** colocar a soma fora do laço (ou o "Mostrar" dentro dele, que aparece 3 vezes).
- **Mensagem:** "O computador repetiu apenas as instruções colocadas dentro da repetição."

### Fase 7 — Troca de variáveis

- **Objetivo:** começar com `a = 5` e `b = 2` e trocar os valores (resultado `a = 2`, `b = 5`).
- **Blocos iniciais:** Definir b = 2 · a recebe b · Mostrar a e b · temp recebe a · Definir a = 5 · b recebe temp
- **Ordem correta:** a = 5 → b = 2 → temp = a → a = b → b = temp → mostrar

```js
let a = 5;
let b = 2;
temp = a;
a = b;
b = temp;
console.log(a, b);
```

- **Explicação:** a variável temporária impede que o valor original de `a` desapareça. Sem `temp = a;`, ao executar `a = b;` o número 5 seria perdido.
- **Erro comum:** sobrescrever uma variável antes de guardar o valor dela.
- **Mensagem:** "O programa perdeu uma informação porque um valor foi substituído antes de ser salvo."

### Fase 8 — Nota G de Ada Lovelace

Simplificação pedagógica inspirada no trabalho de Ada Lovelace com números de Bernoulli. Não pretende reproduzir o algoritmo histórico por completo.

- **Objetivo:** calcular **B₂ = 1/6** a partir de B₀ = 1 e B₁ = −1/2, usando a relação simplificada:
  `soma = B₀ + 3 × B₁` e `B₂ = −soma / 3`
- **Blocos iniciais:** Calcular B2 = −soma / 3 · Mostrar B2 · Definir B0 = 1 · Calcular soma = B0 + 3 × B1 · Definir B1 = −1/2
- **Ordem correta:** Definir B0 → Definir B1 → Calcular soma → Calcular B2 → Mostrar B2

```js
let B0 = 1;
let B1 = -0.5;
let soma = B0 + 3 * B1;
let B2 = -soma / 3;
console.log(B2);
```

- **Cálculo:** soma = 1 + 3 × (−1/2) = −1/2 → B₂ = −(−1/2) / 3 = **1/6** (exibido como 0,1666…)
- **Erro comum:** tentar calcular B₂ antes da variável intermediária `soma`.
- **Mensagem:** "O resultado depende de etapas anteriores. Assim como nos algoritmos estudados por Ada Lovelace, resultados intermediários alimentam as próximas operações."

---

## D) Código

O jogo completo está em [`index.html`](index.html) (HTML + CSS + JavaScript puro, um arquivo só, funciona offline). Ele implementa:

- 8 fases definidas no array `phases`, fácil de ampliar;
- arrastar e soltar com Pointer Events (mouse, caneta e toque);
- movimentação entre as áreas **Algoritmo** e **Não usar**;
- código JavaScript atualizado em tempo real, com destaque de sintaxe simples;
- execução real da sequência montada (incluindo `if/else` e laço de repetição);
- animação passo a passo com velocidade ajustável e destaque da linha em execução;
- painel de variáveis e console didático;
- botões **Testar**, **Dica** e **Reiniciar fase**;
- placar de fases concluídas salvo no navegador (`localStorage`);
- tela inicial sobre Ada Lovelace;
- layout responsivo para computador, tablet e celular.

O jogo **valida pelo resultado da execução**, não por uma "sequência secreta": se duas ordens são logicamente equivalentes (como definir `nota2` antes de `nota1`), as duas são aceitas.

### Como adicionar uma nova fase

Abra `index.html` num editor de texto, procure `const phases = [` e acrescente um objeto no fim da lista, seguindo o modelo das fases existentes:

```js
{
  id: "triplo",                       // identificador único
  title: "Fase 9 — Triplo menos 1",
  intro: "Texto curto que aparece acima do objetivo.",
  objective: "Escolher 4, multiplicar por 3, subtrair 1 e mostrar 11.",
  hint: "Texto do botão Dica.",
  blocks: [                           // ordem em que os blocos aparecem (embaralhada)
    {id:"show", label:"Mostrar resultado", cmd:"SHOW_X"},
    {id:"sub",  label:"Subtrair 1",        cmd:"ADD_X", value:-1},
    {id:"set",  label:"Escolher número 4", cmd:"SET_X", value:4},
    {id:"mul",  label:"Multiplicar por 3", cmd:"MUL_X", value:3}
  ],
  correct: ["set","mul","sub","show"], // ordem de referência
  expected: 11,                        // valor que a máquina precisa mostrar no fim
  success: "Isso! 4 × 3 = 12; 12 − 1 = 11.",
  commonError: "Explicação exibida quando o resultado sai errado."
}
```

Comandos (`cmd`) que a "máquina" já sabe executar:

| Grupo | Comandos |
|---|---|
| Número único `x` | `SET_X`, `ADD_X`, `MUL_X`, `SHOW_X` |
| Variáveis com nome | `SET_VAR`, `ADD_VAR`, `COPY_VAR`, `SHOW_VAR`, `SHOW_PAIR`, `CALC_AVG` |
| Texto | `PRINT_TEXT` |
| Decisão | `IF_EVEN`, `ELSE`, `ENDIF` |
| Repetição | `REPEAT_START`, `REPEAT_END` |
| Blocos específicos | `SANDWICH_*` (fase 2), `ADA_SUM`, `ADA_B2` (fase 8) |

Para ter um bloco "distrator", marque-o com `distractor: true` e liste o `id` dele em `unused: [...]`. Uma fase que precise de um comando novo exige acrescentar esse comando no interpretador (a parte do código que trata cada `cmd`).
