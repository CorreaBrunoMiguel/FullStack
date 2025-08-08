📘 Executando Scripts JavaScript com Node.js

---

Sumário

1. Pré-requisitos
2. Criando seu primeiro script
3. Executando via Terminal (fora do VS Code)
4. Executando dentro do VS Code
5. Resumo dos Comandos
6. Solução de Problemas

---

✅ Pré-requisitos

- Node.js instalado (versão recomendada LTS)  
  https://nodejs.org/
- Visual Studio Code instalado (recomendado)  
  https://code.visualstudio.com/
- Um arquivo `.js` criado no seu computador

Para verificar se o Node.js está instalado, abra seu terminal e digite:

node -v

Se retornar algo como `v18.17.1`, está tudo certo!

---

📝 Criando seu primeiro script

Crie um arquivo chamado `script.js` com o seguinte conteúdo:

console.log('Olá, mundo! Este é meu primeiro script em Node.js!');

Salve o arquivo na pasta desejada.

---

💻 Executando via Terminal (fora do VS Code)

1. Abra o Terminal (Prompt de Comando no Windows, Terminal no Linux/macOS).
2. Navegue até a pasta do arquivo com o comando cd:

cd caminho/da/pasta

3. Execute o script com:

node script.js

Você verá no terminal:

Olá, mundo! Este é meu primeiro script em Node.js!

---

🧑‍💻 Executando dentro do VS Code

1. Abra o VS Code.
2. Abra a pasta do seu projeto pelo menu: File > Open Folder.
3. Abra o arquivo `script.js`.
4. Recomendação: instale a extensão Code Runner para executar código com um clique.
5. Clique com o botão direito no editor de código e escolha Run Code.

⚠️ Alternativa sem extensão

- Abra o terminal embutido pelo menu: Terminal > New Terminal ou atalho:

  - Windows/Linux: Ctrl + ` (tecla acima do Tab)
  - macOS: Cmd + `

- Execute o script com:

node script.js

---

🧩 Resumo dos Comandos

| Ação                            | Comando                     |
| ------------------------------- | --------------------------- |
| Verificar versão do Node.js     | node -v                     |
| Executar um arquivo `.js`       | node nome-do-arquivo.js     |
| Navegar até a pasta do script   | cd caminho/da/pasta         |
| Abrir terminal embutido VS Code | Ctrl + ` ou Menu > Terminal |

---

🛠️ Solução de Problemas

- Erro: “node não é reconhecido”  
  Reinicie o terminal ou o computador, ou reinstale o Node.js corretamente.

- Erro de caminho:  
  Verifique se está na pasta correta onde o script está salvo.

---

🚀 Pronto para o próximo passo?

Agora que você sabe como rodar seus scripts, podemos avançar para os conceitos da linguagem e criação de aplicações reais.

---
