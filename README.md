# 🧘 Finzen

**Finzen** lets you upload and analyze your bank transactions, categorize expenses automatically, and monitor your monthly spending habits.

It’s built with **Hexagonal Architecture**, **DDD**, **CQS**, and **Event-Driven** principles to ensure scalability, modularity, and extensibility from day one.

## 🚀 Features

- 📂 **Import CSV statements** from your bank accounts  
- 🧠 **Automatic transaction categorization** with suggestion learning  
- 📊 **Monthly and yearly spending summaries**  
- 💰 **Multi-account support**  
- 🪞 **Budget tracking** and financial health overview  
- 🔒 **100% self-hosted** — your data stays on your machine  
- ⚙️ **Modular architecture** (ready for plugins or external services)

## 🏁 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/romangzz/finzen.git
cd finzen
```

### 2. Run the API

> **Taskfile is required.** Please refer to [the documentation](https://taskfile.dev/docs/installation) for installation instructions.

```bash
task run-api
```

## 🧱 Folder Structure

```bash
finzen/
├── api/                               # Backend (Go)
│   ├── cmd/
│   │   └── server/                    # Application entry point
│   │       └── main.go
│   ├── internal/
│   │   ├── domain/                    # Entities, Value Objects, Aggregates
│   │   ├── application/               # Commands, Queries, Handlers (CQS)
│   │   └── infrastructure/            # Repositories, Adapters, CSV Importers
│   │       ├── http/                  # HTTP controllers / routers
│   │       ├── persistence/           # DB adapters (Postgres/etc.)
│   │       └── importer/              # CSV parsers & mappers
│   ├── pkg/                           # Shared utilities
│   ├── go.mod
│   └── go.sum
├── web/                               # Frontend (React, placeholder)
│   ├── .gitkeep
│   └── .gitignore
├── configs/                           # Static configuration (YAML/JSON)
│   └── application.yaml
├── Taskfile.yml                       # Tasks for build/test/run
├── .gitignore
└── README.md

```

## 🤝 Contributing

Contributions are welcome!  
If you’d like to help improve Finzen, feel free to open issues or pull requests.

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.

**Finzen** — *Stay Zen with your Finances.*
