# NLW Unite Java - Pass.in

## Sobre o Projeto

O **Pass.in** é uma aplicação de **gestão de participantes em eventos presenciais**. Permite que organizadores criem eventos, abram páginas de inscrição pública, emitam credenciais para check-in e realizem o controle de entrada utilizando um sistema de scan de credenciais.

## Requisitos

### Funcionais

- Organizador pode cadastrar um evento e visualizar seus dados.
- Organizador pode visualizar a lista de participantes inscritos em um evento.
- Participante pode se inscrever em um evento, visualizar seu crachá de inscrição e realizar check-in no evento.

### Regras de Negócio

- Participante só pode se inscrever uma vez em um evento.
- Participante só pode se inscrever em eventos com vagas disponíveis.
- Participante só pode fazer check-in uma vez em um evento.

### Não Funcionais

- Check-in no evento realizado através de um QRCode.

## Criando o Projeto

- [x]  Criar projeto usando Spring Initializr com as dependências necessárias.
- [x]  Configurar banco de dados na aplicação com HSQLDB.
- [x]  Criar migrations para criação das tabelas.
- [x]  Criar entidades para representar os dados: Event, Attendee, Check-in.
- [x]  Criar repositories para cada entidade.
- [x]  Criar controllers para os endpoints `/events` e `/attendees`.

## AULA 2 - Funcionalidade do Organizador

### Funcionalidades Implementadas

- Organizador pode cadastrar um novo evento e visualizar seus dados.
- Organizador pode visualizar a lista de participantes inscritos em um evento.

## AULA 3 - Funcionalidade do Participante

### Funcionalidades Implementadas

- Participante pode se inscrever em um evento, visualizar seu crachá de inscrição e realizar check-in no evento.
- Restrições de negócio implementadas: inscrição única por participante, inscrição em eventos com vagas disponíveis e check-in único por participante.

## Observação

- O retorno do crachá inclui o nome, e-mail, URL do check-in e título do evento.
- Implementação de tratamento de exceções para lidar com situações inesperadas.
