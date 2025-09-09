# Cenário de Análise/Problema

> **_NOTE:_**: A equipe deve pensar em cenários existentes na atualidade (que causam problemas para os usuários) e que a interface prevista ajudará a resolver o problema. Cenário de Análise/Problema é uma história triste. Não descreve a solução. Descreve somente o problema.

## Cenário de Análise/Problema

### Atores: 
Marcos (Analista de Dados do Metrô-SP), Carla (Gerente de Segurança do Metrô-SP) e Ricardo (Técnico de Infraestrutura).

Na sede administrativa do Metrô de São Paulo, o analista Marcos tem uma tarefa crucial: gerar um relatório mensal sobre o fluxo de passageiros nas estações da Linha 3-Vermelha para a diretoria [1, 2]. O objetivo é identificar os horários de pico e a superpopulação em determinadas plataformas para realocar funcionários e otimizar as escalas [3].

Atualmente, o sistema de visão computacional gera dados brutos sobre a contagem de pessoas e reidentificação, mas eles são salvos diretamente em um banco de dados central [4]. Marcos precisa solicitar os dados ao time de infraestrutura e, após recebê-los, usar ferramentas externas como scripts e planilhas para processar, organizar e cruzar as informações [5]. Esse processo, que deveria levar poucas horas, se estende por vários dias. Ele frequentemente comete erros manuais ao exportar e manipular grandes volumes de dados [6], e a falta de uma visualização clara dos resultados torna a análise muito mais lenta e propensa a interpretações equivocadas.

Paralelamente, em outro setor, a gerente de segurança Carla precisa urgentemente identificar e monitorar a presença de vendedores ambulantes ilegais em uma estação específica [7]. As câmeras de segurança capturam as imagens, e o sistema até consegue rastrear os indivíduos, mas a falta de uma interface de monitoramento em tempo real a impede de visualizar as informações de forma clara [8]. Para ter acesso a esses dados, ela depende da equipe de operações para puxar as imagens manualmente, o que gera um atraso significativo. Ela não tem como ver o histórico de aparições ou o trajeto de uma pessoa suspeita de forma imediata, o que compromete a agilidade e a eficácia das ações da equipe de segurança.

Ainda, o técnico Ricardo precisa configurar novas câmeras em uma estação recém-inaugurada [9]. Ele tem que usar comandos de terminal ou ferramentas de terceiros para adicionar cada nova câmera ao sistema e configurar suas permissões [10]. Se algo der errado, a depuração se torna complexa, pois não há um histórico de ações no sistema para verificar as alterações [11].

## Questões de Refinamento

1. Por que o relatório é mensal? Qual o impacto se ele não for entregue a tempo?
2. Onde e quando a atividade de Marcos ocorre? Existem pressões de tempo?
3. Quais as precondições para que Marcos possa iniciar sua análise?
4. Que informações são geradas pelo sistema de visão computacional e como elas são acessadas hoje?
5. Como Marcos processa os dados brutos atualmente? Quais as ferramentas e passos envolvidos?
6. Que erros podem ocorrer durante a manipulação manual dos dados? Como ele os resolve?
7. De quem a gerente Carla depende para conseguir as imagens das câmeras?
8. Que informações Carla gostaria de ver na tela para identificar os vendedores ambulantes mais rapidamente?
9. Por que Ricardo precisa configurar novas câmeras? Qual o objetivo dele ao fazer isso?
10. Como Ricardo adiciona novas câmeras ao sistema hoje? Como ele configura as permissões?
11. Como Ricardo avalia se uma configuração de câmera foi bem-sucedida? Existe algum feedback visual?

## Refinamento do Cenário Análise/Problema
1. O relatório é mensal pois a diretoria precisa de dados consolidados para reuniões de planejamento estratégico e para justificar o orçamento. O atraso na entrega impacta a alocação de recursos, podendo resultar em estações superlotadas em horários de pico, diminuindo a experiência do usuário.

2. A análise de Marcos ocorre no seu computador de trabalho, em um ambiente administrativo, normalmente nos primeiros dias úteis de cada mês. Ele enfrenta a pressão de entregar o relatório antes de reuniões com a diretoria.

3. As precondições para a análise são: o time de infraestrutura deve ter processado e liberado os dados brutos para ele, o que nem sempre ocorre em tempo hábil.

4. O sistema gera dados brutos como contagem de pessoas, coordenadas de reidentificação e timestamps. Eles são salvos diretamente em um banco de dados AWS RDS, e para acessá-los, Marcos precisa solicitar a permissão do time de infraestrutura.

5. Marcos usa scripts para exportar os dados do banco de dados para arquivos CSV, e depois usa o Microsoft Excel para criar tabelas dinâmicas e gráficos. Ele precisa cruzar as informações de diferentes arquivos, como dados de contagem de passageiros com as escalas de trens.

6. Os erros mais comuns são a perda de dados durante a exportação ou a falha no cruzamento de informações nas planilhas, o que resulta em relatórios com inconsistências. Para resolver, ele precisa refazer todo o processo manualmente, o que consome ainda mais tempo.

7. Carla depende do time de operações ou do próprio Ricardo para puxar as imagens manualmente. Ela envia um e-mail com a solicitação e aguarda a resposta, o que não é ideal para situações que exigem agilidade.

8. Carla gostaria de ver na tela: um feed em tempo real de câmeras específicas, a capacidade de buscar por um indivíduo suspeito e ver seu histórico de movimentação (por onde ele passou).

9. Ricardo precisa configurar novas câmeras para expandir a cobertura do sistema ou para substituir câmeras que deram problema. O objetivo é garantir que o novo hardware esteja integrado e funcionando corretamente, e que os dados capturados sejam enviados para o sistema principal.

10. Atualmente, Ricardo usa comandos de terminal para adicionar o identificador da nova câmera e suas coordenadas ao banco de dados. Ele precisa usar uma ferramenta de terceiros para configurar as permissões de acesso, pois não existe uma interface única para isso.

11. A única forma de Ricardo saber se a configuração foi bem-sucedida é verificar o log de dados. Não há um feedback visual imediato no terminal, como um status de 'online' ou uma prévia do vídeo capturado pela câmera, o que o impede de fazer a avaliação de forma rápida.
