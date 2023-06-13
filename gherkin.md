#Funcionalidade: Criar Usuário

#Cenário: Criar um novo usuário com sucesso
Dado que o usuário informa um login válido
E a senha atende aos critérios de segurança
Quando o usuário é criado
Então o sistema retorna o usuário criado

#Cenário: Tentar criar um usuário com uma senha fraca
Dado que o usuário informa um login válido
E a senha é considerada fraca
Quando o usuário é criado
Então o sistema retorna um erro informando que a senha é fraca

#Cenário: Tentar criar um usuário com um login inválido
Dado que o usuário informa um login inválido
E a senha atende aos critérios de segurança
Quando o usuário é criado
Então o sistema retorna um erro informando que o login é inválido
