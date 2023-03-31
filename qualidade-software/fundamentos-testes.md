<h1 align="center"> Fundamentos de testes </h1>

## O que é teste?

É uma maneira de avaliar e garantir a qualidade do software e reduzir o risco de falha durante sua operação. A atividade de testar não se resume apenas a executá-lo e verificar os resultados, mas também em planejar o teste, analisar, modelar e implantar, gerar relatórios de progresso e resultados dos testes e avaliação da qualidade do software.

Há testes dinâmicos e estáticos, e o teste também deve incluir a revisão de requisitos, história do cliente e código-fonte. Além de verificar se o sistema está de acordo com os requisitos de negócio, o teste deve verificar também se o sistema atende às necessidades do usuário e stakeholders em seus ambientes operacionais.

## Principais objetivos dos testes 

    > Prevenir defeitos;
    > Verificar se todos os requisitos foram cumpridos;
    > Verificar se o objeto do teste está completo e validar se funciona como o esperado pelo usuário;
    > Criar confiança no nível de qualidade do software;
    > Encontrar defeitos e falhas;
    > Fornecer informações suficientes aos stakeholders para tomada de decisão;
    > Cumprir os requisitos ou normas contratuais;

## Porque o teste é necessário?
  - Contribuições do Teste para o Sucesso
  
- Entregas de software com bugs é mais comum do que se imagina, mas com o uso de técnicas apropriadas é possível reduzir a frequência de tais entregas defeituosas. Algumas destas técnicas são:
    - Testadores envolvidos nas revisões de requisitos e refinamentos de histórias;
    - Testadores colaborando com os projetistas na fase de projeto;
    - Testadores colaborando juntamente com os desenvolvedores;
    - Testadores de homologação;
    - 
## Garantia da Qualidade e Teste 

Garantir a qualidade é mais do que apenas testar um sistema já desenvolvido, ou garantir que determinada funcionalidade está funcionando. A garantia de qualidade reside em processos ao longo da idealização, planejamento, desenvolvimento e manutenção do software, a ponto de prover um alto grau de confiabilidade na eficácia do sistema, do produto como um todo.

## Erros, Defeitos e Falhas

Erros, sejam de elicitação de requisitos ou em código, podem introduzir defeitos no sistema, pequenas faltas que juntas podem ocasionar uma falha, seja ela pequena ou grande, interrompendo o funcionamento de uma função ou de todo o sistema.

Os erros podem ocorrer por vários motivos: falha humana, falta de comunicação, falta de qualificação, complexidade de código e tecnologias e etc.

## Defeitos, Causas-raiz e Efeitos

Causa-raiz é o motivo principal do aparecimento de um defeito, é o que de real está incorreto, como um código escrito de maneira errada, um cálculo de uma função financeira com problemas de elicitação. 
Os efeitos são justamente as consequências geradas pelo defeito.

## Os sete princípios de testes

    > 1. O teste mostra a presença de defeitos e não a sua ausência;
    > 2. Testes exaustivos são impossíveis;
    > 3. O teste inicial economiza tempo e dinheiro;
    > 4. Defeitos se agrupam;
    > 5. Cuidado com o paradoxo do pesticida;
    > 6. O teste depende do contexto;
    > 7. A ausência de erros é uma ilusão.

## Processo de teste

Não existe um processo universal de teste, como se fosse uma receita de bolo. São muitos os fatores que colaboram para a necessidade específica nos testes e há todo um contexto a ser considerado na elaboração de atividades comuns e essenciais para a boa execução dos testes e do alcance dos objetivos que se pretende com determinado teste.

## Processo de Teste no Contexto

    > Modelo de ciclo de vida e metodologias utilizadas;
    > Níveis e tipos de teste;
    > Domínio do negócio;
    > Restrições operacionais;
    > Políticas e práticas organizacionais;
    > Normas necessárias;

## Atividades e Tarefas de Teste
Um processo de testes consiste nas seguintes atividades principais:

    - Planeamento do teste;
    - Monitoramento e controle do teste;
    - Análise do teste;
    - Modelagem do teste;
    - Implementação do teste:
    - Execução do teste;
    - Conclusão do teste.

## Planejamento do Teste

O planejamento são as atividades que estabelecem os propósitos e as abordagens que serão utilizadas dadas as limitações e contexto do projeto. Veremos os conceitos mais adiante nas próximas aulas. 
Há contextos dentro das organizações que podem influenciar na execução dos testes, tais como:

## Monitoramento e Controle do Teste
O monitoramento é a ação de verificar o processo real das execuções do teste em comparação com o planejado. Essa avaliação pode incluir:

  * Verificar os resultados do teste e os registros em relação aos critérios especificados de cobertura;
  * Avaliar o nível de qualidade do componente ou sistema com base nos resultados e registros dos testes;
  * Determinar se são necessários mais testes (p. ex., se os testes originalmente destinados a atingir um nível de cobertura de risco do produto falharam, exigindo que testes adicionais sejam escritos e executados).

## Análise do Teste

É a etapa em que é definido o que testar baseado nos critérios de cobertura mensuráveis, ou seja, no escopo do projeto.

  * Analisar a base de teste apropriada ao nível de teste que está sendo utilizado;
  * Avaliar a base de teste e os itens de teste para identificar os vários tipos de defeitos;
  * Identificar os recursos e os conjuntos de recursos a serem testados;
  * Definir e priorizar as condições de teste para cada recurso com base na análise da base de teste e considerando as características funcionais, não-funcionais e estruturais, outros fatores comerciais e técnicos e níveis de riscos;
  * Capturar a rastreabilidade bidirecional entre cada elemento da base de teste e as condições de teste associadas (ver capítulos 1.4.3 e 1.4.4).

## Modelagem do Teste

Durante a modelagem de teste, as condições de teste são elaboradas em casos de teste de alto nível, em conjuntos de casos de teste de alto nível e outros testwares. Assim, a análise do teste responde à pergunta “o que testar?”, enquanto a modelagem de teste responde à pergunta “como testar?”

  * Projetar e priorizar casos de teste e conjuntos de casos de teste;
  * Identificar os dados de teste necessários para comportar as condições de teste e os casos de teste;
  * Projetar o ambiente de teste e identificar qualquer infraestrutura e ferramenta necessária;
  * Capturar a rastreabilidade bidirecional entre a base de teste, as condições de teste, os casos de teste e os procedimentos de teste (ver capítulo 1.4.4).

## Implementação do Teste

Durante a implementação do teste, o testware necessário para a execução do teste é criado ou concluído, incluindo o sequenciamento dos casos de teste nos procedimentos de teste. Portanto, a modelagem de teste responde à pergunta "como testar?", enquanto a implementação do teste responde à pergunta "agora temos tudo para executar os testes?"
A implementação do teste inclui principalmente as seguintes atividades:

  * Desenvolver e priorizar os procedimentos de teste e, potencialmente, criar os scripts de teste automatizados;
  * Criar as suítes de teste a partir dos procedimentos de teste e (se houver) os scripts de teste automatizados;
  * Organizar os conjuntos de testes dentro de um cronograma de maneira que resulte em maior eficiência a execução dos testes (ver capítulo 5.2.4);
  * Construir o ambiente de teste (incluindo, potencialmente, estrutura de teste, virtualização de serviços, simuladores e outros itens de infraestrutura), e          verificando se tudo o que é necessário foi configurado corretamente;
  * Preparar os dados de teste e garantir que eles sejam carregados corretamente no ambiente de teste;
  * Verificar e atualizar a rastreabilidade bidirecional entre a base de teste, as condições de teste, os casos de teste, procedimentos de teste e suítes de teste (ver capítulo 1.4.4).

## Execução do Teste

A execução do teste inclui principalmente as seguintes atividades:

  * Gravar os identificadores e versões do(s) item(ns) de teste ou do objeto de teste, da(s) ferramenta(s) de teste e testware;
  * Executar os testes manualmente ou usando ferramentas de execução do teste;
  * Comparar os resultados reais com os resultados esperados;
  * Analisar as anomalias para estabelecer suas prováveis causas;
  * Comunicar os defeitos com base nas falhas observadas;
  * Registrar o resultado da execução do teste (p. ex., passar, falhar, bloquear);
  * Repetir as atividades de teste como resultado de uma ação tomada por uma anomalia, ou como parte do planejado para o teste (p. ex., execução de um teste            corrigido, teste de confirmação ou teste de regressão);
  * Verificar e atualizar a rastreabilidade bidirecional entre a base de teste, as condições de teste, os casos de teste, os procedimentos de teste e os resultados   de teste.

## Conclusão do Teste

As atividades de conclusão do teste coletam os dados das atividades de teste já concluídas para consolidar a experiência, o testware e qualquer outra informação relevante. As atividades de conclusão do teste ocorrem nos marcos do projeto, como quando um sistema de software é lançado, um projeto de teste é concluído (ou cancelado), uma iteração de projeto ágil é concluída (p. ex., como parte de uma reunião retrospectiva), um nível de teste é concluído ou uma liberação de manutenção foi concluída.

A conclusão do teste inclui principalmente as seguintes atividades:

- >  Verificar se todos os relatórios de defeitos estão fechados, inserindo as solicitações de mudança ou itens de lista não processada do produto para quaisquer       defeitos que não foram resolvidos no final da execução do teste;
- >  Criar um relatório de resumo de teste para ser comunicado aos stakeholders;
- >  Finalizar e arquivar o ambiente de teste, os dados de teste, a infraestrutura de teste e outros
   testwares para posterior reutilização;
- >  Entregar o testware para as equipes de manutenção, outras equipes de projeto ou
   stakeholders que poderiam se beneficiar de seu uso;
- >  Analisar as lições aprendidas das atividades de teste concluídas para determinar as alterações
    necessárias para futuras iterações, releases e projetos;
- >  Usar as informações coletadas para melhorar a maturidade do processo de teste.

## Mentalidade do Testador

Os desenvolvedores e testadores geralmente pensam de forma diferente. O objetivo principal do desenvolvimento é projetar e construir um produto. Como discutido anteriormente, os objetivos do teste incluem verificar e validar o produto, encontrar os defeitos antes da liberação e assim por diante. Estes são conjuntos diferentes de objetivos que requerem diferentes mentalidades. Reunir essas mentalidades ajuda a alcançar um nível mais alto de qualidade do produto.

























