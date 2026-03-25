# projeto-integrador--semestre-1
Gerenciador de ONG's
Um aplicativo mobile e um site para desktop voltado para organização, divulgação e doação para ongs de diversas causas.


### UML geral do gerenciador de ongs. 
```mermaid
sequenceDiagram
 participant U as Usuário
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



