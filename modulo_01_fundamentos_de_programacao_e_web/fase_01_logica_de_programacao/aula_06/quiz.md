# :brain: Quiz - aula 06

<!-- markdownlint-disable -->

---

1. Qual loop é mais indicado quando sabemos exatamente quantas vezes queremos repetir uma ação?

- [ ] `while`
- [ ] `do...while`
- [ ] `for`
- [ ] `foreach`

<details>
  <summary>Ver Resposta</summary>

:white_mark_check: `for`

:bulb: O loop `for` é ideal quando sabemos antecipadamente o número exato de repetições, pois a inicialização, condição e atualização ficam explícitas na declaração.

</details>

---

2. O que acontece se a condição de um loop `while` nunca se tornar falsa?

- [ ] O programa ignora o loop
- [ ] O programa executa o loop uma única vez
- [ ] O programa mostra um erro de sintaxe
- [ ] O programa entra em loop infinito

<details>
  <summary>Ver Resposta</summary>

:white_mark_check: `O programa entra um loop infinito

:bulb: Se a condição nunca se torna falsa e não há interrupção interna, o while executa indefinidamente, travando o programa.

</details>

---

3. Qual a principal diferença entre `while` e `do...while`?

- [ ] `do...while` nunca executa
- [ ] `do...while` executa pelo menos uma vez
- [ ] `while` executa pelo menos uma vez
- [ ] ´while`executa sempre mais vezes que`do...while`

<details>
  <summary>Ver Resposta</summary>

:white_mark_check: `do...while` executa pelo menos uma vez

:bulb: O do...while executa o bloco primeiro, antes de testar a condição, garantindo pelo menos uma execução.

</details>

---

4. Qual a palavra-chave usamos para **encerrar** a execução de um loop antes do término natural?

- [ ] `stop`
- [ ] `exit`
- [ ] `break`
- [ ] `end`

<details>
  <summary>Ver Resposta</summary>

:white_mark_check: `break`

:bulb: A instrução break interrompe imediatamente a execução do loop, independentemente da condição.

</details>

---

5. O que a palavra-chave `continue` faz em um loop?

- [ ] Ignora o restante do código na iteração atual e passa para a próxima
- [ ] Sai do loop completamente
- [ ] Reinicia o loop do começo
- [ ] Pausa o loop temporariamente

<details>
  <summary>Ver Resposta</summary>

:white_mark_check: Ignora o restante do código na iteração atual e passa para a próxima

:bulb: `continue` interrompe a iteração corrente e força o loop a continuar com a próxima repetição.

</details>

---

6. No `for (let i = 0; i < 5; i++)`, qual parte é responsável por determinar quando o loop termina?

- [ ] Inicialização (`let i = 0`)
- [ ] Condição (`i < 5`)
- [ ] Atualização (`i++`)
- [ ] Corpo do loop

<details>
  <summary>Ver Resposta</summary>

:white_mark_check: Condição (`i < 5`)

:bulb: O loop só continua enquanto a condição for verdadeira; quando falsa, o loop termina.

</details>

---

7. É obrigatório inicializar a variável de controle antes de um `while`?

- [ ] Sim
- [ ] Não
- [ ] Depende do código
- [ ] Somente em loops `for`

<details>
  <summary>Ver Resposta</summary>

:white_mark_check: Sim

:bulb: A variável deve ser inicializada para evitar loops infinitos e garantir que a condição seja avaliada corretamente.

</details>

---

8. o que pode acontecer se esquecermos de atualizar a variável de controle dentro de um `while`?

- [ ] O loop é executado uma vez
- [ ] O loop termina imediatamente
- [ ] O loop se torna infinito
- [ ] O código gera erro de compilação

<details>
  <summary>Ver Resposta</summary>

:white_mark_check: O loop se torna infinito

:bulb: Sem atualizar a variável que altera a condição, o while nunca terá sua condição falsa, causando loop infinito.

</details>

---
