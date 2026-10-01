Aqui tens o ficheiro **`README.md`** completo e formatado em Markdown, pronto para copiares e colares diretamente na raiz do teu repositório do GitHub.

---

```markdown
# 🐾 PetAgenda — Sistema de Agendamento e Gestão para Pet Shops

> Plataforma web simples e eficiente para a gestão de agendamentos e histórico de serviços em pet shops de pequeno e médio porte, oferecendo autonomia aos clientes e organização aos gestores.

```

---

## 📌 Sumário

* [Problema e Contexto](#-problema-e-contexto)
* [Proposta da Solução](#-proposta-da-solução)
* [Público-Alvo](#-público-alvo)
* [Levantamento e Elicitação de Requisitos](#-levantamento-e-elicitação-de-requisitos)
* [Especificação de Requisitos](#-especificação-de-requisitos)
* [Histórias de Usuário (User Stories)](#-histórias-de-usuário-user-stories)
* [Priorização e Escopo do MVP](#-priorização-e-escopo-do-mvp)
* [Planeamento da Primeira Sprint](#-planeamento-da-primeira-sprint)
* [Tecnologias Utilizadas](#-tecnologias-utilizadas)

---

## 🛑 Problema e Contexto

### Qual é o problema identificado?

Dificuldade na gestão de agendamentos, atrasos frequentes, esquecimento de horários por parte dos clientes e falta de histórico centralizado dos serviços prestados num Pet Shop.

### Quem enfrenta esse problema?

Tutores de pets (clientes) e proprietários/atendentes de pet shops de pequeno e médio porte.

### Como é resolvido atualmente?

O atendimento e agendamento são realizados manualmente via WhatsApp, mensagens de áudio, anotações em papel ou folhas do Excel.

### Dificuldades do processo atual:

* Perda de mensagens durante o horário de pico.
* Agendamentos duplicados no mesmo horário.
* Ausência de lembretes automáticos (gerando *no-show* / faltas).
* Tempo excessivo gasto pelo atendente a confirmar horários.
* Dificuldade em consultar o histórico de vacinas e banhos do pet.

---

## 💡 Proposta da Solução

O **PetAgenda** é uma plataforma web para gestão simplificada de agendamentos e histórico de serviços para Pet Shops. Ele permite que tutores agendem banhos, tosas e consultas veterinárias diretamente pelo navegador em tempo real, enquanto oferece aos donos do estabelecimento um painel centralizado para gestão de horários, controlo de serviços prestados e envio automatizado de confirmações.

* **Objetivo geral:** Otimizar a rotina operacional de pet shops e proporcionar autonomia aos clientes no agendamento de serviços.
* **Principais benefícios:** Redução de faltas nos agendamentos, economia de tempo no atendimento ao cliente, eliminação de conflitos de horário e maior organização do histórico dos pets.

---

## 🎯 Público-Alvo

* **Tutores de animais de estimação:** Necessitam de agendar serviços de forma rápida, em qualquer horário, sem esperar por resposta no WhatsApp.
* **Gestores/Atendentes de Pet Shops:** Necessitam de gerir a agenda da equipa, visualizar atendimentos do dia e evitar sobreposição de horários.

---

## 📋 Levantamento e Elicitação de Requisitos

* **Técnica escolhida:** Entrevista semiestruturada.
* **Justificativa:** Permite recolher dados qualitativos detalhados sobre as dores diárias do gestor e do cliente, mantendo flexibilidade para explorar respostas inesperadas.
* **Aplicação:** Conversas de 15 a 20 minutos com 3 donos de pet shops e 5 tutores de animais de estimação.

---

## ⚙️ Especificação de Requisitos

### Requisitos Funcionais (RF)

| ID | Descrição | Prioridade |
| --- | --- | --- |
| **RF-01** | Permitir o cadastro e autenticação de utilizadores (tutores e administradores). | Alta |
| **RF-02** | Permitir que o tutor cadastre um ou mais pets associados ao seu perfil. | Alta |
| **RF-03** | Permitir que o administrador cadastre os serviços oferecidos com preço e duração. | Alta |
| **RF-04** | Disponibilizar uma agenda interativa com dias e horários livres. | Alta |
| **RF-05** | Permitir que o tutor realize o agendamento escolhendo pet, serviço, data e horário. | Alta |
| **RF-06** | Permitir que o tutor consulte e cancele agendamentos pendentes. | Média |
| **RF-07** | Permitir que o administrador visualize a agenda diária e altere o status dos agendamentos. | Alta |
| **RF-08** | Enviar confirmação/lembrete de agendamento por e-mail para o cliente. | Baixa |

### Requisitos Não Funcionais (RNF)

| ID | Categoria | Métrica / Condição | Meta |
| --- | --- | --- | --- |
| **RNF-01** | Desempenho | Tempo de resposta na consulta de horários. | Em menos de 2 segundos. |
| **RNF-02** | Usabilidade | Interface de utilizador responsiva. | Adaptável a dispositivos móveis e desktops. |
| **RNF-03** | Segurança | Armazenamento de palavras-passe. | Criptografia via algoritmo hash seguro (`bcrypt`). |
| **RNF-04** | Disponibilidade | Medição de uptime da plataforma. | Mínimo de 99% no horário comercial. |

---

## 📖 Histórias de Usuário (User Stories)

* **US-01 — Cadastro de Pet:** Como tutor, quero cadastrar as informações do meu pet no sistema para que o estabelecimento saiba suas necessidades antes do atendimento.
* **US-02 — Consulta de Horários:** Como tutor, quero visualizar os dias e horários livres para que eu possa escolher o momento mais conveniente.
* **US-03 — Realização de Agendamento:** Como tutor, quero confirmar um agendamento para garantir o atendimento do meu pet no horário escolhido.
* **US-04 — Cancelamento:** Como tutor, quero cancelar um agendamento prévio para liberar o horário caso eu tenha um imprevisto.
* **US-05 — Gestão da Agenda (Admin):** Como administrador, quero visualizar a lista de atendimentos do dia para organizar o trabalho da equipa.
* **US-06 — Cadastro de Serviços (Admin):** Como administrador, quero cadastrar os serviços oferecidos com preços e durações para que os clientes saibam o valor e tempo necessário.

---

## 🏆 Priorização e Escopo do MVP

| Item / História | Descrição | Prioridade | Escopo |
| --- | --- | --- | --- |
| **US-01** | Cadastro de Pet | Alta | **MVP** |
| **US-02** | Consulta de Horários Disponíveis | Alta | **MVP** |
| **US-03** | Realização do Agendamento | Alta | **MVP** |
| **US-05** | Painel de Gestão da Agenda (Admin) | Alta | **MVP** |
| **US-06** | Cadastro de Serviços (Admin) | Alta | **MVP** |
| **US-04** | Cancelamento pelo Tutor | Média | Pós-MVP |
| **RF-08** | Envio de Lembretes por E-mail | Baixa | Pós-MVP |

> **Escopo do MVP (Produto Mínimo Viável):** Fluxo essencial onde o administrador cadastra serviços, o tutor cadastra o seu pet, escolhe um horário e realiza a marcação, e o administrador acompanha o agendamento pelo painel.

---

## 🚀 Planeamento da Primeira Sprint

* **Objetivo da Sprint:** Estruturar a base do projeto, o sistema de autenticação de utilizadores e o cadastro de entidades essenciais (serviços e pets).
* **Duração:** 2 semanas (10 dias úteis).

### Issues Selecionadas:

1. **`#1` - Configuração do Repositório e Módulo de Autenticação de Usuários** `[US-01]`
2. **`#2` - Cadastro e Gestão de Serviços** `[US-06]`
3. **`#3` - Cadastro de Pets Associados ao Perfil do Tutor** `[US-01]`

---

## 🛠️ Tecnologias Utilizadas

* **Front-end:** HTML5, CSS3, JavaScript (Layout Responsivo)
* **Back-end:** Node.js / Python / Java *(Ajuste conforme o seu stack)*
* **Base de Dados:** PostgreSQL / SQLite
* **Segurança:** Encriptação de palavras-passe com `bcrypt`
* **Gestão do Projeto:** GitHub (Issues & Projects)

---

### ✒️ Autor

Desenvolvido por **Alice Fugioka**.

```

```
