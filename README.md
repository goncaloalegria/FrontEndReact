# ⚛️ FrontEndReact — App Web com React & Next.js

[![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://appnextalegria2.vercel.app)

**Aplicação web com múltiplas páginas em React e Next.js — desde componentes básicos até uma loja completa com carrinho, pesquisa e checkout**

[Descrição](#-descrição) •
[Funcionalidades](#-funcionalidades) •
[Páginas](#-páginas) •
[Tecnologias](#-tecnologias) •
[Demonstração](#-demonstração) •
[Instalação](#-instalação)

---

## 📋 Descrição

O **FrontEndReact** é uma aplicação web desenvolvida com **React** e **Next.js** (App Router) no âmbito da unidade curricular de Desenvolvimento de Interfaces Web. O projeto demonstra a evolução desde componentes JSX simples até funcionalidades avançadas como gestão de estado, rotas dinâmicas, integração com API REST e checkout com descontos.

A aplicação está deployada na **Vercel** e inclui 9 páginas que cobrem os conceitos fundamentais do desenvolvimento frontend moderno.

---

## ✨ Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| ⚛️ **Componentes React** | Componentes funcionais com JSX e props |
| 🔀 **Routing (App Router)** | Navegação entre páginas com Next.js App Router |
| 🔢 **Contador com Estado** | `useState` com incremento, decremento, reset e histórico |
| 📝 **Input Controlado** | Gestão de formulários com estado React |
| 🛒 **Loja DEISI** | Catálogo de produtos com carrinho de compras |
| 🔍 **Pesquisa e Ordenação** | Filtro em tempo real e ordenação por nome/preço |
| 🎓 **Descontos** | Desconto estudante DEISI e cupão de desconto |
| 💳 **Checkout** | Finalização de compra com validação |
| 📂 **Rotas Dinâmicas** | Páginas de categorias com routing dinâmico |
| 🚀 **Deploy Vercel** | Aplicação live com deploy automático |

---

## 📄 Páginas

| Página | Rota | Descrição |
|---|---|---|
| **Intro** | `/` | Homepage com apresentação e introdução ao JSX |
| **Sobre** | `/sobre` | Contexto sobre desenvolvimento web moderno |
| **Características** | `/caracteristicas` | Features do React e Next.js |
| **Tecnologias** | `/tecnologias` | Stack tecnológica utilizada |
| **Projetos** | `/projetos` | Projetos desenvolvidos |
| **Contador** | `/contador` | Contador interativo com histórico de valores |
| **Input** | `/input` | Formulário com inputs controlados |
| **Produtos** | `/produtos` | Loja DEISI com carrinho, pesquisa, ordenação e checkout |
| **Categorias** | `/categorias` | Listagem de categorias com rotas dinâmicas |

### Página de Produtos — Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| 🛍️ **Catálogo** | Produtos carregados da API DEISIShop |
| 🔍 **Pesquisa** | Filtro em tempo real por nome |
| ↕️ **Ordenação** | Nome (A→Z / Z→A) e preço (crescente / decrescente) |
| 🛒 **Carrinho** | Adicionar/remover produtos com subtotal automático |
| 🎓 **Estudante DEISI** | Toggle de desconto para estudantes |
| 🏷️ **Cupão** | Campo para código de desconto |
| 💳 **Checkout** | Validação de nome e finalização de compra |

---

## 🛠️ Tecnologias

| Tecnologia | Utilização |
|---|---|
| **Next.js** | Framework React com App Router e SSR |
| **React** | Biblioteca de componentes e gestão de estado |
| **TypeScript** | Tipagem estática para maior robustez |
| **Tailwind CSS** | Estilização utilitária e responsiva |
| **ESLint** | Linting e qualidade de código |
| **Vercel** | Deploy e hosting |
| **DEISIShop API** | API REST para produtos e checkout |

---

## 📁 Estrutura do Projeto

```
FrontEndReact/
├── app/                    # Páginas (Next.js App Router)
│   ├── page.tsx            # Homepage (Intro)
│   ├── sobre/
│   ├── caracteristicas/
│   ├── tecnologias/
│   ├── projetos/
│   ├── contador/
│   ├── input/
│   ├── produtos/
│   └── categorias/
│       └── [slug]/         # Rota dinâmica
│
├── components/             # Componentes React reutilizáveis
├── lib/                    # Utilitários e configurações
├── models/                 # Modelos de dados / tipos TypeScript
├── public/                 # Assets estáticos
│
├── package.json
├── tsconfig.json
├── next.config.ts
├── postcss.config.mjs
├── eslint.config.mjs
└── globals.d.ts
```

---

## 🚀 Demonstração

A aplicação está live na Vercel:

### **🔗 [Ver aplicação](https://appnextalegria2.vercel.app)**

---

## 💻 Instalação

### Pré-requisitos

| Requisito | Descrição |
|---|---|
| **Node.js 18+** | Runtime JavaScript |
| **npm / yarn / pnpm** | Gestor de pacotes |

### 1. Clonar o Repositório

```bash
git clone https://github.com/goncaloalegria/FrontEndReact.git
cd FrontEndReact
```

### 2. Instalar Dependências

```bash
npm install
```

### 3. Executar em Desenvolvimento

```bash
npm run dev
```

Abrir [http://localhost:3000](http://localhost:3000) no browser.

### 4. Build de Produção

```bash
npm run build
npm start
```

---

## 🔧 Resolução de Problemas

| Problema | Solução |
|---|---|
| `npm install` falha | Verificar versão do Node.js (18+): `node -v` |
| Produtos não carregam | Verificar ligação à internet (API em `deisishop.pythonanywhere.com`) |
| Porta 3000 ocupada | Usar `npm run dev -- -p 3001` para outra porta |
| Erros de TypeScript | Correr `npx tsc --noEmit` para ver erros detalhados |

---
## 👤 Autor

Gonçalo Alegria —  @goncaloalegria

---

## 🙏 Agradecimentos

- [Universidade Lusófona](https://www.ulusofona.pt/) — Instituição de ensino
- [Next.js](https://nextjs.org/) — Framework React
- [Vercel](https://vercel.com/) — Plataforma de deploy
- [DEISI Shop API](https://deisishop.pythonanywhere.com/) — API de produtos
