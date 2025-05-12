
# Guia Prático: Git e GitHub 🚀

Este guia tem como objetivo demonstrar o uso básico das ferramentas **Git** e **GitHub**, com exemplos práticos e comandos essenciais para o seu dia a dia como desenvolvedor.

---

## ✅ Instalação do Git

### Windows
1. Acesse o site oficial: [https://git-scm.com](https://git-scm.com)
2. Baixe o instalador e siga as instruções padrão.
3. Verifique a instalação:
```bash
git --version
```

### Linux (Debian/Ubuntu)
```bash
sudo apt update
sudo apt install git
```

### macOS
Via Homebrew:
```bash
brew install git
```

---

## ⚙️ Configuração Inicial

Configure seu nome de usuário e email:
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
```

Visualize suas configurações:
```bash
git config --list
```

---

## 🗃️ Criando um Repositório Local e Conectando ao GitHub

### Passo 1: Crie o repositório no GitHub

- Nome: `guia-git-github`
- Pode ser público ou privado
- Marque a opção para inicializar com um `README.md`

### Passo 2: Clone o repositório
```bash
git clone https://github.com/BrunoXHP/guia-git-github.git
cd guia-git-github
```

### Passo 3: Ou crie um repositório local e conecte ao GitHub
```bash
mkdir guia-git-github
cd guia-git-github
git init
git remote add origin https://github.com/BrunoXHP/guia-git-github.git
```

---

## 🧱 Operações Básicas com Git

### Adicionar arquivos ao stage
```bash
git add .
```

### Realizar um commit
```bash
git commit -m "Mensagem do commit"
```

### Enviar para o GitHub
```bash
git push origin main
```

### Atualizar o repositório local com o remoto
```bash
git pull origin main
```

---

## 🌿 Trabalhando com Branches

### Criar uma nova branch
```bash
git branch nome-da-branch
```

### Mudar para outra branch
```bash
git checkout nome-da-branch
```

### Criar e mudar de branch ao mesmo tempo
```bash
git checkout -b nome-da-branch
```

### Subir a branch para o GitHub
```bash
git push origin nome-da-branch
```

---

## 📥 Clonar um Repositório Existente

```bash
git clone https://github.com/usuario/repositorio.git
```

---

## 🔀 Criar um Pull Request

1. Faça alterações em uma branch diferente da `main`.
2. Envie a branch para o GitHub:
```bash
git push origin minha-branch
```
3. No GitHub, clique em "Compare & pull request".
4. Escreva uma descrição clara e envie o PR.

---

## 💡 Dicas e Boas Práticas

- Escreva mensagens de commit **curtas e descritivas**.
- **Commite frequentemente**, para manter o histórico claro.
- Use um arquivo `.gitignore` para ignorar arquivos desnecessários:
  - Exemplo:
    ```gitignore
    node_modules/
    .env
    ```
- Sempre **atualize seu repositório (git pull)** antes de começar novas mudanças.
- Use branches para **organizar tarefas** e facilitar revisões.

---

## 📎 Exemplos de Comandos

```bash
git init
git add .
git commit -m "Iniciando o guia de Git e GitHub"
git push origin main
git pull origin main
git branch nova-feature
git checkout nova-feature
git clone https://github.com/BrunoXHP/guia-git-github.git
```

---

## 📌 Licença

Este projeto está sob a licença MIT.
