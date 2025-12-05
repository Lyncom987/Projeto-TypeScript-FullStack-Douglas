# Project TODO

## Autenticação
- [x] Schema de usuário com campos para autenticação local (email, senha hash)
- [x] Registro de usuários com validação Zod
- [x] Login com geração de JWT
- [x] Middleware de proteção de rotas

## CRUD de Tarefas
- [x] Schema de tarefas com relação ao usuário
- [x] Criar tarefa (título obrigatório, descrição opcional)
- [x] Listar tarefas do usuário autenticado
- [x] Editar tarefa (título, descrição, status)
- [x] Deletar tarefa própria

## Validação com Zod
- [x] Schema de validação para registro
- [x] Schema de validação para login
- [x] Schema de validação para criação de tarefa
- [x] Schema de validação para edição de tarefa
- [x] Validação de formulários no frontend

## Interface de Usuário
- [x] Página de registro com formulário validado
- [x] Página de login
- [x] Dashboard com lista de tarefas
- [x] Funcionalidade de marcar como concluída
- [x] Modal/formulário para adicionar tarefa
- [x] Botões de editar e excluir tarefas

## Funcionalidades Extras
- [x] Filtro de tarefas por status (Todas/Pendentes/Concluídas)
- [x] Busca de tarefas por título
- [x] Campo de data de vencimento nas tarefas

## Segurança
- [x] Senhas armazenadas com hash bcrypt
- [x] Validação de propriedade nas operações
- [x] Isolamento de dados por usuário
