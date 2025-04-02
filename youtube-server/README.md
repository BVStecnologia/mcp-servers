# YouTube MCP Server

Este servidor MCP permite interagir com a API do YouTube, oferecendo:

- Pesquisa de vídeos
- Obtenção de detalhes de vídeos
- Obtenção de detalhes de canais
- Download de transcrições de vídeos
- Obtenção de comentários de vídeos

## Configuração

O servidor requer a seguinte variável de ambiente:

- `YOUTUBE_API_KEY`: Chave de API do YouTube

## Ferramentas Disponíveis

- `search_videos`: Pesquisar vídeos no YouTube
- `get_video_details`: Obter detalhes de um vídeo específico
- `get_channel_details`: Obter detalhes de um canal do YouTube
- `download_youtube_transcript`: Baixar a transcrição de um vídeo do YouTube
- `get_video_comments`: Obter comentários de um vídeo do YouTube

## Instalação

```bash
npm install
```

## Execução

```bash
YOUTUBE_API_KEY=sua-chave-api node src/index.js
```

## Requisitos Adicionais

Para a funcionalidade de download de transcrições, o servidor requer a instalação do `yt-dlp`:

- macOS: `brew install yt-dlp`
- Linux: `pip install yt-dlp`
- Windows: `pip install yt-dlp`