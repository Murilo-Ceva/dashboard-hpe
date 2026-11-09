# Dashboard HPE: follow-up da distribuição

Painel CEVA de follow-up das notas fiscais da HPE Automotores, no padrão visual do Portal Transit Time.

O site abre com a **visão cliente** da base de 09/11/2026 (365 notas), sem transportadora, frete ou e-mail. Para ver outra base, clique em **Carregar base** e escolha o CSV ou o CSV.gz da aba "Base por NF Oficial"; esse arquivo é lido só no seu navegador.

**Atenção:** este repositório é público. Os dados do `index.html` ficam visíveis para qualquer pessoa.

## O que o painel mostra

- Situação de cada nota: entregue no prazo, em trânsito no prazo, vencida sem entrega ou entregue com atraso. A situação vem da previsão original comparada com a data da entrega (dias corridos). Sem entrega, a previsão é comparada com a data do arquivo.
- OTD, vencidas e notas que vencem em até 2 dias, por transportadora, UF, região, modalidade e dealer.
- Gráficos que filtram uns aos outros (Ctrl + clique soma itens), detalhe por nota e CSV do recorte.

## Regras

- Não suba base, CSV, planilha, e-mail nem a visão interna (transportadora e frete): o repositório é público.
- O painel é gerado a partir do projeto `painel_hpe_v2` (template, `scripts/gerar_painel.py` e `scripts/verificar.py`). O `index.html` é a saída `saida/painel_cliente.html`; para o site sem dados, use `saida/publico/index.html`.
