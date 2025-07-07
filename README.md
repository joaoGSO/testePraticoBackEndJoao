# testePraticoBackEndJoao

Para que o banco de dados seja criado, basta abrir o cmd do visual studio e digitar "Update-Database", assim criando todas as tabelas e as relações em um banco local.

*Features solicitadas que consegui implementar (visualizaveis pelo swagger):*

1.Usuários
  - Cadastro: GET/api/Users
  - Um usuário pode seguir outros usuários: POST/api/Users/{id}/follow/{targetId}

2.Posts
  - Um usuário pode criar posts: GET/api/Posts
  - O criador do post pode
    - Editar o post: PUT/api/Posts/{postId}
    - Deletar o post: DELETE/api/Posts/{postId}
    - Adicionar tags ao post: POST/api/Posts/{postId}/tags

3.Tags
  - Tags podem ser criadas dinamicamente: POST/api/tags

4.Interações
  - Usuários podem curtir posts: POST/api/Users/{id}/follow/{targetId}

5.Timeline
  - Posts de usuários seguidos (ordenados por data): GET/api/Users/feed/{userId}
  - Filtro por tags: GET/api/Posts/bytag/{tagName}
  - Posts mais curtidos nas últimas 24h: GET/api/Posts/trending

6.Lista todos os posts do usuário: GET/api/Posts


*Features que ficaram de fora:*

3.Tags
  - Ao tentar adicionar uma tag, tags existentes devem ser listadas como sugestão

4.Interações
  - Usuários podem comentar em posts 
