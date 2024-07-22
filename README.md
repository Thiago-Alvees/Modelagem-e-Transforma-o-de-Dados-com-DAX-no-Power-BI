# Neste projeto, o desafio consiste em transformar uma tabela única de amostra financeira em um modelo de dados baseado no esquema estrela, utilizando o Power BI e a linguagem DAX. O objetivo é criar tabelas dimensão e fato a partir da tabela original, de forma a organizar e otimizar a visualização e análise dos dados.

Processo de Construção do Diagrama:

# Criação das Tabelas Dimensão e Fato:

financials_backup: Tabela principal utilizada como backup e modo oculto.
D_Produtos: Contendo colunas como ID_produto, Produto, Média de Unidades Vendidas, Média e Mediana do Valor de Vendas, Valor Máximo e Mínimo de Venda.
D_Produtos_Detalhes: Incluindo ID_produtos, Discount Band, Sale Price, Units Sold, Manufactoring Price.
D_Descontos: Com ID_produto, Discount, Discount Band.
D_Detalhes: Para informações adicionais não contempladas nas outras tabelas dimensão.
D_Calendário: Criada usando a função DAX calendar().
F_Vendas: Tabela fato com colunas como SK_ID, ID_Produto, Produto, Units Sold, Sales Price, Discount, Band, Segment, Country, Sales, Profit, Date.

# Transformações e Funcionalidades DAX Utilizadas:

Calendar Function: Para criação da tabela de calendário.
Agregações: Cálculos de médias, medianas e valores máximos/mínimos.
Agrupamentos e Condicionais: Reorganização de colunas e criação de novas colunas baseadas em condições específicas, como o Índice de Produtos.

# Reorganização das Colunas:

As colunas foram reorganizadas para facilitar a leitura e análise dos dados, conforme a estrutura do esquema estrela.
