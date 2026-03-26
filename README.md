# projeto-integrador--semestre-1
Gerenciador de ONG's
Um aplicativo mobile e um site para desktop voltado para organização, divulgação e doação para ongs de diversas causas.


### UML geral do gerenciador de ongs. 
```mermaid
sequenceDiagram
 actor U as Usuário
 participant A as APP (FrontEnd)
 participant B as BackAnd
 participant D as Banco de dados

U->>A:Clica em "Ong's"
A->>B:Solicita lista de Ong's 
B->>D:Consulta as Ong's cadastradas e ativas
D-->>B:Retorna lista de Ong's disponíveis
Note over B:Organiza a lista de Ong's em ordem alfabética e ordem de urgência
B-->>A:Retorna lista de Ong's ordenadas
A-->>U:Exibe lista de Ong's em ordem alfabética e de urgência  
```
### Criação de conta
```mermaid
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


