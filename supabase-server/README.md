# Supabase MCP Server

Este servidor MCP permite interagir com projetos Supabase, oferecendo:

- Conexão com projetos Supabase usando URL e chave de API
- Listagem de tabelas como recursos
- Execução de consultas SQL
- Operações CRUD em tabelas

## Configuração

O servidor requer as seguintes variáveis de ambiente:

- `SUPABASE_URL`: URL do projeto Supabase
- `SUPABASE_KEY`: Chave de API do projeto Supabase

## Ferramentas Disponíveis

- `check_token`: Verifica a validade do token e as permissões disponíveis
- `execute_query`: Executa uma consulta SQL personalizada
- `insert_data`: Insere dados em uma tabela
- `update_data`: Atualiza dados em uma tabela
- `delete_data`: Exclui dados de uma tabela
- `get_table_data`: Obtém dados de uma tabela específica

## Recursos Disponíveis

O servidor expõe as tabelas do Supabase como recursos, acessíveis através de URIs no formato `supabase://table/{nome-da-tabela}`.

## Instalação

```bash
npm install
npm run build
```

## Execução

```bash
SUPABASE_URL=https://seu-projeto.supabase.co SUPABASE_KEY=sua-chave-api node build/index.js
```