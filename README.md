
# inOrbit

Este é um aplicativo simples para organização de metas. Ele permite que os usuários criem, gerenciem e acompanhem metas semanais. O foco do projeto é proporcionar uma interface clara e intuitiva para o gerenciamento de metas, além de apresentar um progresso semanal de forma visual.

## Funcionalidades

- **Cadastro de metas**: Os usuários podem cadastrar novas metas que precisam ser concluídas.
- **Visualização de metas pendentes**: Exibe todas as metas que ainda não foram concluídas.
- **Progresso semanal**: Visualização gráfica do progresso da semana, incluindo metas concluídas e porcentagem de conclusão.
- **Histórico de metas concluídas**: Exibe metas concluídas com data e hora específicas.
- **Responsive Design**: O aplicativo foi projetado para ser responsivo, se adaptando a diferentes tamanhos de tela.




## Tecnologias Usadas

- **Drizzle ORM**
- **Postgres**
- **Docker**
- **Fastify**
- **Parallel Drive**
- **DayJs**
- **Zod**
- **Biome**
- **Radix**
- **Hook Form**
- **Tanstack**

Fastify como framework, integração do DrizzleORM + PostgreSQL, Docker e Zod para validação de dados.



## Stack utilizada

**Front-end:** ReactJS, TailwindCSS, Vite

**Back-end:** Typescript, NodeJS, TanStack Query


## Demonstração

Insira um gif ou um link de alguma demonstração


## Documentação da API

#### Cria uma meta

```http
  POST /goals
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `title`      | `string` | **Obrigatório**. O título da meta |
| `desiredWeeklyFrequency`      | `number` | **Obrigatório**. A frequência por semana. |



#### Adiciona uma finalização de meta

```http
  POST /create-completion
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `goalId` | `string` | **Obrigatório**. O ID da meta a ser completada |


#### Listagem de pendências

```http
  GET /pending-goals
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `pendingGoals`      | `array` |Lista as metas pendentes |

#### Listagem geral

```http
  GET /get-week-summary
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `summary`      | `array` |Lista todas as metas |
## Autores

- [@brendondev](https://www.github.com/brendondev)
- [@diego3d](https://github.com/diego3g)

