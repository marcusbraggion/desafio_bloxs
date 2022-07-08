# Desafio Bloxs - Insights

<img src=""/>

## 1.0. Contexto

A Bloxs é um ecossistema de acesso ao Mercado de Capitais, que conecta empresas com investidores de todo o mundo, democratizando os Ativos Alternativos!

## 2.0. Sobre o desafio

Sua missão é criar uma análise de dados, utilizando um dataset em SQL que será disponibilizado ao final deste documento, que é referente a dados de usuários fictícios de uma plataforma de investimento, que realizaram aportes em determinados produtos de investimento. A ideia é criar um dashboard com as análises destes dados, utilizando gráficos, tabelas e o que achar necessário. Para isso foi desenvolvido:
* Dashboard com Power BI;
* Banco de Dados com as propriedades recomendadas;
* Insights geradas pela validação das hipoteses.

## 3.0 Business Assumptions

![diagrama](https://user-images.githubusercontent.com/97288194/177666994-f9699595-b57a-4d21-95a8-a98466a50e8c.png)

## 4.0. Solução

Utilizei um framework de projetos de Ciência de Dados (CRISP-DM) para desenvolver a solução do Desafio, por ser uma abordagem cíclica e de etapas definidas, eu pude em poucos dias desenvolver os entregáveis gerando valor para o negócio com o menor esforço-tempo possível, permitindo que a cada ciclo temos mais know-how do problema/projeto para decidir se devemos continuar ou pivotar a solução.

Além disso utilizei Python, SQL e PowerBI para desenvolver os entregáveis. Com os passos abaixo:

### 4.1. Coleta Dos Dados e Descrição dos Dados

![pipeline](https://user-images.githubusercontent.com/97288194/177668403-9b9717e4-1c26-42d2-ada2-34385c51e058.png)

Os dados foram cedidos através de um arquivo .sql com estrutura e dados de um database MySQL de dados de investidores ficticios. Para entregar uma solução mais completa possível, decidi subir esse banco em uma aplicação na nuvem utilizando Heroku, para isso, realizei a migração do banco para um database PostgreSQL.

<details>
<summary>Dicionario dos Dados Originais</summary>

investor (Dados do Investidor)

id (chave primária)

date_created (data de criação do registro)

birth (data de nascimento)

marital_status (estado civil)

gender (gênero, sendo 1 = masculino, 2 = feminino, 3 = outros)

investor_type (tipo do investidor, podendo ser pf ou pj)

nationality (nacionalidade)

channel (canal de aquisição do usuário)

investor_work (Dados profissionais do investidor)

id (chave primária)

date_created (data de criação do registro)

investor (chave estrangeira para a tabela investor)

office (cargo)

profession (profissão)

investor_address (Dados de endereço do investidor)

id (chave primária)

date_created (data de criação do registro)

investor (chave estrangeira para a tabela investor)

country (país)

state (estado)

investor_company (Dados da empresa, caso investidor seja Pessoa Jurídica)

id (chave primária)

date_created (data de criação do registro)

investor (chave estrangeira para a tabela investor)

constitution_date (data de fundação da empresa)

company_type (tipo da empresa, se é ME, SA, MEI…)

country (Países)

id (chave primária)

date_created (data de criação do registro)

name (nome do país)

investment (Investimento em um determinado produto)

id (chave primária)

date_created (data de criação do registro)

investor (chave estrangeira para a tabela investor)

project (chave estrangeira para a tabela project)

anonymous (se quer ser anônimo ou não no investimento)

value (valor investido)

project (Produto de Investimento)

id (chave primária)

date_created (data de criação do produto)

date_open (data de abertura da oferta do produto de investimento)

validity (prazo final para que produto esteja disponível para investimento)

target (valor alvo mínimo a ser captado)

value (valor alvo máximo a ser captado)

closed (data em que a oferta foi encerrada)

project_category (chave estrangeira para a tabela project_category)

modality (modalidade do investimento, sendo: 1 = Debt, 2 = Equity)

project_category (categoria do produto de investimento)

id (chave primária)

date_created (data de criação da categoria)

name (Nome da categoria)

</details>

### 4.2. Feature Engineering

Aqui é onde eu derivei algumas informações de campos já existentes, criando novos campos, adicionando informação ao conjunto de dados, como: dia, mês, ano, semana do ano.

### 4.3. Filtragem dos Dados

### 4.4. Analise Exploratória dos Dados

Verificação da distribuição das variáveis ​​e validação de hipóteses. Aqui eu já entreguei o primeiro resultado para o negócio, que foram os insights.

### 4.5. Criação do Dashboard

Criei um dashboard com o Power BI para mostrar com visualização de dados os insights. O painel está disponível neste [link].

Ele pode ser acessado em qualquer lugar com um smartphone, tablet ou desktop.

Também fiz um [vídeo] com minhas próprias análises.

## 5.0. Top Insights

### Produtos de Investimentos

**Insight 1.** Agronegócio é a operação mais realizada, seguido por Energia e Comercial.

**Insight 2.** Equity é a modalidade de investimento mais operacionalizada.

**Insight 3.** A média de aporte realizado está na faixa de 4000 mil reais.

**Insight 4.** Google é o canal de aquisição de usuários mais efetivo, seguindo pela Instagram e depois a Indicação.

**Insight 5.** Pessoas Físicas representam os usuários majoritariamente.

**Insight 6.** Apesar da presença do negócio em outros países, Brasil é o pais com maior presença de usuários

### Demais Insights

Disponivel neste [video].

## 6.0. Resultados

## 7.0. Próximos Passos

* Crie um modelo de Machine Learning para prever o preço de retorno por projeto com base nos dados históricos.
* Coletar feedbacks do painéis e implementar melhorias.

## 8.0. Ferramentas Utilizadas

* Python
* Power BI
* Postgres
* Heroku

# Referencias
