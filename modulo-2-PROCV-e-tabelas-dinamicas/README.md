# Módulo 2: Cruzamento de Dados, Funções Lógicas e Tabelas Dinâmicas

Este repositório documenta as soluções desenvolvidas no **Módulo 2** da capacitação da **Santander Open Academy**, utilizando a base de dados oficial de gestão educacional e comercial (`33. BD CURSOS-1.xlsx`).

O projeto foca na integração de matrizes de custo, aplicação de condicionais para apuração de resultados (lucro/despesa) e inteligência de busca.

## 🛠️ Competências Práticas Implementadas

Com base no escopo do módulo (conforme a ementa documentada na imagem `ementa-modulo-2.png`), as seguintes ferramentas intermediárias do Excel foram aplicadas na base:

### 1. Vinculação e Integração de Bases (`PROCV`)
* **Funções que vinculam planilhas:** Configuração da função `PROCV` para correlacionar o catálogo de cursos e os códigos identificadores (`CÓD CURSO`), automatizando o preenchimento de variáveis operacionais entre tabelas de apoio.
* **PROCV com Tabelas:** Aplicação de buscas estruturadas mapeando os registros de `PROFESSOR` e agentes do setor `COMERCIAL` para centralizar receitas e comissões.
* **PROCV VERDADEIRO (Correspondência Aproximada):** Implementação da busca por aproximação para classificação lógica por faixas de valores e precificação.

### 2. Inteligência Condicional e Apuração Financeira (Função `SE`)
* **Cálculo Automatizado de Indicadores:** Uso de condicionais para determinar o status de adimplência na coluna `PAGAMENTO CLIENTE` e validação de comissões em `PAGAMENTO COMERCIAL`.
* **Relação de Lucratividade:** Configuração de regras lógicas estruturadas para calcular dinamicamente a `DESPESA` total (soma do Importe do Professor com o Importe Comercial) e avaliar a margem líquida nas colunas de `LUCRO` e `%LUCRO`.

### 3. Matriz de Consolidação e Tabelas Dinâmicas
Extração de indicadores de performance através do comportamento dinâmico de filtros e agrupamentos na aba `CÁLCULOS TABELA`:
* **Áreas de Tabela Dinâmica e Funções Agregadas:** Estruturação de relatórios para cruzamento geográfico (`PAÍS` e `CIDADE`) e operacional (`TURNO CURSO`).
* **Métricas de Resumo Computadas:**
  * Consolidação do **TOTAL DESPESA** operacional do portfólio.
  * Aplicação de **Contagem** para monitorar o volume total de turmas ativas por `CURSO`.
  * Filtros avançados internos para **Contar o número de cursos com Importe do Professor menor que 500**.
  * **Soma** acumulada da carga horária na métrica de **SOMAR AS DURAÇÕES**.

---

## 📂 Arquivos no Repositório
* `33. BD CURSOS-1.xlsx`: Planilha com a base de dados integrada e as funções de auditoria e tabelas calculadas em pleno funcionamento.
