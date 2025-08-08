# ✅ Exemplos Resolvidos – Aula 04

## **Operadores Aritméticos, Lógicos e Relacionais**

---

### 🔢 1. Soma, Subtração, Multiplicação e Divisão

```js
let a = 10;
let b = 2;

console.log('Soma:', a + b); // 12
console.log('Subtração:', a - b); // 8
console.log('Multiplicação:', a * b); // 20
console.log('Divisão:', a / b); // 5
```

---

### 🧮 2. Resto da Divisão (Módulo)

```js
let x = 17;
let y = 5;

console.log('Resto da divisão:', x % y); // 2
```

---

### 🔍 3. Comparações com Operadores Relacionais

```js
let idade = 18;

console.log(idade > 17); // true
console.log(idade < 18); // false
console.log(idade == '18'); // true (coerção)
console.log(idade === '18'); // false (tipos diferentes)
```

---

### ✅ 4. Comparações Booleanas

```js
let aprovado = true;

console.log(!aprovado); // false
```

---

### 🧠 5. Operadores Lógicos (E, OU, NÃO)

```js
let temIdade = true;
let temDocumento = false;

console.log(temIdade && temDocumento); // false
console.log(temIdade || temDocumento); // true
console.log(!temIdade); // false
```

---

### 📦 6. Comparação de Strings

```js
let nome1 = 'Ana';
let nome2 = 'ana';

console.log(nome1 === nome2); // false
console.log(nome1.toLowerCase() === nome2); // true
```

---

### 📏 7. Expressão Lógica Direta

```js
let idade = 22;
let temCNH = true;

let podeDirigir = idade >= 18 && temCNH;
console.log('Pode dirigir?', podeDirigir); // true
```
