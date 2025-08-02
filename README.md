# Challenge-Telecom-X

# Introdução
O objetivo deste projeto é analisar os dados de clientes de uma empresa de telecomunicações com foco em entender o fenômeno da evasão de clientes, também chamado de churn.
Essa análise é essencial para identificar padrões de comportamento que levam clientes a cancelar seus serviços e, a partir disso, propor estratégias para retenção.

A evasão representa perdas financeiras e indica possíveis falhas no atendimento, nos planos oferecidos ou na experiência do usuário.

# Limpeza e Tratamento de Dados
Para tornar os dados adequados à análise, foram realizados os seguintes passos:

-Importação dos dados JSON via API.

-Renomeação de colunas para nomes mais legíveis e em português.

-Conversão de tipos de dados, como transformar colunas de valores em float ou int, quando necessário.

-Tratamento de valores ausentes (NaN) com pd.to_numeric(..., errors='coerce') e eliminação ou imputação quando necessário.

-Mapeamento de variáveis categóricas como evasão (Evadiu = 1, Permaneceu = 0).

-Criação de colunas auxiliares, como tempo de contrato, tipo de pagamento, entre outras.

# Análise Exploratória de Dados (EDA)

Foi analisada a proporção de clientes que evadiram e os que permaneceram. Gráficos de barras mostraram a presença significativa de evasão em determinadas categorias.

1 - Evasão por variáveis categóricas

*Gênero

*Tipo de contrato

*Método de pagamento

2 - Evasão por variáveis numéricas

*Tempo de permanência (tenure)

*Total gasto

# Conclusões e Insights

Conclusões Gerais da Análise de Evasão de Clientes (Churn)

1 - Gênero:

*Apesar da quantidade de clientes homens ser ligeiramente superior, mulheres apresentaram uma taxa de evasão levemente maior.

*A diferença, no entanto, é quase imperceptível, indicando que o gênero não é um fator decisivo de evasão, mas ainda assim pode ser considerado em estratégias personalizadas.

2 - Tipo de Contrato:

*O tipo de contrato mensal é o mais popular entre os clientes.

*No entanto, também é o que apresenta maior taxa de evasão, tanto em números absolutos quanto percentuais.

*Contratos anuais e bienais possuem uma taxa de evasão muito menor, com o bienal sendo praticamente nulo em evasão.

3 - Método de Pagamento:

*A distribuição entre métodos de pagamento é relativamente equilibrada.

*No entanto, clientes que usam “cheque eletrônico (electronic check)” têm uma taxa de evasão bem superior aos demais métodos, como cartão de crédito e débito automático.

4 - Tempo de Contrato (Meses):

*Clientes com menos de 10 meses de contrato concentram a maior taxa de evasão.

*A taxa cai drasticamente a partir de 20 meses, e clientes com mais de 60 meses dificilmente evadem, indicando forte fidelização com o tempo.

5 - Gasto Total:

*Clientes que não evadiram tendem a gastar muito mais ao longo do tempo.

*A mediana do gasto entre os que permanecem é significativamente mais alta.

*Clientes que evadem geralmente gastam pouco antes de sair — possivelmente por evadirem logo no início do relacionamento com a empresa.

# Sugestões com Base nas Conclusões

1 - Fortalecer Programas de Retenção nos Primeiros Meses:

*Criar campanhas de onboarding mais eficazes para os primeiros 6 meses.

*Oferecer bônus ou benefícios progressivos nos primeiros meses para estimular permanência até o cliente alcançar o “ponto de fidelização”.

2 - Incentivar Contratos de Longo Prazo:

*Oferecer descontos, vantagens ou brindes para migração de contratos mensais para anuais ou bienais.

*Demonstrar claramente os benefícios financeiros e de estabilidade dos planos longos.

3 - Monitorar Clientes com Pagamento via Cheque Eletrônico:

*Aplicar ações específicas para clientes com esse método de pagamento, como:

*Migrar para débito automático ou cartão de crédito.

*Avaliar se esse método está associado a maior inadimplência ou menor engajamento.

4 - Segmentar Ofertas por Perfil de Gasto:

*Clientes que gastam mais tendem a ser mais fiéis — considere oferecer planos personalizados, exclusivos ou com recompensas para esse público.

*Para os de menor gasto, estudar se há barreiras de entrada, como complexidade de serviços ou custo-benefício percebido.
