# :book: Quiz - Aula 05

## <!-- markdownlint-disable -->

---

1.Qual será a saída do seguinte código?

```js
let x = 5;
if (x > 3) {
  x = 10;
}
```

- [ ] 5
- [ ] 3
- [ ] undefined
- [ ] 10

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: 10

:brain: A condição `x > 3` é verdadeira, portanto o bloco `if` é executado e `x` recebe `10`

</details>

---

2.O que o código abaixo imprime no console?

```js
let idade = 18;

if (idade < 18) {
  console.log('Menor de idade');
} else {
  console.log('Maior de idade');
}
```

- [ ] `Menor de idade`
- [ ] `Maior de idade`
- [ ] `undefined`
- [ ] `Nada é impresso`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Maior de idade`

:brain: A condição `idade < 18`é falsa, então o `else` é executado.

</details>

---

3.Qual dessas estruturas é mais adequada para avaliar múltiplos valores de uma mesma variável?

- [ ] `if` e `else if`
- [ ] `for`
- [ ] `switch`
- [ ] `while`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `switch`

:brain: O `switch` é ideal para avaliar **múltiplos casos** de uma mesma variável.

</details>

---

4.Qual será a saída do código abaixo?

```js
let cor = 'verde';

switch (cor) {
  case 'vermelho':
    console.log('Pare');
    break;
  case 'amarelo':
    console.log('Atenção');
    break;
  case 'verde':
    console.log('Siga');
    break;
  default:
    console.log('Cor inválida');
}
```

- [ ] `Pare`
- [ ] `Atenção`
- [ ] `Siga`
- [ ] `Cor inválida`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Siga`

:brain: A variável `cor` é `verde`, então o `case "verde"` é executado

</details>

---

5. Qual é a saída do código abaixo?

```js
let idade = 17;
if (idade >= 18) {
  console.log('Pode entrar');
} else {
  console.log('Entrada negada');
}
```

- [ ] Pode entrar
- [ ] Entrada permitida
- [ ] Não pode entrar
- [ ] Entrada negada

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Entrada Negada`

:brain: A condição `idade >= 18` é **falsa** (17 não é maior ou igual a 18), então o bloco do `else` é executado

</details>

---

6.O que o código a seguir imprimirá?

```js
let cor = 'azul';
switch (cor) {
  case 'vermelho':
    console.log('Cor quente');
    break;
  case 'azul':
    console.log('Cor fria');
    break;
  default:
    console.log('Cor não reconhecida');
}
```

- [ ] Cor quente
- [ ] Cor fria
- [ ] Cor não reconhecida
- [ ] Erro no código

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Cor fria`

:brain: O `switch` compara `cor` com cada `case`. Quado encontra `"azul"`, executa o bloco correspondente e para no `break`.

</details>

---

7.O que acontece se removermos todos os `break` de um `switch`?

- [ ] Nada muda, o código funciona igual
- [ ] O código executa apenas o primeiro caso encontrado e para automaticamente
- [ ] Todos os casos a partir do correspondente são executados até o final
- [ ] O `switch` não funciona sem o `break`

<details>
  <summary>Ver Resposta</summary>

:white_check_mark: `Todos os casos a partir do correspondente são executados até o final`

:brain: Sem `break`. o Javascript faz o chamado "fall through", executando todos os blocos seguintes.

</details>
