# Exemplos Aula 03 - Conversão de Tipos e Coerção

---

## :book: Exemplo 1 - Conversão Explícita (`String()`, `Number()`, `Boolean()`)

```js
let numero = 42;
let convertidoEmTexto = String(numero); // Converte para "42"
console.log(typeof convertidoEmTexto); // string

let texto = '123';
let convertidoEmNumero = Number(texto); // Converte para 123
console.log(typeof convertidoEmNumero); // number

let vazio = '';
let convertidoEmBoolean = Boolean(vazio); // Converte para false
console.log(typeof convertidoEmBoolean); // boolean
```

> :bulb: Aqui usamos as funções `String()`, `Number()` e ´Boolean()` para **forçar a conversão** de um tipo para outro (conversão explícita).

---

## :book: Exemplo 2 - Conversão Implícita (Coerção automática)

```js
let resultado = '5' + 3;
console.log(resultado); // "53"
console.log(typeof resultado); // string
```

> :warning: O JavaScript identifica que há uma **string** com operador `+`, então converteu o número `3` para `"3"` e concatenou: `"5" + "3"` -> "53"

---

## :book: Exemplo 3 - Coerção com subtração

```js
let resultado = '10' - 2;
console.log(resultado); // 8
console.log(typeof resultado); // number
```

> :brain: Aqui, o operador `-` **força a coerção** da string "10" para número", e faz a operação normalmente.

---

## :book: Exemplo 4 = Resultado estranho por coerção com `true` e `false`

```js
console.log('5' + true); // "5true"
console.log('5' - true); // 4
console.log(true + false); // 1
```

> :white_check_mark: `true` é tratado como 1 e false como 0 quando coeridos para números.
> :warning: Mas com `+` e um string, tudo vira texto (ex: `"5" + true` -> `"5true"`)

---

## :book: Exemplo 5 - Uso de `parseInt()` e `parseFloat()`

```js
let valor1 = '42.9';
let valor2 = '100 anos';

console.log(parseInt(valor1)); // 42
console.log(parseFloat(valor1)); // 42.9
console.log(parseInt(valor2)); // 100
console.log(parseInt('abc')); // NaN
```

> :lupe: `parseInt` lê números inteiros no início da string, `parseFloat` lê com decimais. Se não encontrar nenhum número no início, retorna `NaN`.

---

## :book: Booleanos com diferentes contextos

```js
console.log(Boolean('')); // false
console.log(Boolean('texto')); // true
console.log(Boolean(0)); // false
console.log(Boolean(123)); // true
console.log(Boolean(null)); // false
console.log(Boolean(undefined)); // false
```

> :white_check_mark: Em coerção para booleano, alguns valores são considerados "falsy":

- `""`, `0`, `NaN`, `null`, `undefined`, `false` (**Todos os demais são "truthy"**)
