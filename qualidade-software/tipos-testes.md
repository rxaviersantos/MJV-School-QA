<h1 align="center"> Tipos de testes </h1>

## O que é o tipo do teste? 



É um grupo de atividades de teste destinado a testar características específicas de um sistema de software, ou parte de um sistema, com base em objetivos de teste especificos:

> - Avaliar as características de qualidade funcional, tais como integridade, correção e adequação;
> - Avaliar as característias de qualidade não-funcionais, como confiabilidade, eficiência de performace, segurança, compatibilidade e usabilidade;
> - Avaliar se a estrutura ou arquitetura do componmente ou sistema está correta, completa e especificada;
> - Avaliar os efeitos das alterações, como a confirmação da correção dos defeitos (teste de confirmação) e procurar alterações não internacioabnis no comportamento como resultado de alterações no software ou no aambiente (teste de regreção).

## Testes unitários 

<p align="center">
  <img alt="Pirâmide de automação" src="https://user-images.githubusercontent.com/85380530/227749503-fe041095-d92e-41bb-826e-e68df68036bc.png" width="80%">
</p>

<p align="center">
  <img alt="Pirâmide de automação" src="https://user-images.githubusercontent.com/85380530/227749545-b4ad0e06-c1b7-4719-9cb4-be98c2ddfa5d.png" width="80%">
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

## Testes de componentes 

O teste de componente é uma forma de teste de caixa fechada, o que significa que o teste avalia o comportamento do programa sem considerar os detalhes do código subjacente. O teste de componentes é feito na seção de código em sua totalidade, após a conclusão do desenvolvimento.

O teste de componente leva mais tempo para ser conduzido do que o teste de unidade, porque um componente é composto de várias unidades de código. Embora possa ser demorado, ainda é muito necessário. Às vezes, as unidades individuais funcionam sozinhas, mas começam a ter problemas quando você as usa juntas.

O teste de componentes examina casos de uso, portanto, pode ser considerado uma forma de teste de ponta a ponta. Testes de ponta a ponta e testes de componentes replicam cenários da vida real e testam o sistema em relação a esses cenários da perspectiva do usuário.

A implementação do teste de componentes é benéfica porque pode revelar bugs e erros que os usuários podem encontrar. É sempre melhor detectar e corrigir esses erros antes que os usuários os conheçam.

Existem dois tipos de teste de componentes: testes de componentes pequenos e testes de componentes grandes.

### Teste de componentes pequenos

Com o teste de componentes pequeno, os componentes que estão sendo testados ainda são segregados de outros componentes do sistema. Você ainda deve fazer uso de mock-ups e endpoints de teste para simular os componentes que se conectam com o que está sendo testado. Essa forma de teste garante que o componente esteja pronto para ser integrado ao restante do sistema.

### Teste de componentes grande

O teste de componentes grande escala é feito sem segregação, o que significa que o componente testado terá acesso a componentes externos. Com o teste de componentes em geral, ainda é apenas o componente principal que está sendo testado, não os componentes conectados ou como os componentes interagem entre si. Isso seria um teste de integração.

## Teste interface do usuário 

O teste de usabilidade é uma forma de provar a consistência e a solidez de uma interface ao colocá-la para uso em situações comuns. Ou seja, é um teste que busca entender como o sistema se comporta no dia a dia, na naturalidade da utilização, e se ele atende aos requisitos pensados e estabelecidos.

- `` Usabilidade:`` Focado na experiência do usuário, consistência da interface, layout, acesso às funcionalidades etc.
- `` Acessibilidade:`` Subconjunto de usabilidade, visa atender pessoas de diferentes habilidades: deficiência visual, física, auditiva, comprometimento cognitivo, dificuldade de aprendizagem entre outros.

## Teste de carga 

O teste de carga pode ocorrer de várias maneiras diferentes, mas seu objetivo principal é estressar o sistema com uma quantidade grande de dados, entradas e saídas, para testar como o sistema lida com um grande volume de dados. 

## Testes exploratórios 

De acordo com Bach, testes exploratórios é como “design e execução de teste ao mesmo tempo”. Mas nem sempre é compreendido da forma certa, alguns profissionais de TI entendem como se fosse uma prática realizada de maneira aleatória e a executa um monte de coisa sem sentido. Segundo Kaner, testes exploratório é “um estilo de teste de software que enfatiza a liberdade pessoal e responsabilidade do testador individual para continuamente otimizar a qualidade do seu trabalho tratando aprendizado relacionado a teste, projeto de teste, execução de testes e interpretação de resultados”.

<p align="center">
  <img alt="Pirâmide de automação" src="https://user-images.githubusercontent.com/85380530/228687828-411f5a25-c3db-4e39-823c-dc6cb75bcc64.png" width="80%">
</p>

Não há casos de teste predefinidos nos testes exploratórios, isso não significa que o tester encarregue de levar a cabo o teste não os prepare, isto conduz a menos restrições para o tester e a uma maior liberdade, e responsabilidade pessoal, para aprender e iterar sem procurar uma resposta pré-desenhada da qual não se possa desviar.

Uma das boas práticas que devem cumprir os testes exploratórios é que devem poder responder às seguintes perguntas:

    - A aplicação realiza a função para a que foi desenhada?
    - A aplicação funciona em múltiplos cenários?
    - O desempenho da aplicação é suficientemente bom?
    - Que potenciais erros existem?

Para o qual seguiremos para as seguintes etapas que não são independentes entre si e existem como uma única função coesa ou ciclo de testes.

<p align="center">
  <img alt="Pirâmide de automação" src="https://user-images.githubusercontent.com/85380530/228695477-d07a8d62-db20-4720-bfea-b9f9d23eae70.png" width="80%">
</p>

### Aprendizagem 

Uma das capacidades mais importantes que necessita um tester é a de compreender a aplicação ou o website que está a testar, grande parte desta aprendizagem ocorrerá em tempo real, à medida que comece a explorar e a testar o software. Esta compreensão proporciona contexto e inclui informação como dados comparativos competitivos, conhecimento da indústria e detalhes da empresa. Para certo tipo de aplicações pode ser necessário um tutorial.

### Desenho

Os testers exploratórios podem realizar o teste da maneira que considerem adequada e não tendo à partida um resultado desejado ou esperado. Muitas vezes, a técnica de teste exploratório conduz ao desenvolvimento de cenários de testes com guiões mais rigorosos ao longo do tempo.

A gestão do teste pode ajudar a decidir o dispositivo, as circunstâncias ou as condições se o solicitante do teste ainda não o tiver estabelecido.

### Execução

O tester tem a liberdade de completar o teste como quiser. Esta liberdade significa que ninguém está à espera dos resultados escritos e pode começar o trabalho criativo assim que seja solicitado. O tester pode começar a observar e aprender sobre a aplicação ou o website. Uma vez finalizada esta fase, os resultados são compilados e comunicados através dos métodos apropriados.

## Técnicas de testes exploratórios

Existem diferentes formas de realizar testes exploratórios. Os três principais tipos são:

- ``Testes de estilo livre:``
Como sugere o nome, trata-se de testes nos quais cada tester seleciona um módulo ou a aplicação completa e a executa de forma aleatória. É como um smoke test rápido que se realiza para assegurar que tudo é implementado como esperado.

- ``Testes baseados em cenários:``
Neste tipo de testes exploratórios, cada tester seleciona um cenário de utilizador e testa os fluxos da aplicação relativos a esse caso de uso. Tentam cobrir todas as navegações, permutação de dados e fluxo que sejam possíveis para assegurar a estabilidade e funcionalidade desse cenário.

- ``Testes baseados em estratégias:``
Este tipo de testes implica implementar as metodologias de teste centrais num teste exploratório. Neste teste, o tester especializado aplicaria técnicas de black-box testing à aplicação.

## Vantagens dos testes exploratórios

> Encontrar mais defeitos:

Um benefício importante dos testes exploratórios é que encontram defeitos que a automatização simplesmente não consegue encontrar. Os testes automatizados limitam-se aos casos de testes que se escrevem para os mesmos. Não encontrará nenhum erro fora deste âmbito

> Velocidade dos ciclos de teste: 

Os testes exploratórios não requerem uma planificação extensa. O alcance de um ciclo de teste deve ser claro, mas não são necessários casos de teste detalhados. Isso deve-se ao facto de se confiar nos testers para testar o que acreditam que deve ser testado. Em comparação, os testes automatizados são rápidos na execução de testes, mas a sua planificação pode levar muito tempo.

> Geração de ideias:

A criatividade requerida dos testers e o rápido ritmo dos testes exploratórios significa que se criam mais ideias.

## Desvantagens dos testes exploratórios

> Fazer as coisas bem é difícil:

Os testes exploratórios dependem em grande medida do tester. Pode ser uma habilidade cara e difícil de adquirir, pelo que pode ser complicado encontrar os tester exploratórios que se estão à procura.

> Medir o ROI pode ser complexo: 

Medir o sucesso dos testes exploratórios a curto prazo pode ser complexo. 

## Testes de usabilidade

O teste de usabilidade existe para avaliar o quão facilitada é a utilização do software para o usuário. Ele analisa a interface (UX/UI) do sistema, a maneira como é desenhado o fluxo (design pattern) e a integridade da interação com o usuário.

Normalmente, durante um teste, os participantes tentarão concluir tarefas típicas enquanto os observadores assistem, ouvem e fazem anotações. O objetivo é identificar eventuais problemas de usabilidade, coletar dados qualitativos e quantitativos e determinar a satisfação do participante com o produto.

### Benefícios do teste de usabilidade

O teste de usabilidade permite que as equipes de design e desenvolvimento identifiquem problemas antes de serem codificados. Quanto mais cedo os problemas forem identificados e corrigidos, menos dispendiosas serão as correções em termos de tempo da equipe e possível impacto no cronograma. Durante um teste de usabilidade, você irá:

    - Saiba se os participantes são capazes de concluir as tarefas especificadas com sucesso e
    - Identifique quanto tempo leva para concluir as tarefas especificadas
    - Descubra como os participantes estão satisfeitos com seu site ou outro produto
    - Identificar as mudanças necessárias para melhorar o desempenho e a satisfação do usuário
    - E analise o desempenho para ver se ele atende aos seus objetivos de usabilidade

É importante ter em mente que o teste de usabilidade não é apenas um marco a ser verificado no cronograma do projeto. A equipe deve ter uma meta para o motivo pelo qual está testando e, em seguida, implementar os resultados.

## Testes funcionais e não funcionais 

### Teste Funcional

Teste funcional é um processo de garantia de qualidade, e um tipo de teste de caixa preta que baseia seus casos de teste nas especificações do componente de software sob teste. As funções são testadas alimentando-as com entrada e examinando a saída, e a estrutura interna do programa raramente é considerada (ao contrário do teste de caixa branca). O teste funcional é realizado para avaliar a conformidade de um sistema ou componente com os requisitos funcionais especificados. O teste funcional geralmente descreve o que o sistema faz.

Como o teste funcional é um tipo de teste de caixa preta, a funcionalidade do software pode ser testada sem conhecer o funcionamento interno do software. Isso significa que os testadores não precisam conhecer linguagens de programação ou como o software foi implementado. Isso, por sua vez, pode levar à redução do viés do desenvolvedor (ou viés de confirmação) nos testes, uma vez que o testador não esteve envolvido no desenvolvimento do software.

O teste funcional não implica que você está testando uma função (método) de seu módulo ou classe. O teste funcional testa uma fatia da funcionalidade de todo o sistema.

## Técnicas comuns do teste funcional e teste de software

### Teste de Caixa-branca:

Também chamada de teste estrutural, a técnica de caixa-branca avalia o comportamento interno do software.
Esta técnica de teste avalia o comportamento interno do componente de software, trabalhando diretamente sobre o código fonte do componente de software para avaliar aspectos tais como: teste de condição, teste de fluxo de dados, teste de ciclos e teste de caminhos lógicos.

#### Teste de Caixa-preta:

Esta técnica de teste em que o componente de software a ser testado é abordado como se fosse uma caixa-preta, ou seja, não se considera o comportamento interno do mesmo. Dados de entrada são fornecidos, o teste é executado e o resultado obtido é comparado a um resultado esperado previamente conhecido. Haverá sucesso no teste se o resultado obtido for igual ao resultado esperado. O componente de software a ser testado pode ser um método, uma função interna, um programa, um componente, um conjunto de programas e/ou componentes ou mesmo uma funcionalidade. A técnica de teste funcional é aplicável a todos os níveis de teste.

### Teste não funcional 

São técnicas utilizadas para verificar a operação correta do sistema em relação a casos inválidos ou inesperados de entrada. Outras técnicas de teste existem para testar aspectos não-funcionais do software, como por exemplo, os testes de desempenho, teste de carga ou teste de usabilidade. As técnicas não funcionais verificam atributos de um componente ou sistema que não se relacionam com a funcionalidade (por exemplo, confiabilidade, eficiência, usabilidade, performance, manutenção e portabilidade).




