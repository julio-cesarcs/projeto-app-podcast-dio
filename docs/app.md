# Podcast Manager

### Descrição

Um app ao estilo Netflix, aonde possa centralizar diferentes epsódios de podcasts separados por categoria

### Dominio

Podcast feitos em vídeo

### Features

- Listas os epsódios em sessões de categorias
  - [basquete, futebol, quadrinhos, game, desenvolvimento]
- Filtrar epsódios por nome de podcast

## Como

### Features

Listas os epsódios em sessões de categorias

### Como vou implemantar

Vou retornar em uma api rest (json) o nome do podcast, o nome do epsódio, a imagem de capa, o link e a categoria.

GET: retorna lista de episódios

response:

```js
[
  {
    podcastName: "99Vidas",
    episode: "99Vidas 635 – Previsões para 2026",
    videoId: "Ue7yV9ZbN9U",
    cover: "https://i.ytimg.com/vi/Ue7yV9ZbN9U/hqdefault.jpg",
    link: "https://www.youtube.com/watch?v=Ue7yV9ZbN9U",
    category: ["game"],
  },
  {
    podcastName: "99Vidas",
    episode: "99Vidas 643 – Os Melhores Jogos de 1987",
    videoId: "sZu5xSEODhg",
    cover: "https://i.ytimg.com/vi/sZu5xSEODhg/hqdefault.jpg",
    link: "https://www.youtube.com/watch?v=sZu5xSEODhg",
    category: ["game", "nostalgia"],
  },
];
```

GET: retorna lista de episódios baseado no parametro enviado pelo cliente do nome do podast
