<h1 align="center"> Planos de testes </h1> 


## Especificação de software 

O analista é o profissional responsével pela escrita do documento de especificação do software. Este documento pode ser escrito de várias formas:

- Descrito por tela;
- Descritivo por funcionalidade;
- Histórias;
- Histórias com BDD;

O documento descritivo deve conter uma relação das:

- Funcionalidades/telas;
- O conjunto de regras de negócio;
- Requisitos funcionais;
- Requisitos não funcionais;
- Tabelas e imagens de apoio quando necessário.

## O que é um cenário?

É o enredo das atividades a serem executados no teste. Ele pode ser descrito em uma sequência de ações onde se pretende criar um roadmap, um passo a passo.

1. Priemeiramente se analisa o cenário descrito pelo analista;
2. Divide a tela/funcionalidade/cenário em ações menores e atômicas;
3. Coloca-se estas ações em ordem lógica;
4. Acrescenta as informações as informações de regras específicas a serem observadas (quando necessário);
5. Executa o cenário; 

### Exemplo de um cenário de teste 

> Cenário / Efetuar login 
````
- Regra de negócio 01: O usuário deverá inserir matricula, e-mail e CPF

- FA: Se o usuário preencher o campo login e senha incorretos, o sistema emite mensagem "Usuário ou senha inválidos"

1. Usuário preenche o campo login (Regra 01)
2. Usuário preenche o campo senha 
3. Usuário clica em login
4. O sistema acessa a página principal 

Resultado esperado: "O sistema acessa a página principal"

> Possibilidades a serem testadas 

    1.1 Login com matricula e senha corretos
    1.2 Login com e-mail e senha corretos
    1.3 Login com CPF e senha corretos
    2.1 Login matricula e senha incorretos 
    2.2 Login e-mail e senha incorretos 
    3. Login incorreto 
    4. Senha incorreta
    5. Login e senha em branco
    6. Somente login em branco
    7. Somente senha em branco
````






