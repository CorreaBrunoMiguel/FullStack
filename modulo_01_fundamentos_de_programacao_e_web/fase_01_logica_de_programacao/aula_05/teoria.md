# Aula 05 - Estruturas de Controle (if, else, switch)

---

## 1.Introdução

Estruturas de controle (ou estruturas de decisão) permitem que seu programa **execute blocos diferentes de código** dependendo de condições. Sem elas, todo programa seria linear - sem possibilidade de reagir a dados de entrada ou estados diferentes.

Em JavaScript usamos `if`, `else`, `else if` e `switch` para isso. Dominá-los é essencial para escrever lógica condicional limpa, legível e correta.

---

## 2.Condição = booleanos e truthy/false

Uma **condição** é uma expressão que será avaliada com `true` ou `false`. Mas em JavaScript muitas expressões não são booleanas pura; por isso existe o conceito de truthy (avaliado como `true`) e falsy (avaliado como `false`) quando convertidas para booleano.

Valores **falsy**:

- `false`
- `0` e (`-0`)
- `on` (BigInt zero)
- `""` (string vazia)
- `null`
- `undefined`
- `NaN`

Tudo que não for falsy é **truthy** - por exemplo, `[]`, `{}`, `"0"`, `function(){}` são truthy.

**Dica:** Usar `Boolean(valor)` ou `!!valor` para inspecionar como algo será avaliado.

---

## 3. `if` - sintaxe básica e exemplos

Sintaxe:

```js
if (condição) {
  // bloco executado se condição for true
}
```

Exemplo:

```js
const idade = 20;

if (idade >= 18) {
  console.log('Maior de idade');
}
```

**Observações:**

- A condição dentro dos parênteses pode ser qualquer expressão que resulte em valor truthy/falsy.
- É fortemente recomendado **sempre usar chaves**, mesmo para uma única linha - evita erros ao adicionar linhas depois.

---

## 4. `else` e `else if` - encadeamento

Uso do `else`:

```js
if (condição) {
  // quando true
} else {
  // quando false
}
```

Uso de `else if`:

```js
if (condição1) {
  // bloco 1
} else if (condição2) {
  // bloco 2
} else {
  // nenhum dos anteriores
}
```

**Importante:** `else if` é avaliado **em ordem** - assim que um bloco é satisfeito, o restante é ignorado.

Exemplo (classificação por nota):

```js
const nota = 78;

if (nota >= 90) {
  console.log('A');
} else if (nota >= 80) {
  console.log('B');
} else if (nota >= 70) {
  console.log('C');
} else {
  console.log('D');
}
```

Observe a ordem: `>= 90` primeiro, depois `>= 80`, etc. Se invertemos a ordem, a lógica quebra.

---

## 5. `switch` - sintaxe, `case`, `break` e fall-trough

`switch` é adequado quando você precisa compara **um expressão** contra vários valores definidos.

Sintaxe:

```js
switch (expressão) {
  case valor1:
    // código
    break;
  case valor2:
    // código
    break;
  default:
  // código caso nenhum case encaixe
}
```

**Pontos importantes:**

- `switch` usa comparação estrita (`===`) entre `expressão` e cada `case` (portanto tipos importam).
- `break` evita o fall-trough (continuação para os próximos `case`). Sem `break`, o código "cai" até encontrar um `break` - às vezes desejado (agrupamento), às vezes bug.
- `default` é executado quando nenhum `case` corresponde.

Exemplo simples:

```js
const dia = 2;

switch (dia) {
  case 0:
    console.log('Domingo');
    break;
  case 1:
    console.log('Segunda');
    break;

  case 2:
    console.log('Terça');
    break;
  default:
    console.log('Outro dia');
}
```

**Agrupando casos:**

```js
switch (letra) {
  case 'a':
  case 'e':
  case 'i':
  case 'o':
  case 'u':
    console.log('Vogal');
    break;
  default:
    console.log('Consoante');
}
```

**Padrão para ranges:**

```js
const x = 72;
switch (true) {
  case x >= 90:
    console.log('A');
    break;
  case x >= 80:
    console.log('B');
    break;
  case x >= 70:
    console.log('C');
    break;
  default:
    console.log('D');
}
```

Essa técnica funciona porque cada `case` é comparado com `true` usando `===`.
