Gerenciador de salas de aula / de turmas — projeto em Java para gerenciamento de alunos, turmas, professores etc.

Visão geral

Este projeto se propõe a facilitar operações comuns de gerenciamento escolar, como:

cadastro e consulta de turmas

associação de alunos e professores a turmas

CRUD (criar, ler, atualizar, deletar) de entidades como aluno, professor, turma

persistência via banco de dados (configuração via pom.xml)

estrutura modular em camadas (model, repository, service, controller)


O código é escrito em Java (utilizando Maven) e segue boas práticas de separação de responsabilidades.


---

Tecnologias utilizadas

Java (versão compatível conforme pom.xml)

Maven para gerenciamento de dependências e build

JPA / Hibernate (ou outro framework de persistência, conforme implementação)

Banco de dados relacional (via configuração externa)

Design em camadas (model, repository, service, controller)
[16:21, 26/10/2025] Lucas: Exemplos de uso (REST API)

Método HTTP	Endpoint	Descrição

GET	/turmas	Listar todas as turmas
POST	/turmas	Criar nova turma
GET	/alunos/{id}	Obter dados de um aluno específico
PUT	/alunos/{id}	Atualizar dados de aluno
DELETE	/professores/{id}	Deletar professor


(Ajuste esses exemplos conforme a real implementação do seu projeto.)


---

Testes

A pasta src/test deve conter testes unitários ou de integração para service, repository e controller.

Use frameworks como JUnit, Mockito, etc.

Execute:

mvn test



---

Boas práticas aplicadas

Separação de camadas (controlador, serviço, repositório)

Inversão de dependência / injeção de dependência

Tratamento de exceções padronizado

Uso de DTOs (se houver) para controlar dados trafegados

Validações (ex: campos obrigatórios)



---

Próximas melhorias / planos futuros

Implementar autenticação e autorização

Paginação e filtros em endpoints de listagem

Documentação automática de API (Swagger, OpenAPI)

Upload / download de arquivos (ex: planilhas de alunos)

Front-end web ou interface gráfica