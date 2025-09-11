# Cenário de Análise/Problema

> **_NOTE:_**: A equipe deve pensar em cenários existentes na atualidade (que causam problemas para os usuários) e que a interface prevista ajudará a resolver o problema. Cenário de Análise/Problema é uma história triste. Não descreve a solução. Descreve somente o problema.

## Cenário de Análise/Problema

**Atores**: Antônio (Administrador do Metrô), Marcos (Analista de Dados do Metrô) e Carla (Operadora de Câmeras do Metrô).

No centro de operações do Metrô de São Paulo, o Analista de Dados Marcos está em uma corrida contra o tempo. O Administrador Antônio, que toma as decisões estratégicas da empresa, precisa urgentemente de um relatório sobre o fluxo de passageiros nas estações da Linha 3-Vermelha para justificar investimentos e alocar recursos humanos para o próximo trimestre.

Marcos tem o objetivo de entregar a análise completa e precisa, mas enfrenta uma série de obstáculos. O sistema de visão computacional gera os dados brutos de contagem e reidentificação, mas ele precisa solicitá-los ao time de infraestrutura para acessá-los. Ele não tem acesso direto a essas informações. Depois de receber os dados, Marcos usa softwares externos como planilhas e scripts para processar e cruzar os dados. Esse processo manual não é eficiente e costuma levar dias para ser concluído, além de ser propenso a erros de digitação e inconsistências que comprometem a qualidade do relatório final.

Enquanto isso, em uma sala de monitoramento, a Operadora de Câmeras Carla tem a missão de garantir a segurança. Ela recebeu a denúncia de que um grupo de vendedores ambulantes ilegais está atuando em uma estação específica. Embora o sistema de visão computacional consiga rastrear a movimentação de pessoas, Carla não tem uma interface visual que permita monitorar as câmeras em tempo real e de forma unificada. Para saber o que está acontecendo, ela depende da equipe de operações para puxar manualmente as imagens das câmeras. Esse processo de comunicação e espera é demorado, prejudicando a agilidade para tomar medidas contra a atividade ilegal. Além disso, Carla também precisa configurar novas câmeras que foram instaladas. Ela tem que usar linhas de comando no terminal para adicionar cada câmera ao sistema e não tem um feedback visual imediato para saber se a configuração funcionou, o que a faz perder tempo verificando logs de dados.

O Administrador Antônio está no seu escritório aguardando o relatório de Marcos. Ele não consegue visualizar o progresso da análise e tem que se comunicar com Marcos por e-mail, solicitando atualizações. Ele também precisa justificar os investimentos em segurança para a diretoria, mas não tem como saber o quão eficiente a equipe de Carla está sendo. Ele gostaria de ver os resultados de segurança consolidados, como a quantidade de atividades ilegais detectadas, em um painel simples e claro. A ausência de uma plataforma centralizada o impede de tomar decisões rápidas e baseadas em dados em tempo real.

## Questões de Refinamento

1. Por que o Administrador Antônio precisa do relatório? Qual o impacto se ele não for entregue a tempo?
2. Quais as precondições para que o Analista de Dados Marcos possa iniciar sua análise?
3. Como Marcos processa os dados brutos atualmente? Quais as ferramentas e passos envolvidos?
4. Que erros podem ocorrer durante a manipulação manual dos dados? Como ele os resolve?
5. De quem a Operadora Carla depende para conseguir as imagens das câmeras e fazer as configurações?
6. Que informações Carla gostaria de ver na tela para identificar os vendedores ambulantes mais rapidamente?
7. Como Carla adiciona novas câmeras ao sistema hoje? Como ela configura as permissões?
8. Como Carla avalia se uma configuração de câmera foi bem-sucedida? Existe algum feedback visual?
9. Onde e quando a atividade de Marcos e Carla ocorre? Existem pressões de tempo?
10. Como o Administrador Antônio monitora o progresso do relatório de Marcos? E como ele avalia o trabalho da equipe de Carla?
11. Que tipo de informação o Administrador Antônio precisa para justificar o investimento em segurança para a diretoria?

## Refinamento do Cenário Análise/Problema
1. O Administrador Antônio precisa do relatório para tomar decisões estratégicas, como justificar o orçamento e a alocação de recursos humanos. O atraso na entrega impacta diretamente o planejamento operacional, podendo resultar em estações superlotadas em horários de pico e diminuir a experiência do passageiro.
2. A principal precondição é que o time de infraestrutura tenha processado e liberado os dados brutos para ele. A falta de integração dos sistemas exige que Marcos espere a equipe técnica fornecer as informações, o que nem sempre ocorre em tempo hábil.
3. Marcos usa scripts para exportar os dados do banco de dados para arquivos CSV. Em seguida, utiliza o Microsoft Excel para criar tabelas dinâmicas e gráficos, cruzando manualmente informações de diferentes arquivos.
4. Os erros mais comuns são a perda de dados durante a exportação ou falhas no cruzamento de informações nas planilhas, o que gera relatórios inconsistentes. Para resolver, ele precisa refazer todo o processo manualmente, consumindo ainda mais tempo.
5. Carla depende do time de operações ou do próprio Marcos para puxar as imagens e as informações do banco de dados. Ela envia um e-mail com a solicitação e aguarda a resposta, o que não é ideal para situações que exigem agilidade.
6. Carla gostaria de ver um feed em tempo real de câmeras específicas, a capacidade de buscar por um indivíduo suspeito e ver seu histórico de movimentação em tempo real.
7. Atualmente, Carla usa comandos de terminal para adicionar o identificador da nova câmera e suas coordenadas ao banco de dados. Ela também precisa usar uma ferramenta de terceiros para configurar as permissões de acesso, pois não existe uma interface única para isso.
8. A única forma de Carla saber se a configuração foi bem-sucedida é verificando o log de dados. Não há um feedback visual imediato no terminal, como um status de 'online' ou uma prévia do vídeo, o que a impede de fazer a avaliação de forma rápida.
9. Marcos trabalha em um ambiente de escritório, sob pressão para cumprir prazos da gerência. Carla atua em uma sala de monitoramento, onde a pressão é para tomar decisões rápidas em situações de segurança.
10. Antônio monitora o progresso de Marcos por meio de comunicações manuais, como e-mails e reuniões, pois não tem uma ferramenta para acompanhar o status da análise. Ele também não consegue avaliar a eficiência da equipe de Carla em tempo real, já que não tem acesso a painéis de segurança consolidados ou a dados sobre atividades ilegais.
11. Antônio precisa de métricas claras e consolidadas, como a quantidade de atividades ilegais detectadas e a eficácia das intervenções. A ausência de dashboards e relatórios consolidados em uma interface única dificulta seu trabalho de justificar o investimento.

No centro de operações do Metrô de São Paulo, o Analista de Dados Marcos está em uma corrida contra o tempo. O Administrador Antônio, que toma as decisões estratégicas da empresa, precisa urgentemente de um relatório sobre o fluxo de passageiros nas estações da Linha 3-Vermelha para justificar investimentos e alocar recursos humanos para o próximo trimestre [1].

Marcos tem o objetivo de entregar a análise completa e precisa, mas enfrenta uma série de obstáculos. O sistema de visão computacional gera os dados brutos de contagem e reidentificação, mas ele precisa solicitá-los ao time de infraestrutura para acessá-los. Ele não tem acesso direto a essas informações [2]. Depois de receber os dados, Marcos usa softwares externos como planilhas e scripts para processar e cruzar os dados [3]. Esse processo manual não é eficiente e costuma levar dias para ser concluído, além de ser propenso a erros de digitação e inconsistências que comprometem a qualidade do relatório final [4].

Enquanto isso, em uma sala de monitoramento, a Operadora de Câmeras Carla tem a missão de garantir a segurança. Ela recebeu a denúncia de que um grupo de vendedores ambulantes ilegais está atuando em uma estação específica. Embora o sistema de visão computacional consiga rastrear a movimentação de pessoas, Carla não tem uma interface visual que permita monitorar as câmeras em tempo real e de forma unificada. Para saber o que está acontecendo, ela depende da equipe de operações para puxar manualmente as imagens das câmeras [5]. Esse processo de comunicação e espera é demorado, prejudicando a agilidade para tomar medidas contra a atividade ilegal. Além disso, Carla também precisa configurar novas câmeras que foram instaladas. Ela tem que usar linhas de comando no terminal para adicionar cada câmera ao sistema e não tem um feedback visual imediato para saber se a configuração funcionou, o que a faz perder tempo verificando logs de dados [7, 8].

O Administrador Antônio está no seu escritório aguardando o relatório de Marcos [9]. Ele não consegue visualizar o progresso da análise e tem que se comunicar com Marcos por e-mail, solicitando atualizações [10]. Ele também precisa justificar os investimentos em segurança para a diretoria, mas não tem como saber o quão eficiente a equipe de Carla está sendo. Ele gostaria de ver os resultados de segurança consolidados, como a quantidade de atividades ilegais detectadas, em um painel simples e claro [11]. A ausência de uma plataforma centralizada o impede de tomar decisões rápidas e baseadas em dados em tempo real.
