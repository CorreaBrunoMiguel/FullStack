# 📘 Executando Scripts JavaScript com Node.js

Antes de escrever grandes aplicações, é essencial saber como **executar um script JavaScript** fora do navegador — diretamente no seu computador. Isso é feito usando o **Node.js**, uma poderosa ferramenta que permite rodar JavaScript no terminal.

Este guia mostra como executar seus scripts `.js` de três formas:

1. Via **terminal (prompt de comando / shell)**
2. Via **Visual Studio Code (VS Code)**
3. Usando o próprio **terminal embutido do VS Code**

---

## ✅ Pré-requisitos

- [ ] Node.js instalado: [https://nodejs.org/](https://nodejs.org/)
- [ ] Editor de código recomendado: [Visual Studio Code](https://code.visualstudio.com/)
- [ ] Um arquivo `.js` criado no seu computador

Para verificar se o Node.js está instalado, abra seu terminal e digite:

```bash
node -v
```

Se retornar algo como `v18.17.1`, está tudo certo!

---

## 📝 1. Criando seu primeiro script

Crie um novo arquivo chamado `script.js` com o seguinte conteúdo:

```javascript
console.log('Olá, mundo! Este é meu primeiro script em Node.js!');
```

Salve o arquivo na pasta desejada.

---

## 💻 2. Executando via terminal (fora do VS Code)

1. Abra o terminal (Prompt de Comando no Windows, Terminal no Linux/Mac).
2. Navegue até a pasta onde está o arquivo usando o comando `cd`:

   ```bash
   cd caminho/da/pasta
   ```

   Exemplo no Windows:

   ```bash
   cd C:\Users\seu_usuario\Documentos\projetos
   ```

   Exemplo no Linux/macOS:

   ```bash
   cd ~/Documentos/projetos
   ```

3. Execute o script com:

   ```bash
   node script.js
   ```

Você verá no terminal:

```txt
Olá, mundo! Este é meu primeiro script em Node.js!
```

---

## 🧠 Dica rápida: caminho da pasta

Se estiver com o explorador de arquivos aberto, você pode:

- **Windows:** digitar `cmd` na barra de endereço da pasta → abre o terminal direto ali.
- **Linux/macOS:** clique com o botão direito e escolha "Abrir no terminal".

---

## 🧑‍💻 3. Executando dentro do VS Code

1. Abra o **VS Code**.
2. Vá em **File > Open Folder** e selecione a pasta do seu projeto.
3. Abra o arquivo `script.js`.
4. Clique com o botão direito dentro do código e escolha **“Run Code”** _(requer a extensão "Code Runner")_.

### ⚠️ Alternativa (sem extensão)

Use o terminal embutido do VS Code:

- Vá em **Terminal > New Terminal** ou use o atalho:

  - **Windows/Linux:** `Ctrl + \``
  - **Mac:** `Cmd + \``

- O terminal será aberto na parte inferior. Rode o script com:

```bash
node script.js
```

---

## 🧩 Resumo dos Comandos

| Ação                           | Comando                        |
| ------------------------------ | ------------------------------ |
| Verificar versão do Node.js    | `node -v`                      |
| Executar um arquivo `.js`      | `node nome-do-arquivo.js`      |
| Navegar até a pasta do script  | `cd caminho/da/pasta`          |
| Abrir terminal embutido VSCode | `Ctrl + \`` ou Menu > Terminal |

---

## 🛠️ Solução de Problemas

- **Erro: “node não é reconhecido”**  
  Isso significa que o Node.js não foi instalado corretamente ou o terminal não foi reiniciado. Tente reiniciar o computador ou reinstalar o Node.

- **Erro de caminho:**  
  Verifique se você está **na pasta correta** onde o script foi salvo.

---

## 🚀 Pronto para o próximo passo?

Agora que você sabe como rodar seus scripts, podemos avançar com os conceitos da linguagem e a criação de aplicações reais.
