# :rocket: Exercícios - Aula 05

<!-- markdownlint-disable -->

**Observação:** Existe mais de uma forma de resolver cada exercício,a resposta gerada é apenas uma de muitas possibilidades.

---

## :seedling: Exercício 1 - Maioridade

Receba a idade de uma pessoa e informe se ela é maior de idade (18 anos oou mais) ou menor

<details>
  <summary>Ver Resposta</summary>

```js
const idade = 17;

if (idade >= 18) {
  console.log('Maior de idade');
} else {
  console.log('Menor de idade');
}
```

```bash
Menor de idade
```

:bulb: Usamos `if` para comparar a idade e decidir a mensagem

</details>

---

## :seedling: Exercício 2 - Número Par ou Ímpar

Receba um número inteiro para comparar se ele é par ou ímpar.

<details>
  <summary>Ver Resposta</summary>

```js
const num = 10;

if (num % 2 === 0) {
  console.log('Par');
} else {
  console.log('Ímpar');
}
```

```bash
Par
```

:bulb: Operador `%` determina o resto da divisão; se zero, é par.

</details>

---

## :pencil2: Exercício 3 - Classificação de Números

Receba um número e informe se ele é positivo, negativo ou zero.

<details>
  <summary>Ver Resposta</summary>

```js
const numero = 0;

if (numero > 0) {
  console.log('Positivo');
} else if (numero < 0) {
  console.log('Negativo');
} else {
  console.log('Zero');
}
```

```bash
Zero
```

:bulb: `if`, `else if` e `else` cobrem todas as possibilidades.

</details>

---

## :pencil2: Exercício 4 - Faixa Etária

Receba a idade e informe e a pessoa é Criança (0-12), Adolescente (13-17), Adulto(18-59) ou Idoso(60+)

<details>
  <summary>Ver Resposta</summary>

```js
const idade = 14;

if (idade >= 0 && idade <= 12) {
  console.log('Criança');
} else if (idade >= 13 && idade <= 17) {
  console.log('Adolescente');
} else if (idade >= 18 && idade <= 59) {
  console.log('Adulto');
} else if (idade >= 60) {
  console.log('Idoso');
} else {
  console.log('Idade inválida');
}
```

```bash
Adolescente
```

:bulb: Sequência de testes encadeados para categorizar a idade.

</details>

---

## :muscle: Exercício 5 - DIas da Semana (switch)

Receba um número (1 a 7) e mostre o nome do dia da semana correspondente. Se inválido, mostre mensagem de erro

<details>
  <summary>Ver Resposta</summary>

```js
const dia = 5;

switch (dia) {
  case 1:
    console.log('Domingo');
    break;
  case 2:
    console.log('Segunda-feira');
    break;
  case 3:
    console.log('Terça-feira');
    break;
  case 4:
    console.log('Quarta-feira');
    break;
  case 5:
    console.log('Quinta-feira');
    break;
  case 6:
    console.log('Sexta-feira');
    break;
  case 7:
    console.log('Sábado');
    break;
  default:
    console.log('Dia inválido');
}
```

```bash
quinta-feira
```

:bulb: `switch` avalia o valor e executa o caso correspondente.

</details>

---

## :muscle: Exercício 6 - Validação de Senha

Receba uma senha (string) e informe se ela é válida (mínimo 6 caracteres)

:dart: Para contar quantos caracteres tem uma senha (string - nesse caso), você pode usar a propriedade .length do JavScript.

```js
const senha = 'abc123';
console.log(senha.length); // mostra 6
```

<details>
  <summary>Ver Resposta</summary>

```js
const senha = '12345';

if (senha.length >= 6) {
  console.log('Senha válida');
} else {
  console.log('Senha inválida');
}
```

```bash
Senha inválida
```

:bulb: Propriedade `.length` indica o tamanho da string (quantos caracteres tem na string)

</details>

---

## :exploding_head: Exercício 7 - Calculadora Simples

Receba dois números e uma operação (`+`, `-`, `*`, `/`). Use `switch` para calcular e mostrar o resultado.

<details>
  <summary>Ver Resposta</summary>

```js
const num1 = 12;
const num2 = 2;
const operacao = '/';

let resultado;

switch (operacao) {
  case '+':
    resultado = num1 + num2;
    break;
  case '-':
    resultado = num1 - num2;
    break;
  case '*':
    resultado = num1 * num2;
    break;
  case '/':
    if (num2 !== 0) {
      resultado = num1 / num2;
    } else {
      resultado = 'Erro: divisão por zero';
    }
    break;
  default:
    resultado = 'Operação inválida';
}

console.log(resultado);
```

```bash
6
```

:bulb: `12 / 2 = 6`

</details>

---

## :exploding_head: Exercício 8 - Verificação de Nota para Aprovação

Receba uma nota (0 a 10) e informe:

- "Aprovado" para nota >= 7
- "Recuperação" para nota entre 5 e 6.9
- "Reprovado" para nota < 5

<details>
  <summary>Ver Resposta</summary>

```js
const nota = 6.9;

if (nota >= 7) {
  console.log('Aprovado');
} else if (nota >= 5) {
  console.log('Recuperação');
} else {
  console.log('Reprovado');
}
```

```bash
Recuperação
```

:bulb: Condições sequenciais para definir situação do aluno

</details>

---
