# :book: Aula 04 - Operadores Aritméticos, Lógicos e Relacionais

---

## :brain: Objetivo da aula

Compreender e aplicar os principais operadores utilizados em expressões matemáticas, comparativas e lógicas em JavaScript.

Essa base será essencial para a construção de **estruturas de decisão**, que veremos nas próximas aulas.

---

## :books: Teoria

---

### 1.Operadores Aritméticos

São utilizados para realizar **operações matemáticas** básicas entre valores numéricos.

| Operador | Nome          | Exemplo (`a = 10`, `b = 4`) |
| -------- | ------------- | --------------------------- |
| `+`      | Adição        | `a + b = 14`                |
| `-`      | Subtração     | `a - b = 6`                 |
| `*`      | Multiplicação | `a * b = 40`                |
| `/`      | Divisão       | `a / b = 2.5`               |
| `%`      | Módulo        | `a % b = 2`                 |
| `**`     | Exponenciação | `a ** b = 10000`            |

> :bulb: O operador `%` retorna o **resto** da divisão inteira, muito útil para saber se um número é par, por exemplo.

---

### 2.Operadores de Incremento e Decremento

Usados para **aumentar ou diminuir valores** numéricos de forma rápida.

| Operador | Nome       | Exemplo        | Resultado   |
| -------- | ---------- | -------------- | ----------- |
| `++`     | Incremento | `a++` ou `++a` | `a = a + 1` |
| `--`     | Decremento | `a--` ou `--a` | `a = a - 1` |

:bulb: Pré e pós-incremento

> - `++a`**incrementa antes de usar o valor**
> - `a++`**usa o valor atual, e só depois incrementa**

```js
let x = 5;
console.log(++x); // 5
console.log(x); // 5
console.log(x++); // 6
```

---

### 3.Operadores Relacionais (de Comparação)

Usados para comparar dois valores. O resultado sempre será um **booleano** (`true` ou `false`).

| Operador | Significado            | Exemplo (`a = 5`, `b = "5"`) |
| -------- | ---------------------- | ---------------------------- |
| `==`     | Igual (valor)          | `a == b` -> `true`           |
| `===`    | Estritamente igual     | `a === b` -> false           |
| `!=`     | Diferente (valor)      | `a != b` -> false            |
| `!==`    | Estritamente diferente | `a !== b` -> true            |
| `>`      | Maior que              | `a > 3` -> true              |
| `<`      | Menor que              | `a < 3` -> false             |
| `>=`     | Maior ou igual que     | `a >= b` -> true             |
| `<=`     | Menor ou igual que     | `a <= b` -> false            |

> :fire: Prefira sempre usar `===` e `!==` para evitar erros por coerção implícita.

---

### 4.Operadores Lógicos

Utilizados para combinar ou inverter expressões booleanas.

| Operador | Nome      | Exemplo           | Resultado |
| -------- | --------- | ----------------- | --------- |
| `&&`     | E (AND)   | `true && false`   | `false`   |
| `\|\|`   | OU (OR)   | `true \|\| false` | `true`    |
| `!`      | NÂO (NOT) | `!true`           | `false`   |

**Tabela verdade** - `&&` (E - AND)

| A     | B     | A && B |
| ----- | ----- | ------ |
| true  | true  | true   |
| true  | false | false  |
| false | true  | false  |
| false | false | false  |

**Tabela verdade** - `\|\|` (OU - OR)

| A     | B     | A \|\| B |
| ----- | ----- | -------- |
| true  | true  | true     |
| true  | false | true     |
| false | true  | true     |
| false | false | false    |

**Exemplo Prático**

```js
const idade = 20;
const temCarteira = true;

// Pode dirigir se tiver 18 anos u mais E tiver carteira
const podeDirigir = idade >= 18 && temCarteira;

console.log(podeDirigir);
```

```bash
true
```

---

### 5. Precedência de Operadores

A ordem em que os operadores são avaliados **pode influenciar o resultado** de uma expressão.

**Ordem de precedência básica (da mais alta para a mais baixa)**:

1. `()` - Parênteses
2. `!` - Negação Lógica
3. `**` - Exponenciação
4. `*`, `/`, `%`
5. `+`, `-`
6. Relacionais: `>`, `<`, `>=`, `<=`
7. Igualdades: `==`, `!=`, `===`, `!==`
8. `&&`
9. `||`

**Use sempre parênteses para deixar a expressão mais clara!**

---
