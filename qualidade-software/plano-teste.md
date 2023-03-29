## Documentação de análose 
## Técnicas de escrita de cenário 


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

- Efetuar login 

1. Usuário preenche o campo login (Regra 01)
2. Usuário preenche o campo senha 
3. Usuário clica em login
4. O sistema acessa a página principal 

FA: Se o usuário preencher o campo login e senha incorretos, o sistema emite mensagem "Usuário ou senha inválidos"

Regra de negócio 01: O usuário deverá inserir matricula, e-mail e CPF



## Para que serve o BDD 




### Estrutura do BDD 
- Dado: Local em que o usuário realiza a ação;
- Quando: Ação realizada pelo usuário;
- Então: Resultado esperado da ação;
- E: Conector de ações ou resultados;

Exemplo de BDD 

Relaizar Login 

  Dado que o usuário esteja na página de login do gmail
  Quando preencher o campo com e0mail válido
  E clicar no botão avançar 
  Então o sistema exibe tela com o campo e senha 





