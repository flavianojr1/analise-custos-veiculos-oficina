# Análise de Dados de Oficina Mecânica

Este projeto realiza uma análise dos dados de ordens de serviço de uma oficina localizada em uma única cidade. O objetivo é obter uma visão geral dos veículos que aparecem com maior frequência, além de identificar os maiores valores relacionados a peças, serviços e totais.

## Estrutura do Projeto

- **ordens-de-servico-por-carro-2024.ipynb**  
  Notebook principal com todo o processo de leitura, tratamento, análise e exportação dos dados.

- **ordens-de-servico-por-carro-2024.csv**  
  Arquivo de dados original, tratado manualmente no Excel antes da análise.

- **ordens-de-servico-por-carro-2024-tratado.csv**  
  Arquivo exportado para uso no Power BI, com dados limpos e formatados.

## Principais Etapas

1. **Leitura e limpeza dos dados:**  
   Remoção de colunas desnecessárias e tratamento de valores monetários para o padrão americano.

2. **Transformação de colunas:**  
   Conversão de valores de moeda para `float` e ajuste de casas decimais.

3. **Filtragem de veículos menos frequentes:**  
   Exclusão de veículos que aparecem duas ou menos vezes para evitar viés nos gráficos.

4. **Criação da coluna Fabricante:**  
   Associação de cada modelo de veículo ao seu fabricante usando um dicionário.

5. **Ajuste de nomes redundantes:**  
   Remoção do nome do fabricante do campo "Veículo" quando necessário.

6. **Exportação para Power BI:**  
   Alteração do formato dos valores monetários para o padrão brasileiro e exportação do arquivo final.

## Como usar

1. Abra o notebook `ordens-de-servico-por-carro-2024.ipynb` no Jupyter ou VS Code.
2. Execute as células sequencialmente para realizar o tratamento e análise dos dados.
3. O arquivo final será gerado como `ordens-de-servico-por-carro-2024-tratado.csv`, pronto para importação no Power BI.

## Requisitos

- Python 3.8+
- Pandas

## Observações

- Os resultados refletem apenas a realidade da oficina analisada e podem conter vieses.
- O dicionário de fabricantes pode ser expandido conforme novos modelos sejam incluídos.

## Autor

Projeto criado por Flaviano Astolfo Junior.  
Contato: [flavianoastolfojunior@gmail.com]
