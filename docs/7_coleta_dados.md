# Coleta de Dados

## 1. Identificação de Necessidades dos Usuários e Requisitos de IHC:

### Que dados coletar?
* **Dados do Usuário:**
  * Dados demográficos e profissionais: Confirmar o cargo atual (Administrador, Analista, Operador), tempo de experiência na função e no Metrô, e área de formação.  
  * Idiomas e jargões: Entender a terminologia específica que eles usam no dia a dia para descrever locais, eventos e operações. 

* **Dados sobre a relação com a tecnologia:**
  * Alfabetismo computacional: Nível de conforto e habilidade no uso de computadores e softwares em geral.
  * Experiência com ferramentas semelhantes: Investigar se já utilizam outros sistemas de dashboard, sistemas de monitoramento por vídeo (CFTV) ou softwares de gestão. Qual o nível de satisfação ou frustração com as ferramentas atuais? 
  * Tecnologia disponível: Entender em que tipo de hardware o sistema será usado (tamanho e quantidade de monitores, tipo de computador).

* **Dados sobre o conhecimento do domínio:**
  * Avaliar o nível de profundidade do conhecimento sobre a operação do Metrô, gestão de fluxo e protocolos de segurança.
 
* **Dados sobre as tarefas:**
  * Objetivos e frequência: Quais são os objetivos primários de cada persona ao usar um sistema como este? Com que frequência precisam gerar relatórios, consultar históricos ou monitorar câmeras?
  * Dores e dificuldades atuais: Quais são os maiores obstáculos enfrentados hoje para realizar essas tarefas?
  * Gravidade dos erros: Qual o impacto de um erro ao usar o sistema?
 
* **Dados sobre motivações e valores:**
  * Atitudes: Qual a postura deles em relação a novas tecnologias no ambiente de trabalho? São abertos a mudanças ou preferem métodos já estabelecidos?
  * Valor percebido: O que eles consideram mais valioso em um sistema de interface: agilidade, precisão dos dados, facilidade de uso, capacidade de personalização?

### De quem coletar?
Os dados devem ser coletados primariamente dos usuários finais do sistema, que são as três personas muito bem definidas no seu projeto:

 * Administrador do Metrô (Carlos): Para entender as necessidades estratégicas, a importância dos relatórios consolidados e a visão gerencial.
 * Analista de Dados do Metrô (Mariana): Para compreender as necessidades técnicas de manipulação de dados, personalização de dashboards e exportação de informações.
 * Operador de Câmeras do Metrô (João): Para levantar os requisitos da operação em tempo real, a usabilidade da interface de monitoramento e o registro de ocorrências.

Secundariamente, poderíamos considerar outros como stakeholders, a diretoria do Metrô (que consome os relatórios gerados) ou a equipe de TI (responsável pela manutenção).

## 2. Aspectos Éticos
Sim, o projeto deverá considerar aspectos éticos de forma rigorosa. Qualquer pesquisa envolvendo pessoas, mesmo que para fins técnicos, precisa zelar pelo bem-estar e pelos direitos dos participantes.

* Princípio da Autonomia : Os funcionários do Metrô (participantes) devem dar seu consentimento livre e esclarecido. Eles precisam saber que a participação é para um projeto acadêmico, que os dados serão usados para melhorar uma ferramenta de trabalho e que eles podem se recusar a participar ou desistir a qualquer momento sem qualquer prejuízo profissional.
* Princípio da Não Maleficência e Beneficência : É fundamental garantir que a coleta de dados não causará nenhum dano aos participantes. As respostas sobre dificuldades no trabalho ou falta de habilidade com tecnologia, por exemplo, não podem ser usadas para avaliá-los profissionalmente. O benefício esperado é o desenvolvimento de uma interface mais eficiente e menos estressante, o que melhora a qualidade do trabalho deles (máximo de benefícios, mínimo de danos).
* Privacidade e Confidencialidade: Deve-se garantir que os dados brutos coletados serão confidenciais e que qualquer relatório ou apresentação usará dados de forma anônima e agregada.
* Princípio da Justiça e Equidade: A pesquisa deve ter uma relevância social, que neste caso é a melhoria do sistema de transporte público através de ferramentas mais eficazes para seus operadores e gestores. Os benefícios (uma ferramenta melhor) devem ser compartilhados com os participantes, e o ônus da participação (o tempo dedicado) deve ser minimizado.  

## 3. Ferramentas de Coleta de Dados (três técnicas diferentes)

### 3.1 Nome do instrumento: Questionário de Perfil de Usuário e Priorização de Funcionalidades.
* Objetivo da aplicação:
  * Validar o Perfil: Coletar dados demográficos e técnicos para confirmar e quantificar as características das personas.
  * Mapear Dores Atuais: Entender, em uma escala maior, as principais dificuldades e frustrações dos usuários com os processos e ferramentas atuais.
  * Medir o grau de importância que cada perfil de usuário atribui às funcionalidades propostas para a nova interface.

* Explicar como aplicar:
  * Criação da Ferramenta: O questionário será implementado na plataforma Google Forms, pois é de fácil acesso e permite a exportação dos dados para análise.
  * Teste Piloto: Antes de enviar aos usuários do Metrô, o questionário será testado por 2 ou 3 pessoas da própria equipe do projeto para verificar se as perguntas são claras, se não há erros e se o tempo de preenchimento é adequado (idealmente entre 10-15 minutos).
  * Recrutamento e Contato: O contato com os funcionários do Metrô será feito através do professor orientador ou de um ponto focal dentro da empresa. Será solicitada a distribuição do link para um grupo de funcionários que se enquadrem nos três perfis desejados.
  * Aplicação: Um e-mail ou mensagem de convite será enviado aos participantes. Esta mensagem deve conter:
    * O objetivo do projeto e da pesquisa.
    * O tempo estimado para resposta.
    * O Termo de Consentimento, garantindo anonimato, confidencialidade e o uso dos dados apenas para fins acadêmicos.
    * O link para o questionário.
  * Coleta e Análise: O questionário ficará disponível por um período determinado. Após o encerramento, os dados serão exportados, e as respostas serão segmentadas por perfil de usuário para análise comparativa. 
* Instrumento: https://docs.google.com/forms/d/e/1FAIpQLSdZe7frUYFTtuKlD0lgFdDkp8FblTm7opph0tC6GPYdgpjnUA/viewform?usp=header

### 3.2 Nome do instrumento: Observação Simples.

* Objetivo de Aplicação:
  * Entender o fluxo de trabalho real do usuário, incluindo interrupções e improvisos.
  * Identificar problemas de usabilidade e ineficiências nas ferramentas atuais.
  * Coletar dados contextuais que os usuários muitas vezes esquecem de mencionar em entrevistas.

* Explicar como aplicar:
  * Peça permissão para observar o usuário por um período, garantindo que você não vai atrapalhar e que não se trata de uma avaliação de desempenho.
  * Sente-se ao lado ou um pouco atrás do usuário. Fique em silêncio na maior parte do tempo.
  * Anote suas observações em um caderno ou notebook, seguindo o roteiro de pontos de atenção abaixo. Anote ações, ferramentas utilizadas e qualquer sinal de dúvida ou frustração.

* Instrumento: Roteiro/Checklist de Observação
  * Participantes: 1 ou 2 funcionários com o perfil de Analista de Dados (Mariana) e 1 ou 2 com o perfil de Operador de Câmeras (João).
  * Para a Analista de Dados (Mariana):
    * [ ] Quais softwares ela abre primeiro para começar a tarefa de criar um relatório?
    * [ ] Quantas janelas diferentes ela precisa usar?
    * [ ] Conte quantas vezes ela precisa copiar e colar informações entre diferentes programas.
    * [ ] Anote qualquer momento em que ela pareça confusa, suspire ou demonstre frustração.
    * [ ] Ela precisa contatar outra pessoa para pedir dados ou tirar dúvidas?
    * [ ] Ela usa alguma ferramenta "não oficial" para se organizar?
          
  * Para o Operador de Câmeras (João):
    * [ ] Como é o ambiente físico? Quantas telas ele olha ao mesmo tempo?
    * [ ] Qual é a ação mais repetitiva que ele faz durante o monitoramento?
    * [ ] Quando precisa configurar uma câmera, quais são os primeiros passos que ele toma?
    * [ ] Anote o tempo que leva desde a identificação de um problema até a comunicação com a equipe de segurança.
    * [ ] Ele parece confiante ao usar as ferramentas atuais ou precisa consultar anotações?
    * [ ] Há algum alarme ou notificação visual/sonora? Como ele reage?

 ### 3.3 Nome do instrumento: Sessão de Brainstorming.

* Objetivo de Aplicação:
  * Gerar rapidamente uma lista de funcionalidades desejadas para a nova plataforma.
  * Entender as prioridades dos diferentes usuários de forma colaborativa.
  * Promover um sentimento de participação e co-criação da ferramenta.

* Explicar como aplicar:
  * Reúna o grupo em uma sala com um quadro branco e post-its.
  * O moderador explica o problema central e a regra principal: "Nenhuma ideia é ruim. O objetivo é quantidade, não qualidade neste momento".
  * Siga o roteiro simples abaixo para guiar a sessão.

* Instrumento: Roteiro/Agenda do Brainstorming
  * Participantes: Um grupo misto de 3 a 5 pessoas, incluindo pelo menos um de cada persona (Carlos, Mariana e João).
  1. Introdução e Apresentação do Problema (5 minutos)
    * "Olá a todos, obrigado por virem. Hoje vamos fazer um exercício rápido e criativo. Como sabem, estamos projetando uma nova plataforma para integrar o monitoramento e a análise de dados. O problema que queremos resolver é: a informação está espalhada, os processos são manuais e a comunicação entre as equipes é lenta."

  2. Geração de Ideias Individuais (10 minutos)
    * "Agora, quero que cada um de vocês pense individualmente na seguinte pergunta: 'Se você tivesse uma varinha mágica para criar a ferramenta perfeita para o seu trabalho, o que ela faria por você?'"
"Escrevam cada ideia em um post-it separado. Tentem escrever o máximo de ideias que conseguirem."

  3. Compartilhamento e Agrupamento (20 minutos)
    * "Ótimo. Agora, um de cada vez, por favor, leia suas ideias em voz alta e cole os post-its no quadro branco."
    * (Enquanto eles colam, o moderador agrupa os post-its com ideias semelhantes em áreas do quadro, criando "grupos" como "Relatórios Automáticos", "Visualização de Câmeras", "Alertas", "Configuração Fácil").

  4. Votação e Priorização (5 minutos)
    * "Excelente! Temos muitas ideias boas aqui. Agora, vou dar a cada um de vocês 3 adesivos (ou 3 votos com uma caneta)."
    * "Por favor, coloquem seus votos nas ideias ou grupos de ideias que vocês consideram mais importantes e urgentes."

  5. Encerramento (5 minutos)
    * "Perfeito. Com isso, já temos uma visão clara do que é mais importante para vocês. Este material é extremamente útil e vai guiar nosso projeto."
    * "Muito obrigado pela participação e por todas as ótimas ideias!"
