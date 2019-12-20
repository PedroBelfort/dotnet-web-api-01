# dotnet-web-api-01
WEB-API ( REST ) desenvolvida em dotnet core com entity framework e sql server para manipular os atributos usuarioID, nome, 
senha e email da entidade "Usuário".


Siga os seguintes passos para executar a API


1 - Crie um banco de dados chamado "Usuarios" no SQL Server.

2 - Atualize o valor da string connection em appsettings.json.

3 - Execute migrações para criar as tabelas.

4 - Popule o banco de dados com algumas informações.

5 - Acesse a api por meio da rota https://localhost:5001/api/usuarios


Os seguintes métodos foram implementados


1 - GetAll() - http://localhost:5000/api/usuarios/

2 - GetById(long id) - http://localhost:5000/api/usuarios/{id}

3 - Create([FromBody]Usuario usuario) - Pode ser testado no postman enviando um objeto json no corpo da requisição.

4 - Update(long id,[FromBody] Usuario usuario) - Pode ser testado no postman enviando um objeto json no corpo da requisição. 
    obs: o atributo senha não pode ser alterado. 
	
5 - Delete(long id) - http://localhost:5000/api/usuarios/{id}




