# Exercícios Práticos - Aula 02: Variáveis (`let`, `const`) e tipos primitivos

## 🧪 Exercício 1: Criando variáveis

Crie três variáveis usando `let` para representar:

- O nome de um aluno  
- Sua idade  
- Seu status de matrícula (`true` para matriculado, `false` para não)

> 💡 Dica: use `let` e imprima os valores com `console.log`.

<!-- markdownlint-disable-next-line -->
<details>
  <summary>Ver resposta</summary>

```js
// TODO: declare as variáveis e imprima seus valores no console

let nome = "João";
let idade = 20;
let matriculado = true;

console.log(nome);
console.log(idade);
console.log(matriculado);
```

</details>

---

## 🧪 Exercício 2: Usando `const` corretamente

Crie uma constante para representar o número de CPF de uma pessoa.  
Tente reatribuir um novo valor a essa constante. Observe o que acontece.

> 💡 Dica: `const` não pode ser reatribuída.

<!-- markdownlint-disable-next-line -->
<details>
  <summary>Ver resposta</summary>

```js
// TODO: declare uma constante e tente reatribuir seu valor para ver o erro

const cpf = "123.456.789-00";
// cpf = "987.654.321-00"; // Isso causará erro!

console.log(cpf);
```

</details>

---

## 🧪 Exercício 3: Identificando tipos primitivos

Declare as seguintes variáveis e imprima seus tipos usando `typeof`:

- Um nome (texto)  
- Uma idade (número)  
- Uma altura (número decimal)  
- Um status de aprovação (booleano)

<!-- markdownlint-disable-next-line -->
<details>
  <summary>Ver resposta</summary>

```js
// TODO: declare as variáveis e use console.log com typeof para imprimir os tipos

let nome = "Maria";
let idade = 25;
let altura = 1.68;
let aprovado = true;

console.log(typeof nome);     // string
console.log(typeof idade);    // number
console.log(typeof altura);   // number
console.log(typeof aprovado); // boolean
```

</details>

---

## 🧪 Exercício 4: `let` vs `const`

Explique a diferença entre `let` e `const` em termos de reatribuição de valor.  
Depois, escreva um código que mostre um exemplo para cada um.

<!-- markdownlint-disable-next-line -->
<details>
  <summary>Ver resposta</summary>

```js
// TODO: escreva código que exemplifique o uso de let e const

// let permite reatribuição
let contador = 1;
contador = 2;
console.log(contador); // 2

// const não permite reatribuição
const pi = 3.14;
// pi = 3.1415; // Isso geraria um erro

console.log(pi);
```

</details>

---

## 🧪 Exercício 5: Atribuindo valores diferentes

Crie uma variável chamada `anoNascimento` com valor `1995`.  
Depois, atribua o valor `"mil novecentos e noventa e cinco"` a ela e observe o tipo.

> 💡 Dica: Repare como o tipo pode mudar devido à tipagem dinâmica do JavaScript.

<!-- markdownlint-disable-next-line -->
<details>
  <summary>Ver resposta</summary>

```js
// TODO: declare e reatribua a variável, mostrando os tipos com typeof

let anoNascimento = 1995;
console.log(typeof anoNascimento); // number

anoNascimento = "mil novecentos e noventa e cinco";
console.log(typeof anoNascimento); // string
```

</details>

---
