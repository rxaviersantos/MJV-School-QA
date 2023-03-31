
<h1 align="center"> Escrita de cenários em BDD<h1>
  
## O que é BDD 

BDD é uma técnica de desenvolvimento de software ágil, criado por Dan North, em 2003, com o intuito de melhorar a comunicação entre um time de desenvolvimento (PO, QA e DEV) para que todos tenham o mesmo entendimento sobre uma determinada funcionalidade.

O BDD foi criado em resposta a problemas que Dan North presenciava através do uso da técnica do TDD – Test Driven Development (Desenvolvimento orientado a testes). A maioria dos times de desenvolvimento e seus alunos tinham dificuldade em como escrever seus testes de acordo com uma determinada User Story. 

Então,  surge o BDD trazendo a proposta que cenários serão escritos exemplificando comportamentos de uma funcionalidade para que a mesma atinja um objetivo real, agregando valor ao negócio, e assim, dando um suporte ao TDD para que os testes sejam feitos de acordo com os cenários que foram descritos.   

### Estrutura do BDD 

O BDD utiliza uma estrutura simples para descrever cada um dos cenários, essa estrutura tem como objetivo garantir a clareza dos cenários.
  
<p align="center">
  <img alt="Pirâmide de automação" src="https://user-images.githubusercontent.com/85380530/228935726-2ec8f25a-3895-46e3-8deb-8a5b74b43666.png" width="80%">
</p>

## O BDD apresenta um framework baseado em três princípios
```
- A área de negócios e o time de desenvolvimento precisam se referir a mesma parte do sistema da mesma forma;

- Toda parte do sistema precisa ter um valor identificável e verificável para o negócio;

- Analisar, projetar e planejar tudo de cima a baixo tem retorno decrescente;

```   
  
Podemos definir o BDD como a união de várias práticas consideradas ágeis e úteis no desenvolvimento de software, cuja ênfase está nas funcionalidades de alto valor e na redução dos custos de mudança por meio da identificação do que de fato está sendo testado/desenvolvido.
 
## Processos para iniciar o BDD   

Como toda metodologia, o BDD também possui um processo a ser seguido, passando pelas etapas de Descoberta, Definição, Formalização e Entrega. A Automação de Testes não entra nessas etapas, mas durante o processo poderá ser decidido qual caminho a ser seguido para sua construção.  
  
> Processo de BDD:

`` Descoberta:``  Nesta fase fazemos as reuniões de Refinamento da história, onde o PO apresenta a User Story que fará parte daquela sprint.
  
`` Definição:``  Nesta etapa definimos as Regras de negócio daquela história, mostrado exemplos de funcionamento e entendimento compartilhado. 

`` Formalização:``  Nesta fase elaboramos os protótipos funcionais e os critérios de aceitação (Gherkin).  
  
`` Entrega:``  Aqui é feita a entrega da funcionalidade, monitoramento, feedbacks do usuário final e testes de aceitação na aplicação(podendo ser utilizado os cenários de Gherkin para os testes).   

## BDD na prática
  
O processo de desenvolvimento do BDD se baseia na escrita de cenários de testes. Cada cenário é um exemplo escrito para ilustrar um aspecto específico de comportamento esperado da aplicação. 

Para a escrita do BDD utilizamos uma DSL conhecida como Gherkin, sendo uma linguagem estruturada que se inicia com a sintaxe Given, When e Then (Dado que, Quando, Então). 
  
```   
- A cláusula ‘Dado’ descreve as condições e pré-condições; 
  
- Já cláusula ‘Quando’, tem o objetivo de descrever um evento ou uma ação;
  
- A cláusula ‘Então’, trata-se de todas as saídas e resultados esperados, descrevendo as informações 
  
  visíveis ao usuário ou sistemas externos. 
  
``` 
  
## Exemplos de boas práticas na construção de cenários de um BDD:   
  
> Exemplo 1  
```  
Feature: Compra de produtos 

- Como lojas americanas

- Eu quero permitir frete grátis para clientes

- Para compra acima de R$100,00 de modo que o cliente seja

- Estimulado a comprar mais.
  
  
Cenário: Permitir frete grátis para clientes que realizam compras acima de R$100,00 

Dado que eu esteja realizando uma compra de no mínimo R$100,00 

Quando o cliente calcular seu frete 

Então será exibido que ele terá o frete grátis para seu pedido  
  
```  
  
> Exemplo 1.1
  
```  
Feature: Compra de produtos 

- Como lojas americanas 

- Eu quero permitir frete grátis para clientes 

- Para compra acima de R$100,00 de modo que o cliente seja 

- Estimulado a comprar mais. 
  

Cenário: Taxa de frete será cobrada para compras abaixo de R$ 100,00 

Dado que o cliente esteja realizando uma compra abaixo de R$100,00 

Quando o cliente calcular seu frete 

Então será exibido um valor de frete a ser cobrado   
  
```  
  
  
> Exemplo 2  (Nesse exemplo uso a técnica  Outline) 

```  
Feature: Cadastrar um Estudante corretamente 

- Como um usuário do sistema acadêmico 

- Eu quero cadastrar dados dos alunos 

- Para manter os dados dos alunos registrados no sistema acadêmico       
  
  
Cenário: Realizar cadastro de estudante

Dado que eu tenha clicado no botão <novo cadastro> 

E tenha preenchido  todos os campos de cadastro 

   | Last Name | First Name | Enrollment Data  | 

   | ”Silva”   |  ”João”    | ”10/03/2017”     | 

   | ”Santos”  |  ”Joana”   | ”10/03/2017”     | 

   | ”Carlos”  |  ”Roberto” | ”10/03/2017”     |  

Quando eu clicar no botão <Cadastrar> 

Então aluno será cadastrado e exibido na lista de alunos cadastrados 
```  
  
> Exemplo 3
  
```
Feature: Transferir dinheiro através da modalidade PIX 

- Como cliente do banco 

- Quero realizar uma transferência de dinheiro pela modalidade Pix 

- Para que meus amigos recebam o dinheiro em segundos
  

Cenário A: Realizar transferência PIX com chave válida

Dado que eu esteja realizando um PIX para uma <chave> válida 

| Celular         | CPF           | E-mail          | Chave aleatória | 

|(31) 989161-0329 | 0XX.0X3.15X-8X| amanda87@gmail.com | NSAND-SDK37 | 

|(32) 998214-5849 | 02X.0X5.15X-X3| eliza64@gmail.com | NAAOS-S1K4Y |                                                                                                                                                                                                                                           

Quando eu confirmar a transferência para aquela chave 

Então o dinheiro será transferido para o favorecido no mesmo segundo   
```
  
```  
Cenário B: Realizar transferência PIX  com chave inválida

Dado que eu esteja realizando um PIX para uma <chave> inválida 

Quando eu inserir uma chave inexistente para aquele tipo de chave escolhida 

| Celular         | CPF            |E-mail           | Chave aleatória |

|(31) 976141-6389 | 0XX.0X3.15X-88X| amanda87@gmail.com.com | NSAND/SDK/NSLK |

|(32) 987294-4869 | 02X.0X5.15X-X37| elizabe64@gmail.com| NA/AO/-S1K/LK |                                                                                                                                                                   

Então transferência PIX não será permitida  
  
```  

## Prós e Contras do BDD   
  
`` Prós:``  O time se une em um entendimento comum, conseguindo definir os cenários para a geração real de valor ao cliente, e também identificam possíveis falhas de negócio que foram definidos na User Story. A Técnica de Gherkin contribui para pensar em inúmeros caso de falhas quando utilizado a sintaxe Dado, Quando e Então.   
  
`` Contras:``  O BDD pode virar um elefante branco caso você se empolgue em escrever inúmeros cenários, pois a maioria das pessoas não gostam de ler, tampouco realizar manutenção na escrita dos cenários. Então, o BDD pode ser uma armadilha caso não seja usado com moderação. É importante ressaltar que os Cenários precisam ser claros, curtos e objetivos, definindo somente as principais regras de negócio daquela Feature, para os demais cenários identificados, eles poderão ser incluídos através da metodologia TDD ou até mesmo em fluxogramas.   
  
  

