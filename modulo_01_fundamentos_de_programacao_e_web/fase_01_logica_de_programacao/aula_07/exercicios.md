# :rocket: Exercícios - Aula 07

<!-- markdownlint-disable -->

---

## :seedling: 1. Dobrar número

Crie uma função chamada `dobrar` que receba um número e retorne o dobro desse número.

<details>
  <summary>Ver Resposta</summary>

```js
function dobrar(n) {
  return n * 2;
}
console.log(dobrar(8)); // 16
```

:dart: Função simples com parâmetro e retorno

</details>

---

## :seedling: 2. Mensagem de boas-vindas

Crie uma função `mensagemBoasVindas` que exiba `"Bem-vido ao sistema!"` no console

<details>
  <summary>Ver Resposta</summary>

```js
function mensagemBoasVindas() {
  console.log('Bem-vindo ao sistema!');
}
mensagemBoasVindas();
```

:dart: Função sem parâmetro e sem retorno

</details>

---

## :pencil: 3. Escopo local e global

Crie uma variável global `usuario` com o valor `"Bruno"`.
Dentro de uma função `mostrarUsuario`, crie uma variável local `usuario` com valor `"Maria"` e exiba dentro e fora da função.

<details>
  <summary>Ver Resposta</summary>

```js
let usuario = 'Bruno';

function mostrarUsuario() {
  let usuario = 'Maria';
  console.log(usuario); // Maria
}

mostrarUsuario();
console.log(usuario); // Bruno
```

:dart: Variáveis locais não afetam a global com mesmo nome.

</details>

---

## :pencil: 4. Cálculo de área com parâmetros

Crie uma função `calcularArea` que receba largura e altura e retorne a área. Chame a função para largura 5 e altura 3.

<details>
  <summary>Ver Resposta</summary>

```js
function calcularArea(largura, altura) {
  return largura * altura;
}
console.log(calcularArea(5, 3)); // 15
```

:dart: Uso de múltiplos parâmetros e retorno

</details>

---

## :muscle: 5. Hoisting em função declarada

Escreva um código que chame a função `somar` antes de ser declarada.
A função deve receber dois números e retornar a soma.

<details>
  <summary>Ver Resposta</summary>

```js
console.log(somar(2, 4)); // 6

function somar(a, b) {
  return a + b;
}
```

:dart: Funções declaradas com `function` são içadas (hoisting)

</details>

---

## :muscle: 6. Contador de chamadas

Crie uma função `registrarVisita` que use uma variável local para contar quantas vezes foi chamada e exiba esse úmero no console.
Dica: use variável global ou externa para manter a contagem.

<details>
  <summary>Ver Resposta</summary>

```js
let contador = 0;

function registrarVisita() {
  contador++;
  console.log(`Visita número ${contador}`);
}

registrarVisita();
registrarVisita();
registrarVisita();
```

:dart: Variável externa à função mantém estado entre chamadas

</details>

---

## :exploding_head: 7. Função que altera variável global

Crie uma variável global `saldo` com valor `1000`
Crie uma função `sacar` que receba um valor, subtraia do saldo e retorne o novo saldo.
Não permita saques maiores que o saldo disponível.

<details>
  <summary>Ver Resposta</summary>

```js
let saldo = 1000;

function sacar(valor) {
  if (valor > saldo) {
    return 'Saldo insuficiente';
  }
  saldo -= valor;
  return saldo;
}

console.log(sacar(300)); // 700
console.log(sacar(800)); // Saldo insuficiente
```

:dart: Uso de escopo global com controle de fluxo

</details>

---

## :exploding_head: 8. Multiplicação segura

Crie uma função `multiplicarSegura` que receba dois parâmetros.
Antes de multiplicar, verifique se ambos são números (use `typeof`).
Se não forem, retorne `"Parâmetros inválidos"`.

<details>
  <summary>Ver Resposta</summary>

```js
function multiplicarSegura(a, b) {
  if (typeof a !== 'number' || typeof b !== 'number') {
    return 'Parâmetros inválidos';
  }
  return a * b;
}

console.log(multiplicarSegura(3, 4)); // 12
console.log(multiplicarSegura(3, 'x')); // Parâmetros inválidos
```

:dart: Validação de parâmetros antes da operação.

</details>

---
