# CadastroVeiculosUsuario
API para cadastro de Usuarios e Veiculos utilizando Spring REST

O cadastro de usuário obedece a algumas diretrizes, não aceita duplicidade de dados como CPF e e-mail, e não aceita cadastro de campos nulos ou em branco

Para o cadastro do veículo o uusuário precisa inserir na requisição os dados referentes a marca, modelo e ano de fabricação, a API consome um serviço externo e consulta 
os dados em outro serviço, em caso de resposta positiva, (encontrando-os), ela retorna com o modelo, marca, ano e valor venal conforme a tabela FIPE, como exercício para 
o desafio existe uma comparação do último dígito do ano de fabricação do veículo e uma hipotética tabela de rodizio.


a API possui ainda um método List, com o qual através de uma requisição contendo o número do ID do usuário ela traz uma resposta de quais veículos estão atribuidos àquele
usuário, retornando também se de acordo com ano de fabricação daquele veículo o rodizio está ativo ou não.
