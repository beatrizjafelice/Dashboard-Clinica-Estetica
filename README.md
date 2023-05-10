# Dashboard para Clínica de Estética
Esse relatório foi produzido para uma clínica de estética e contém dados sobre (1) atendimentos e procedimentos realizados, (2) faturamento e (3) visão geral da base de clientes e classificação destes. O relatório apresenta a análise de diversos indicadores por período (pacientes atendidos, procedimentos realizados, faturamento, entre outros), além da classificação dos procedimentos segundo alguns desses critérios. A última página apresenta a classificação dos pacientes de acordo com regras estabelecidas pelo negócio, acompanhada de informações demográficas sobre a base de clientes.

### Visões:
#### Página 1 – Atendimentos
- Quantidade de agendamentos e procedimentos realizados, além de pacientes atendidos
- Análise dessas métricas por período (com opção de drill down por ano, trimestre, mês e dia)
- Filtros de parâmetro (agendamentos, procedimentos ou pacientes), data, tipo de procedimento, paciente e classificação do paciente
- Top 5 procedimentos por número de agendamentos, procedimentos e pacientes
- Número de novos pacientes e de pacientes repetidos por mês e ano
- Evolução do número de novos pacientes por ano (gráfico de cascata)

#### Página 2 – Financeiro
- Faturamento bruto e faturamento médio por procedimento, por hora e por paciente
- Análise dessas métricas por período (com opção de drill down por ano, trimestre, mês e dia)
- Filtros de data, tipo de procedimento, paciente e classificação do paciente
- Top 5 procedimentos por faturamento total e por faturamento/hora
- Histograma com a distribuição de pacientes por gasto médio mensal

#### Página 3 – Classificação
- Número de pacientes com classificação ouro, prata e bronze
- Filtros de data, classificação do paciente, paciente, tipo de procedimento, e cidade
- Tabela com faturamento, procedimentos agendados, cidade e classificação de cada paciente
- Gráfico com pacientes atendidos pela última vez há mais de 2 meses
- Top 5 cidades por quantidade de pacientes 
- Quantidade de pacientes por sexo 

### Tabelas:
- Análise Faturamento: tabela criada a partir de Field Parameters do Power BI, permitindo ao usuário filtrar o tipo de faturamento (bruto, por hora, por paciente e por procedimento) nas visões da página 2
- Análise Overview: tabela criada a partir de Field Parameters do Power BI, permitindo ao usuário filtrar a quantidade de agendamentos realizados, procedimentos feitos e de pacientes atendidos
- consultas: tabela fato com dados das consultas (data, horário, código do paciente, etc.)
- pacientes: tabela dimensão com dados de pacientes
- servicos: tabela dimensão com dados sobre os procedimentos oferecidos
- DIM_DATA: tabela calendário para filtrar as datas das consultas
- Distribuição de Gastos: tabela criada para o histograma de distribuição de gasto mensal, na página 2
