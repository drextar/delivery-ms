# Projeto de Delivery de Pedidos

Implementação para fins de estudos e aperfeiçoamento em habilidades de desenvolvimento, levantamento de requisitos, análise de sistemas.

O projeto foi desenvolvido tendo em mente um sistema de delivery.

O desafio é transformar o sistema monolito em microsserviços.

Vantagens:

- Facilidade de manutenção e/ou mudanças no projeto.

- Escalabilidade independente.

- Experimentação tecnológica.

## Roadmap desenvolvimento

Cada microsserviços foi desenvolvido utilizando padrão MVC.

Construção de microsserviços de pagamentos: 

- Construir a API, inserir um banco de dados isolado e separar os pacotes por camadas de responsabilidade.

- Utilização de migrations para fazer a criação do SQL e versionar o banco de dados, implementado Service Discovery com o Service Registry, registrando os microsserviços para eles poderem descobrir um ao outro através dos nomes.

- Implementado parte de balanceamento de cargas e a inclusão do Gateway na aplicação, sendo um ponto chave quando estamos trabalhando com arquitetura de microsserviços. Comunicação síncrona entre os serviços de pedido e pagamentos.

- Tratadas as falhas caso o serviço de pedidos fique indisponível, foi possível programar como seriam tratadas essas falhas.

- Utilizado o Eureka e feitas todas as solicitações através do Postman para testar a aplicação.

## Ferramentas e Tecnologias

- Java 17
- MySQL Workbench
- Maven
- Postman
- Spring Boot
- Spring Feign
- Eureka Server
- Resilience 4j
