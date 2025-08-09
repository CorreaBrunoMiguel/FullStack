# :book: Aula 06 - Laços de repetição (`for`, `while`, `do...while`)

---

## 1. Por que repetição é fundamental

Laços de repetição permitem que um bloco de código seja executado várias vezes automaticamente, sem duplicação manual.

Eles expressam iteração - essencial para percorrer sequências, repetir verificações, implementar contadores, processar dados em lote e modelar processos que evoluem no tempo.

Benefícios práticos:

- Redução de duplicação (DRY)
- Manutenção facilitada
- Expressão natural de algoritmos (contagem, busca, acumulação, filtragem)

---

## 2. Modelo de execução (mental mode)

Antes de aprender sintaxe, é útil um modelo mental comum:

1. **Inicialização** (quando aplicável): prepara variáveis de controle.
2. **Teste de condição**: decide se executa o corpo do loop.
3. **Execução do corpo**: instruções dentro do loop.
4. **Atualização** (quando aplicável): muda a variável de controle.
5. volta ao **teste de condição**.

:warning: a ordem exata (quando cada parte é executada) difere entre `for`, `while` e `do...while`.

---

## 3. `for` - quando e como usar

### 3.1 Sintaxe

```js
for (inicialização; condição; atualização) {
  // corpo
}
```

Exemplo simples:

```js
for (let i = 1; i <= 5; i++) {
  console.log(`Contagem: ${i}`);
}
```

### 3.2 Ordem de execução no `for`

1. Executa **inicialização** uma vez
2. Avalia **condição**. Se falsa, sai imediatamente
3. Executa **corpo**
4. Executa **atualização**
5. Repete do passo 2

### 3.3 Florestas de variações úteis

- Vários controladores:

```js
for (let i = 0, j = 10; i < j; i++, j--) {
  // corpo do loop
}
```

- Pulando passos:

```js
for (let i = 0; i < 10; i += 2) {
  // corpo do loop
}
```

- Contagem decrescente:

```js
for (let i = 10; i > 0; i--) {
  // corpo do loop
}
```

### 3.4 Erros comuns com `for`

- Off-by-one: usar `i <= n` vc `i < n` indevidamente
- Modificar a variável de controle dentro do corpo sem cuidado (pode causar saltos inesperados)
- Declarar com `var` (hoisting/escopo) - prefira `let` para escopo de bloco

### 3.5 Exemplo

`for` básico - contagem

```js
for (let i = 0; i < 5; i++) {
  console.log(i); // 0, 1, 2, 3, 4, 5
}
```

---

## 4. `while` - laço por condição

### 4.1 Sintaxe

```js
while (condição) {
  // corpo
}
```

### 4.2 Comportamento

- Avalia a **condição** antes de cada execução do corpo.
- Se condição for verdadeira, executa o corpo; quando for falsa, sai.
- Útil quando não sabemos a quantidade de iterações à priori (repetir até que uma condição externa mude).

Exemplo:

```js
let n = 0;
while (n < 3) {
  console.log(n);
  n++; // atualização manual — essencial
}
```

### 4.3 Perigo: loop infinito

Se a condição nunca ficar falsa, o programa fica preso. Sempre garanta:

- Uma variável de controle que progrida em direção a falso, ou
- Um `break` atingível para sair.

Padrão seguro (controle explícito)

```js
let attempts = 0;
while (attempts < 10) {
  // lógica
  attempts++;
}
```

---

## 5. `do...while` - executar pelo menos uma vez

### 5.1 Sintaxe

```js
do {
  // corpo
} while (condição);
```

### 5.2 Quando usar

Quando você precisa executar o corpo ao menos **uma vez** antes de verificar a condição - por exemplo, quando solicita uma entrada inicial do usuário e só depois decide continuar.

Exemplo:

```js
let resposta = '';
do {
  resposta = obterResposta(); // função hipotética
} while (resposta !== 'sair');
```

Mesmo se a condição for falsa já na primeira verificação, o corpo executará uma vez.

---

## 6. `break` e `continue` - controle fino do fluxo

## 6.1 `break`

Interrompe imediatamente o loop atual e transfere execução para a instrução após o loop.

```js
for (let i = 1; i <= 10; i++) {
  if (i === 5) break; // sai do loop quando i == 5
  console.log(i);
}
```

:dart: `break` afeta apenas o loop mais interno; para sair de loops aninhados, há alternativas (ex.: variáveis sinalizadoras - use labels com parcimônia).

### 6.2 `continue`

Interrompe a iteração atual e salta para próxima verificação (no `for` isso passa pela atualização)

```js
for (let i = 1; i <= 5; i++) {
  if (i === 3) continue; // pula o 3
  console.log(i);
}
```

## 7. Boas práticas de estilo e manutenção

- **Prefira** `let`/`const` em vez de `var`
- **Nomeie bem a variável de controle**: `i`, `j` são aceitáveis em loops simples; em loops com significado semântico, use `index`, `count`, `attempts`.
- **Evite lógica complexa dentro de condições** - extraia para uma função nomeada quando necessário (melhora legibilidade e testes)
- **Mantenha a atualização do controlador perto do início do loop ou claramente visível** para evitar esquecimento.
- **Comente o propósito do loop** quando não for óbvio - especialmente a condição de escape.

---

## 8. Complexidade e performance (noções básicas)

- Na maioria dos casos simples, loops são 0(n) - tempo linear proporcional ao número de iterações.
- Evite computações pesadas dentro do teste de condição se elas puderem ser pré-calculadas.
- Em ambientes com I/O (input/output) ou operações custosas, minimize trabalho dentro do corpo do loop (cache local de valores, usar variáveis temporárias).

---

## 9. Razões para escolher cada loop (resumo prático)

- Use `for` quando a contagem for conhecida ou quando você precisa de inicialização/atualização claras.
- Use `while` quando depender de uma condição externa que muda ao longo do tempo.
- Use `do...while` quando o corpo deve rodar pelo menos uma vez.

---

## 10. Erros e armadilhas frequentes (lista prática)

- Esquecer de atualizar a variável de controle em `while` - causa loop infinito.
- Usar `<=` quando deveria usar `<`
- Declarar o contador com `var` e depois acessar fora do laço sem querer.
- Alterar a variável de controle dentro do corpo sem clareza - gera bugs difíceis de rastrear
- Confiar em comportamento de ponto flutuante para contagens inteiras.

---

## 11. Depuração de loops

- Inserir `console.log` no início/fim do corpo para inspecionar valores.
- Verificar condições iniciais antes de executar
- Testar com pequenos valores antes de dados grandes
- Usar breakpoints no depurador (IDE/DevTools) para inspecionar estado por iteração
