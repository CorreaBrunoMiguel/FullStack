# :book: Exemplos - Aula 05

---

## 1.Uso simples de `if`

```js
const idade = 18;

if (idade >= 18) {
  console.log('Maior de idade');
}
```

Resultado:

```bash
Maior de idade
```

**Explicação:** Se `idade` for 10 ou mais, a mensagem será exibida.

---

## 2. `if...else` para decisão binária

```js
const nota = 7;

if (nota >= 6) {
  console.log('Aprovado');
} else {
  console.log('Reprovado');
}
```

Resultado:

```bash
Aprovado
```

**Explicação:** Mostra `Aprovado` se a nota for maior ou igual a 6, caso contrário `Reprovado`

---

## 3. Uso de `else if` para múltiplas condições

```js
const temperatura = 30;

if (temperatura < 20) {
  console.log('Frio');
} else if (temperatura < 30) {
  console.log('Agradável');
} else {
  console.log('Quente');
}
```

Resultado:

```bash
Quente
```

**Explicação:** Classifica a temperatura em três faixas.

---

## 4. `swicth` básico

```js
const dia = 3;

switch (dia) {
  case 1:
    console.log('Segunda-feira');
    break;
  case 2:
    console.log('Terça-feira');
    break;
  case 3:
    console.log('Quarta-feira');
    break;
  default:
    console.log('Dia inválido');
}
```

Resultado:

```bash
Quarta-feira
```

**Explicação:**
Exibe o nome do dia baseado no número. Caso não reconhecido, exibe, `Dia inválido`.

---

## 5. `switch` com agrupamento de casos

```js
const letra = 'a';

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

Resultado:

```bash
Vogal
```

**Explicação:** Agrupa várias opções para executar o mesmo código.

---

## 6.Uso de `switch(true)` para intervalos (técnica comum)

```js
const nota = 85;

switch (true) {
  case nota >= 90:
    console.log('A');
    break;
  case nota >= 80:
    console.log('B');
    break;
  case nota >= 70:
    console.log('C');
    break;
  default:
    console.log('F');
}
```

Resultado:

```bash
B
```

**Explicação:** Como `switch` compara estritamente, usamos `switch(true)` para avaliar condições booleanas.

---
