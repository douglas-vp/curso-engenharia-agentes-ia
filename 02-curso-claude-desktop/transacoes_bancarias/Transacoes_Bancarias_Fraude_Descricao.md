### Análise Detalhada do Comportamento Transacional e Detecção de Anomalias

![[Pasted image 20260323134145.png]]

## Sobre o Dataset

Este conjunto de dados oferece uma visão detalhada do comportamento transacional e dos padrões de atividade financeira. Ele contém **2.512 amostras** de dados de transações, cobrindo diversos atributos da transação, características demográficas do cliente e padrões de uso. Cada entrada fornece informações completas sobre o comportamento da transação, possibilitando análises para **segurança financeira** e **aplicações de detecção de fraude**.

### Principais Características:
- **TransactionID**: Identificador alfanumérico único para cada transação.
- **AccountID**: Identificador único da conta, com múltiplas transações por conta.
- **TransactionAmount**: Valor monetário de cada transação, variando de pequenas despesas do dia a dia até compras maiores.
- **TransactionDate**: Data e hora (timestamp) da transação.
- **TransactionType**: Campo categórico indicando transações **'Credit'** ou **'Debit'** (crédito ou débito).
- **Location**: Localização geográfica da transação, representada por nomes de cidades dos EUA.
- **DeviceID**: Identificador alfanumérico do dispositivo usado para realizar a transação.
- **IP Address**: Endereço IPv4 associado à transação, com alterações ocasionais para algumas contas.
- **MerchantID**: Identificador único de comerciantes/estabelecimentos, mostrando comerciantes preferidos e outliers (fora do padrão) para cada conta.
- **AccountBalance**: Saldo da conta após a transação, com correlações lógicas baseadas no tipo de transação e no valor.
- **PreviousTransactionDate**: Timestamp da última transação da conta, ajudando no cálculo da frequência de transações.
- **Channel**: Canal pelo qual a transação foi realizada (por exemplo, **Online**, **ATM**, **Branch**).
- **CustomerAge**: Idade do titular da conta, com agrupamentos lógicos com base em ocupação.
- **CustomerOccupation**: Profissão do titular da conta (por exemplo, **Doctor**, **Engineer**, **Student**, **Retired**), refletindo padrões de renda.
- **TransactionDuration**: Duração da transação em segundos, variando conforme o tipo de transação.
- **LoginAttempts**: Número de tentativas de login antes da transação; valores mais altos podem indicar possíveis anomalias.

## Finalidade do Dataset

Este conjunto de dados é ideal para cientistas de dados, analistas financeiros e pesquisadores que desejam analisar padrões transacionais, detectar fraudes e construir modelos preditivos para aumentar a segurança financeira.
