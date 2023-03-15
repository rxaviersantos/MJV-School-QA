<h1 align="center"> Tipos de testes </h1>

## O que é o tipo do teste? 



É um grupo de atividades de teste destinado a testar características específicas de um sistema de software, ou parte de um sistema, com base em objetivos de teste especificos:

> - Avaliar as características de qualidade funcional, tais como integridade, correção e adequação;
> - Avaliar as característias de qualidade não-funcionais, como confiabilidade, eficiência de performace, segurança, compatibilidade e usabilidade;
> - Avaliar se a estrutura ou arquitetura do componmente ou sistema está correta, completa e especificada;
> - Avaliar os efeitos das alterações, como a confirmação da correção dos defeitos (teste de confirmação) e procurar alterações não internacioabnis no comportamento como resultado de alterações no software ou no aambiente (teste de regreção).

## Testes unitários 

<p align="center">
  <img alt="Pirâmide de automação" src="https://user-images.githubusercontent.com/85380530/225403308-54a26450-05c5-495e-aa67-2e61fa501fce.png" width="80%">
</p>

O teste unitário consiste em verificar o comportamento das menores unidades em sua aplicação. Tecnicamente, isso seria uma classe ou até mesmo um método de classe em línguas orientadas a objetos, e seria um procedimento ou função em línguas processuais e fucnionais. 

O objetivo do teste unitário é assegurar que cada unidade está funcionando de acordo com sua especificação funcional. Estes tipos de testes são frequentemente escritos por desenvolvedores quando trabalham no código, para assegurar que a função específica está executando como esperado. Uma função deve ter muitos testes para dar cobertura a todos os caminhos possíveis do seu código. Sozinho, o teste unitário não pode verificar a funcionalidade de uma parte do software, mas em contrapartida é usado para assegurar que os blocos constituintes do software trabalham independentes dos demais.

Todo o teste unitário necessita de um planejamento prévio. Deve ser de entendimento do desenvolvedor os requisitos que aquela funcionalidade tem que cobrir, qual a sua entrada e qual a sua saída e como se processa o fluxo interno dos dados. Então casos de testes deverão ser formulados para garantir que todos os pontos do fluxo serão verificados pelo menos uma vez pelos testes.

## 5 principios dos testes de unidade 

    1. Desenvolva código testável > Clean code 
    2. Saiba o que testar         > Comportamento de funnção
    3. Comece pelo domínio        > Regras de negócio 
    4. Utilize técnicas           > Red, Green and refactor 
    5. Adote cultura de testes    > TDD, BDD e ATDD
    
## Testes de integração 

Os testes de integração são realizados para validar se as unidades do sistema se comunicam e estão em perfeita sincronia. Ocorrem geralmente após os testes unitários, o que envolve o teste de módulos e unidades individuais. Uma vez determinado que cada unidade funciona isoladamente, os testes de integração avaliam como todas as unidades funcionam quando combinadas.

O objectivo dos testes de integração é verificar se a integração de vários módulos e componentes numa aplicação satisfaz ou não os requisitos do utilizador, bem como os requisitos técnicos e de desempenho da organização.

### Etapas relevantes para um teste de integração 

    – Preparar um plano de teste de integração

    – Decidir que abordagem vai adoptar para os testes

    – Desenho de casos de teste, cenários de teste, e roteiros de teste

    – Implantem os módulos escolhidos em conjunto e realizem os vossos testes

    – Rastrear bugs identificados e registar os resultados dos testes

    – Corrigir bugs e implementar alterações

    – Repita os passos acima até que os seus testes estejam completos

Os testes de integração podem ajudar as equipas de desenvolvimento a identificar e corrigir problemas antecipadamente e a maximizar o desempenho da aplicação e a satisfação do utilizador de uma forma eficiente e eficaz.

## Teste de carga 

O teste de carga pode ocorrer de várias maneiras diferentes, mas seu objetivo principal é estressar o sistema com uma quantidade grande de dados, entradas e saídas, para testar como o sistema lida com um grande volume de dados. 













