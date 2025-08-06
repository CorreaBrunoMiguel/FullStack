# :book: Aula 03 - Conversão de Tipos e Coerção em JavaScript

---

## 1.Introdução

Em Javascript, manipular diferentes tipos de dados é comum e essencial para o desenvolvimento. Muitas vezes, precisamos converter valores entre tipos, como de string para número, ou de booleano para string. Essa ação se chama **conversão de tipos**.

Além disso, JavaScript realiza, automaticamente, algumas conversões de tipo quando necessário, um comportamento chamado **coerção de tipos** (type coercion).

Esta aula aborda esses conceitos fundamentais para evitar erros e escrever códigos mais previsíveis.

---

## 2.Tipos Primitivos e Conversão Explícita

JavaScript como vimos anteriormente, possui alguns tipos primitivos importantes:

- **String**: sequência de caracteres
- **Number**: números (inteiros ou decimais)
- **Boolean**: valores lógicos `true` ou `false`
- **Undefined** e **null**: ausência de valor

\*\*Conversão Explícita

É quando o programador força a conversão de um valor de um tipo para outro, utilizando funções ou métodos específicos.

Principais funções para conversão:

- `String(valor)` - converte para string
- `Number(valor)` - converte para número (ou `NaN` se inválido)
- `Boolean(valor)` - converte para booleano

Exemplos:

```js
let valor1 = 123;
console.log(String(valor1)); // "123"

let valor2 = '456';
console.log(Number(valor2)); // 456

let valor3 = 0;
console.log(Boolean(valor3)); // false
```

Observação: nem toda conversão funciona perfeitamente. Por exemplo:

```js
console.log(Number('abc')); // NaN (Not a Number)
```

---

## 3.Coerção Implícita (Coerção Automática)

O javaScript, em algumas operações, tenta converter valores automaticamente para tipos compatíveis, para executar a operação. Isso pode causar resultados inesperados se não compreendido.

**Exemplos comuns:**

- Operador `+` com string e número;

```js
console.log('5' + 10); // "510" - número é convertido para string e concatenado
```

- Operadores aritméticos com strings numéricas:

```js
console.log('5' * 2); // 10 - string é convertida para número e multiplicado
```

- Comparações com `==` (2 sinais `=`)

```js
console.log(5 == '5'); // true - o valor string é convertido para número antes da comparação
```

Por isso, sempre prefira o operador de comparação estrita `===` (3 sinais de `=`), que compara valor e tipos sem coerção

```js
console.log(5 === '5'); // false
```

---

## 4.Conversão de Booleanos em Operações

Valores considerados **falsy** (equivalentes a falso) em JavaScript são:

- `false`
- `0`
- `""` (string vazia)
- `null`
- `undefined`
- `NaN`

Todos os outros valores são considerados **truthy** (equivalentes a verdadeiro).

---

## 5. Funções Úteis para Testar Conversão

> :warning: Estudaremos melhor o que são funções nas próximas aulas.

- `isNaN(valor)` - verifica se o valor é `NaN` (não número)
- `typeof` - retorna o tipo de dado

---
