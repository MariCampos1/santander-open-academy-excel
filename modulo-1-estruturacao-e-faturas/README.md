# Módulo 1: Estruturação, Tabelas de Dados e Auditoria

Este projeto prático consistiu na aplicação de regras de negócio, estruturação e auditoria de dados operacionais utilizando a base de faturamento de clientes e fornecedores (`09. BD FATURAS`).

## 🛠️ Desafio Técnico Executado

A partir das diretrizes estabelecidas na capacitação, o projeto foi solucionado seguindo rigorosamente as seguintes etapas:

1. **Estruturação Matriz:** O intervalo bruto de dados foi convertido em uma tabela estruturada nativa para garantir integridade e automação.
2. **Nomenclatura Padrão:** A tabela foi formalmente nomeada como `T_FATURAS`.
3. **Classificação Multinível:** Aplicação de ordenação crescente combinada baseada primeiro na coluna **DESCRIÇÃO** e, consecutivamente, na coluna **IMPORTE CLIENTE**.
4. **Configuração de Métricas (Linha de Totais):** Ativação e parametrização de funções agregadas específicas para auditoria gerencial instantânea:
   * **NÚMERO FATURA CLIENTE:** Configurado para **Contagem** (volume de faturas).
   * **IMPORTE CLIENTE:** Configurado para **Soma** (receita bruta total).
   * **IMPORTE FORNECEDOR:** Configurado para **Soma** (custo operacional total).
5. **Painel Interativo:** Inclusão de botões de segmentação de dados (Slicers) para as colunas **PROVÍNCIA** e **TIPO**.
6. **Simulação de Auditoria e Filtro Avançado:** Extração de dados aplicando múltiplos critérios simultâneos para tomada de decisão:
   * Filtro Geográfico: Apenas províncias de **MADRI** e **BARCELONA**.
   * Filtro Temporal: Apenas registros contidos nos **primeiros 4 meses (Janeiro a Abril) de 2019 e 2020**.
   * Filtro de Categoria e Valor: Restrito ao **TIPO INTERNO** com **IMPORTE CLIENTE MAIOR QUE 1000**.
   * Consulta e validação imediata do resultado através do comportamento dinâmico da linha de totais.
7. **Homologação e Entrega da Planilha:** Para encerramento e entrega limpa do projeto, foram removidos todos os filtros aplicados, a linha de totais foi ocultada e a segmentação do campo **PROVÍNCIA** foi removida, mantendo a planilha pronta para o próximo operador.
