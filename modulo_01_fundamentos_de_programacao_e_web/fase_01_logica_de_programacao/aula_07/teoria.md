# :books: Aula 07 - Funções e Escopo

---

## :book: 1. Introdução

No desenvolvimento, funções são como pequenas "máquinas" dentro do seu código: vocÊ coloca algo dentro (argumentos), a máquina processa, e ela pode ou não devolver algo (retorno).
Elas servem para **reutilizar código**, **organizar lógica** e **reduzir repetição**.

---

## :pencil2: Funções: O uqe são e por que usar

Uma **função** é um bloco de código nomeado que pode ser executado sempre que necessário.

**Benefícios:**

- Reuso de código
- Clareza e organização
- Facilidade de manutenção

Exemplos básico:

```js
function saudacao() {
  console.log('Olá, mundo!');
}

saudacao(); // Chama a função
```

---

## :scroll: Estrutura básica de uma função

Formato padrão:

```js
function nomeDaFuncao(param1, param2) {
  // bloco de código
  return valor; // opcional
}
```

**Palavra-chave:**

- `function`: indica que estamos declarando uma função
- `nomeDaFuncao`: identificador (pode seguir regras de nomes de variáveis)
- `param1, param2`: parâmetros
- `return`: devolve um valor para quem chamou

---

## :clipboard: 4. Parâmetros e argumentos

- **Parâmetros**: variável declarada na função, usada para receber um valor.
- **Argumentos**: valor passado quando a função é chamada

```js
function soma(a, b) {
  return a + b;
}

soma(5, 3); // retorna 8
```

Aqui:

`a` e `b` -> parâmetros
`5` e `3` -> argumentos

---

## 5. :file_folder: Retorno de valores

Funções podem ou não devolver um valor usando `return`.

```js
function quadrado(numero) {
  return numero * numero;
}

let resultado = quadrado(4);
console.log(resultado); // 16
```

:warning: Após executar `return`, a função é encerrada

---

## :paperclip: 6. Escopo e variável: global vs local

**Escopo** é a área do código onde uma variável existe.

- **Global**: variável declarada fora de qualquer função -> acessível em todo o código.
- **Local**: variável declarada dentro de uma função -> só acessível dentro dela.

```js
let globalVar = 'Sou global';

function teste() {
  let localVar = 'Sou local';
  console.log(globalVar); // funciona
  console.log(localVar); // funciona
}

teste();
console.log(globalVar); // funciona
console.log(localVar); // ERRO: localVar is not defined
```

## :book: 7. Escopo de bloco (`let` e `const`)

Com `let` e `const`, variáveis respeitam **blocos** (entre `{ }`), não apenas funções.

```js
if (true) {
  let x = 10;
  const y = 20;
  console.log(x, y); // 10 20
}

console.log(x); // ERRO
```

---

## :pencil: Escopo léxico e contexto de execução

O **escopo léxico** é definido no momento em que a função é escrita, não quando é executada.

```js
let nome = 'Bruno';

function falarNome() {
  console.log(nome);
}

falarNome(); // Bruno
```

mesmo que seja chamada em outro lugar, a função lembra o ambiente onde foi criada.

---

## :dart: 9. Boas práticas

- Nomear funções de forma descritiva(`calcularMedia`, `validarEmail`)
- Funções curtas e focadas em um única responsabilidade.
- Evitar variáveis globais quando possível
- Comentar funções complexas
