
```mermaid

flowchart TD
    A([Apresentações]) --> B{Login/ sign in}
    B --> O{Ong}
    B --> D {Doador}
    O --> C [Página da Ong]
    C -->|Perfil;
          Local;
          Sobre;
          Colaboradores;
          Imagens;
          Redes sociais.|
    C --> [Página central]
    D --> F [Explorar + Como fazer a 1° doação]
    F --> E [Página central]
    F --> |Apenas Pix|
    E --> |Configurações;
           Denúncias;
           Perfis;
           Urgências;
           Histórico de doações;
           Comunicação entre os usuários.|
   
