# Aula 05 - Estruturas de Controle: if, else, switch

## 1. Introdução às Estruturas de Controle

Até agora, aprendemos a fazer operações, usar variáveis, operadores e exibir resultados. Mas para tomar decisões no programa, precisamos que ele "escolha" caminhos diferentes dependendo das condições.

As **estruturas de controle** permitem isso. As principais que veremos nesta aula são:

- `if` - executa um bloco se a condição for verdadeira.
- `else` - executa um bloco alternativo caso a condição do `if` seja falsa.
- `else if` - verifica outra condição caso a anterior seja falsa.
- `switch` - permite múltiplas escolhas com base no valor de uma expressão.

---

## 2. Estrutura `if`

A sintaxe do `if` é:

```js
if (condição) {
  // código executado se a condição for verdadeira
}
```

Exemplo:

```js
let idade = 18;

if (idade >= 18) {
  console.log('Você é maior de idade.');
}
```

Aqui, se a variável `idade` for maior ou igual a 18, a mensagem será exibida.

---

## 3. Estrutura `if...else`

Para executar um código alternativo quado a condição for falsa, usamos `else`:

```js
let idade = 16;

if (idade >= 18) {
  console.log('Você é maior de idade.');
} else {
  console.log('Você é menor de idade.');
}
```

---

## 4. Estrutura `if...else if..else`

Para testar múltiplas condições sequenciais:

```js
let nota = 7;

if (nota >= 7) {
  console.log('Aprovado');
} else if (nota >= 5) {
  console.log('Recuperação');
} else {
  console.log('Reprovado');
}
```

---

## 5. Estrutura `switch`

èrmite testar o valor de uma expressão para várias possibilidades:

```js
let dia = 3;

switch (dia) {
  case 1:
    console.log('Domingo');
    break;
  case 2:
    console.log('Segunda-feira');
    break;
  case 3:
    console.log('Terça-feira');
    break;
  default:
    console.log('Dia inválido');
}
```

---

## 6. Considerações finais

- Use `if` para condições simples.
- Use `else` para alternativas.
- Use `else if` para múltiplas verificações.
- Use `switch` quando precisar comparar uma variável contra múltiplos valores.
