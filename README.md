# project-azure-db

Esse repo tem como objetivo demonstrar um passo a passo para criar uma instância de banco de dados SQL na Azure.

Passo 1

Acessar o painel de gerenciamento Azure e na barra lateral selecionar 'Banco de dados SQL'.

Passo 2

Clicar em criar para adicionar novo banco de dados.
Nas configurações básicas é obrigatório informar grupo de recursos, nome do banco de dados e o servidor do banco de dados.

Para fins de testes, podemos criar um novo grupo e um novo servidor.
Para criar o grupo, informamos somente um nome.
Para criar o servidor de banco de dados, informamos o nome, a localização (adicionar mais próximo a área onde pretendemos disponibilizar o serviço por questão de menor custo e menor latencia),
no meu caso, selecionei 'South america Brazil', método de autenticação que podemos selecionar a opção 'Usar autenticação SQL' e definir um user admin e uma senha de acesso.

Passo 3

Acessar a guia 'Segurança' e na opção 'Habilitar o Microsoft Defender para SQL' selecionar 'Agora não'. Para fins de criar uma base de teste não é necessário adicionar esse recurso.

Passo 4

E por fim, acessar a guia 'Configurações adicionais' para selecionar o tipo de collate que será aplicado. No caso, vamos manter o padrão SQL_Latin1_General_CP1_CI_AS

CI (que não diferencia maiúsculas de minúsculas)
AS (que diferencia acentuação)

Fonte: https://learn.microsoft.com/pt-br/sql/t-sql/statements/collations?view=sql-server-ver17

