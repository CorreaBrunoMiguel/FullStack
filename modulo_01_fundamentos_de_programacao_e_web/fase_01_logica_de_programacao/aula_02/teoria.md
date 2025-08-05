# :books: Aula 02 - Variáveis (`let`, `const`) e Tipos Primitivos

Neste aula, vamos entender como **armazenar valores na memória** usando variáveis em JavaScript e como o JavaScript representa diferentes tipos de dados. Dominar esses conceitos é essencial para qualquer aplicação - desde um simples script até um sistema completo.

---

## :brain: O que são variáveis?

Variáveis são **nomes simbólicos** que usamos para **armazenar valores na memória**. Esses valores podem ser alterados ou mantidos fixos, dependendo da forma como declaramos a variável.

Imagine variáveis como **caixas** com rótulos: cada caixa guarda um tipo de valor, e podemos acessar ou trocar esse conteúdo a qualquer momento.

---

## :page_with_curl: Declarando variáveis com `let` e `const`

- `let` - Variável com valor que pode maudar

```js
let nome = 'Ana';
nome = 'Carlos'; // permitido
```

- `const` - Variável com valor fixo (constante)

```js
const idade = 25;
idade = 30; // :x: Erro! Não pode reatribuir
```

---

## :bookmark_tabs: Regras para nomes de variáveis

- Devem **começar com letra**, `$` ou `_`
- **Não podem começar com números**
- **Não podem conter espaços ou símbolos**
- **Não podem ser palavras reservadas** do JavaScript (como `if`, `let`, `function`)

Exemplos válidos:

```js
let & total;
let nome;
let _idade;
let nomeCompleto;
```

Exemplos inválidos:

```js
let 1nome; // começa com número
let meu-nome; // contém hífen
let let; // palavra reservada
```

---

## :pushpin: Tipos primitivos

O JavaScript é uma linguagem de **tipagem dinâmica**, o que significa que o tipo de uma variável **é determinada automaticamente** com base no valor atribuído. Os principais tipos primitivos são:

| Tipo        | Exemplo                      | Descrição                             |
| ----------- | ---------------------------- | ------------------------------------- |
| `string`    | `"Olá, Mundo", "texto", "25" | Texto entre aspas simples ou duplas   |
| `number`    | `10`, `2.5`, `-12`           | Números inteiros ou decimais          |
| `boolean`   | `true`, `false`              | Valores lógicos (verdadeiro/falso)    |
| `undefined` | `let x;`                     | Variável declarada, mas **sem valor** |
| `null`      | `let x = null`               | Valor **intencionalmente vazio**      |
| `bigint`    | `584026430374568n`           | Para números muito grande             |
| `symbol`    | `Symbol("id")`               | Identificadores únicos (avançado)     |

---

## :lupe: Usando `typeof` para descobrir o tipo

O operador `typeof` retorna o tipo variável:

```js
let nome = 'Bruno';
typeof nome; // "string"

let idade = 39;
typeof idade; // "number"

let ativo = true;
typeof ativo; // boolean

let indefinido;
typeof indefinido; // "undefined"
```

---

## :warning: Curiosidade: `null` é do tipo "object"

```js
let x = null;
typeof x; // "object"
```

Isso é um **bug histórico** do JavaScript. Apesar de `null` ser um tipo primitivo, `typeof null` retorna `object` por razões de compatibilidade antiga.

---

## :dart: Diferença entre `undefined` e `null`

| Conceito    | Exemplo         | Significado                                 |
| ----------- | --------------- | ------------------------------------------- |
| `undefined` | `let x;`        | Variável existe, mas **não recebeu valor**  |
| `null`      | `let x = null;` | Valor foi **intensionalmente zerado/vazio** |

---

## :paperclip: Boas práticas com variáveis

- Use `const` por padrão sempre que o valor **não for mudar**.
- Use `let` somente quando você **precisar reatribuir** o valor depois.
- Evite `var` - é um modo antigo, com escopo confuso. Abordaremos mais adiante.

---

## :repeat: Recapitulando

- **Variáveis** armazenam dados para uso posterior.
- `let` permite reatribuição; `const` não.
- Os **tipos primitivos** incluem: `string`, `number`, `boolean`, `undefined`, `null`, `bigint`, `symbol`.
- O operador `typeof` mostra o tipo de um valor.
- `udefined` != `null`: o primeiro é ausência de valor, o segundo é ausência **intencional**
