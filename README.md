# Projeto de Análise de Dados com Azure e Power BI
## Descrição do Projeto
Este projeto envolve a implementação e análise de um banco de dados utilizando a Azure e o Power BI. O objetivo é criar um banco de dados que armazene informações de funcionários e projetos, e realizar análises detalhadas sobre os dados utilizando o Power BI. As principais análises incluem:

 - Horas Trabalhadas em Projetos: Visualização das horas trabalhadas pelos funcionários em diferentes projetos.
 - Distribuição Salarial: Análise da distribuição de salários dos funcionários.
 - Proporção de Funcionários por Sexo: Representação da proporção de funcionários do sexo masculino e feminino.
 - Distribuição Salarial por Localização: Análise da distribuição salarial dos funcionários com base em suas localizações.
## Implementação do Banco de Dados
### Ambiente
O banco de dados foi implementado na Azure SQL Database, uma solução gerenciada de banco de dados na nuvem que oferece alta disponibilidade, segurança e escalabilidade.

### Estrutura do Banco de Dados
O banco de dados inclui as seguintes tabelas principais:

1. department: Armazena informações sobre os departamentos da empresa.

 - Dname: Nome do departamento
 - Dnumber: Número do departamento (chave primária)
 - Mgr_ssn: Número da seguridade social do gerente (chave estrangeira)
 - Mgr_start_date: Data de início do gerente
 - Dept_create_date: Data de criação do departamento
   
2. employee: Armazena informações sobre os funcionários.

 - Fname: Primeiro nome
 - Minit: Inicial do meio
 - Lname: Sobrenome
 - Ssn: Número da seguridade social (chave primária)
 - Bdate: Data de nascimento
 - Address: Endereço
 - Sex: Sexo
 - Salary: Salário
 - Super_ssn: Número da seguridade social do supervisor (chave estrangeira)
 - Dno: Número do departamento (chave estrangeira)

3. project: Armazena informações sobre os projetos.

 - pname: Nome do projeto
 - pnumber: Número do projeto (chave primária)
 - plocation: Localização do projeto
 - dnum: Número do departamento associado ao projeto (chave estrangeira)
 - 
4. works_on: Relaciona funcionários aos projetos e as horas trabalhadas.

 - essn: Número da seguridade social do funcionário (chave estrangeira)
 - pno: Número do projeto (chave estrangeira)
 - hours: Horas trabalhadas no projeto
   
 ## Análise de Dados no Power BI
Com os dados importados do banco de dados, foram realizadas as seguintes análises no Power BI:

1. Horas Trabalhadas em Projetos:

Gráfico de Barras: Exibe a quantidade total de horas trabalhadas pelos funcionários em cada projeto.
Detalhamento: Permite visualizar quais funcionários estão alocados em cada projeto e o número de horas trabalhadas.
Distribuição Salarial:

2. Gráfico de Pizza: Mostra a distribuição dos salários dos funcionários.
Detalhamento: Permite identificar a proporção de funcionários em diferentes faixas salariais.
Proporção de Funcionários por Sexo:

3. Gráfico de Pizza: Representa a proporção de funcionários do sexo masculino e feminino.
Detalhamento: Permite visualizar a distribuição de funcionários entre os sexos.
Distribuição Salarial por Localização:

4. Mapa: Exibe a distribuição salarial dos funcionários com base em suas localizações.
Detalhamento: Permite visualizar as diferenças salariais em diferentes áreas geográficas.
## Como Executar o Projeto

1. Importar Dados:
   
 - Conecte o Power BI à sua instância Azure SQL Database para importar os dados das tabelas department, employee, project e works_on.
2. Criar Relatórios:

 - Utilize as visualizações mencionadas para criar relatórios detalhados sobre horas trabalhadas, distribuição salarial, proporção de sexo e distribuição por localização.
3. Personalizar e Analisar:

 - Ajuste e personalize os gráficos e mapas conforme necessário para obter insights mais detalhados.
## Conclusão
Este projeto demonstra a integração eficaz entre o banco de dados Azure SQL e o Power BI para realizar análises profundas sobre os dados de funcionários e projetos. A análise dos dados fornece insights valiosos para a tomada de decisões e a gestão eficiente da equipe e dos recursos.
