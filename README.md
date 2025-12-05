Task Manager - Documentação Completa

🎯 Visão Geral

O Task Manager é uma aplicação web full-stack para gerenciamento de tarefas com autenticação segura, notificações em tempo real e interface intuitiva. Desenvolvido com tecnologias modernas e boas práticas de desenvolvimento.





🏗️ Arquitetura do Projeto

Frontend

• React 19 com TypeScript

• Vite como bundler

• Tailwind CSS 4 para estilização

• tRPC para comunicação type-safe com backend

• Zod para validação de dados

• Lucide React para ícones



Backend

• Node.js + Express 4 com TypeScript

• tRPC 11 para RPC type-safe

• Drizzle ORM para gerenciamento de banco de dados

• MySQL/TiDB como banco de dados

• JWT para autenticação

• bcryptjs para hash de senhas

• Vitest para testes unitários



Banco de Dados

• MySQL/TiDB hospedado na nuvem

• Drizzle ORM com migrations automáticas

• Schema com tabelas `users` e `tasks`





📦 Funcionalidades Principais

1. Autenticação e Segurança

• Registro de usuários com email e senha

• Login com geração de JWT

• Hash de senhas com bcryptjs

• Proteção de rotas com middleware de autenticação

• Isolamento de dados por usuário



2. CRUD Completo de Tarefas

• ✅ Criar tarefas com título (obrigatório) e descrição (opcional)

• ✅ Listar tarefas do usuário autenticado

• ✅ Editar título, descrição, status e data/hora de vencimento

• ✅ Deletar tarefas próprias

• ✅ Marcar tarefas como concluídas



3. Sistema de Favoritos

• ⭐ Marcar tarefas como favoritas com estrela

• 📊 Contagem de tarefas favoritas no resumo

• 🎨 Estrela preenchida em amarelo quando favorita



4. Notificações em Tempo Real

• 🚨 Alerta quando faltam 5 minutos para tarefa vencer

• 🚨 Alerta quando tarefa está vencendo (hora chega)

• 📦 Caixa de resumo com contagem de tarefas

• Notificações persistentes com toast



5. Filtros e Busca

• 🔍 Busca por título de tarefa

• 📌 Filtro por status (Todas/Pendentes/Concluídas)

• 📅 Campo de data de vencimento

• ⏰ Campo de hora de vencimento (HH:mm)



6. Interface Responsiva

• 🌓 Modo claro e escuro

• 📱 Design responsivo

• ♿ Acessibilidade

• 🎨 Gradientes e animações suaves





🔐 Validação de Dados

Frontend (Zod)

• Validação de formulários antes do envio

• Feedback visual de erros

• Schemas para registro, login e criação/edição de tarefas



Backend (Zod)

• Validação de todas as rotas da API

• Proteção contra dados inválidos

• Mensagens de erro estruturadas





🛠️ Rotas da API

Autenticação

Tarefas



📊 Schema do Banco de Dados

Tabela: users

Tabela: tasks



🎨 Design e UX

Paleta de Cores

• Modo Escuro: Azul escuro (#0f172a) com acentos azuis (#3b82f6)

• Modo Claro: Branco (#ffffff) com gradientes azuis suaves

• Destaques: Amarelo (#facc15) para favoritos, Verde (#22c55e) para concluídas, Vermelho (#ef4444) para logout



Componentes

• Cards com gradientes

• Botões com hover effects

• Inputs com validação visual

• Modais para edição

• Toast notifications

• Skeleton loaders



Responsividade

• Mobile-first design

• Breakpoints Tailwind padrão

• Navegação adaptativa





🚀 Como Executar

Pré-requisitos

• Node.js 18+

• pnpm (gerenciador de pacotes)

• Banco de dados MySQL/TiDB



Instalação

Configuração

1. Criar arquivo `.env` com variáveis de ambiente

2. Configurar `DATABASE_URL` para conexão com banco

3. Gerar chaves JWT e OAuth



Desenvolvimento

Acessa em: https://taskmanager.manus.space



Build

Testes

Migração do Banco



📁 Estrutura de Pastas



🧪 Testes

O projeto inclui 10 testes vitest cobrindo:



• ✅ Registro de usuários

• ✅ Login com JWT

• ✅ Criação de tarefas

• ✅ Edição de tarefas

• ✅ Deleção de tarefas

• ✅ Toggle de conclusão

• ✅ Toggle de favorito

• ✅ Logout



Executar testes:





🔄 Fluxo de Autenticação

1. Usuário acessa página inicial

2. Clica em “Criar Conta” → Página de registro

3. Preenche email e senha → Validação Zod

4. Backend cria usuário com senha hash

5. Usuário faz login → Recebe JWT

6. JWT armazenado em cookie seguro

7. Cada requisição inclui JWT no header

8. Backend valida JWT e retorna dados do usuário





🌐 Deploy

Frontend

• Vercel, Netlify ou Manus Platform

• Build automático via CI/CD

• CDN global para assets



Backend

• Render, Heroku ou Manus Platform

• Containers gerenciados

• Auto-scaling



Banco de Dados

• Supabase, Neon ou Manus Platform

• Backups automáticos

• SSL/TLS habilitado





📝 Variáveis de Ambiente



🎓 Tecnologias Aprendidas

Este projeto demonstra:



• ✅ Full-stack development com TypeScript

• ✅ Autenticação segura com JWT

• ✅ ORM com Drizzle

• ✅ Type-safe RPC com tRPC

• ✅ Validação com Zod

• ✅ UI moderna com Tailwind CSS

• ✅ Testes unitários com Vitest

• ✅ Notificações em tempo real

• ✅ Dark mode/Light mode

• ✅ Boas práticas de segurança





👥 Desenvolvido por

Lyncom - Gustavo, João Vitor, João Lucas





📄 Licença

MIT - Livre para uso pessoal e comercial





🤝 Suporte

Para dúvidas ou sugestões sobre o projeto, entre em contato com o time de desenvolvimento.
