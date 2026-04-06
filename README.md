![Relatório de cobertura JaCoCo](images/jacoco-report.png)

Java REST API - Testes Unitários

Descrição do Projeto

Este projeto é uma API REST simples desenvolvida com Spring Boot para gerenciamento de itens.
A aplicação oferece suporte aos formatos JSON e XML e foi utilizada para implementar e validar testes unitários automatizados.

O objetivo desta atividade foi completar a suíte de testes do projeto base fornecido na branch UnitCompleto, cobrindo cenários de sucesso, falhas, exceções e validações de regras de negócio.

---

Tecnologias Utilizadas

- Java
- Spring Boot
- JUnit 5
- Mockito
- MockMvc
- Maven
- JaCoCo

---

Estrutura do Projeto

java-rest-api
|-- images
|   |-- jacoco-report.png
|-- src
|-- pom.xml
|-- README.md

---

Endpoints da API

Endpoints existentes:
- GET /api/items
- GET /api/items/{id}
- POST /api/items
- PUT /api/items/{id}
- DELETE /api/items/{id}

Novos endpoints adicionados:
- GET /api/items/search?name=...
- PATCH /api/items/{id}/description

---

Regras de Negócio

- name é obrigatório
- description é obrigatório
- não permitir valores vazios
- JSON inválido retorna 400
- item inexistente retorna 404

---

Como Executar

cd java-rest-api
mvn spring-boot:run

---

Executar Testes

mvn test

---

Gerar Cobertura

mvn clean verify

Relatório:
target/site/jacoco/index.html

---

Relatório de Cobertura

Imagem localizada em:
images/jacoco-report.png

---

Resultado

Projeto com alta cobertura de testes, cobrindo cenários de sucesso e falhas conforme solicitado.
