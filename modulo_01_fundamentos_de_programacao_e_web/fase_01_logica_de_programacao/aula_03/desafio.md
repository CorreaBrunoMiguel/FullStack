# Desafio - Aula 03

## :brain: Tema: Conversão de Tipos e Coerção em JavaScript

## :dart: Aplicar os conhecimentos de conversão implícita e explícita em um cenário real

---

## :scroll: Cenário

Você foi contratado por uma empresa que está desenvolvendo um sistema de checkout simples para uma loja virtual. O problema é que o sistema está apresentando **comportamentos estranhos nos cálculos de valores**, pois os dados recebidos vêm em formato mistos (strings e números).

Sua tarefa é identificar e corrigir os erros de tipos, garantindo que o sistema faça os cálculos corretamente.

---

## :straight_ruler: Requisitos do sistema:

1. O sistema recebe:

   - `precoUnitario`: string que representa um número
   - `quantidade`: número
   - `cupomDesconto`: string que pode conter um número ou estar vazia (`""`)

2. Você deve:

   - Calcular o total sem desconto: `precoUnitario * quantidade` (`*` sinal de multiplicação)
   - Subtrair o valor do cupom, se houver (`cupomDesconto`)
   - Garantir que todas as operações sejam feitas corretamente com **números**

## :pushpin: Exemplo:

**Entrada:**

```js
const precoUnitario = '29.90';
const quantidade = 3;
const cupomDesconto = '10';

// TODO - Calcular o preço final
// Sua lógica aqui
```

**Saída:**

```bash
Preço: R$ 49.80
```

## :bulb: Dicas

- Use `Number()` para conversões
- Use apenas os conteúdos ensinados até agora: variáveis, tipos primitivos, conversão de tipos
- :dart: tente usar concatenação (soma de strings) para uma resposta mais detalhada `Preço R$49.80`, apenas o valor também é aceitável `49.80`
- :rocket: pesquise método `toFixed()`, veja se consegue usar

---
