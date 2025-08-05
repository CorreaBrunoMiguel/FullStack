# Exemplos Resolvidos

---

## :tomato: Exemplo 01: Criando variáveis com `let`

```js
let nome = 'Bruno';
console, log(nome); // Saída: Bruno

nome = 'Miguel';
console.log(nome); // Saída: Miguel
```

> :white_check_mark: Com `let` é possível **declarar e reatribuir valores.**

---

## :banana: Exemplo 02: Criando constantes com `const`

```js
const pi = 3.14;
console.log(pi); // Saída: 3.14

pi = 3.14159; // Erro! Não é possível reatribuir uma constante
```

> :warning: Constantes precisam ser **inicializadas no momento da declaração e não podem ser reatribuídas**.

---

## :apple: Exemplo 03: Tipos primitivos com `typeof`

```js
let nome = 'Joana';
let idade = 28;
let ativo = true;
let indefinido;
let nulo = null;

console.log(typeof nome); // string
console.log(typeof idade); // number
console.log(typeof ativo); // boolean
console.log(typeof indefinido); // undefined
console.log(typeof nulo); // object (curiosidade: isso é uma "falha" histórica do JS)
```

> :white_check_mark: `typeof` retorna o tipo primitivo da variável
> :warning: `null` retorna `object` por uma questão de compatibilidade histórica no JavaScript.

---

## :peach: Exemplo 04: Reatribuindo valores com `let`

```js
let status = 'ativo';
console.log(status); // ativo

status = true;
console.log(status); // true

status = 1;
console.log(status); // 1
```

> :bulb: Uma variável declarada com `let` pode mudar de tipo durante a execução - isso é característica da **tipagem dinâmica** do JavaScript.

---

## :melon: Exemplo 05: Diferença entre `null`e `undefined`

```js
let produto;
let preco = null;

console.log(produto); // undefined (não foi atribuído nenhum valor)
console.log(preco); // null (valor intencionalmente vazio)
```

> :white_check_mark: `undefined`: valor padrão de uma variável não inicializada.
> :white_check_mark: `null` valor vazio \*\*intencional`, usado para "zerar" ou "limpar" um valor.
