Este projeto é um sistema simples de **Kanban** desenvolvido em **Java puro**, com um servidor HTTP embutido.  
Ele permite criar, visualizar e mover tarefas entre colunas (A Fazer, Fazendo, Feito).  
Os dados são salvos em um arquivo CSV, garantindo persistência entre execuções.


Funcionalidades :
Criar novas tarefas.
Mover tarefas entre colunas (A Fazer, Fazendo, Feito).
Persistência em arquivo CSV.
Interface HTML gerada dinamicamente.


Limitações:
Armazenamento em arrays fixos, o que limita a escalabilidade.
Não há autenticação, permitindo que qualquer usuário modifique os dados.
Persistência em arquivo CSV simples, inadequada para grandes volumes de informação.
Interface HTML básica, sem recursos modernos como drag-and-drop.


Avaliação do Projeto:

Pontos fortes:
Simplicidade: desenvolvido apenas com Java SE, sem uso de frameworks adicionais.
Facilidade de compilação e execução, sem dependências externas.
Persistência garantida em arquivo CSV, evitando perda de dados entre execuções.

Pontos fracos:
Escalabilidade limitada devido ao uso de arrays fixos e ausência de banco de dados.
Falta de segurança e autenticação.
Interface pouco interativa, sem recursos visuais mais avançados.
Dificuldade de manutenção e expansão do sistema.


Proposta de Substituição:

Para tornar o sistema mais robusto e moderno, recomenda-se migrar para uma arquitetura web full-stack:

Backend:
Uso do framework Spring Boot (Java) para criar uma API REST estruturada, com suporte a autenticação e integração com banco de dados.
Substituição do arquivo CSV por um banco de dados relacional (PostgreSQL, MySQL) ou NoSQL (MongoDB).

Frontend:
Desenvolvimento de uma interface em React ou Vue.js, permitindo maior interatividade e recursos como drag-and-drop.
Comunicação entre frontend e backend por meio de API REST.
