Estratégia de Trading com Stop Loss e Take Profit Dinâmicos
Este repositório contém um código de estratégia de trading automatizada, desenvolvido para plataformas de backtesting e execução de ordens em mercados financeiros. A estratégia implementa uma abordagem baseada no padrão 123, com o uso de médias móveis para filtragem de tendência e mecanismos de controle de risco como Stop Loss e Take Profit.

Principais Funcionalidades
Identificação da Estratégia 123:

Detecta padrões de reversão baseados em três pontos principais (fundo, máxima da correção e rompimento).
Condições de entrada baseadas na confirmação de rompimento e tendência das médias móveis.
Gestão de Risco:

Stop Loss Dinâmico: Ajustado automaticamente com base no lucro da posição aberta, começando com uma perda fixa inicial (por exemplo, R$ 30).
Take Profit: Definido para garantir o fechamento da posição em um lucro predeterminado.
Limite Diário de Perdas:

Bloqueia novas operações quando o limite de perda acumulada no dia é atingido, garantindo proteção contra perdas excessivas.
Cálculo de Médias Móveis:

Usa três médias móveis exponenciais (rápida, lenta e longa) para identificar a tendência do mercado e evitar entradas em mercados laterais.
Execução Automatizada:

Entradas e saídas são feitas por ordens condicionais (BuyStop, SellShortStop) e controles para fechamento de posições com base nos limites configurados.
Parâmetros Ajustáveis
offSet: Define o deslocamento em pontos para a execução de ordens.
stopLoss: Valor inicial do Stop Loss (dinamicamente ajustado durante a operação).
takeProfit: Valor do lucro alvo por contrato.
limiteDiario: Limite máximo de perda acumulada permitido por dia.
Requisitos
Plataforma de trading ou backtesting compatível com a linguagem utilizada.
Dados históricos para simulação e validação da estratégia.
Como Usar
Copie o código para a sua plataforma de trading ou ambiente de backtesting.
Configure os parâmetros de entrada conforme a sua necessidade.
Execute o backtest para validar a eficácia em diferentes condições de mercado.
Ajuste os valores de Stop Loss, Take Profit e Limite Diário para alinhar à sua gestão de risco.
