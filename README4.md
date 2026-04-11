
```mermaid

flowchart TD
    A([Usuário acessa sistema]) --> B{Primeiro acesso}
    B -->|Sim| C[Criar conta com tipo]
    B -->|Não| D[Fazer login]
    C --> D
    D --> E{Credenciais válidas}
    E -->|Não| F[Mostrar erro]
    F --> D
    E -->|Sim| G{Qual o tipo?}
    G -->|Usuário comum| H[DirecionamentoU → InterfaceU]
    G -->|Gestor ONG| I[DirecionamentoG → InterfaceG]
    H --> J([Fim])
    I --> J
