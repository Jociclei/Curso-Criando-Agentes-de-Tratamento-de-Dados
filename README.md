# dashboard-vendas-porsche

Dashboard interativa (HTML de arquivo único) sobre 100 vendas da Porsche.

**Dashboard publicada:** `https://SEU-USUARIO.github.io/dashboard-vendas-porsche/`  <!-- troque pelo seu link -->

## Perguntas de negócio e por quê
1. **Quais modelos concentram a receita?** Volume e faturamento não são a mesma coisa; a decisão por trás é onde focar estoque e venda.
2. **O ticket médio muda conforme o ano do modelo?** Mostra quanto o mercado paga por carros mais novos ou mais velhos.
3. **Como os clientes pagam?** Entender a participação de cada método na receita ajuda a priorizar condições comerciais.

Usei o **ano do modelo** (não a data da venda) porque 24 das 100 datas ficaram `INVALID` na sanitização.

## Tratamento da base
- Mantive apenas as colunas `*Sanitized` (modelo, ano, preço, pagamento, cidade, estado, status).
- Converti preço e ano para número e salvei como valores (`base_sanitizada.csv`).
- Criei a coluna `familia` (911, 718, Cayenne, Macan, Panamera, Taycan) a partir do início do nome do modelo.
- Removi nome do cliente e vendedor: não há dado pessoal no HTML.
- Datas `INVALID` ficaram de fora da análise.

## Prompt
Escreva aqui o prompt que você usou e o que mudou entre versões (v1 → final).

## Ferramenta
Indique se usou ChatGPT com Canvas, agente com skill, ou os dois. (Esta versão foi gerada com Claude.)

## Evidências
Adicione prints da tela e de um filtro aplicado (ex.: Família = Macan).
