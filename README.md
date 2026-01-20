# MEU PROJETO NEXT

> Projeto de uma LP em Next.js para estudo.

---

## 📌 Sobre o Projeto
Esse projeto foi criado para um estudo de como utilizar o Next.js em um projeto real, com a finalidade de acrescentar em um portifólio.

* **Objetivo:** Criar uma LP com o Next.js
* **Status:** Em desenvolvimento

## 🛠️ Tecnologias e Ferramentas
* **Linguagem Principal:** TypeScript
* **Frameworks/Bibliotecas:** Next.js e Tailwind CSS
* **Outras Ferramentas:** VS Code
---

## 📖 Guia de Git (Referência Rápida)

Este repositório também serve como material de estudo para os comandos fundamentais do Git.

### 🏗️ Conceitos Básicos
* **Commit:** "Fotografia" do código em um momento específico.
* **Branch:** Ramificação para desenvolver funções sem afetar o código principal.
* **Staging Area:** Área de preparação antes do commit (`git add`).
* **Repositório Remoto:** Versão do código hospedada online (GitHub).

### 🚀 Comandos Principais
| Ação | Comando |
| :--- | :--- |
| **Inicializar/Clonar** | `git init` ou `git clone <url>` |
| **Ver Status** | `git status` |
| **Histórico** | `git log --oneline` |
| **Preparar Arquivos** | `git add .` |
| **Salvar Alterações** | `git commit -m "mensagem"` |
| **Sincronizar** | `git pull` (receber) / `git push` (enviar) |
| **Branches** | `git checkout -b <nome>` (criar) / `git merge <nome>` (unir) |

### 🛠️ Desfazer Alterações
* `git restore <arquivo>`: Desfaz alterações não salvas.
* `git reset --soft HEAD~1`: Volta um commit, mantém o código.
* `git reset --hard HEAD~1`: **Cuidado!** Apaga o último commit e as alterações.

### 🔄 Fluxo de Trabalho Recomendado
1. `git pull` ➡️ 2. *Alterações no código* ➡️ 3. `git add .` ➡️ 4. `git commit` ➡️ 5. `git push`

---

## ⚙️ Como Executar o Projeto
```bash
# 1. Clone o repositório
git clone [URL-DO-REPOSITORIO]

# 2. Entre na pasta
cd [NOME-DA-PASTA]

# 3. [Comando para instalar dependências, ex: npm install]

# 4. [Comando para rodar o projeto, ex: python main.py]
```
-----------------------------------------------------------------------------------------
# Guia Prático de Next.js

Este guia reúne os principais conceitos, comandos e boas práticas do Next.js, servindo como referência rápida tanto para iniciantes quanto para desenvolvedores experientes.

---

## O que é Next.js
Next.js é um framework React que facilita a criação de aplicações web modernas, oferecendo renderização no servidor, rotas automáticas e otimizações de performance.

---

## Principais Conceitos

### Renderização
Next.js permite diferentes formas de renderização, como:
* **Server Side Rendering (SSR)**
* **Static Site Generation (SSG)**
* **Client Side Rendering (CSR)**

### App Router
Estrutura moderna baseada na pasta `app`, que organiza páginas, layouts e rotas de forma mais clara.

### Pages Router
Estrutura tradicional baseada na pasta `pages`, onde cada arquivo representa uma rota.

### Componentização
Divisão da interface em componentes reutilizáveis, facilitando manutenção e escalabilidade.

---

## Criação e Execução de Projetos

### Inicialização
```bash
npx create-next-app@latest nome-do-projeto]
```
Cria um novo projeto Next.js com as configurações iniciais.

## Comandos de Script
* **npm run dev**: Inicia o servidor de desenvolvimento. O projeto roda, por padrão, em **http://localhost:3000**.
* **npm run build**: Gera a versão otimizada do projeto para produção.
* **npm run start**: Executa o projeto em modo de produção após o build.

## Gerenciamento de Dependências
* **npm install**: Instala todas as dependências do projeto.
* **npm install nome-do-pacote**: Instala uma dependência específica.
* **npm uninstall nome-do-pacote**: Remove uma dependência do projeto.

## Estrutura Comum de Pastas
* **app**: Contém a estrutura principal de rotas, layouts e páginas usando o App Router.
* **pages**: Contém as rotas no modelo tradicional do Pages Router.
* **components**: Armazena componentes reutilizáveis da aplicação.
* **public**: Armazena arquivos estáticos como imagens e ícones.
* **services**: Contém arquivos responsáveis por comunicação com APIs.
* **hooks**: Armazena hooks personalizados.

## Solução de Problemas e Manutenção

### Limpeza de Cache
Em alguns casos, erros podem ser resolvidos limpando o cache do Next.js.

* **No Windows**: `rmdir /s /q .next`
* **No macOS ou Linux**: `rm -rf .next`

### Portas em Uso (Windows)
Se a porta 3000 já estiver ocupada:

1. **Identificar o processo**: `netstat -ano | findstr :3000`
2. **Finalizar o processo (substituindo o PID)**: `taskkill /PID 1234 /F`

## Fluxo Básico de Desenvolvimento
1. `npm install`
2. `npm run dev`

## Boas Práticas
* Manter componentes pequenos e reutilizáveis.
* Utilizar nomes claros para arquivos e pastas.
* Versionar o projeto com Git desde o início.
* Separar lógica de negócio da interface.
