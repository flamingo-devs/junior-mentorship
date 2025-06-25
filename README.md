# Desafio Full Stack: Sistema de Reservas de Salas

> Projeto orientado para aprendizado prático de desenvolvimento full stack. O desafio é construir, do zero, uma aplicação completa que permita a reserva de salas em diferentes horários, simulando um sistema usado por empresas.

---

## 🧠 Objetivo

Você irá construir um sistema web de **reserva de salas de reunião**, permitindo que usuários se cadastrem, visualizem salas disponíveis e reservem horários. O sistema deve prevenir conflitos de horário e oferecer uma interface clara para os usuários acompanharem suas reservas.

Esse projeto visa simular um ciclo de desenvolvimento completo, desde o planejamento até a entrega e apresentação.

Registre tudo: ideias que gostaria de implementar se tivesse tempo (explique como você as resolveria, se houvesse tempo), decisões que forem tomadas e seus porquês, arquiteturas que forem testadas, os motivos de terem sido modificadas ou abandonadas, instruções de instalação, etc. Crie um único arquivo "COMMENTS.md" no repositório para isso.

---

## 🛠️ Stack Tecnológica

Você tem liberdade para escolher as tecnologias que preferir. Algumas sugestões:

* **Frontend**: React / Vue / Next.js / outro framework SPA. Ps: se quiser usar só html/css/js puro, também é válido, mas considere que o desafio é mais interessante com um framework moderno e usado por empresas.
* **Backend**: Node.js (Express) ou PHP (Laravel, Symfony) ou Python (Django, Flask) ou outro framework de sua preferência.
* **Banco de Dados**: PostgreSQL, Supabase, MySQL, SQLite

---

## 📆 Requisitos Funcionais (MVP)

* Listagem de salas de reunião (com nome, capacidade, descrição)
* Reservar uma sala para um horário e data específicos
* Visualizar minhas reservas futuras
* Cancelar reserva (antes do horário marcado)
* Impedir conflito de horários na mesma sala

---

## ✨ Requisitos Opcionais (Extras)

* Filtros de salas por capacidade ou nome
* Painel de administrador para criar, editar ou excluir salas
* Restrições (ex: reserva só em horário comercial)
* Visualizar um calendário de reservas
* Layout responsivo

---

## 🔧 Entregáveis Esperados

* ✅ **Repositório no GitHub** com código fonte separado por frontend/backend (ou monorepo, se preferir)
    ps: monorepo pode ser melhor pra visualizar o projeto como um todo, mas sinta-se à vontade para usar a estrutura que preferir.

* ✅ **README** explicando o projeto, como rodar localmente e quais decisões técnicas foram tomadas
* ✅ **Diagrama do Banco de Dados (ERD)** — pode ser feito com [dbdiagram.io](https://dbdiagram.io/), [draw.io](https://draw.io) ou outro
* ✅ **Desenho da Arquitetura** da aplicação (ex: fluxograma simples, onde entram backend, banco, frontend)
* ✅ **Apresentação**: simulação de entrevista explicando o projeto, suas escolhas e aprendizados

---

## 📊 Sugestão de Estrutura de Dados

* **users** (id, name, email, password\_hash, createdAt, updatedAt)
* **rooms** (id, name, capacity, description, createdAt, updatedAt)
* **reservations** (id, user\_id, room\_id, startReservation, endReservation, status, createdAt, updatedAt)

Relacionamentos:

* 1 usuário → muitas reservas
* 1 sala → muitas reservas

ps: são apenas sugestões, sinta-se à vontade para adaptar, inclusive adicionar mais entidades se achar necessário.

---

## 🗓️ Etapas Sugeridas

### Semana 1: Planejamento e modelagem

* Defina as entidades do banco
* Faça o diagrama ER
* Esboce telas ou fluxos principais

### Semana 2: Backend

* Configure o projeto (Express, banco de dados)
* Implemente autenticação e endpoints principais (login, listar salas, reservar)

### Semana 3: Frontend

* Crie as páginas principais (login, dashboard, reservas)
* Conecte com a API

### Semana 4: Deploy e Apresentação

* Publique o projeto
* Reforce o README
* Prepare-se para apresentar o projeto como se fosse uma entrevista

---

## 🧪 Como será avaliado

* Clareza na modelagem e estrutura
* Entendimento do fluxo e regras de negócio
* Organização do código
* Raciocínio técnico por trás das decisões
* Capacidade de buscar soluções e aprender durante o processo

## Cuidados importantes
* **Documentação**: mantenha o README atualizado com instruções claras de instalação e uso
* **Controle de Versão**: use commits claros e significativos no Git, documentando o que foi feito em cada etapa.
* **Inteligencia Artificial**: evite usar IA para gerar código ou resolver problemas, não ao menos sem saber o que ela está cuspindo. O objetivo é aprender e praticar suas habilidades de programação, então busque resolver os desafios por conta própria. Use IA apenas para tirar dúvidas ou buscar explicações sobre conceitos.
    Caso você use IA pra gerar algum código, cuide para que você entenda o que está sendo gerado.

# Lins úteis
* [Roadmap Full Stack](https://roadmap.sh/full-stack) - Pode ajudar a entender alguns temas que esteja com dúvida, com links pra estudo.
* [Como começar seu projeto Full Stack](https://www.reddit.com/r/react/comments/1kwej4g/how_to_start_your_own_full_stack_project_without/?tl=pt-br) - Dicas de como começar um projeto Full Stack do zero, reddit é uma boa fonte de informação.

# Boa sorte!
Espero que você aprenda muito com esse desafio! O objetivo é praticar e se divertir, então não hesite em explorar, errar e aprender com o processo. Boa sorte e bora sujar as mãos no código! 🚀