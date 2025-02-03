# Esquema Conceitual para Oficina Mecânica

Este projeto tem como objetivo modelar um esquema conceitual para um sistema de controle e gerenciamento de ordens de serviço em uma oficina mecânica. O sistema permite o registro de veículos, clientes, mecânicos e ordens de serviço, garantindo um fluxo estruturado para acompanhamento das manutenções e revisões realizadas.

## Entidades e Atributos

- **Cliente**
- **Veículo**
- **Equipe**
- **Mecânico**
- **Ordem de Serviço (OS)**
- **Serviço**
- **Peça**

## Relacionamentos

- Um cliente pode possuir vários veículos (1:N).

- Um veículo pode ter várias ordens de serviço (1:N).

- Uma ordem de serviço é atribuída a uma equipe (N:1).

- Uma equipe é composta por vários mecânicos (1:N).

- Um mecânico pode pertencer a várias equipes (N:M).

- Uma ordem de serviço pode envolver vários serviços (N:M).

- Uma ordem de serviço pode utilizar várias peças (N:M).


## Considerações Adicionais

- O valor total da OS é calculado somando o valor de todos os itens (serviços e peças) associados à OS.
- O status da OS pode ser "Em andamento", "Concluída", "Aguardando aprovação", etc.
- A especialidade do mecânico pode ser "Motor", "Suspensão", "Elétrica", etc.

## Diagrama Conceitual

O diagrama conceitual pode ser visualizado [aqui](./Oficina%20Mecânica.png).