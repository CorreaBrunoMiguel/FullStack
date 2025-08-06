# Quiz Aula 03 - COnversão de Tipos e Coerção

<!-- markdownlint-disable -->

1. O que é conversão explícita em JavaScript?

- [ ] Quando o JavaScript converte valores automaticamente para outro tipo.
- [ ] Quando o programador força a conversão de tipos usando funções específicas.
- [ ] Quando se usa apenas o operador `==` para comparação.
- [ ] Quando o valor permanece no mesmo tipo sem alteração

<details>
  <summary>Ver Resposta</summary>

> [x] Quando o programador força a conversão de tipos usando funções específicas.

> **Explicação:** Conversão explícita ocorre quando o programador usa funções como `String()`, `Number()` ou `Boolean()` para converter um valor de um tipo para outro.

</details>

---

2.Qual resultado do código abaixo?

```js
console.log('5' + 10);
```

- [ ] "510"
- [ ] 15
- [ ] NaN
- [ ] Erro

<details>
  <summary>Ver Resposta</summary>

> [x] "510"

> **Explicação:** O operador `+` concatena strings. Como um dos operadores é string, o número `10` é convertido para string e concatenado, formando "510".

</details>

---

3.Qual das opções representa um valor considerado falsy em JavaScript?

- [ ] "false"
- [ ] 1
- [ ] "0"
- [ ] 0

<details>
  <summary>Ver Resposta</summary>

> [x] 0

> **Explicação:** O valor `0` é falsy, ou seja, avaliado como falso em contextos booleanos, diferentes das strings, que são truthy mesmo que contenham "false" ou "0". Apenas strings vazias "" são falsy neste contexto.

</details>

---

4.O que acontece ao comparar `5 == "5"`?

- [ ] Retorna false, porque os tipos são diferentes.
- [ ] Gera um erro de tipo.
- [ ] Retorna true,pois ocorre coerção implícita convertendo a string em número.
- [ ] Retorna true somente se usar o operador `===`.

<details>
  <summary>Ver Resposta</summary>

> [x] Retorna true, pois ocorre coerção implícita convertendo a string em número.

> **Explicação:** O operador == permite coerção de tipo, então "5" é convertido para número 5 antes da comparação.

</details>

---

5.Qual é o valor do seguinte código?

```js
console.log(Boolean(''));
```

- [ ] true
- [ ] undefined
- [ ] NaN
- [ ] false

<details>
  <summary>Ver Resposta</summary>

> [x] false

> **Explicação:** A string vazia `""` é considerada falsy e, portanto convertida para false pelo `Boolean()`

</details>

---

6.Como evitar problemas causados pela coerção implícita em comparações?

- [ ] Evitando usar comparações entre tipos diferentes
- [ ] Usando sempre o operador `==`
- [ ] Usando o operador `===` para comparações estrita
- [ ] Convertendo tudo para string antes de comparar

<details>
  <summary>Ver Resposta</summary>

> [x] Usando o operador `===` para comparação estrita

> **Explicação:** O operador `===` compara valor e tipo, sem realizar coerção automática, evitando resultados inesperados.

</details>

---

7.Qual função verifica se um valor é `NaN` (não número)?

- [ ] `isNumber()`
- [ ] `typeof`
- [ ] `Number()`
- [ ] `isNaN()`

<details>
  <summary>Ver Resposta</summary>

> [x]`isNaN()`

> **Explicação:** A função `isNaN()` verifica se um valor é `NaN`, indicando uma conversão inválida para número.

</details>
