# Pegasus - Sistema de Gerenciamento para Empresa de Turismo

## Capa
- Título do Projeto: Sistema de Gerenciamento de Viagens para Empresa de Turismo
- Nome do Estudante: Lucas Willian de Souza Serpa
- Curso: Engenharia de Software
- Data de Entrega: 

## Resumo
Este documento apresenta a especificação de um sistema de gerenciamento de viagens para uma empresa de turismo. O sistema permitirá o cadastro de motoristas e viagens, além de fornecer controle financeiro detalhado das operações. O objetivo principal é facilitar a administração das viagens e fornecer cálculos financeiros precisos, incluindo custos de pedágio e combustível. O projeto será desenvolvido com React no front-end, NestJS no back-end, e utilizará MySQL como banco de dados, com suporte a notificações via SMS para motoristas.

## Introdução
### Contexto
Empresas de turismo precisam gerenciar motoristas, ônibus e viagens de maneira eficiente para garantir organização e controle financeiro. Atualmente, a administração dessas informações pode ser complexa e suscetível a erros manuais.

## Justificativa
A criação deste sistema busca otimizar o gerenciamento da empresa de turismo do usuário, proporcionando um ambiente centralizado para o controle de viagens, motoristas e custos operacionais. Isso reduzirá o trabalho manual e melhorará a precisão dos cálculos financeiros.

## Objetivos
- Desenvolver um sistema para cadastro e gerenciamento de motoristas e viagens.
- Automatizar o cálculo de receitas e despesas, incluindo custos com pedágios e combustível.
- Enviar notificações via SMS aos motoristas sobre as viagens agendadas.

## Descrição do Projeto
### Tema do Projeto
O sistema de gerenciamento de viagens permitirá que o administrador cadastre viagens com informações detalhadas, como data, horário, origem, destino, valor, ônibus utilizado e motorista responsável.

## Problemas a Resolver
- Falta de organização no controle manual de viagens.
- Dificuldade em calcular receitas e despesas das viagens.
- Comunicação ineficiente com motoristas.

Limitações
- O sistema não incluirá funcionalidades de rastreamento em tempo real dos ônibus.
- Não será implementado um módulo de pagamento online.

## Especificação Técnica

### Requisitos de Software

Lista de Requisitos

Requisitos Funcionais (RF):

- RF01: O sistema deve permitir o cadastro de motoristas.
- RF02: O sistema deve permitir o cadastro de viagens com data, horário, origem, destino, valor, ônibus e motorista.
- RF03: O sistema deve calcular automaticamente o lucro bruto e líquido de cada viagem.
- RF04: O sistema deve obter o preço do combustível em tempo real.
- RF05: O sistema deve enviar um SMS para o motorista com os detalhes da viagem ao ser confirmada.

Requisitos Não Funcionais (RNF):

- RNF01: O sistema deve ter uma interface responsiva desenvolvida em React.
- RNF02: O sistema deve utilizar um banco de dados MySQL.
- RNF03: O backend deve ser desenvolvido utilizando NestJS.
- RNF04: O sistema deve ser executado em contêineres Docker para facilitar a implantação.

Representação dos Requisitos
Os requisitos funcionais serão representados por meio de um Diagrama de Casos de Uso em UML.

## Considerações de Design

Visão Inicial da Arquitetura

A aplicação seguirá uma arquitetura baseada em três camadas principais:

- Frontend (React): Interface para o administrador realizar o gerenciamento das viagens e motoristas.
- Backend (NestJS): Lógica de negócios e comunicação com o banco de dados.
- Banco de Dados (MySQL): Armazena todas as informações do sistema.

Padrões de Arquitetura
- MVC (Model-View-Controller): Separação entre interface, lógica de negócio e persistência de dados.
- Modelos C4
- Contexto: O administrador acessa o sistema via navegador e gerencia as viagens.
- Contêineres: Backend

Componentes: Módulo de cadastro, cálculo financeiro, notificações.

## Stack Tecnológica
Linguagens de Programação

- Frontend: JavaScript/TypeScript com React.
- Backend: TypeScript com NestJS.
- Banco de Dados: SQL com MySQL.

Frameworks e Bibliotecas

- React (UI)
- NestJS (API)
- Twilio (envio de SMS)
- Axios (requisições HTTP para buscar preço do combustível)
- Typeorn (gerenciamento do banco de dados)

Ferramentas de Desenvolvimento e Gestão de Projeto

- Docker (contêineres)
- GitHub (controle de versão)
- Github Actions (gestão do projeto)

Considerações de Segurança

- Autenticação e autorização para garantir que apenas usuários autorizados acessem o sistema.
- Uso de HTTPS para comunicação segura.
- Proteção contra SQL Injection e XSS.

## Próximos Passos
- Desenvolvimento do MVP com as principais funcionalidades.
- Testes internos para validação do sistema.
- Implementação do módulo de notificação via SMS.
- Revisão final e ajustes conforme feedback do usuário.

## Referências

- Documentação oficial do React e NestJS.
- APIs para consulta de preços de combustível.
- Serviços de envio de SMS como Twilio.
- Diagramas detalhados de arquitetura.
- Explicação sobre o cálculo do lucro líquido.

## Avaliações de Professores
Considerações Professor/a:
Considerações Professor/a:
Considerações Professor/a:
