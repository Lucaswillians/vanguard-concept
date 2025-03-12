# **Pegasus - Sistema de Gerenciamento para Empresa de Turismo**

## 📌 Capa
- **Título do Projeto:** Sistema de Gerenciamento de Viagens para Empresa de Turismo  
- **Nome do Estudante:** Lucas Willian de Souza Serpa  
- **Curso:** Engenharia de Software  
- **Data de Entrega:**  

---

## 📌 Resumo
Este documento apresenta a especificação de um sistema de gerenciamento de viagens para uma empresa de turismo. O sistema permitirá o cadastro de motoristas e viagens, além de fornecer controle financeiro detalhado das operações.  

Além disso, contará com um módulo de orçamentos para cálculo automático de custos e um sistema de cálculo de salários dos motoristas, considerando diferentes métodos de pagamento.  

O projeto será desenvolvido com **React** no front-end, **NestJS** no back-end e utilizará **MySQL** como banco de dados, com suporte a notificações via **SMS** para motoristas.

---

## 📌 Introdução

### **Contexto**
Empresas de turismo precisam gerenciar motoristas, ônibus e viagens de maneira eficiente para garantir organização e controle financeiro. Atualmente, a administração dessas informações pode ser complexa e suscetível a erros manuais.

### **Justificativa**
A criação deste sistema busca otimizar o gerenciamento da empresa de turismo do usuário, proporcionando um ambiente centralizado para o controle de viagens, motoristas, custos operacionais e orçamentos. Isso reduzirá o trabalho manual e melhorará a precisão dos cálculos financeiros.

---

## 📌 Objetivos

### 🎯 **Objetivos Gerais**
- Desenvolver um sistema para **cadastro e gerenciamento de motoristas e viagens**.
- Automatizar o cálculo de **receitas e despesas**, incluindo custos com pedágios e combustível.
- Implementar um módulo de **orçamentos**, permitindo a geração de propostas automáticas e exportação para **PDF**.
- Criar um **sistema de cálculo de salários** para os motoristas.
- Enviar **notificações via SMS** aos motoristas sobre as viagens agendadas.

### 🎯 **Objetivos Específicos**
- Permitir a geração e edição de **orçamentos** com base nas informações da viagem.
- Criar um histórico de **orçamentos aprovados**, vinculando-os às viagens realizadas.
- Implementar diferentes formas de **cálculo de salário** para os motoristas, com base em salário fixo, comissão ou por km rodado.
- Criar um **relatório financeiro** detalhado das operações.

---

## 📌 Descrição do Projeto

### **Tema do Projeto**
O sistema de gerenciamento de viagens permitirá que o administrador cadastre viagens com informações detalhadas, como data, horário, origem, destino, valor, ônibus utilizado e motorista responsável.  

Além disso, contará com um **módulo de orçamentos**, que possibilitará a geração automática do custo de uma viagem antes de sua confirmação.

---

## 📌 Problemas a Resolver

- **Falta de organização** no controle manual de viagens.  
- **Dificuldade em calcular receitas e despesas** das viagens.  
- **Falta de um sistema de orçamentos**, resultando em cálculos manuais demorados.  
- **Gestão ineficiente dos salários dos motoristas**, dificultando a previsão de custos.  
- **Comunicação ineficiente com motoristas** sobre as viagens confirmadas.  

---

## 📌 Especificação Técnica

### **Lista de Requisitos**

#### ✅ **Requisitos Funcionais (RF)**

- **RF01**: O sistema deve permitir o cadastro de motoristas.  
- **RF02**: O sistema deve permitir o cadastro de viagens com data, horário, origem, destino, valor, ônibus e motorista.  
- **RF03**: O sistema deve calcular automaticamente o lucro bruto e líquido de cada viagem.  
- **RF04**: O sistema deve obter o preço do combustível em tempo real.  
- **RF05**: O sistema deve enviar um SMS para o motorista com os detalhes da viagem ao ser confirmada.  
- **RF06**: O sistema deve permitir a criação de orçamentos de viagens antes da confirmação.  
- **RF07**: O sistema deve gerar **PDFs de orçamentos** para envio ao cliente.  
- **RF08**: O sistema deve permitir que orçamentos sejam convertidos em viagens confirmadas.  
- **RF09**: O sistema deve calcular automaticamente o **salário dos motoristas**, com base no tipo de pagamento (fixo, comissão ou por km rodado).  
- **RF10**: O sistema deve gerar um **relatório financeiro**, incluindo receita, despesas e custos com motoristas.  

#### ✅ **Requisitos Não Funcionais (RNF)**

- **RNF01**: O sistema deve ter uma interface responsiva desenvolvida em React.  
- **RNF02**: O sistema deve utilizar um banco de dados MySQL.  
- **RNF03**: O backend deve ser desenvolvido utilizando NestJS.  
- **RNF04**: O sistema deve ser executado em contêineres Docker para facilitar a implantação.  

---

## 📌 Módulo de Cálculo de Salários dos Motoristas

### 🔹 **Métodos de Pagamento Suportados**
1️⃣ **Salário Fixo + Adicionais por Viagem**  
   - O motorista recebe um valor fixo mensal.  
   - Pode haver bônus por viagem realizada.  

2️⃣ **Pagamento por Viagem**  
   - O motorista recebe um valor fixo por quilômetro rodado ou por viagem concluída.  

3️⃣ **Comissão sobre o Valor da Viagem**  
   - O motorista recebe uma porcentagem do valor total da viagem.  

### 🔹 **Funcionalidades do Módulo**
✅ Cadastro de motoristas com tipo de pagamento.  
✅ Cálculo automático de salários com base nas viagens realizadas.  
✅ Geração de relatório mensal de pagamento.  
✅ Histórico de pagamentos anteriores.  
✅ Exportação do salário em **PDF** (como um "holerite").  

---

## 📌 Considerações de Design

### **Visão Inicial da Arquitetura**
A aplicação seguirá uma arquitetura baseada em três camadas principais:

- **Frontend (React)**: Interface para o administrador realizar o gerenciamento das viagens e motoristas.  
- **Backend (NestJS)**: Lógica de negócios e comunicação com o banco de dados.  
- **Banco de Dados (MySQL)**: Armazena todas as informações do sistema.  

### **Padrões de Arquitetura**
- **MVC (Model-View-Controller)**: Separação entre interface, lógica de negócio e persistência de dados.  
- **Modelos C4**: Para representação da arquitetura.  

---

## 📌 Stack Tecnológica

### **Linguagens de Programação**
- **Frontend**: JavaScript/TypeScript com React.  
- **Backend**: TypeScript com NestJS.  
- **Banco de Dados**: SQL com MySQL.  

### **Frameworks e Bibliotecas**
- React (UI)  
- NestJS (API)  
- Twilio (envio de SMS)  
- Axios (requisições HTTP para buscar preço do combustível)  
- TypeORM (gerenciamento do banco de dados)  

### **Ferramentas de Desenvolvimento e Gestão**
- Docker (contêineres)  
- GitHub (controle de versão)  
- GitHub Actions (gestão do projeto)  

---

## 📌 Próximos Passos

- Desenvolvimento do **MVP** com as principais funcionalidades.  
- Testes internos para validação do sistema.  
- Implementação do módulo de **cálculo de salários** dos motoristas.  
- Revisão final e ajustes conforme feedback do usuário.  

---

## 📌 Referências
- Documentação oficial do React e NestJS.  
- APIs para consulta de preços de combustível.  
- Serviços de envio de SMS como Twilio.  
- Explicação sobre o cálculo do lucro líquido.  
