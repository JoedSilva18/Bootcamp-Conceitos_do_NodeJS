<h1  align="center">
<img  alt="GoStack"  src="https://rocketseat-cdn.s3-sa-east-1.amazonaws.com/bootcamp-header.png"  width="200px" />
</h1>
<h3 align="center">
  Desafio 1: Conceitos do NodeJS
</h3>
<blockquote align="center">“Sua única limitação é você mesmo”!</blockquote>

<h3>Descrição:</h3>
O projeto se resume em uma aplicação para armazenamento de projetos e suas tarefas utilizando Express.

  
### Rotas

- `POST /projects`: A rota deve receber `id` e `title` dentro do corpo e cadastrar um novo projeto dentro de um array no seguinte formato: `{ id: "1", title: 'Novo projeto', tasks: [] }`.

- `GET /projects`: Rota que lista todos projetos e suas tarefas;

- `PUT /projects/:id`: A rota deve alterar apenas o título do projeto com o `id` presente nos parâmetros da rota;

- `DELETE /projects/:id`: A rota deve deletar o projeto com o `id` presente nos parâmetros da rota;

- `POST /projects/:id/tasks`: A rota deve receber um campo `title` e armazenar uma nova tarefa no array de tarefas de um projeto específico escolhido através do `id` presente nos parâmetros da rota;

### Exemplo

Chamando a rota `POST /projects` repassando `{ id: 1, title: 'Novo projeto' }` e a rota `POST /projects/1/tasks` com `{ title: 'Nova tarefa' }`, o array de projetos deve ficar assim:

```js
[
  {
    id: "1",
    title: "Novo projeto",
    tasks: ["Nova tarefa"]
  }x
];
