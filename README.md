# Oferta e Demanda de aluguel de bicicletas da Capital Bikeshare 
Este repositório é destinado ao desenvolvimento do trabalho proposto durante a disciplina "Projeto Aplicado I" do curso de Ciência de Dados da Universidade Presbiteriana Mackenzie.

## Integrantes
- [Daniel Rodrigues da Silva](https://www.linkedin.com/in/danielrod147/)
- [Dianna Mayumi Santos Katayama Rodrigues](https://www.linkedin.com/in/dianna-katayama-016274216/)
- [inserir nomes]

## Objetivo
Desenvolvimento de um estudo prático sobre dados de utilização de serviços da empresa [Capital Bikeshare](https://capitalbikeshare.com), apresentando dois produtos, a saber: 
- Análise exploratória de dados; 
- Recomendação de locais para amplicação das estações de bicicletas, ou, maior frequência de redistribuição de bicicletas com base na demanda histórica de cada localidade.

### Sobre a Capital Bikeshare
A Capital Bikeshare é uma empresa de responsabilidade da Autoridade de Trânsito da Área Metropolitana de Washington (Metro DC) que visa facilitar a mobilidade de pessoas fornecendo bicicletas para locomoção por meio de planos e pacotes de serviços, visando menor utilização de veículos emissores de gases do efeito estufa, reduzindo a poluição e intensidade do trâncito.

## Base de dados
A base de dados utilizada está disponível em [Trip History Data](https://s3.amazonaws.com/capitalbikeshare-data/index.html), contendo dados sobre a utilização de bicicletas, desde tempo de viagem até destino final e tipo de consumidores.

Para fins didáticos, apenas o histórico de dados de Setembro/2022 a Fevereiro/2023 serão utilizados.

### Descrição das colunas contidas na base:

- **Duration** – Duração da viagem
- **Start Date** – Data e hora do início da viagem
- **End Date** – Data e hora do fim da viagem
- **Start Station** – Nome da estação de início da viagem
- **End Station** – Nome da estação de fim da viagem
- **Bike Number** – ID único da bicicleta utilizada na viagem
- **Member Type** – Indica se o utilizador é um membro registrado ('registered' - Membro anual, mensal ou de dias fixos), casual ('casual' - viagem única, passe de 5, 3 ou 1 dia)

### Termos de uso
A empresa responsável pelos dados garante total liberdade para utilização, modificação e compartilhamento dos dados, desde que o objetivo do uso não envolva atividades ilegais ou venda dos dados disponibilizados gratuitamente.

Para mais detalhes, acessar os [Termos de Uso](https://ride.capitalbikeshare.com/data-license-agreement) na íntegra.

## Cronograma
```mermaid
gantt
title Cronograma de Atividades - Parte 1
axisFormat %a - %d/%B

section 1ª Sem
Aquisição dos datasets da Capital Bikeshare:active, crit, s1a1, 2023-03-26, 7d
Entendimento dos dados: active, s1a2, 2023-03-26, 7d
Seleção de variáveis para análise: active, s1a3, 2023-03-26,7d

section 2ª Sem
Avaliação de medidas de centralidade: active, s2a1, after s1a3,7d 
Caracterização das distribuições de variáveis: active, s2a2, after s1a3, 7d 
Definição dos métodos de visualização: active, s2a3, after s1a3, 7d

section 3ª Sem
Correlação das variáveis: active, s3a1, after s2a3, 7d
Visualização das correlações geradas (mapa de calor):active, s3a2, after s2a3, 7d

section 4ª Sem
Análise de sazonalidade: active, s4a1, after s3a2, 7d
Visualização de histórico de demandas e coletas:active, s4a2, after s3a2, 7d
```
```mermaid
gantt
title Cronograma de Atividades - Parte 2
axisFormat %a - %d/%B

section 5ª Sem
Identificação e tratamento de outliers e dados: active, s5a1, 2023-04-23, 7d
Impactos da sazonalidade:active, s5a2, 2023-04-23, 7d
Deep dive na duração, rotas e localidades das viagens: active, s5a3, 2023-04-23, 7d

section 6ª Sem
Previsão de demanda das bicicletas: active, s6a1, after s5a3, 7d
Definir modelo de ML:active, s6a2, after s5a3, 7d
Validar erro do modelo: active, s6a3,after s5a3, 7d

section 7ª Sem
Avaliação de melhorias: active, s7a1, after s6a3, 7d
Comparativos com diferentes abordagens:active, s7a2, after s6a3, 7d

section 8ª Sem
Organização da apresentação de resultados: active, s8a1, after s7a2, 7d
Revisao:active, s8a2, after s7a2, 7d
Ensaio de apresentação:active, s8a3, after s7a2, 7d
```
