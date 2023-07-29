# GymPass

## 🎯 Sobre

O projeto GymPass tem como objetivo o usuário encontrar uma academia perto dele para fazer o check-in.

## 🖥️ Tecnologias

* NodeJS
* Typescript
* Fastify
* Docker
* Prisma
* Vitest

## 😁 Como utilizar

* `npm install` - Para instalar as dependências`
* `docker compose up -d` - Para criar um container no docker
* `npm run test` - Para rodar testes unitários
* `npm run test:e2e` - Para rodar testes de integração
* `npm run dev` - Para rodar a aplicação em desenvolvimento
* `npm run build` - Para fazer o build
* `npm start` - Para rodar a aplicação em produção

---

## RFs (Requisitos funcionais)

- [X] Deve ser possível se cadastrar;
- [X] Deve ser possível se autenticar;
- [X] Deve ser possível obter o perfil de um usuário logado;
- [X] Deve ser possível obter o número de check-ins realizado pelo usuário logado;
- [X] Deve ser possível o usuário obter seu histórico de check-ins;
- [X] Deve ser possível o usuário buscar academias próximas (até 10km);
- [X] Deve ser possível o usuário buscar uma academias pelo nome;
- [X] Deve ser possível o usuário realizar check-in em uma academia;
- [X] Deve ser possível validar o check-in de um usuário;
- [X] Deve ser possível cadastrar uma academia; 

## RNs (Regras de negócios)

- [X] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [X] O usuário não pode fazer 2 check-ins no mesmo dia;
- [X] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [X] O check-in só pode ser validado até 20 minutos após criado;
- [X] O check-in só pode ser validado por administradores;
- [X] A academia só pode ser cadastrada por administradores;

## RNFs (Requisitos não-funcionais)

- [X] A senha do usuário precisa estar criptografada;
- [X] Os dados da aplicação precisa estar persistidos em um banco PostgreSQL;
- [X] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [X] O usuário deve ser identificado por um JWT (JSON Web Token);
