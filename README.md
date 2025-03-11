# Connectopia

## 📌 Introdução  

Bem-vindo ao **Connectopia**, um sistema de fórum acadêmico projetado para promover a troca de conhecimento entre estudantes e professores. A plataforma permite que estudantes publiquem perguntas sobre diversos assuntos, enquanto outros estudantes e professores podem interagir fornecendo respostas.  

O projeto foi desenvolvido utilizando os princípios de **Domain-driven Design (DDD)** e **Clean Architecture**, garantindo modularidade e escalabilidade.  

---

## 🔹 O que é o Connectopia?  

O **Connectopia** é uma plataforma robusta que organiza as interações dentro de um fórum acadêmico de forma estruturada e eficiente.  

O sistema é dividido em dois **domínios principais**:  

- **Fórum:** Responsável pelo gerenciamento das perguntas e respostas.  
- **Notificação:** Responsável por enviar alertas e manter os usuários informados sobre interações relevantes.  

Essa separação permite gerenciar discussões de forma independente da camada de comunicação, garantindo flexibilidade na evolução da aplicação.  

---

## ⚙️ Como Funciona?  

### 📝 Publicação de Perguntas  
Os estudantes podem criar novas perguntas no fórum, categorizando os tópicos para facilitar a organização das discussões. Cada pergunta possui um título e uma descrição detalhada do problema, ajudando na busca por soluções.  

### 💬 Respostas e Interações  
Outros usuários podem responder às perguntas, criando discussões produtivas dentro da plataforma.  
As respostas podem ser **votadas**, destacando as mais relevantes e garantindo que o melhor conteúdo fique visível para todos.  

### 🔔 Gerenciamento de Notificações  
O sistema conta com um **domínio específico para notificações**, garantindo que os usuários sejam informados sobre novas respostas ou interações em suas perguntas. Isso melhora a experiência do usuário, mantendo-o atualizado sobre as discussões que participa.  

### 🏗️ Arquitetura Baseada em DDD e Clean Architecture  
A plataforma é estruturada seguindo os princípios de **Domain-driven Design (DDD)**, separando os conceitos de Fórum e Notificação em **domínios distintos**.  
Isso permite **maior organização, escalabilidade e facilidade de manutenção** do código.  

### 📦 Camada de Aplicação  
A camada de aplicação contém os **casos de uso e repositórios** necessários para interagir com o domínio.  
As regras de negócio são encapsuladas em casos de uso específicos, garantindo que cada ação siga as diretrizes do sistema.  

### 🏛️ Camada de Domínio e Enterprise  
- O domínio do **Fórum** possui entidades como `Pergunta` e `Resposta`, além de eventos que podem acionar notificações.  
- O domínio de **Notificação** gerencia alertas e mensagens para os usuários, garantindo que sejam informados sobre interações relevantes.  

### 🔄 Sistema de Eventos e Assinantes  
A arquitetura conta com um **sistema de eventos dentro do domínio de Notificação**, permitindo que novos eventos **disparem ações específicas**, como alertar um usuário quando sua pergunta for respondida.  

### 💡 Desenvolvimento com TypeScript  
A aplicação foi construída em **TypeScript**, garantindo **maior segurança no código** e facilitando sua escalabilidade.  

---

## 🚀 Tecnologias Utilizadas  

- **Linguagem:** TypeScript  
- **Framework:** Nestjs  
- **Testes:** Vitest  
- **Arquitetura:** Domain-driven Design (DDD) + Clean Architecture  

---




<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>
