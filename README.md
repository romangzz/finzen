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

### 2. Initialize Go module
```bash
go mod tidy
```

### 3. Run the API
```bash
go run cmd/api/main.go
```

### 4. Import your first CSV
```bash
curl -X POST -F "file=@transactions.csv" http://localhost:8080/import
```

## 🧱 Folder Structure

```bash
finzen/
├── cmd/
│   └── api/                 # Application entry point
├── internal/
│   ├── domain/              # Entities, Value Objects, Aggregates
│   ├── application/         # Commands, Queries, Handlers
│   ├── infrastructure/      # Repositories, Adapters, CSV Importers
├── pkg/                     # Shared utilities
└── go.mod
```

## 🤝 Contributing

Contributions are welcome!  
If you’d like to help improve Finzen, feel free to open issues or pull requests.

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.

**Finzen** — *Stay Zen with your Finances.*
