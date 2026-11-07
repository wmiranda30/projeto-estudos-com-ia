# Guia de Recursos de Estudo e Atividades Práticas

Este documento reúne materiais recomendados para consulta (priorizando opções acessíveis e gratuitas) e fornece o roteiro detalhado para as atividades práticas de cada semana, garantindo a aplicação do método **20% teoria e 80% prática**.

---

## 🛠️ Recursos para os Compromissos Fixos

### 1. Inglês Técnico (30 minutos/dia)
* **Objetivo Diário:** 5 novas palavras, construção de frases contextuais e revisão espaçada.
* **Ferramentas Recomendadas:**
  - [Anki](https://apps.ankiweb.net/): Aplicativo gratuito para memorização e repetição espaçada (SRS).
  - [BBC Learning English](https://www.bbc.co.uk/learningenglish): Conteúdo modular e gratuito.
  - [W3Schools / MDN Web Docs](https://developer.mozilla.org/): Leitura de artigos e glossários em inglês para habituar-se com termos técnicos de dados e TI.

### 2. Faculdade (Análise e Desenvolvimento de Sistemas - 1h/dia)
* Priorizar os materiais didáticos e os exercícios das disciplinas vigentes da grade curricular da faculdade.

---

## 📊 Módulo 1: Excel (Semanas 1 a 4)

---

### Semana 1: Base e Organização

#### 📚 Materiais de Consulta Recomendados
* [Central de Ajuda e Treinamento do Microsoft Excel](https://support.microsoft.com/pt-br/excel): Guias rápidos oficiais sobre navegação, atalhos e tipos de dados.
* Cursos introdutórios gratuitos na plataforma Microsoft Learn ou tutoriais práticos no YouTube (foco em navegação básica e organização de células).

#### 🧪 Atividade Prática: Planilha de Despesas e Receitas
* **Desafio:** Construir do zero uma planilha pessoal de controle financeiro mensal.
* **Estrutura sugerida:**
  * Colunas: `Data`, `Descrição`, `Categoria` (ex.: Moradia, Alimentação, Faculdade, Lazer), `Tipo` (Receita ou Despesa), `Valor (R$)`, `Forma de Pagamento`.
  * Boas práticas:
    1. Aplicar formatação contábil (`R$ #.##0,00`) na coluna de valor.
    2. Utilizar formatação de data padronizada (`DD/MM/AAAA`).
    3. Destacar cabeçalhos com cor de preenchimento neutra e texto em negrito.
    4. Congelar a linha de cabeçalho para facilitar a rolagem.

---

### Semana 2: Fórmulas Essenciais

#### 📚 Materiais de Consulta Recomendados
* [Documentação da Função SOMA](https://support.microsoft.com/pt-br/office/fun%C3%A7%C3%A3o-soma-043e1c7d-7726-4e80-8f32-07b23e057f89)
* [Documentação da Função MÉDIA](https://support.microsoft.com/pt-br/office/fun%C3%A7%C3%A3o-m%C3%A9dia-047bac88-d466-426c-a32b-8f33732f1833)
* Artigos/vídeos sobre **Referências Relativas vs. Referências Absolutas** (uso do caractere `$`, ex.: `$A$1`).

#### 🧪 Atividade Prática: Planilha de Vendas Fictícias
* **Desafio:** Criar uma tabela com 15 a 20 registros de vendas de produtos fictícios e extrair métricas de negócio.
* **Estrutura sugerida:**
  * Colunas: `ID Pedido`, `Vendedor`, `Produto`, `Quantidade`, `Preço Unitário`, `Valor Total` (calculado via fórmula `= Quantidade * Preço Unitário`).
  * Cálculos a realizar (área de resumo/indicadores):
    * **Faturamento Total:** Utilizando `=SOMA(...)`.
    * **Ticket Médio de Venda:** Utilizando `=MÉDIA(...)`.
    * **Maior Venda Registrada:** Utilizando `=MÁXIMO(...)`.
    * **Menor Venda Registrada:** Utilizando `=MÍNIMO(...)`.
    * **Total de Transações:** Utilizando `=CONT.VALORES(...)`.

---

### Semana 3: Análise e Limpeza de Dados

#### 📚 Materiais de Consulta Recomendados
* [Visão Geral de Tabelas do Excel](https://support.microsoft.com/pt-br/office/vis%C3%A3o-geral-de-tabelas-do-excel-7ab0bb7d-3a9e-4b56-a3c9-6c94334e492c)
* [Documentação da Função SE](https://support.microsoft.com/pt-br/office/fun%C3%A7%C3%A3o-se-69aed7c9-4e8a-4755-a9bc-aa8bbff73be2)
* Tutoriais de classificação e aplicação de filtros avançados em listas de dados.

#### 🧪 Atividade Prática: Organização de Base de Clientes e Prioridades
* **Desafio:** Limpar e enriquecer uma base de 30 clientes fictícios, classificando-os de acordo com regras de negócio.
* **Estrutura sugerida:**
  * Colunas: `Código Cliente`, `Nome do Cliente`, `Estado (UF)`, `Segmento`, `Volume de Compras Acumulado (R$)`, `Dias sem Comprar`.
  * Etapas de limpeza e análise:
    1. Converter o intervalo de dados em **Tabela Oficial do Excel** (`Ctrl + Alt + T`).
    2. Identificar e remover linhas duplicadas ou inconsistentes.
    3. Criar uma nova coluna calculada chamada `Prioridade de Atendimento` usando a função `=SE()`:
       * *Regra de exemplo:* `=SE([@[Volume de Compras Acumulado (R$)]] >= 5000; "Alta Prioridade"; "Padrão")`.
    4. Aplicar filtros rápidos para exibir apenas clientes de "Alta Prioridade" de um determinado estado.

---

### Semana 4: Mini Projeto — Relatório de Vendas

#### 📚 Materiais de Consulta Recomendados
* [Criar um Gráfico no Excel do Início ao Fim](https://support.microsoft.com/pt-br/office/criar-um-gr%C3%A1fico-do-in%C3%ADcio-ao-fim-0baf399e-dd61-4e18-8a73-b3fd5d5680c2)
* Noções fundamentais de *Storytelling com Dados* (escolha correta entre gráficos de colunas para comparações, linhas para tendências temporais e barras horizontais para rankings).

#### 🧪 Atividade Prática: Relatório Executivo de Vendas
* **Desafio:** Construir um mini relatório (dashboard simples de uma página) integrando base de dados, cartões de indicadores e gráficos limpos.
* **Entregáveis do Projeto:**
  1. **Aba de Dados Brutos:** Tabela formatada e tratada com o histórico de vendas.
  2. **Aba de Relatório Executivo:**
     * **KPIs no topo:** Total Faturado, Total de Itens Vendidos e Média por Pedido.
     * **Gráfico 1 (Colunas ou Barras):** Comparativo de vendas por vendedor ou por categoria de produto.
     * **Gráfico 2 (Linhas):** Evolução das vendas ao longo das semanas do mês.
  3. **Autoavaliação de Conclusão:** Preencher a checklist do `cronograma.md` e validar se está apto a iniciar a etapa de **SQL**.

---

## 🚀 Próximas Etapas da Trilha (Visão Futura)

Conforme a sequência do plano de estudos, os recursos para as fases seguintes serão desbloqueados após a consolidação do módulo de Excel:

1. **SQL:** Banco de dados relacional (PostgreSQL/MySQL), consultas `SELECT`, filtros `WHERE`, agrupamentos `GROUP BY` e junções `JOIN`.
2. **Power BI:** Conexão com bases tratadas, modelagem de dados, medidas em DAX e dashboards interativos.
3. **Power Platform:** Automação de fluxos com Power Automate e aplicativos no-code com Power Apps.
4. **Python para Dados:** Manipulação de dados com Pandas e NumPy; visualizações com Matplotlib/Seaborn.
5. **Git/GitHub + Portfólio:** Controle de versão e publicação dos projetos práticos em repositórios públicos no GitHub.

