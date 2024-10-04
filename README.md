# inOrbit

This is a simple goal management app. It allows users to create, manage, and track weekly goals. The focus of the project is to provide a clear and intuitive interface for goal management, as well as to present weekly progress in a visual format.

## Features

- **Goal Tracker**: Users can register new goals that need to be completed.
- **Pending Goal View**: Displays all goals that have not yet been completed.
- **Weekly Progress**: Graphical view of weekly progress, including completed goals and percentage of completion.
- **Completed Goal History**: Displays completed goals with a specific date and time.
- **Responsive Design**: The app is designed to be responsive, adapting to different screen sizes.

## Technologies Used

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

Fastify as a framework, DrizzleORM + PostgreSQL integration, Docker and Zod for data validation.

## Stack used

**Front-end:** ReactJS, TailwindCSS, Vite

**Back-end:** Typescript, NodeJS, TanStack Query

## Demo

https://github.com/user-attachments/assets/5068cf16-52a0-459d-b220-2e4ef9e2c5c1

## API documentation

#### Create a goal

```http
POST /goals
```

| Parameter | Type | Description |
| :--------- | :--------- | :-------------------------------------------- |
| `title` | `string` | **Required**. The title of the goal |
| `desiredWeeklyFrequency` | `number` | **Required**. The frequency per week. |

#### Add a goal completion

```http
POST /create-completion
```

| Parameter | Type | Description |
| :---------- | :--------- | :----------------------------------- |
| `goalId` | `string` | **Required**. The ID of the goal to be completed |

#### Pending list

```http
GET /pending-goals
```

| Parameter | Type | Description |
| :--------- | :--------- | :-------------------------------------------- |
| `pendingGoals` | `array` |Lists pending goals |

#### General list

```http
GET /get-week-summary
```

| Parameter | Type | Description |
| :--------- | :--------- | :--------------------------- |
| `summary` | `array` |List all goals |
## Authors

- [@brendondev](https://www.github.com/brendondev)
- [@diego3g](https://github.com/diego3g)
