# Qualificação do Doutorado - Mercado Artificial de Fundos Imobiliários

Este repositório contém o código-fonte e a documentação do experimento computacional apresentado na qualificação de doutorado de Gilberto Gil Passos, no Programa de Pós-Graduação em Informática da UFRJ. O trabalho investiga como a modelagem baseada em agentes (ABM) pode ser aplicada para simular um mercado artificial de fundos de investimento imobiliário (FIIs).

## Objetivo do Projeto

O objetivo principal é construir um ambiente de simulação que reproduza comportamentos realistas de um mercado de FIIs no Brasil, incorporando características heterogêneas dos agentes, expectativas macroeconômicas e microeconômicas e mecanismos de formação de preços via book de ofertas para a reprodução dos fatos estilizados do mercado real.

## Descrição do Experimento

O modelo implementado neste notebook simula o comportamento diário de investidores (individuais e institucionais) em um mercado de FIIs, considerando:

- **Agentes heterogêneos**: com diferentes níveis de literacia financeira, memória, perfil de risco e estratégias de decisão.

- **Ativos simulados**: cotas de fundos imobiliários que pagam dividendos mensais, influenciadas por variáveis macroeconômicas como inflação e taxa de juros.

- **Formação de preços**: baseada em um mecanismo de book de ofertas, em que as ordens são registradas e cruzadas a cada rodada da simulação.

- **Ambiente de incertezas**: inclui expectativas, notícias divulgadas pela mídia, comportamento coletivo emergente (sentimento de mercado) e a propagação desse sentimento entre os agentes.

- **Ciclo de simulação**: a cada período, agentes avaliam o mercado, atualizam expectativas, emitem ordens de compra ou venda e ajustam seus portfólios.

## Estrutura do Código

O notebook está dividido em células que estruturam o experimento nas seguintes etapas:

1. **Definição das classes principais:** `BancoCentral`, `Midia`, `Imoveis`, `FII`, `Investidor`, `Ordem`, `Transacao` e `Mercado`.

2. **Inicialização dos parâmetros da simulação:** Número de agentes, ativos, capital inicial, horizonte de simulação e modelagem do ambiente.

3. **Execução da simulação:** Etapas diárias com geração de ordens, cálculo de preços, distribuição de dividendos e coleta de dados.

4. **Visualização de resultados:** Gráficos de preços, retornos e comparação dos momentos das médias e fatos estilizados da série sintética gerada com as do IFIX.
