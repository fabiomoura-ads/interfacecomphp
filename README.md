# interfacePHP
Scripts PHP com exemplo funcional de utilização de Interface.

Serviço /service/cadastros_interface_service.php, neste arquivo existem dois métodos implementados com utilização de Interface, criaObjetoDaInterfaceWeb() e cadastrar();

"Este script foi criado para utilização em um aplicativo mobile, que iria realizar cadastros em uma outra aplicação web."
--

Para testar

-Criar um banco com nome teste, e importar o arquivo teste.sql, localizado na pasta 'extra' do projeto.

-Mysql usuário root, sem senha

Acessando o arquivo Testes_de_Cadastros.html, poderá ser realizado testes de inserção de registros para constatar o funcionamento da interface aplicada.

No formulário é preciso enviar dois inputs adicionais:

1 - Nome do serviço: 
input type="text" name="servico" value="cadastros_interface_service"

2 - Nome da classe do registro
input type="text" name="classeRegistroDaInterfaceWeb" value="Categoria" /><br /

Com isso o arquivo cadastros_interface_service.php vai instanciar uma classe a partir do input 'classeRegistroDaInterfaceWeb', depois irá popular o objeto com o método criaObjetoDaInterfaceWeb(), passando o $_POST carregado com os atributos específicos do objeto, logo em seguida o objeto será gravado efetivamente, com o método cadastar();

Fim





