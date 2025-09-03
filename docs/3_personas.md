# Personas

## Público-alvo

O projeto é direcionado principalmente para organizações de transporte público urbano (nesse caso, especificamente o Metrô de São Paulo). Foi feita uma análise de expansão do projeto, e ele também pode alcançar como público alvo grandes centros movimentados (como shoppings, ou centros automotivos), pois criaria uma base de dados de fluxo baseado nas câmeras espalhadas pelo ambiente, e facilitaria a otimização da alocação de recursos operacionais, baseado na análise desses dados, similar ao Metrô.

## Personas

### Administrador do Metrô
O Administrador é um profissional de nível gerencial, com idade entre 35 e 55 anos, ensino superior completo (geralmente em administração, engenharia ou gestão de transportes). Atua em um contexto de alta responsabilidade, tomando decisões estratégicas sobre alocação de recursos, manutenção do sistema, segurança dos passageiros e liderança de funcionários. Ele geralmente pertence a classe média, inserido em ambiente corporativo e de políticas públicas. É focado em resultados e em relatórios que sustentem decisões de médio e longo prazo para seus superiores. Para utilizar o sistema de controle de câmeras e fluxo, ele geralmente acessa dashboards, relatórios consolidados com os dados gerados a partir da captura de passageiros, justificar investimentos e organizar recursos humanos e técnicos, históricos de ações (para saber o que os analistas estão fazendo no sistema) e logs de captura de passageiros. Suas informações que precisam ser guardadas no sistema sã: credenciais de login (que serão definidas préviamente), permissões de acesso (nível administrativo), relatórios gerados e histórico de decisões registradas no sistema.

### Analista de dados do Metrô
O analista de dados é um profissional técnico (25 a 40 anos), com formação em estatística, ciência de dados ou TI. Trabalha diretamente com os dados gerados pelo sistema, transformando-os em relatórios e insights para a administração e seus superiores. Ele geralmente é de classe média, com perfil altamente analítico e rotina voltada ao uso de ferramentas digitais para análise de dados. Acostumado a lidar com grandes volumes de informação e preocupado com a precisão e clareza dos dados. No sistema, ele foca mais na parte técnica da tela de Dashboards, como exportar dados, gerar dashboards personalizáveis, acompanhar indicadores em tempo real e elaborar relatórios que criam motivo para tomadas de decisões estratégicas e operacionais. Seus dados que precisam ser armazenados: credenciais de login no sistema, configurações de relatórios/dashboards e logs de acesso e atividades de análise realizadas.

### Operador de câmeras do Metrô
O operador é um funcionário operacional (25 a 50 anos), ensino médio ou técnico, responsável por monitorar em tempo real as imagens capturadas nas estações. Atua na linha de frente da segurança, interagindo diretamente com o sistema de vigilância. É geralmente de classe baixa, com forte pressão do ambiente de trabalho (grande volume de pessoas, situações de risco, necessidade de atenção constante e alta cobrança de seus superiores). Seu principal trabalho com o sistema é acompanhar a interface de câmeras em tempo real, além de inicializá-las no início do dia. Dados a serem salvos: credenciais de login, logs de monitoramento e ações no sistema e registro de câmeras configuradas sob sua responsabilidade.

### Outras personas (secundárias)
- Público de passageiros do Metrô.
- Outros funcionários do Metrô (seguranças, operadores de bilheteria, time de manutenção, etc).

# Mapa de empatia

![Mapa de empatia](imagens/empatia.png)

- Determine o mapa de empatia[1] de pelo menos uma persona primária e uma sercundária.
  - O que o usuário vê: aqui estamos falando do ambiente visual em que o usuário se encontra. Ou seja, o que ele efetivamente enxerga, as pessoas e objetos que estão ao seu redor. Isso ajuda a entender o contexto em que o usuário está inserido e as influências visuais que está recebendo.
  - O que o usuário ouve: neste quadrante, buscamos entender o que o usuário está ouvindo, os sons que o cercam e como eles influenciam suas ações.
  - O que o usuário diz e faz: aqui consideramos ações e comportamentos que o usuário apresenta durante sua interação com serviço ou poduto.
  - O que o usuário pensa e sente: neste quadrante, buscamos entender os pensamentos, sentimentos, emoções e percepções que o usuário tem em relação ao serviço ou poduto. Quais expectativas o usuário cria sobre o serviço ou poduto?
  Que tipo de serviço ou poduto mais agrada essa persona?
  - Dores: quando falamos sobre dores do usuário, estamos fazendo referência a quaisquer obstáculos, necessidades ou frustrações que o usuário possa experimentar ao tentar realizar uma tarefa ou alcançar um objetivo. Isso inclui, por exemplo, problemas de usabilidade, dificuldades de acesso ou outros desafios que podem afetar a experiência do usuário.
  - Ganhos: nesse caso estamos falando de quaisquer benefícios ou recompensas que o usuário possa experimentar ao utilizar o serviço ou poduto. Isso pode incluir economia de tempo ou facilidade de uso, por exemplo. Que desejos do usuário o serviço ou poduto satisfaz?

# Contexto de uso

O sistema será utilizado principalmente nas estações do Metrô de São Paulo e em seus centros de monitoramento, ambientes caracterizados por um fluxo intenso e contínuo de passageiros. No nível operacional, os operadores de câmeras utilizam o sistema em salas de controle para acompanhar imagens em tempo real e responder a situações de segurança. Já no nível analítico e gerencial, analistas de dados e administradores acessam dashboards, relatórios e históricos em ambientes administrativos para planejar recursos, organizar escalas e otimizar a operação do transporte. Esse contexto envolve fatores sociais, econômicos e culturais complexos: o metrô atende milhões de pessoas diariamente, em sua maioria trabalhadores e estudantes de classes média e baixa. Além disso, existe uma forte preocupação com eficiência operacional, redução de custos e aumento da segurança, tanto para proteger os passageiros quanto para monitorar e proibir certas atividades ilegais dentro das estações.
Antes de iniciar a interação, o sistema precisa guardar informações cruciais do ambiente, como a configuração das câmeras (identificador, localização e estação), credenciais e permissões dos usuários e dados de históricos de ações anteriores no sistema e dados. Durante a interação, o ambiente está em constante movimento, com milhares de passageiros circulando pelas estações a cada hora. Enquanto isso, os operadores monitoram eventos em tempo real com os logs de captura de passageiros, os analistas de dados transformam dados em relatórios e administradores utilizam esses resultados para embasar decisões estratégicas.

# Jornada do usuário

- Criar uma narrativa para o o seu serviço ou poduto com o usuário.
- Determine o que o usuário realiza desde a primeira até o última interação com o serviço ou poduto.
  - Descreva o que acontece ou pode acontecer passo a passo
  - Como a tarefa começa? Como a tarefa se desenvolve? Como a tarefa termina?




[1] Fonte: Adaptado de <https://hazeshift.com.br/mapa-de-empatia/>
