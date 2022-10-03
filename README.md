# MYSQL-COM-DJANGO---TUTORIAL
O objetivo desse tutorial é demostrar de forma simples como fazer a integração do Banco de Dados MySql com o Framework Django.

Antes de começar mantenha o Django e o Poetry(se estiver utilizando) na versão mais atualizada.

# MYSQL-COM-DJANGO---Instalando a Biblioteca do MySql no VSCode.
Utilize o seguinte comando para instalar a biblioteca mysqlclient ou o comando para instalação no linux. 

![2](https://user-images.githubusercontent.com/107952878/193669289-055716c9-b500-4440-969b-0e90cc01e8fe.JPG)

# MYSQL-COM-DJANGO---Configurando o banco de Dados no Django.
Após a instalação da biblioteca mysqlclient é necessário fazer a configuração do Banco de Dados Mysql no arquivo SETTINGS.PY. 
No comando “NAME” coloque o nome do banco do seu projeto.
A senha padrão é root, porém se o banco de dados estiver configurado com outro usuário ou outra senha configure conforme a autenticação da máquina que está utilizando.

![3](https://user-images.githubusercontent.com/107952878/193669315-2619edf7-4980-43fb-b973-0f8378ebe9c2.JPG)

# MYSQL-COM-DJANGO---Criando o Banco de Dados. 
Após a configuração do arquivo settings.py , precisamos criar o banco de dados conforme o exemplo abaixo:

Não é necessário criar as tabelas do Banco de Dados , cria apenas o Banco de dados do seu projeto conforme a configuração que fez no arquivo settings.py.

A tabelas serão criadas pelo Django posteriormente.

![8](https://user-images.githubusercontent.com/107952878/193669446-cbfaa39a-610d-4527-a1cc-f170a19279fc.JPG)


# MYSQL-COM-DJANGO---Criando as Classes. 

Agora é o momento de criar todas as classes do seu projeto no arquivo models.py ,  seus atributos e os relacionamentos entre as classes conforme o exemplo abaixo.

![4](https://user-images.githubusercontent.com/107952878/193702722-3e5385eb-dc3d-4be4-97bc-d39ac939a097.JPG)

# MYSQL-COM-DJANGO--- Executando as migrações das classes;
Após a criação das classes e relacionamentos do projeto é o momento de executar os comandos makemigrate para verificar as alterações da estrutura dos código e depois execute o  migrate.

![5](https://user-images.githubusercontent.com/107952878/193702802-8760e7b8-8b5c-40b0-8ef3-4c6116bf8dbf.JPG)

![6](https://user-images.githubusercontent.com/107952878/193702817-f091a701-dcad-4f4d-ba17-12a6e4856773.JPG)

O Django reconhecerá as classes criadas e enviará as informações para o banco de dados criando todas as tabelas do seu projeto. 
Veja conforme o exemplo abaixo que o Django além de criar as classes(tabelas) no banco de Dados, ele cria as tabelas do próprio Django que é padrão do framework. 

![7](https://user-images.githubusercontent.com/107952878/193703009-71e614ca-9116-4031-a23e-da67f039da68.JPG)

# MYSQL-COM-DJANGO--- Criando o Diagrama do Workbench;

Após a criação do Banco de Dados do projeto, precisamos criar o diagrama usando o Workbench seguindo os passos.

1º Selecione o Banco de Dados do Projeto

![8](https://user-images.githubusercontent.com/107952878/193702942-ca678c86-dc3b-4554-bf55-23282ffada98.JPG)

2º Clique no menu superior: Database>Reverse Enginner > Next > Next

3º Selecione o banco de dados do Projeto > Next

![9](https://user-images.githubusercontent.com/107952878/193703272-f3429b42-b94a-4de0-9b20-e36cf721644c.JPG)

4º Selecione a opção show filter

![10](https://user-images.githubusercontent.com/107952878/193703313-d18fc108-a599-47b7-a4cb-6fa4450a811d.JPG)

5º Selecione as tabelas que são do Django e deixe apenas as tabelas as tabelas do seu projeto. 

![11](https://user-images.githubusercontent.com/107952878/193703353-eaa9f641-5244-4ec9-a88e-af9517c95c47.JPG)

6º Depois que separar as tabelas deixando apenas as tabelas do projeto clique em Execute

![12](https://user-images.githubusercontent.com/107952878/193703392-5bab157c-7c00-4703-ad69-62edc3b3ed94.JPG)

![13](https://user-images.githubusercontent.com/107952878/193703456-f6561a2b-87d3-4835-ba33-87631d07299b.JPG)

7º Vai apresentar a quantidade de tabelas que estarão no diagrama, clicar em Finish

![14](https://user-images.githubusercontent.com/107952878/193703489-d89375cb-621d-44e3-8824-db1490fcc7e0.JPG)

Exemplo de apresentação do Diagrama das tabelas do Banco de Dados já relacionados conforme definido no Django.

![15](https://user-images.githubusercontent.com/107952878/193703535-b8149846-7dd7-44d0-b048-e84b1c9b2bea.JPG)


Agora será possivel fazer toda manipulação do sistema gravando e manipulando informações no Banco de Dados MySql.

Bons Estudos !!!

Prof. Alann Perini
