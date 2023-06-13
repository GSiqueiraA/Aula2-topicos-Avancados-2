# Funcionalidade: Criar Usuário

## Cenário: Criar um novo usuário com sucesso
Dado que o usuário informa um login válido
E a senha atende aos critérios de segurança
Quando o usuário é criado
Então o sistema retorna o usuário criado

## Cenário: Tentar criar um usuário com uma senha fraca
Dado que o usuário informa um login válido
E a senha é considerada fraca
Quando o usuário é criado
Então o sistema retorna um erro informando que a senha é fraca

## Cenário: Tentar criar um usuário com um login inválido
Dado que o usuário informa um login inválido
E a senha atende aos critérios de segurança
Quando o usuário é criado
Então o sistema retorna um erro informando que o login é inválido

# Funcionalidade: Realizar Login
Fluxo Principal:
O cliente insere seu nome de login e senha. O sistema verifica as informações de login e senha do cliente. Se as informações forem válidas, o sistema autentica o cliente.

Fluxo Alternativo:
Se as informações de login e senha forem inválidas, o sistema exibe uma mensagem de erro.

# Funcionalidade: Adicionar Produto
Fluxo Principal:
O atendente realiza o login no sistema. O atendente seleciona a opção de adicionar produto. O sistema solicita as informações do novo produto (nome, preço e quantidade). O atendente insere as informações do produto. O sistema registra o novo produto no estoque.

Fluxo Alternativo:
Se houver campos em branco ou informações inválidas, o sistema exibe uma mensagem de erro.

# Funcionalidade: Vender Produtos Localmente
Fluxo Principal:
O atendente realiza o login no sistema. O atendente seleciona a opção de registrar venda. O sistema exibe a lista de produtos disponíveis. O atendente seleciona os produtos vendidos e informa a quantidade de cada produto. O sistema verifica se há estoque suficiente dos produtos selecionados. Se houver estoque suficiente, o sistema registra a venda e atualiza o estoque dos produtos vendidos.

Fluxo Alternativo:
Se não houver estoque suficiente, o sistema exibe uma mensagem de erro.

# Funcionalidade: Vender Produtos Remotamente
Fluxo Principal:
O cliente realiza o login no sistema. O cliente seleciona o produto que deseja. O sistema exibe a lista de produtos disponíveis. O cliente seleciona os produtos a serem comprados e informa a quantidade de cada produto. O sistema verifica se há estoque suficiente dos produtos selecionados. Se houver estoque suficiente, o sistema registra a venda e atualiza o estoque dos produtos vendidos.

Fluxo Alternativo:
Se não houver estoque suficiente, o sistema exibe uma mensagem de erro.
