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


### **Mapa de Empatia – Persona 1: Administrador do Metrô (Carlos)**

**Perfil resumido:** Carlos, 45 anos, é administrador do Metrô. Ele atua em nível gerencial e é responsável por acompanhar a operação, analisar indicadores e tomar decisões estratégicas sobre recursos, segurança e desempenho.

**O que ele vê?**
* Dashboards com indicadores de fluxo de passageiros, segurança e status das câmeras.
* Relatórios detalhados de movimentação e ocorrências.
* Registro das atividades de operadores e analistas.
* Um sistema centralizado que reúne todas as informações.

**O que ele ouve?**
* Pressão da diretoria por resultados claros e justificativas objetivas.
* Feedback dos analistas e operadores sobre suas rotinas.
* Cobranças externas (governo, opinião pública) por segurança e eficiência.
* Conversas internas sobre alocação de recursos e incidentes em estações críticas.

**O que ele pensa e sente?**
* Sente-se seguro quando vê transparência e rastreabilidade no sistema.
* Tem confiança em tomar decisões quando as informações estão organizadas.
* Preocupa-se em justificar investimentos para garantir recursos.
* Valoriza soluções que otimizam tempo e diminuem riscos.
* Busca a tranquilidade de que tudo ficará registrado para consulta futura.

**O que ele fala e faz?**
* Relata para a diretoria dados objetivos para apoiar solicitações de recursos.
* Reforça a importância de relatórios consolidados e rastreáveis.
* Solicita melhorias baseadas em dados (ex.: reforço de segurança em estação crítica).
* Cobra responsabilidade e cumprimento de funções da equipe.
* Compartilha a importância da centralização de informações.

**Dores (Medos, Obstáculos)**
* Ter que tomar decisões sem dados confiáveis.
* Falta de transparência ou relatórios incompletos da equipe.
* Exposição a críticas em caso de falhas de segurança ou operação.
* Sobrecarga de informações difíceis de interpretar.
* Dificuldade em demonstrar a necessidade de recursos sem dados sólidos.

**Ganhos (Necessidades, Benefícios esperados)**
* Relatórios rápidos, claros e consolidados, prontos para a diretoria.
* Dashboards intuitivos, que mostrem indicadores essenciais sem sobrecarga.
* Histórico rastreável de decisões e atividades (transparência).
* Base sólida para justificar recursos e investimentos.
* Tranquilidade e confiança de que suas decisões estão documentadas e bem fundamentadas.

### **Mapa de Empatia – Persona 2: Analista de Dados do Metrô (Mariana)**

**Perfil resumido:** Mariana, 32 anos, é analista de dados. Ela trabalha diariamente com dashboards, relatórios e dados brutos do sistema. Seu foco é gerar insights confiáveis para apoiar gestores e garantir que a operação do metrô seja eficiente e baseada em evidências.

**O que ela vê?**
* Dashboards em tempo real com fluxo de passageiros e alertas de ocorrências.
* Gráficos atualizados que podem ser personalizados com filtros.
* Relatórios exportados em PDF e planhas para análises externas.
* Logs de atividades que registram cada ação.

**O que ela ouve?**
* Demandas do administrador e da diretoria por relatórios claros.
* Feedback da equipe sobre a necessidade de análises mais rápidas.
* Conversas técnicas com colegas sobre integrações e ferramentas externas.
* Reconhecimento quando suas análises embasam decisões estratégicas.

**O que ela pensa e sente?**
* Sente-se responsável pela qualidade e confiabilidade dos dados.
* Tem satisfação quando vê que seu trabalho ajuda nas decisões estratégicas.
* Busca eficiência, evitando retrabalho em relatórios.
* Pode sentir pressão ao lidar com grande volume de dados em pouco tempo.
* Valoriza sistemas que oferecem flexibilidade e personalização.

**O que ela fala e faz?**
* Gera relatórios comparativos para identificar tendências.
* Solicita melhorias em filtros e exportações para facilitar o trabalho.
* Reforça a importância da rastreabilidade e padronização dos dados.
* Compartilha insights sobre padrões de fluxo e falhas técnicas.
* Usa ferramentas externas de estatística para análises mais avançadas.

**Dores (Medos, Obstáculos)**
* Dados inconsistentes que comprometam a análise.
* Limitações no sistema para cruzar variáveis complexas.
* Perda de tempo com relatórios manuais ou mal configurados.
* Risco de que suas análises não sejam valorizadas pela gestão.
* Sobrecarga de trabalho em horários de pico de demandas.

**Ganhos (Necessidades, Benefícios esperados)**
* Dashboards altamente configuráveis e salvos automaticamente.
* Exportações rápidas e completas para diferentes formatos.
* Logs transparentes, que garantem confiança no processo.
* Facilidade para cruzar dados complexos sem depender de soluções externas.
* Reconhecimento profissional por entregar informações de qualidade.
* Sensação de dever cumprido ao fornecer relatórios claros e úteis.

### **Mapa de Empatia – Persona 3: Operador de Câmeras do Metrô (João)**

**Perfil resumido:** João, 38 anos, é operador do centro de controle. Sua função é monitorar as câmeras em tempo real, registrar ocorrências e manter os equipamentos em pleno funcionamento. Ele é o “olho da operação” no dia a dia, garantindo segurança e rastreabilidade.

**O que ele vê?**
* Interface do sistema de câmeras em tempo real.
* Notificações sobre ocorrências ou mudanças de configuração.
* Painel de inicialização e atualização dos equipamentos.
* Histórico de atividades realizadas durante o turno.

**O que ele ouve?**
* Alertas da equipe de segurança pedindo atenção em determinadas áreas.
* Orientações de supervisores sobre câmeras críticas.
* Comunicação entre colegas de turno durante a troca de plantão.
* Feedback sobre a importância de registrar cada ocorrência corretamente.

**O que ele pensa e sente?**
* Sente-se responsável pela segurança imediata dos passageiros.
* Confia no sistema porque sabe que suas ações ficam registradas (transparência).
* Pode sentir pressão constante, pois qualquer distração pode causar falhas.
* Busca tranquilidade ao confirmar que todas as câmeras estão ativas.
* Tem satisfação em cumprir bem o turno e entregar tudo em ordem ao próximo operador.

**O que ele fala e faz?**
* Inicializa e monitora câmeras diariamente.
* Registra ocorrências no sistema e notifica a segurança.
* Atualiza identificações de câmeras após manutenção.
* Compartilha informações relevantes durante a troca de turno.
* Reforça para colegas a importância de manter os registros precisos.

**Dores (Medos, Obstáculos)**
* Falha em uma câmera crítica durante seu turno.
* Sobrecarga de atenção, monitorando várias telas ao mesmo tempo.
* Sistema lento para registrar ocorrências em situações urgentes.
* Ser responsabilizado por algo que não estava sob seu controle.
* Comunicação falha entre operadores em trocas de plantão.

**Ganhos (Necessidades, Benefícios esperados)**
* Sistema rápido e confiável, que não trave em situações críticas.
* Histórico completo e transparente, protegendo sua atuação.
* Interface clara, com alertas visuais fáceis de identificar.
* Integração fluida com a equipe de segurança, reduzindo o tempo de resposta.
* Sensação de dever cumprido ao encerrar o turno com tudo registrado e em ordem.
 
- Determine o mapa de empatia[1] de pelo menos uma persona primária e uma sercundária.

# Contexto de uso

O sistema será utilizado principalmente nas estações do Metrô de São Paulo e em seus centros de monitoramento, ambientes caracterizados por um fluxo intenso e contínuo de passageiros. No nível operacional, os operadores de câmeras utilizam o sistema em salas de controle para acompanhar imagens em tempo real e responder a situações de segurança. Já no nível analítico e gerencial, analistas de dados e administradores acessam dashboards, relatórios e históricos em ambientes administrativos para planejar recursos, organizar escalas e otimizar a operação do transporte. Esse contexto envolve fatores sociais, econômicos e culturais complexos: o metrô atende milhões de pessoas diariamente, em sua maioria trabalhadores e estudantes de classes média e baixa. Além disso, existe uma forte preocupação com eficiência operacional, redução de custos e aumento da segurança, tanto para proteger os passageiros quanto para monitorar e proibir certas atividades ilegais dentro das estações.
Antes de iniciar a interação, o sistema precisa guardar informações cruciais do ambiente, como a configuração das câmeras (identificador, localização e estação), credenciais e permissões dos usuários e dados de históricos de ações anteriores no sistema e dados. Durante a interação, o ambiente está em constante movimento, com milhares de passageiros circulando pelas estações a cada hora. Enquanto isso, os operadores monitoram eventos em tempo real com os logs de captura de passageiros, os analistas de dados transformam dados em relatórios e administradores utilizam esses resultados para embasar decisões estratégicas.

# Jornada do usuário

### Administrador do Metrô
Carlos chega cedo ao seu escritório na sede administrativa do Metrô. Como administrador, ele tem a responsabilidade de acompanhar os resultados da operação e tomar decisões estratégicas. Liga o computador, abre o navegador e acessa o sistema. Digita suas credenciais administrativas e, em poucos segundos, a tela inicial aparece. Ele vê o dashboard principal com indicadores de fluxo de passageiros, segurança e status das câmeras. Sua primeira ação é consultar os relatórios consolidados do dia anterior. Ele ajusta os filtros, seleciona o intervalo de tempo desejado e observa os gráficos com os picos de movimentação e registros de ocorrências. Em seguida, gera um relatório detalhado e salva no sistema. Esse documento será usado em uma reunião de diretoria, servindo de justificativa para solicitação de novos recursos.
Após isso, Carlos acessa o módulo de histórico. Lá, verifica os registros de atividade dos analistas e operadores, confirmando que o time está cumprindo suas funções. Ele se sente mais seguro, pois sabe que cada ação está registrada, e isso garante transparência e responsabilidade. Antes de encerrar sua rotina, Carlos acessa a área de decisões, onde registra sua análise sobre a necessidade de reforço de segurança em uma estação crítica. Salva o parecer dentro do sistema, que automaticamente vincula o documento ao relatório que serviu como base. Ao sair do sistema, Carlos tem a tranquilidade de que todas as informações ficaram centralizadas, organizadas e disponíveis para consulta futura.

### Analista de dados do Metrô
Mariana inicia o dia abrindo o sistema de monitoramento em sua estação de trabalho. Como analista de dados, sua rotina é intensiva no uso de dashboards e relatórios. Após digitar seu login e senha, acessa a tela de visualização em tempo real. Lá, os gráficos já aparecem atualizados, exibindo a quantidade de passageiros por linha e os alertas de ocorrências. Ela personaliza o dashboard, adicionando filtros específicos para cruzar informações de fluxo em horários de pico com os registros de falhas técnicas. Observa uma tendência de aumento no número de passageiros em duas estações estratégicas e decide gerar um relatório comparativo. O sistema exporta o documento em formato PDF e salva automaticamente em sua pasta de relatórios.
Logo depois, Mariana acessa os dados brutos. Aplica filtros avançados e exporta uma planilha que usará em ferramentas externas de análise estatística. Enquanto trabalha, todas as suas atividades ficam registradas nos logs do sistema, garantindo rastreabilidade. No fim do dia, Mariana acessa novamente seus dashboards e confere se as configurações personalizadas foram salvas corretamente. Fecha o sistema com a sensação de dever cumprido: entregou relatórios claros para a administração e deixou os dados prontos para embasar decisões estratégicas do Metrô.

### Operador de câmeras do Metrô
João chega ao centro de controle do Metrô para assumir seu turno. Ele faz login no sistema e acessa imediatamente a interface de câmeras. Sua primeira tarefa é inicializar os equipamentos sob sua responsabilidade. Passa por cada câmera, seleciona no menu e clica em “inicializar”. Em poucos minutos, todas estão transmitindo imagens em tempo real, cobrindo as áreas críticas da estação. Com as câmeras ativas, João mantém atenção constante às telas. Ao notar uma aglomeração incomum em uma plataforma, registra a ocorrência no sistema e notifica a equipe de segurança. Cada ação realizada fica automaticamente registrada nos logs, o que traz segurança ao operador: sabe que, se alguém precisar conferir, haverá um rastro claro de sua atuação.
Mais tarde, João recebe uma notificação no sistema avisando que uma câmera foi reposicionada após manutenção. Ele acessa o painel de configuração, atualiza a identificação da câmera e salva a mudança. O sistema confirma a alteração e João segue monitorando o restante do turno. Antes de encerrar o expediente, João acessa o histórico de suas ações: visualiza o horário do login, as câmeras que inicializou, a ocorrência registrada e a atualização feita. Fecha o sistema, faz logout e passa o plantão para o próximo operador. Sai satisfeito, certo de que cumpriu seu papel de manter a segurança e o registro das atividades sob controle.

[1] Fonte: Adaptado de <https://hazeshift.com.br/mapa-de-empatia/>
