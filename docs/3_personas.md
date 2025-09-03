# Personas

## Público-alvo

O projeto é direcionado principalmente para organizações de transporte público urbano (nesse caso, especificamente o Metrô de São Paulo). Foi feita uma análise de expansão do projeto, e ele também pode alcançar como público alvo grandes centros movimentados (como shoppings, ou centros automotivos), pois criaria uma base de dados de fluxo baseado nas câmeras espalhadas pelo ambiente, e facilitaria a otimização da alocação de recursos operacionais, baseado na análise desses dados, similar ao Metrô.

## Personas

### Administrador do Metrô
O Administrador é um profissional de nível gerencial, com idade entre 35 e 55 anos, ensino superior completo (geralmente em administração, engenharia ou gestão de transportes). Atua em um contexto de alta responsabilidade, tomando decisões estratégicas sobre alocação de recursos, manutenção do sistema, segurança dos passageiros e liderança de funcionários. Ele geralmente pertence a classe média, inserido em ambiente corporativo e de políticas públicas. É focado em resultados e em relatórios que sustentem decisões de médio e longo prazo para seus superiores. Para utilizar o sistema de controle de câmeras e fluxo, ele geralmente acessa dashboards, relatórios consolidados com os dados gerados a partir da captura de passageiros, justificar investimentos e organizar recursos humanos e técnicos, históricos de ações (para saber o que os analistas estão fazendo no sistema) e logs de captura de passageiros. Suas informações que precisam ser guardadas no sistema sã: credenciais de login (que serão definidas préviamente), permissões de acesso (nível administrativo), relatórios gerados e histórico de decisões registradas no sistema.

<img width="200" height="300" alt="image" src="https://github.com/user-attachments/assets/7775d20f-1dd2-4255-98a3-a4162d884349" />

### Analista de dados do Metrô
O analista de dados é um profissional técnico (25 a 40 anos), com formação em estatística, ciência de dados ou TI. Trabalha diretamente com os dados gerados pelo sistema, transformando-os em relatórios e insights para a administração e seus superiores. Ele geralmente é de classe média, com perfil altamente analítico e rotina voltada ao uso de ferramentas digitais para análise de dados. Acostumado a lidar com grandes volumes de informação e preocupado com a precisão e clareza dos dados. No sistema, ele foca mais na parte técnica da tela de Dashboards, como exportar dados, gerar dashboards personalizáveis, acompanhar indicadores em tempo real e elaborar relatórios que criam motivo para tomadas de decisões estratégicas e operacionais. Seus dados que precisam ser armazenados: credenciais de login no sistema, configurações de relatórios/dashboards e logs de acesso e atividades de análise realizadas.

<img width="500" height="280" alt="image" src="https://github.com/user-attachments/assets/572b9fa1-1e49-414e-b874-8b8397962201" />

### Operador de câmeras do Metrô
O operador é um funcionário operacional (25 a 50 anos), ensino médio ou técnico, responsável por monitorar em tempo real as imagens capturadas nas estações. Atua na linha de frente da segurança, interagindo diretamente com o sistema de vigilância. É geralmente de classe baixa, com forte pressão do ambiente de trabalho (grande volume de pessoas, situações de risco, necessidade de atenção constante e alta cobrança de seus superiores). Seu principal trabalho com o sistema é acompanhar a interface de câmeras em tempo real, além de inicializá-las no início do dia. Dados a serem salvos: credenciais de login, logs de monitoramento e ações no sistema e registro de câmeras configuradas sob sua responsabilidade.

<img width="500" height="310" alt="image" src="https://github.com/user-attachments/assets/21bdccd8-26e3-4f6d-96bf-b4c0e2e2d1a3" />

### Outras personas (secundárias)
- Público de passageiros do Metrô.
- Outros funcionários do Metrô (seguranças, operadores de bilheteria, time de manutenção, etc).

<img width="500" height="280" alt="image" src="https://github.com/user-attachments/assets/20c84986-0f71-4212-b943-c7a4fa22dd11" />
<br><br>
<img width="500" height="310" alt="image" src="https://github.com/user-attachments/assets/fd87f5db-1cc5-4d66-a3c6-a64961c40ad0" />

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

José chega cedo ao centro de controle do Metrô de São Paulo. Ele é operador há alguns anos e já conhece bem a rotina, mas desde que o novo sistema de monitoramento foi implantado, seu trabalho ficou mais ágil e organizado. Assim que se acomoda em sua estação de trabalho, José liga o computador, abre o navegador e acessa o sistema. Digita seu e-mail e senha, confirmando o login. Em poucos segundos, a tela inicial aparece, mostrando as opções disponíveis. Ele sente uma sensação de segurança: sabe que todo o seu trabalho ficará registrado e poderá ser consultado depois. <br>
A primeira tarefa de José é monitorar as câmeras. Ele acessa a interface de câmeras e abre o menu dropdown. Escolhe a câmera da entrada principal da estação e clica em “inicializar câmera”. Ao incializar, a câmera liga e começa a capturar as pessoas que ali passam. Em seguida, repete o processo com as demais, garantindo que cada ponto crítico esteja ativo. Ao ver as imagens em tempo real, José se concentra, atento a qualquer movimento fora do normal.
Com as câmeras em funcionamento, José decide verificar como foi o dia anterior. Ele navega até a tela de dashboard, onde os gráficos já começam a ser gerados automaticamente. Ajusta os filtros para visualizar o fluxo de passageiros do último dia e observa os picos de movimento, dentro da estação em que trabalha e entre as estações do Metrô de São Paulo. Em seguida, gera um gráfico detalhado e exporta um relatório em PDF, que seu computador faz download automaticamente. Esse documento será enviado mais tarde para a equipe de gestão, que usa as informações para tomar decisões sobre alocação de trens e pessoal. <br>
Pouco depois, José recebe um aviso interno: uma das câmeras da linha azul, a câmera X, foi reposicionada após manutenção. Ele acessa a tela de configuração, localiza a câmera no sistema e atualiza os dados — ajusta a identificação e salva a alteração. Agora o sistema reflete a nova disposição física da estação, dando um aviso para José que sua ação foi bem sucedida.
Para finalizar sua rotina, José acessa a tela de histórico. Ali, encontra o registro completo de suas ações: o horário em que fez login, as câmeras que inicializou, o relatório que gerou e a configuração que alterou. Isso lhe dá tranquilidade, pois sabe que, se alguém precisar conferir, haverá um rastro claro e organizado de tudo que foi feito, e que seus superiores terão controle do seu trabalho no dia.
Antes de encerrar o turno, José desliga as câmeras na página de Inteface de câmera, encerrando a captura de imagem, fecha o sistema e faz logout. Ele se levanta satisfeito, certo de que cumpriu seu papel: monitorar, analisar e registrar.

[1] Fonte: Adaptado de <https://hazeshift.com.br/mapa-de-empatia/>
