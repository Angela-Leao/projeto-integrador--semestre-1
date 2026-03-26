


### Criação de conta 
```mermaid
sequenceDiagram
actor U as Usuário
participant A as APP(Frontend)
participant B as Backend
participant C as Banco de dados
 U->>A: Clica em "Primeiro acesso"
 A->>B: Prepara o ambiente de criação de conta
 B->>D: Armazena os dados da conta no banco de dados
 D-->>B: Verificação de conta
 B-->>A: Retorna o acesso a conta
 A-->>B:Retorna a página inicial  
