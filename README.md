# Introdução

## Essa API REST terá como objetivo a criação e gerenciamento de decks de Magic: The Gathering (MTG).

# Rotas da API
| Método | Rota                     | Descrição                       | Status Codes |
|--------|--------------------------|---------------------------------|--------------|
| GET | /decks                                | Listar todos os decks            | 200, 500 |
| GET | /decks{id}                        | Buscar deck por id               | 200, 404, 500 |
| GET | /decks/usuario/{idUsuario}  | Listar os decks de um usuário específico | 200, 404, 500 |
| GET | /cartas                         | Listar todas as cartas           | 200, 500 |
| GET | /cartas{id}                     | Buscar carta por id                | 200, 404, 500 | 
| GET | /usuarios                    | Listar todos os usuarios         | 200, 500 |
| GET | /decks/{id}/comentarios        | Listar os comentáris de um deck         | 200, 500 |
| GET | /usuarios{id}                | Buscar usuário por id                | 200, 404, 500 |
| POST | /deck                      | Criar novo deck                  | 201, 400, 500 |
| POST | /decks/{id}/cartas         | Adicionar carta a um deck            | 201, 400, 404, 500 |
| POST | /decks/{id}/comentarios    | Adicionar comentário a um deck   | 201, 400, 404, 500 |
| POST | /cartas                    | Criar nova carta                   | 201, 400, 500 |
| POST | /usuarios                      | Criar novo usuário                 | 201, 400, 500 |
| PUT | /decks/{id}                   | Atualizar dados do deck          | 200, 400, 404, 500 |
| PUT | /usuario/{id}                   |  Atualizar dados do usuário      | 200, 400, 404, 500 |
| PUT | /cartas/{id}                |  Atualizar dados da carta            | 200, 400, 404, 500 |
| DELETE | /decks/{id}/cartas/{idCarta} | Remover carta de um deck     | 204, 404, 500 |
| DELETE | /cartas/{id}                   | Remover uma carta                       | 204, 404, 500 |
| DELETE | /usuarios{id}              | Reover um usuário                       | 204, 404, 500 |
| DELETE | /decks{id}                     | Remover um deck                       | 204, 404, 500 |
