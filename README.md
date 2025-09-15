# Netflix Remake

Remake do aplicativo Netflix, desenvolvido em Kotlin para a plataforma Android. O projeto visa replicar a experiência de navegação e visualização de conteúdo de vídeo, com foco na exibição de categorias de filmes e detalhes de cada título, incluindo filmes similares.

## Funcionalidades

### Listagem de Categorias de Filmes

A tela principal exibe uma lista horizontal de categorias de filmes, permitindo ao usuário navegar por diferentes gêneros e coleções. Cada categoria é apresentada com um título e uma prévia dos filmes associados.

### Detalhes do Filme

Ao selecionar um filme, o usuário é direcionado para uma tela de detalhes que exibe informações como título, descrição, imagem de capa e uma lista de filmes similares. Esta funcionalidade aprimora a descoberta de conteúdo e a experiência do usuário.

### Carregamento Assíncrono de Dados

O aplicativo utiliza tarefas assíncronas para buscar dados de categorias e filmes de uma API externa, garantindo que a interface do usuário permaneça responsiva durante o carregamento. Imagens são carregadas de forma eficiente para otimizar o desempenho.

## Tecnologias Utilizadas

*   **Kotlin**: Linguagem de programação principal para o desenvolvimento Android.
*   **Android SDK**: Conjunto de ferramentas de desenvolvimento para a plataforma Android.
*   **Picasso**: Biblioteca eficiente para carregamento e cache de imagens, otimizando a exibição de capas de filmes.
*   **RecyclerView**: Utilizado para exibir listas de categorias e filmes de forma performática e customizável.
*   **AsyncTask**: Para gerenciar operações de rede em segundo plano, mantendo a UI fluida.

## Estrutura do Projeto

O projeto é organizado da seguinte forma:

*   `MainActivity.kt`: A atividade principal que exibe a lista de categorias de filmes e gerencia a navegação para a tela de detalhes.
*   `MovieActivity.kt`: Exibe os detalhes de um filme selecionado, incluindo sua descrição e uma lista de filmes relacionados.
*   `CategoryAdapter.kt`: Adaptador para a `RecyclerView` da tela principal, responsável por exibir as categorias de filmes.
*   `MovieAdapter.kt`: Adaptador para a `RecyclerView` dentro das categorias e para a lista de filmes similares na tela de detalhes.
*   `model/`: Contém as classes de modelo de dados (`Category.kt`, `Movie.kt`, `MovieDetail.kt`) que representam a estrutura dos dados consumidos da API.
*   `util/`: Inclui classes utilitárias como `CategoryTask.kt`, `MovieTask.kt` (para requisições de rede assíncronas) e `DownloadImageTask.kt` (para carregamento de imagens).

Contribuições são bem-vindas! 
