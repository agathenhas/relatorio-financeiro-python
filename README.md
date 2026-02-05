Relatório Financeiro em Python (CSV → TXT/CSV)

Projeto em Python que lê um arquivo CSV com lançamentos financeiros (receitas e despesas), valida os dados e gera um resumo financeiro automatizado.

O relatório inclui:

Total geral (saldo)

Total de receitas

Total de despesas

Quantidade de lançamentos pagos e pendentes

Resumo por categoria

Lista detalhada de lançamentos pendentes

Tecnologias Utilizadas

Python 3

Leitura e escrita de arquivos CSV

Execução via linha de comando (CLI)

Estrutura do Projeto

src/
main.py
dados/
dados_exemplo.csv
requirements.txt
README.md

Como Executar

Tenha Python 3 instalado

Abra o terminal na pasta do projeto

Execute o comando:

python src/main.py --arquivo dados/dados_exemplo.csv

Formato do CSV (Entrada)

O arquivo CSV deve conter as colunas:

data

descricao

categoria

valor (positivo = receita | negativo = despesa)

status (pago ou pendente)

Exemplo:

data,descricao,categoria,valor,status
2026-01-02,Pagamento cliente A,Receita,1500.00,pago
2026-01-03,Internet,Despesa,-120.50,pago
2026-01-08,Pagamento cliente B,Receita,2200.00,pendente

Saída Gerada

O script cria automaticamente uma pasta chamada output/ contendo:

Relatório em TXT

Resumo em CSV

Possíveis Melhorias

Exportar relatório em PDF

Ler arquivos Excel

Gerar gráficos financeiros

Autora

Agatha
Estudante de Tecnologia da Informação – ESAMC Santos

status (ex: pago, pendente)

Exemplo:

data,descricao,categoria,valor,status
2026-01-02,Pagamento cliente A,Receita,1500.00,pago
2026-01-03,Internet,Despesa,-120.50,pago
2026-01-08,Pagamento cliente B,Receita,2200.00,pendente

### Saída gerada

O script cria uma pasta output/ e gera:

relatorio_YYYYMMDD_HHMMSS.txt (relatório em texto)

resumo_YYYYMMDD_HHMMSS.csv (métricas em CSV)

✅ Ideias de melhorias (Roadmap)

Exportar relatório em PDF

Suporte a leitura de Excel (.xlsx)

Gráficos por categoria/mês

Interface simples (CLI mais amigável ou página web)

👩‍💻 Autora

Agatha — Estudante de TI (ESAMC Santos)
