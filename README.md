

### 1. Você pode cloná-lo no github executando o seguinte comando

`` ``
  $ git clone https://github.com/joabsonborges/javafullstack.git
`` ``

### 2. Importar projeto para o eclipse
`` ``
  Arquivo -> Importar -> Maven -> Projetos existentes do Maven -> Procurar projeto a partir do local clonado
`` ``
### 3. Clique com o botão direito do mouse no projeto no eclipse e depois em Maven -> Atualizar Projetos

### 4. Atualize as credenciais do banco de dados e outras configurações em application.properties disponíveis em src / main / java / resources

`` ``

spring.datasource.url = jdbc:mysql://localhost:3306/world?useSSL=false
spring.datasource.username = root
spring.datasource.password = root123


`` ``
### 5. Clique com o botão direito do mouse no arquivo FuncionarioApplication.java e execute como Java Application

### 6. Depois que o aplicativo de inicialização Sprint for iniciado com êxito,
	pode chamar os seguintes pontos de extremidade usando POSTMAN

### 7. Para obter a lista de funcionarios, chame o seguinte endpoint com GET Request
`` ``
  http: // localhost: 8080 /compania/funcionarios
`` ``
### 8.Para criar novo funcionario, use o seguinte URL com solicitação POST
`` ``
  http: // localhost: 8080 /compania/funcionarios
`` ``
`` ``
### define o tipo de conteúdo como no cabeçalho como `application / json`
### definir o corpo
`` ``
  {
    "nome": "Joao",
    "designacao": "gerente",
    "experiencia": "Senior",
  }

`` ``
### 9.Para obter um funcionario específico, use o seguinte URL com o tipo de solicitação `GET` 
`` ``
  http: // localhost: 8080 /compania/funcionarios/<id>
`` `` 
`` ``
### 10.Para atualizar o funcionario no banco de dados, use o seguinte URL com o tipo de solicitação `PUT` 
`` ``
http: // localhost: 8080 /compania/funcionarios/<id>
`` ``
`` ``
### define o tipo de conteúdo como no cabeçalho como `application / json`
### definir o corpo 

`` ``
  {
    "nome": "Joao",
    "designacao": "gerente",
    "experiencia": "Senior",
  }
`` ``
### 11.Para excluir um funcionario, use o seguinte URL com o tipo de solicitação `DELETE` 
`` ``
  http: // localhost: 8080 /compania/funcionarios/<id>
`` `` 
`` ``

### Nota - Substitua <id> pelo ID real