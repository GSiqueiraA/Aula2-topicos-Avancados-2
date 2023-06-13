# Use Cases

## Criar Usuário

### Fluxo Principal
1. O sistema recebe os dados de login e senha do usuário.
2. O sistema gera um ID único (UUID) para o usuário.
3. O sistema encripta a senha do usuário.
4. O sistema cria um novo usuário com o ID, login e senha encriptada.
5. O sistema retorna o usuário criado.

### Fluxo Alternativo - Senha Fraca
1. O sistema recebe os dados de login e uma senha fraca do usuário.
2. O sistema retorna um erro informando que a senha não atende aos critérios de segurança.

### Fluxo Alternativo - Login Inválido
1. O sistema recebe um login inválido (por exemplo, vazio ou contendo caracteres inválidos).
2. O sistema retorna um erro informando que o login é inválido.
