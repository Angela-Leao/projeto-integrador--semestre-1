
```mermaid

flowchart TD
    A[Apresentações] --> B([Login/ sign in])
    B -->O{Ong}
    B -->D{Doador}
    O -->C[Página da Ong]
    C -->|Perfil; Local; Sobre; Colaboradores; Imagens; Redes sociais.| E [Página central]
    D -->F[Explorar + Como fazer a 1° doação]
    F -->E
    E -->|Configurações;
           Denúncias;
           Perfis;
           Urgências;
           Histórico de doações;
           Comunicação entre os usuários.| G([Fim])
   
