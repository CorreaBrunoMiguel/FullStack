# Desafio - Aula 05

---

## Enunciado

Você foi contratado para desenvolver um sistema simples de atendimento para uma clínica médica. O sistema deve receber informações do paciente e decidir algumas ações com base nelas.

---

## Requisitos

1. Receber a idade do paciente e informar a faixa etária:

   - Criança (0 a 12 anos)
   - Adolescente (13 a 17 anos)
   - Adulto (18 a 59 anos)
   - Idoso (60 anos ou mais)

2. Receber o tipo de plano de saúde do paciente, que pode ser:

   - "Basic"
   - "Standard"
   - "Premium"

   Usar `switch` para exibir a mensagem correspondente:

   - Basic: "Cobertura básica"
   - Standard: "Cobertura intermediária"
   - Premium: "Cobertura completa"

3. Com base na faixa etária e no plano, exibir uma mensagem adicional:

   - Se for criança e plano Premium, exibir "Atendimento prioritário para crianças Premium"
   - Se for idos e plano Basic, exibir "Recomendamos upgrade para melhor cobertura"
   - Caso contrário, apenas exibir "Atendimento padrão"

---

**Exemplo de saída esperada:**

```bash
Faixa etária: Adulto
Plano: Standard
Atendimento padrão
```
