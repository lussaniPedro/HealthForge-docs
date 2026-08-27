# Arquitetura do backend

> Comando Tree na raiz do projeto

```text
src/
├── config
├── exception
├── modules
│   ├── auth
│   │   ├── controller
│   │   ├── dto
│   │   ├── entity
│   │   ├── exception
│   │   ├── repository
│   │   ├── security
│   │   └── service
│   ├── user
│   │   ├── linkRequest
│   │   │   ├── controller
│   │   │   ├── dto
│   │   │   ├── entity
│   │   │   ├── enums
│   │   │   ├── exception
│   │   │   ├── repository
│   │   │   └── service
│   │   └── user
│   │       ├── controller
│   │       ├── dto
│   │       ├── entity
│   │       ├── enums
│   │       ├── exception
│   │       ├── repository
│   │       └── service
│   ├── diet
│   │   ├── dietPlan
│   │   │   ├── controller
│   │   │   ├── dto
│   │   │   ├── entity
│   │   │   ├── enums
│   │   │   ├── exception
│   │   │   ├── repository
│   │   │   └── service
│   │   └── food
│   │       ├── controller
│   │       ├── dto
│   │       ├── entity
│   │       ├── enums
│   │       ├── exception
│   │       ├── repository
│   │       └── service
│   └── workout
│       ├── exercise
│       │   ├── controller
│       │   ├── dto
│       │   ├── entity
│       │   ├── enums
│       │   ├── exception
│       │   ├── repository
│       │   └── service
│       ├── trainingPlan
│       │   ├── controller
│       │   ├── dto
│       │   ├── entity
│       │   ├── exception
│       │   ├── repository
│       │   └── service
│       └── workout
│           ├── controller
│           ├── dto
│           ├── entity
│           ├── exception
│           ├── repository
│           └── service
└── util
```