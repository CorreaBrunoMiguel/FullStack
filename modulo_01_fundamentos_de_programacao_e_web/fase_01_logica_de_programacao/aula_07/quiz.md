# :books: Quiz - Aula 07

## <!-- markdownlint-disable -->

---

## 1. Qual a principal vantagem de criar funções em um programa JavaScript?

- [ ] Elas evitam o uso de variáveis globais
- [ ] Elas permitem reutilizar código e organizar a lógica
- [ ] Elas sempre aumentam a velocidade de execução
- [ ] Elas impedem o uso de loops

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Elas permitem reutilizar código e organizar a lógica`

:dart: Funções encapsulam blocos de códigos que podem ser executados múltiplas vezes, evitando repetição e facilitando a organização.

</details>

---

## 2. O que o código abaixo imprime no console?

```js
function saudacao(nome) {
  return 'Olá, ' + nome;
}
console.log(saudacao('Bruno'));
```

- [ ] `Olá, Bruno`
- [ ] `undefined`
- [ ] `Olá, nome`
- [ ] `null`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Olá, Bruno`

:dart: A função `saudacao` recebe o parâmetro `"Bruno"` e retorna a string concatenada, que é impressa no console.

</details>

---

## 3. Qual é a diferença entre **escopo global** e **escopo local**?

- [ ] Global só existe dentro de funções, local fora delas
- [ ] Local é acessível de qualquer lugar, global não
- [ ] Não existe diferença
- [ ] Global é acessível em qualquer parte do código, local apenas dentro do bloco onde foi declarado

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Global é acessível em qualquer parte do código, local apenas dentro do bloco onde foi declarado`

:dart: Escopo global é visível por todo o programa. Escopo local é limitado ao bloco `{ }` ou função onde foi criado.

</details>

---

## 4. O que será impresso no console?

```js
let x = 10;
function teste() {
  let x = 5;
  console.log(x);
}
teste();
console.log(x);
```

- [ ] `5` e depois `10`
- [ ] `5` e depois `5`
- [ ] `10` e depois `10`
- [ ] `10` e depois `5`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `5 e depois 10`

:dart: Dentro da função `teste`, a variável `x` local tem valor 5. Fora da função, a `x` global continua sendo 10.

</details>

---

## 5. Sobre **hoisting** em funções, qual afirmação é verdadeira?

- [ ] Funções declaradas com `function nome() {}` são carregadas antes da execução do código
- [ ] Funções atribuídas a variáveis com `const` são carregadas antes da execução
- [ ] Nenhum tipo de função sofre hoisting
- [ ] Apenas arrow functions sofrem hoisting

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Funções declaradas com `function nome() {}` são carregadas antes da execução do código`

:dart: Declarações de função são içadas (hoisted) para o topo do escopo antes da execução, permitindo chamá-las antes da declaração.

</details>

---

## 6. Qual será a saída no console?

```js
if (true) {
  var a = 1;
  let b = 2;
}
console.log(a);
console.log(b);
```

- [ ] `1` e depois `2`
- [ ] `1` e depois `erro`
- [ ] `erro` e depois `2`
- [ ] `erro` e depois `erro`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `1 e depois erro`

:dart: Variáveis declaradas com `var` têm escopo de função/global, então `a` existe fora do bloco. Já `b` tem escopo de bloco e gera erro de referência fora dele.

</details>

---
