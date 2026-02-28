Segue o **README.md completo** pronto para você copiar e colar no seu projeto:

---

````markdown
# Guia Completo — React + Vite + Git + GitHub

Este projeto documenta o passo a passo completo para:

- Criar um projeto ReactJS utilizando Vite
- Inicializar o Git
- Subir o projeto para o GitHub
- Criar uma nova branch
- Realizar uma alteração
- Fazer merge da branch na `main`

---

# Tecnologias Utilizadas

- React
- Vite
- Node.js
- Git
- GitHub

---

# Pré-requisitos

Antes de começar, é necessário ter instalado:

- Node.js (versão LTS recomendada)
- NPM
- Git
- Conta no GitHub

Verifique se está tudo instalado:

```bash
node -v
npm -v
git --version
````

---

# 1. Criando o Projeto React com Vite

No terminal, execute:

```bash
npm create vite@latest meu-projeto -- --template react
cd meu-projeto
npm install
npm run dev
```

O projeto estará disponível normalmente em:

```
http://localhost:5173
```

---

# 2. Inicializando o Git no Projeto

Dentro da pasta do projeto:

```bash
git init
git add .
git commit -m "chore: projeto React criado com Vite"
```

Garantir que a branch principal seja `main`:

```bash
git branch -M main
```

---

# 3. Criando e Conectando ao Repositório no GitHub

## 3.1 Criar repositório no GitHub

1. Acesse [https://github.com](https://github.com)
2. Clique em **New repository**
3. Nomeie como `meu-projeto`
4. NÃO selecione a opção de criar README automaticamente
5. Clique em **Create repository**

## 3.2 Conectar repositório local ao remoto

Copie a URL do repositório criado e execute:

```bash
git remote add origin https://github.com/SEU_USUARIO/meu-projeto.git
git push -u origin main
```

Agora o projeto já está no GitHub ??

---

# 4. Criando uma Nova Branch

Criar uma branch para nova funcionalidade:

```bash
git switch -c feature/ajuste-texto
```

ou:

```bash
git checkout -b feature/ajuste-texto
```

Verificar branch atual:

```bash
git branch
```

---

# 5. Realizando uma Pequena Alteração

Exemplo:

Editar o arquivo:

```
src/App.jsx
```

Alterar algum texto visível na tela, como:

```jsx
<h1>Vite + React (Alterado na Feature)</h1>
```

Testar alteração:

```bash
npm run dev
```

---

# 6. Commitando e Enviando a Nova Branch

```bash
git add .
git commit -m "feat: pequeno ajuste de texto no App"
git push -u origin feature/ajuste-texto
```

A branch agora está disponível no GitHub.

---

# 7. Realizando o Merge na Branch Main

## ? Método Recomendado: Pull Request (via GitHub)

1. Acesse o repositório no GitHub
2. Clique em **Compare & pull request**
3. Base branch: `main`
4. Compare branch: `feature/ajuste-texto`
5. Clique em **Create pull request**
6. Depois clique em **Merge pull request**
7. Confirme o merge

Atualizar a main local:

```bash
git switch main
git pull
```

---

## Método Alternativo: Merge via Terminal

```bash
git switch main
git pull origin main
git merge feature/ajuste-texto
git push origin main
```

---

# 8. Removendo a Branch Após o Merge

Remover branch local:

```bash
git branch -d feature/ajuste-texto
```

Remover branch remota:

```bash
git push origin --delete feature/ajuste-texto
```

---

# Fluxo Completo Resumido

```bash
# Criar projeto
npm create vite@latest meu-projeto -- --template react
cd meu-projeto
npm install

# Inicializar git
git init
git add .
git commit -m "init"
git branch -M main

# Conectar ao GitHub
git remote add origin https://github.com/SEU_USUARIO/meu-projeto.git
git push -u origin main

# Criar nova branch
git switch -c feature/ajuste-texto

# Fazer alteração
git add .
git commit -m "feat: ajuste"
git push -u origin feature/ajuste-texto

# Merge via PR (recomendado)
# ou merge via terminal
git switch main
git merge feature/ajuste-texto
git push origin main
```

---

# Estrutura do Projeto

```
meu-projeto/
?
??? public/
??? src/
?   ??? App.jsx
?   ??? main.jsx
?   ??? assets/
?
??? package.json
??? vite.config.js
??? README.md
```

---

# Objetivo

Este projeto demonstra um fluxo básico e profissional de desenvolvimento utilizando:

* Versionamento com Git
* Estratégia de Branch
* Pull Request
* Merge na branch principal (`main`)
* Organização de commits

---

# Licença

Projeto para fins educacionais.

```

---

Se quiser, posso gerar agora:

- ?? Versão com badges (React, Vite, GitHub)
- ?? Padrão profissional com Conventional Commits
- ?? README mais corporativo para portfólio
- ?? Versão pronta para deploy na Vercel

Só me dizer qual você prefere.
```
