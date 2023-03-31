<h1 align="center">
 BDD e Scrum: A união das metodologias
</h1>

Metodologias de desenvolvimento e gerenciamento, quando combinadas, podem gerar melhores resultados na produção de software. Dito isto, vamos a um caso do casamento de duas metodologias que se completam, o Scrum e o BDD.  

O Scrum é uma metodologia ágil muito utilizada no processo de desenvolvimento, sendo que uma das exigências do Scrum é uma melhoria constante no processo de desenvolvimento. A melhoria constante no backlog de produtos é essencial para a melhoria dos projetos em que a equipe trabalha dentro Scrum, pois é através dela que a equipe compartilha o que será desenvolvido, possuindo o que é essencial para o produto e permite ainda a equipe compreender o que deve ser feito e o que vai ainda ser produzido.

O refinamento do backlog de produto indica que a equipe está compreendendo o que deve ser feito. Uma forma de refinar o backlog de produto é a utilização da metodologia BDD - Behavior-Driven Development ou Desenvolvimento orientado por comportamento.
O BDD aponta como foco do teste de implementação o comportamento que o sistema deve ter, ou seja, teste por comportamento exigido, neste caso, ao invés de testar a unidade, testaríamos algo que o sistema deveria fazer. Por exemplo:

Quando eu preencher os campos do formulário de cadastro e clicar no botão cadastrar, se o cadastro foi bem sucedido, o sistema deve exibir uma mensagem no topo da tela: “Cadastro efetuado com sucesso” e o id do usuário.  
  
A principal vantagem de se utilizar o BDD é que comportamentos não mudam na mesma intensidade da codificação, de um modo geral, o BDD possui três princípios segundo Lapolli et al, sendo eles:
```
1. A área de negócio e a tecnologia precisam se referir à mesma parte do sistema da mesma forma;
2. Toda parte do sistema precisa ter um valor identificável e verificável para o negócio;
3. Analisar, projetar e planejar tudo de cima a baixo tem retorno decrescente.
 ``` 
> O BDD possui um ciclo, que é denominado outside-in, que possui 5 passos, sendo eles:
> 
``` 
1. Foco em cenário;
2. Escreva a especificação para o cenário;
3. Escreva a especificação das unidades;
4. Faça a especificação da unidade passar;
5. Refatore.
``` 

## Scrum e BDD, o casamento
Zia Malik afirma que o BDD deve ser utilizado para apoiar equipes Scrum no Backlog de produtos, desta forma temos nosso casamento. Claro que além do backlog de produto, podemos utilizar para a etapa de desenvolvimento, ou seja, a forma que vamos desenvolver durante o Sprint, pode ser utilizado o BDD.

<p align="center">
  <img alt="Pirâmide de automação" src="https://user-images.githubusercontent.com/85380530/229005947-e961b3f6-9e0d-41e3-9052-c45b41ff7a41.png" width="80%">
</p>

O Backlog possui requisitos, normalmente organizados por prioridade: alta prioridade no topo e baixa prioridade na parte inferior. É no backlog que o BDD começa o casamento com o Scrum, pois as histórias de usuário (requisitos), se seguirem o padrão do BDD, possuirão foco na funcionalidade. Exemplo:

Item 1 do Backlog: O cliente deseja que o site tenha login e que ao fazer o acesso, seja possível ver e alterar o perfil (foco na funcionalidade).

O Scrum auxilia justamente nos processos que possuem rápida mudança de requisitos, o BDD vai auxiliar no processo de qualificação do backlog.

O PO pode inserir critérios de aceitação de alto nível para que as histórias de usuário sejam aceitas. Exemplo de critérios de aceitação do Item 1.
  
```  
- O cliente para fazer login, deve utilizar usuário e senha únicos;

- Caso ocorra erro, deve ser exibida uma mensagem apropriada.  
```` 

Neste ponto o BDD deve apoiar positivamente o entendimento da equipe e as partes interessadas do que está sendo entregue, para isso deve ser utilizada linguagem de negócio simples. Este fato implica em melhor qualidade, além disso, as aplicações que utilizam o BDD como método de desenvolvimento, tem como base, semelhante ao TDD, os testes automatizados, garantindo maior qualidade a aplicação e melhor entendimento nos cenários a serem desenvolvidos. Assim, o refinamento do backlog do Scrum deve ser realizado de forma a melhorar a compreensão do sistema, melhorando a confiança da equipe e aperfeiçoando a adaptabilidade dos desenvolvedores em relação ao projeto.

Mas por que o BDD pode auxiliar no backlog de produto?

O BDD utiliza uma linguagem ubíqua para o entendimento de comportamentos, que segue três passos, segundo ECQUalisBR:

`` Dado que (Given):``  que especificam as pré-condições para que ocorra a ação de interesse do cenário;

`` Quando (When):``  cuja função é especificar os eventos que devem ocorrer para que o cenário seja executado;

`` Então (Then):``  que especificam as expectativas a respeito dos resultados da execução dos eventos do cenário.

Desta forma, o BDD tem como objetivo obter uma compreensão mais clara dos comportamentos desejados no software. Para este entendimento, discussões são realizadas com os envolvidos no projeto, de forma a melhorar o entendimento, ao criar as histórias de usuários do Scrum serão utilizadas técnicas do BDD, utilizando um conjunto de língua nativa e de linguagem ubíqua do BDD com o objetivo de descrever a finalidade e o beneficio da funcionalidade, permitindo que os desenvolvedores, durante a Sprint, concentrem-se no código a ser criado, ao invés de se preocupar com detalhes técnicos desnecessários, minimiza ainda problemas de entendimento.

O BDD então fornece uma plataforma completa com o objetivo de transformar a exigência do usuário em comportamentos funcionais, resultando em uma forma melhor de compreensão da aplicação que o cliente deseja. Além disso, torna mais fácil a escrita dos testes, pois são realizados testes por funcionalidades e também mais prática a implementação de teste de aceitação com foco em resultados esperados.

A evolução do backlog é constantemente discutida na fase de Sprint Planning e Sprint Review. E diariamente os desenvolvedores podem utilizar a reunião diária para melhorar o entendimento das funcionalidades. O BDD deve fornecer a plataforma comum de compreensão das atividades a serem desenvolvidas, evitando-se assim confusões e/ou falta de conhecimento entre a equipe. Por isso o contato constante com os interessados faz com que os resultados sejam melhor atendidos.

E quais os benefícios reais desta fusão Scrum e BDD?

```
- Evita-se erros de compreensão e interpretação das histórias de usuário;

- O que antes eram requisitos funcionais e requisitos não funcionais são transformados em comportamentos funcionais do software e critérios de aceitação;

- Fornece uma forma de comunicação (vocabulários) comum a todos envolvidos, facilitando a compreensão por parte de todos;

 - A equipe fica ciente dos comportamentos serão aceitos pelos usuários com antecedência;

- A equipe entende como os comportamentos são relacionados, evitando confusão;

- As reuniões de planejamento, revisão e diárias tornam-se mais eficazes.
``` 

O resultado de utilizar o BDD para melhorar o Backlog de produto será a redução de falhas de requisito, já a utilização do BDD durante a fase de desenvolvimento busca reduzir o número de falhas utilizando testes automatizados, isso buscando garantir a qualidade do produto.

O Scrum é uma metodologia para desenvolvimento aberta e adaptável, que pode ser unida a outras metodologias. Nota-se que a união com o BDD, técnica que tem como objetivo melhorar o entendimento dos requisitos e amplia a qualidade no processo de designer e desenvolvimento da aplicação, traz como retorno requisitos melhor entendido e software com maior qualidade e mais adequado as necessidades do cliente.
  
  
  
  
  
  
## Referência

 - [scrumalliance](https://www.scrumalliance.org/articles/500-value-of-behaviordriven-development-for-backlog-refinement-in-scrum)
 - [dannorth](https://dannorth.net/introducing-bdd/)

  
