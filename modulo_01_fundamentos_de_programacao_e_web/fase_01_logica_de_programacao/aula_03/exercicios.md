# Exercícios Aula 03 - Conversão de Tipos e Coerção

:bulb: Não existe apenas uma forma de responder as questões dos exercícios propostos abaixo. A respostas para cada exercícios é apenas uma de muitas formas de se fazer.

---

<!-- markdownlint-disable -->

1. Converta o valor da variável `idade` em string e exiba seu tipo.

```js
let idade = 30;

// Sua lógica aqui
```

<details>
  <summary>Ver Resposta</summary>

```js
let idade = 30;
let idadeTexto = String(idade);
console.log(typeof idadeTexto); // "string"
```

> `String(idade) converte explicitamente o número para texto

</details>

---

2. Transforme a string `"99.5"` em número decimal e exiba o resultado somado com `0.5`

```js
let valor = '99.5';

// Sua Lógica aqui
```

<details>
  <summary>Ver Resposta</summary>

```js
let valor = '99.5';
let resultado = parseFloat(valor) + 0.5;
console.log(resultado); // 100
```

> `parseFloat` mantém os decimai. A soma resulta em 100

</details>

---

3. Qual será o resultado e o tipo da variável `resultado`?

```js
let resultado = '100' - 50;
console.log(resultado);
console.log(typeof resultado);
```

> **Resposta:**

<details>
  <summary>Ver Resposta</summary>

```txt
50
number
```

> `"100"` é convertido implicitamente para número por causa do `-`

</details>

---

4. Use `parseInt()` para extrair o número inicial da string e ignore o restante.

```js
let entrada = '42px';
// Sua lógica aqui
```

<details>
  <summary>Ver Resposta</summary>

```js
let numero = parseInt(entrada);
console.log(numero); // 42
```

> `parseInt` ignora tudo após o número

</details>

---

5. COnverta os seguintes valores para booleanos e comente o resultado:

```js
console.log(Boolean(0));
console.log(Boolean(' '));
console.log(Boolean(null));
console.log(Boolean('false'));
```

<details>
  <summary>Ver Resposta</summary>

```txt
false // 0 é falsy
true // espaço em branco é truthy
false // null é falsy
true // string "false" é uma string não vazia, logo é truthy
```

</details>

---

6. O que será impresso no console?

```js
console.log('7' + true);
console.log('7' - true);
```

<details>
  <summary>Ver Resposta</summary>

```txt
7true // + faz coerção para string
6     // true -> 1 : "7" - 1 = 6
```

</details>

---

7. Complete a operação para que o resultado final seja o número 10, não a string "510".

```js
let a = '5';
let b = 5;

// Sua lógica aqui
```

<details>
  <summary>Ver Resposta</summary>

```js
let a = '5';
let b = 5;
let resultado = Number(a) + b;
console.log(resultado); // 10
```

> `Number(a)` força a conversão da string para número

## </details>

8. Complete a lógica para converter `valor` em números inteiro.

```js
let valor = '75.8';

// Sua lógica aqui
```

<details>
  <summary>Ver Resposta</summary>

```js
let valor = '75.8';
let inteiro = parseInt(valor);
console.log(inteiro); // 75
```

> `parseInt` ignora a parte decimal

</details>

---

9. Converta o booleano `true` em número e some com 2.

```js
let status = true;

// Sua lógica aqui
```

<details>
  <summary>Ver Resposta</summary>

```js
let status = true;
let resultado = Number(status) + 2;
console.log(resultado); // 3
```

> `true` -> 1. Soma com 2 -> 3

## </details>

---

10. Identifique qual das variáveis abaixo será considerada `false` ao ser convertido para booleano.

```js
let a = '';
let b = '0';
let c = 0;
let d = 'false';

// Sua análise aqui
```

<details>
  <summary>Ver Resposta</summary>

```txt
a = ""      → false
b = "0"     → true
c = 0       → false
d = "false" → true
```

> Somente `a` e `c` são falsy

## </details>
