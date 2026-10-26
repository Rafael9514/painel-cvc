# Painel de Indicadores — CVC Corp (CVCB3)

Painel independente de indicadores financeiros da CVC Corp, elaborado a partir de documentos públicos de Relações com Investidores. **Não é publicação oficial da CVC Corp** e não constitui recomendação de investimento.

## O que o painel mostra

- Seletor de trimestres (4T25, 1T26 e 2T26; 3T26 e 4T26 aguardando divulgação)
- Resumo: receita líquida, EBITDA ajustado, lucro líquido e dívida líquida / EBITDA
- Índices de liquidez, rentabilidade e endividamento, com fórmula, comparativo e semáforo
- Gráficos de resultado, margens e composição da dívida
- Reservas confirmadas (base reportada e comparável)
- Demonstrações financeiras completas: balanço, DRE, DMPL e fluxo de caixa (Controladora e Consolidado)
- Conferência: testes de soma de todas as demonstrações e comparação entre valores calculados e divulgados
- Notas metodológicas e página do PDF de origem de cada número

## Fontes

Demonstrações Financeiras e Release de Resultados de cada trimestre, disponíveis na [Central de Resultados](https://www.cvccorp.com.br/ri/central-de-resultados/) do site de RI da CVC Corp.

## Arquivos

- `painel-cvc-2T26.html` — o painel (arquivo único, sem servidor; usa Chart.js 4.4.1 e a fonte Raleway via CDN)
- `vercel.json` — faz a raiz do site abrir o painel

## Como atualizar

Os dados ficam no objeto `DADOS.periodos`, no início do script. Cada trimestre é um bloco; os ainda não divulgados estão como `null`. Para liberar um trimestre, troque o `null` pelo bloco de dados com a mesma estrutura dos demais: o botão do trimestre e todos os cálculos são atualizados automaticamente.

## Autoria

© 2026 · APP desenvolvido por Rafael Miranda Feitosa | Controladoria | CVC Corp

Marca, logotipo e imagens pertencem à CVC Corp. Dados extraídos de documentos públicos de Relações com Investidores.
