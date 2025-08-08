# ❓ Quiz - Aula 04

<!-- markdownlint-disable -->

---

1.Qual será o resultado da expressão `10 % 3` em JavaScript?

- [ ] `3`
- [ ] `0`
- [ ] `1`
- [ ] `10`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `1`

:brain: **Explicação:** O operador `%` retorna o **resto da divisão inteira**. Como `10 / 3 = 3 (sobra 1)`

</details>

---

2.Dados o código abaixo, qual será o valor impresso?

```js
let a = 5;
console.log(a++);
```

- [ ] `6`
- [ ] `5`
- [ ] `Erro`
- [ ] `undefined`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `5`

:brain: **Explicação:** O `a++` é um **pós-incremento**, ou seja, o valor é usado **antes de ser incrementado**. Depois disso, `a` se torna `6`.

</details>

---

3.Qual operador lógico retorna `true` apenas quando ambos os operandos forem `true`?

- [ ] `&&`
- [ ] `||`
- [ ] `==`
- [ ] `!==`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `&&`

:brain: **Explicação:** O operador `&&` (E lógico) só retorna `true` quando **os dois lados** da expressão forem verdadeiros.

</details>

---

4.O que retorna a expressão `5 === "5"`?

- [ ] `true`
- [ ] `"true"`
- [ ] `false`
- [ ] `"false"`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `false`

:brain: **Explicação:** O operador `===` verifica o **valor e tipo**. Aqui temos um número e uma string - tipos diferentes - portanto, `false`.

</details>

---

5.Dado o código:

```js
let x = 4;
let y = 2;
console.log(x > y && y > 3);
```

Qual será a saída?

- [ ] `false`
- [ ] `true`
- [ ] `undefined`
- [ ] `Erro`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `false`

:brain: **Explicação:** `x > y` é `true`, mas `y > 3` é `false`. Com `&&` ambos precisam ser verdadeiros para o resultado ser `true`, logo `true && false` é `false`

</details>

---

6.O que significa o operador `!==`?

- [ ] Igual em tipo e valor
- [ ] Diferente apenas em tipo
- [ ] Diferente em tipo **ou** valor
- [ ] Nenhuma das anteriores

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: Diferente em tipo **ou** valor

:brain: **Explicação:** O `!==` retorna `true` quando os valores **ou** os tipos **são diferentes**.

</details>

---

7.O que acontece ao executar:

```js
console.log(2 + 3 * 4);
```

- [ ] 20
- [ ] 24
- [ ] 18
- [ ] 14

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `14`

:brain: **Explicação:** A multiplicação (`3 * 4 = 12`) ocorre **antes** da soma, por causa da **precedência de operadores**. Depois `2 + 12 = 14`.

</details>

---

8.Se `a = 3` e `b = 7`, qual o resultado de `a <= b || b > 10`?

- [ ] `true`
- [ ] `false`
- [ ] `undefined`
- [ ] `Erro`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `true`

:brain: **Explicação:** `a <= b` é `true`, e `b > 10` é `false`. Comm `||`, basta que uma opção seja `true` para resultado ser `true` (`true || false -> true`)

</details>
