# Aula 01 - Variáveis, Tipos Primitivos e Constantes

---

## :book: 1. Variáveis

Variáveis são espaços nomeados para armazenar dados que podem ser usados e modificados durante a execução do programa.

Em javascript moderno, usamos:

- `let` - para variáveis que podem mudar de valor.
- `const` - para variáveis cujo valor não será reatribuído (constantes).
- `var` - forma antiga, com escopo menos previsível

**Exemplo:**

```js
let idade = 30;
let user = 'bruno';
const meuNome = 'Bruno Miguel Corrêa';
```

---

## :pencil2: 2. Tipos Primitivos

JavaScript possui sete tipos primitivos básicos:

- **String:** texto, exemplo: `"Olá Mundo"`, `"256"`, `'a'`, são especificados através de aspas duplas ou simples
- **Number:** números -> `42`, `253`, `2.4`, `2/3`
- **Boolean:** valores lógicos -> `true` ou `false`
- **Undefined:** variável declarada mas não incializada
- **Null:** ausência intencional de valor
- **Symbol:** identificadores únicos (avançado)
- **BigInt:** números inteiros muito grandes -> `3452745300n`

### :tube: O operador `typeof`

Usamos `typeof` para descobrir o tipo de uma variável:

```js
let idade = 20;
console.log(typeof idade); // "number"
```

> :warning: `console.log()` usado para exibir mensagens no console do navegador ou do ambiente de desenvolvimento
> :dart: Curiosidade: `typeof null` retorna "object". Esse é um 'bug' histórico do JavaScript!

### :link: Escopo de variáveis

Entender **onde** uma variável vive é fundamental. Veja:

| Palavra-chave | Escopo           | Pode ser reatribuída?  |
| ------------- | ---------------- | ---------------------- |
| `var`         | Função ou global | :white_check_mark: Sim |
| `let`         | Bloco `{}`       | :white_check_mark: Sim |
| `const`       | Bloco `{}`       | :x: Não                |

---

## :clipboard: 3. Constantes

Usamos `const` para valores que não devem ser reatribuídos. Se tentar reatribuir, o JavaScript lança erro.

```js
const PI = 3.14159;
```

---

## :scroll: 4. regras para nomes de variáveis

- Devem começar com letras, `_` ou `$`. Não podem começar com números.
- Podem conter letras, números, `$` e `_`
- Case-sensitive (`nome` é diferente de `Nome`)
- Evitar palavras reservadas (`let`, `const`, `if`, etc)

---

## :bulb: 5. Boas práticas

- Use nomes claros e descritivos -> `idadeUsuario`, `precoProduto`
- Prefira `const` sempre que possível para evitar bugs
- Use `let` apenas quando o valor precisa mudar
- Evite `var` - ela ainda existe por questão de compatibilidades, mas pode causar bugs difíceis de rastrear.
- Para projetos reais, use nomes claro e em inglês sempre que possível

---

## :rocket: 6. Exemplos práticos

```js
let contador = 0;
contador = 2; // let permite reatribuir outros valores

const nomeCompleto = 'Bruno Miguel Corrêa';
nomeCompleto = 'Outro nome'; // Erro

let estaLogado = true;
let saldo = 250.9;
```
