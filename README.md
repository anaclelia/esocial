# eSocial

## Visão Geral

O Tribunal Superior do Trabalho está em uma fase avançada de desenvolvimento de uma solução para transmitir os dados
da vida funcional dos seus servidores para sistema eSocial do Governo Federal, atendendo às necessidades legais do
<a href="http://www.planalto.gov.br/ccivil_03/_ato2011-2014/2014/decreto/d8373.htm">Decreto N° 8.373, de 11 de Dezembro de 2014</a>.

Essa iniciativa converge na publicação desse trabalho como projeto Open Source (OSS), uma vez que entendemos que essa solução
pode ser reusada, trazendo economia de esforços em quaisquer entidades públicas ou privadas.

## Escopo

### O que esse software **faz**?

Esse pedaço da solução compreende:

- Recepção de ocorrências provenientes dos sistemas de origem, via API RESTful;
- Conversão dessas ocorrências em eventos do eSocial, no formato XML;
- Orquestração do envio dos eventos ao eSocial-GOV;
- Consulta do resultado do processamento dos eventos enviados; e
- Gerência dos detalhes de conexão com o eSocial-GOV (assinatura dos eventos, conexão com certificado, etc.).

### O que esse software **não faz**?

Não tratamos nesse projeto de:

- Extração e/ou transformação de dados dos sistemas finalísticos das organizações usuárias;
- Manipulação de qualquer forma que seja dos dados recebidos; e
- Validação semântica dos dados recebidos.

## Estado atual

Atualmente, o sistema já é capaz de receber dados de eventos de tabela, transmitir de forma automática
para o eSocial-GOV e exibir o resultado do processamento (sucesso ou mensagens de erro).

A priorização dos eventos a serem transmitidos foi feita com base na necessidade atual do TST e
demais órgãos da Justiça do Trabalho. No entanto, o projeto pode ser estendido para quaisquer tipos
de eventos especificados pelo eSocial-GOV.
