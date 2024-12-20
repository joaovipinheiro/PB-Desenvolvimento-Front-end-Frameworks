# React Native Movie App

## Visão Geral
Este aplicativo foi desenvolvido em React Native para proporcionar uma experiência interativa no celular, permitindo aos usuários:
- Buscar e visualizar informações sobre filmes.
- Marcar filmes como favoritos.
- Navegar facilmente entre as telas do aplicativo.

A aplicação utiliza a API da TMDb (The Movie Database) para obter dados detalhados, como título, sinopse, gêneros, avaliações e trailers de filmes.

---

## Funcionalidades Principais

### 1. Tela Inicial (Home)
- **Barra de Pesquisa:** Busca filmes por título ou gênero.
- **Lista de Filmes:** Apresenta os resultados da busca em uma lista otimizada.
- **Interatividade:** O usuário pode clicar em um filme para visualizar mais detalhes.

### 2. Tela de Detalhes do Filme (MovieDetailPage)
- Exibe informações completas sobre o filme selecionado:
  - Título, sinopse, gêneros e avaliação.
  - Trailer do filme, adaptado para o ambiente móvel.
- Permite marcar o filme como favorito.

### 3. Tela de Favoritos (FavoritesPage)
- Exibe os filmes favoritos do usuário.
- Possibilita a remoção de filmes da lista de favoritos.
- Dados armazenados localmente com `AsyncStorage`.

---

## Estrutura do Aplicativo

### Navegação
Utilizamos o **React Navigation** com um `Stack Navigator` para facilitar a navegação entre as telas:
- Home
- MovieDetailPage
- FavoritesPage

### Componentes Principais
- **MovieCard:** Representa cada filme com título, imagem e botão de favorito.
- **SearchBar:** Componente para pesquisa por título ou gênero.

### Armazenamento Local
O armazenamento de dados foi implementado com `AsyncStorage`, garantindo que os filmes favoritos sejam persistidos mesmo após o fechamento do aplicativo.

---

## Integração com a API da TMDb

### Configuração
- **Chave da API:** `b861b99806c1aaa1c6f8b636986937fe`
- **EndPoints:**
  - Busca de filmes por título e gênero.
  - Detalhes completos de filmes.

### Tecnologias Utilizadas
- `fetch` para requisições HTTP assíncronas.
- Manipulação de dados e exibição na interface do usuário.

---

## Desempenho e Experiência do Usuário
- **FlatList:** Para renderizar listas grandes com eficiência.
- **Responsividade:** Interfaces adaptadas para diferentes tamanhos de tela.
- **Otimização:** Uso de técnicas como lazy loading e compactação de imagens.

---

## Telas Futuras
- **Tela de Login:** Com integração para autenticação via Face ID (iOS) e impressão digital (Android).
- **Notificações:** Alertar o usuário sobre novos filmes adicionados aos favoritos.

---

## Instalação

### Pré-requisitos
- Node.js
- Expo CLI

### Passos para Execução
1. Clone este repositório:
   ```bash
   git clone https://github.com/usuario/react-native-movie-app.git
   ```
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Inicie o servidor Expo:
   ```bash
   npm start
   ```
4. Abra o aplicativo no dispositivo móvel utilizando o Expo Go.

---

## Links Relevantes
- [Código Fonte no CodeSandbox](https://codesandbox.io/p/sandbox/sweet-kowalevski-q9pcfs)
- [Projeto no Snack Expo](https://snack.expo.dev/@joaovpinheiro/movie-search-app)

---

## Conclusão
A adaptação do aplicativo para React Native proporcionou uma experiência fluida e eficiente em dispositivos móveis. Com integração robusta à API da TMDb e foco na usabilidade, o aplicativo atende às necessidades de usuários que buscam explorar e gerenciar filmes de maneira interativa e responsiva.

---

### Autor
- Desenvolvedores: João Martins, Marlon Passeri, Gabriel Maurity, Lucas.
