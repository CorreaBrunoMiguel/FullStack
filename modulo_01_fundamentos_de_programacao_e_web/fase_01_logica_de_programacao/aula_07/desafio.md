# :construction: Desfio - Aula 07

<!-- markdownlint-disable -->

---

## Calculadora de Orçamento Pessoal

Crie um programa em JavaScript que ajude uma pessoa a calcular o saldo do seu orçamento mensal usando funções e escopo:

1. Criar variáveis **globais** para armazenar:

   - `saldo` (número inicial fornecido pelo usuário)
   - `nomeUsuario` (string com o nome do usuário)

2. Criar funções

   - `adicionarReceita(valor)` -> soma o valor ao saldo, validando que seja número positivo.
   - `registrarDespesa(valor, descricao)` -> subtrai o valor do saldo, validando que sejam números positivo e que não ultrapasse o saldo disponível.
   - `exibirSaldo()` -> mostra no console o saldo atual formatado.
   - `mostrarResumo()` -> exibe o nome do usuário e o saldo final.

3. O fluxo do programa deve:

- Definir o nome do usuário e o saldo inicial.
- Adicionar pelo menos 2 receita.
- Registrar pelo menos duas despesas.
- Exibir o saldo final e o resumo

---

<details>
  <summary>Implementação Sugerida</summary>

```js
// Variáveis globais
let saldo = 0;
let nomeUsuario = '';

// Função para definir nome e saldo inicial
function iniciarUsuario(nome, saldoInicial) {
  nomeUsuario = nome;
  saldo = saldoInicial;
  console.log(`Bem-vindo, ${nomeUsuario}! Seu saldo inicial é R$${saldo}.`);
}

// Função para adicionar receita
function adicionarReceita(valor) {
  if (typeof valor !== 'number' || valor <= 0) {
    console.log('Valor inválido para receita.');
    return;
  }
  saldo += valor;
  console.log(`Receita de R$${valor} adicionada. Saldo atual: R$${saldo}.`);
}

// Função para registrar despesa
function registrarDespesa(valor, descricao) {
  if (typeof valor !== 'number' || valor <= 0) {
    console.log('Valor inválido para despesa.');
    return;
  }
  if (valor > saldo) {
    console.log('Saldo insuficiente para essa despesa.');
    return;
  }
  saldo -= valor;
  console.log(`Despesa "${descricao}" de R$${valor} registrada. Saldo atual: R$${saldo}.`);
}

// Função para exibir saldo
function exibirSaldo() {
  console.log(`Saldo atual: R$${saldo}.`);
}

// Função para mostrar resumo
function mostrarResumo() {
  console.log(`Resumo: Usuário ${nomeUsuario}, saldo final de R$${saldo}.`);
}

// --- Fluxo de execução ---
iniciarUsuario('Bruno', 1000);
adicionarReceita(500);
adicionarReceita(300);
registrarDespesa(200, 'Mercado');
registrarDespesa(150, 'Transporte');
exibirSaldo();
mostrarResumo();
```

</details>
