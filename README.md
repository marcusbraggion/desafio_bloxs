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

## 4.0. Solução

Utilizei Python, SQL e PowerBI para desenvolver a solução.

### 4.1. Coleta Dos Dados e Descrição dos Dados

Os dados foram coletados através de consultas a um Banco de Dados hospedado na nuvem utilizando Heroku.

<details>
<summary>Feature dos Dados Originais</summary>

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

### 4.3. Filtragem dos Dados

### 4.4. Analise Exploratória dos Dados

Verificação da distribuição das variáveis e validação de hipóteses. Aqui eu já entreguei o primeiro resultado para o negócio, que foram os insights.

### 4.5. Criação do Banco de Dados

### 4.6. Criação do Dashboard

Criei um dashboard com o Power BI para mostrar com visualização de dados os insights. O painel está disponível neste [link]).

Ele pode ser acessado em qualquer lugar com um smartphone, tablet ou desktop.

Também fiz um [vídeo] com minhas próprias análises.

## 5.0. Top Insights

H1

H2

H3

### Demais Insights

Disponível neste [video].

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
