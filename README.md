# 🐾 Pet Mania API - Desafio Spring Boot

Este repositório contém a resolução do **Desafio Pet Mania API**, um projeto desenvolvido em Java com Spring Boot para gerenciamento de cadastro de animais. O objetivo principal da atividade foi investigar, identificar e corrigir falhas de arquitetura, mapeamento, sintaxe e regras de rotas da aplicação, restabelecendo a funcionalidade total do CRUD.

---

## 🛠️ Tecnologias Utilizadas

- **Java 17**
- **Spring Boot** (Spring Data JPA, Spring Web)
- **Banco de Dados:** H2 Database / MySQL
- **Testes e Validação:** Postman & Front-end HTML/JS

---

## 🔧 Correções Realizadas no Projeto

1. **Camada de Controller (`PetController`):**
   - Correção e padronização das anotações REST (`@RestController` e `@RequestMapping("/api/pets")`).
   - Implementação dos endpoints completos para operações CRUD:
     - `GET /api/pets`: Listagem de todos os animais.
     - `GET /api/pets/{id}`: Busca individual por ID.
     - `POST /api/pets`: Cadastro de novos animais.
     - `DELETE /api/pets/{id}`: Remoção de cadastro por ID.
   - Ajuste dos retornos e códigos de Status HTTP (`200 OK`, `201 Created` e `204 No Content`).

2. **Camada de Persistência & Entidade:**
   - Padronização do tipo de chave primária (`Integer`) da entidade `Pet`.
   - Ajuste do repositório `PetRepository` herdando de `JpaRepository<Pet, Integer>`.
   - Correção do mapeamento ORM `@Table(name = "tb_pet")`.

3. **Integração & Repositório Git:**
   - Sincronização e configuração dos remotos para a cópia pessoal (Fork) do projeto.

---
