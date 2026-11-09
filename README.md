# Dashboard HPE: follow-up da distribuição

Painel CEVA de follow-up das notas fiscais da HPE Automotores, no padrão visual do Portal Transit Time.

**Este repositório não guarda dados.** O site abre vazio. Clique em **Carregar base** e escolha o CSV ou o CSV.gz da aba "Base por NF Oficial". O arquivo é lido só no seu navegador; nada é enviado para a internet.

## O que o painel mostra

- Situação de cada nota: entregue no prazo, em trânsito no prazo, vencida sem entrega ou entregue com atraso. A situação vem da previsão original comparada com a data da entrega (dias corridos). Sem entrega, a previsão é comparada com a data do arquivo.
- OTD, vencidas e notas que vencem em até 2 dias, por transportadora, UF, região, modalidade e dealer.
- Gráficos que filtram uns aos outros (Ctrl + clique soma itens), detalhe por nota e CSV do recorte.

## Regras

- Não suba base, CSV, planilha nem e-mail para este repositório: ele é público.
- O painel é gerado a partir do projeto `painel_hpe_v2` (template, `scripts/gerar_painel.py` e `scripts/verificar.py`), com a saída `saida/publico/index.html`.
