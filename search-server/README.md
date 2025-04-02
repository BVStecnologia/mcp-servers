# Search MCP Server

Este servidor MCP fornece ferramentas para realizar pesquisas na web usando diferentes provedores:

- Google Custom Search Engine
- Bing Search
- SerpAPI

## Configuração

O servidor pode utilizar as seguintes variáveis de ambiente:

- `SERPAPI_API_KEY`: Chave de API do SerpAPI
- `BING_SEARCH_API_KEY`: Chave de API do Bing Search
- `GOOGLE_CSE_API_KEY`: Chave de API do Google Custom Search Engine
- `GOOGLE_CSE_ID`: ID do mecanismo de pesquisa personalizado do Google

## Ferramentas Disponíveis

- `web_search`: Realiza uma pesquisa na web usando o provedor padrão
- `provider_search`: Realiza uma pesquisa na web usando um provedor específico
- `multi_provider_search`: Realiza uma pesquisa na web usando todos os provedores configurados
- `list_providers`: Lista os provedores de pesquisa disponíveis

## Instalação

```bash
npm install
```

## Execução

```bash
SERPAPI_API_KEY=sua-chave-serpapi BING_SEARCH_API_KEY=sua-chave-bing GOOGLE_CSE_API_KEY=sua-chave-google GOOGLE_CSE_ID=seu-id-cse node src/index.js
```