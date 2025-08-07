# 🧪 Exercícios Práticos – Aula 04

## **Operadores Aritméticos, Lógicos e Relacionais (sem condicionais)**

---

### 01. Operações Aritméticas

Exiba os resultados das 4 operações básicas com dois números.

```js
let x = 12;
let y = 4;

console.log('Soma:', x + y);
console.log('Subtração:', x - y);
console.log('Multiplicação:', x * y);
console.log('Divisão:', x / y);
```

---

### 02. Resto da Divisão

Exiba o resto da divisão entre dois números.

```js
let a = 15;
let b = 6;

console.log('Resto da divisão:', a % b); // 3
```

---

### 03. Comparações Simples

Mostre o resultado (true ou false) das comparações abaixo.

```js
let n1 = 10;
let n2 = 20;

console.log('n1 > n2:', n1 > n2);
console.log('n1 < n2:', n1 < n2);
console.log('n1 == n2:', n1 == n2);
console.log('n1 != n2:', n1 != n2);
```

---

### 04. Comparando Strings

Compare duas strings e exiba se são iguais ou diferentes.

```js
let nome1 = 'joao';
let nome2 = 'Joao';

console.log('São iguais?', nome1 === nome2);
console.log('São diferentes?', nome1 !== nome2);
```

---

### 05. Operações com Booleanos

Use operadores lógicos (`&&`, `||`, `!`) para exibir os resultados abaixo.

```js
let idade = 25;
let temCarteira = true;

console.log('Pode dirigir (idade >= 18 E tem carteira)?', idade >= 18 && temCarteira);
console.log('Precisa de autorização especial?', !(idade >= 18 && temCarteira));
```

---

### 06. Verificando Intervalo (sem if)

Use apenas expressões e `console.log()` para saber se um número está entre 50 e 100.

```js
let numero = 75;

console.log('Está entre 50 e 100?', numero >= 50 && numero <= 100);
```

---

### 07. Testando igualdade com diferentes tipos

Mostre a diferença entre `==` e `===`.

```js
let valor1 = '123';
let valor2 = 123;

console.log('Usando == :', valor1 == valor2); // true (coerção)
console.log('Usando ===:', valor1 === valor2); // false (tipos diferentes)
```

---

### 08. Inversão com NOT

Use o operador `!` para inverter um valor booleano.

```js
let logado = false;

console.log('Está logado?', logado);
console.log('Não está logado?', !logado);
```

---

### 09. Expressões compostas

Avalie as expressões lógicas abaixo e exiba os resultados.

```js
let a = 5;
let b = 10;

console.log('a > 2 && b < 15:', a > 2 && b < 15); // true
console.log('a < 2 || b == 10:', a < 2 || b == 10); // true
```

---

### 10. Comparações com resultado direto

Declare três números e exiba se todos são iguais, ou se algum é diferente, apenas com expressões.

```js
let n1 = 7;
let n2 = 7;
let n3 = 7;

console.log('Todos são iguais?', n1 === n2 && n2 === n3);
console.log('Algum é diferente?', n1 !== n2 || n2 !== n3);
```
