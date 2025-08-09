# Exercícios - Aulas 06

<!-- markdownlint-disable -->

**Observação:** Existe mais de uma forma de resolver cada exercício,a resposta gerada é apenas uma de muitas possibilidades.

---

:seedling: 1. Imprima no console os números de 1 a 10 usando um laço `for`

<details>
  <summary>Ver Resposta</summary>

```js
for (let i = 1; i <= 10; i++) {
  console.log(i);
}
```

:dart: O `for` inicializa `i` em 1, executa enquanto `i <= 10` e incrementa `i` em 1 a cada passo.

</details>

---

:seedling: 2. Utilizando um laço `while`, imprimir os números pares de 2 a 20.

<details>
  <summary>Ver Resposta</summary>

```js
let num = 2;
while (num <= 20) {
  console.log(num);
  num += 2; // Incrementa de 2 em 2 para pegar apenas pares
}
```

:dart: Variável `num` é incrementada de 2 em 2 para garantir que só pares sejam exibidos.

</details>

---

:pencil2: 3. Usando `for`, calcule a soma dos números de 1 até 100.

<details>
  <summary>Ver Resposta</summary>

```js
let soma = 0;
for (let i = 1; i <= 100; i++) {
  soma += i;
}
console.log(soma); // Deve imprimir 5050
```

:dart: Soma acumulada dentro do loop, exemplo clássico para entender acumulação

</details>

---

:pencil2: 4. Simule uma repetição que solicita uma "senha" armazenada numa variável, e repita até que o valor seja "1234"

<details>
  <summary>Ver Resposta</summary>

```js
let senha = ''; // variável que simula entrada do usuário
let tentativa = 0;

do {
  // Simulação de entrada — altere o valor de "senha" manualmente para testar
  senha = '0000'; // simula entrada errada
  tentativa++;

  // para testar sucesso, mude senha para "1234" após algumas tentativas
  if (tentativa === 3) senha = '1234';
} while (senha !== '1234');

console.log('Senha correta! Acesso liberado.');
```

:dart: Aqui simulamos a entrada trocando o valor manualmente no código, e usamos `do...while` para garantir a execução pelo menos uma vez.

</details>

---

:muscle: 5. Utilize um laço `for` para imprimir os números de 10 até 1 em ordem decrescente.

<details>
  <summary>Ver Resposta</summary>

```js
for (let i = 10; i >= 1; i--) {
  console.log(i);
}
```

:dart: Laço decrescente com `i--` decrementando a variável a cada iteração.

</details>

---

:muscle: 6. Escreva um programa usando `while` que imprima a tabuada do 5.

<details>
  <summary>Ver Resposta</summary>

```js
let contador = 1;
while (contador <= 10) {
  console.log(`5 x ${contador} = ${5 * contador}`);
  contador++;
}
```

:dart: O loop repete enquanto o contador for menor ou igual a 10, imprimindo a tabuada.

</details>

---

:exploding_head: 7. Crie um laço `for` que percorra de 1 a 50 e imprima somente os números múltiplos de 3, usando `continue`

<details>
  <summary>Ver Resposta</summary>

```js
for (let i = 1; i <= 50; i++) {
  if (i % 3 !== 0) continue;
  console.log(i);
}
```

:dart: A condição `i % 3 !== 0` pula as iterações que não são múltiplos de 3 com `continue`

</details>

---
