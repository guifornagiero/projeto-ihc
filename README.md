# Projeto de Interface Humano-Computador

Projeto apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interface Humano-Computador (CC8122) do curso de Ciencia da Computação, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](https://github.com/fagnerpimentel) e Prof. Dr. Plino Thomaz Aquino Junior.

Este projeto se baseia no Trabalho de Conclusão de Curso (TCC) entitulado **IDENTIFICAÇÃO E REIDENTIFICAÇÃO CONTÍNUA DE PESSOAS EM AMBIENTES DE TRÁFEGO INTENSO UTILIZANDO ALGORITMOS DE VISÃO COMPUTACIONAL** sob orientação do Professor **Prof. Dr. Ricardo de Carvalho Destro** e desenvolvido pelos seguintes alunos:

- Gianluca Mariano Sobreiro - 22.122.011-4
- Guilherme Fornagiero de Carvalho - 22.122.016-3
- Paulo Vinícius Bessa de Brito - 22.122.005-6
- Pedro Augusto Bento Rocha - 22.122.028-8
- Thiago Garcia Santana - 22.122.003-1

## Conhecendo o problema

Sobre o produto ou serviço que seu grupo está desenvolvendo, responda:
O projeto consiste no desenvolvimento de um sistema distribuído de larga escala, focando na identificação e reidentificação contínua de pessoas em ambientes de tráfego intenso, com foco no Metrô de São Paulo e em sua necessidade de mapeamento de fluxos em suas estações. O sistema utiliza algoritmos de visão computacional e aprendizado de máquina para rastrear passageiros entre diferentes câmeras, mesmo em condições adversas como mudanças de iluminação, ângulos de filmagem e pequenas alterações na aparência. O objetivo principal é fornecer ao Metrô de São Paulo uma ferramenta capaz de monitorar o fluxo de passageiros, identificar indivíduos de forma contínua e precisa, e auxiliar na gestão operacional e segurança do transporte público. Além disso, focado na disciplina de Interface Humano-Computador, aumentamos o escopo do projeto para trabalhar também com a análise dos dados capturados, e a geração de resultados a partir destes, a partir de telas como: Login, Configuração (usuários e câmeras), Histórico de ações, Dashboards e gráficos e Interface de câmera.

Usuário final: Companhia do Metropolitano de São Paulo (Metrô-SP) equipes de segurança e de gestão operacional do sistema metroviário.

Baseado em uma geração de base de dados diária/semanal do fluxo de pessoas que passam pelas estações do Metrô de São Paulo, e o envio/análise desses dados, podemos ter a otimização da alocação de recursos operacionais (trens, funcionários, segurança) pela diretoria do Metrô, focada em melhorar a experiência do usuário final (o passageiro). Além disso, o aumento da segurança, com possibilidade de detectar indivíduos específicos (como vendedores ambulantes ilegais) e um melhor mapeamento de rotas para os passageiros, permitindo decisões estratégicas baseadas nesse dados.

Funcionalidades iniciais:
- Captura de imagens em tempo real por câmeras instaladas nas estações.
- Detecção e reconhecimento facial de pessoas préviamente detectadas.
- Armazenamento temporário e sincronização diária de dados em banco central (que servirá de base de dados para o Metrô).

Funcionalidades para a disciplina:
- Login.
- Configurar novos usuários e câmeras.
- Visualizar interface de câmera.
- Gerar dashboards e relatórios com os dados gerados do projeto.
- Histórico de ações.

Tecnologias utilizadas:
- Backend: .NET 8.0, C#, FaceAISharp (biblioteca para reconhecimento facial)
- Infraestrutura em Cloud: Amazon AWS, AWS EC2
- Mensageria: AWS SQS
- Banco de Dados: AWS RDS, MongoDB
- Frontend (exclusivo para a disciplina): JavaScript, React JS

Contexto de uso:
- O sistema será utilizado principalmente nas estações do Metrô de São Paulo e em seus centros de monitoramento, ambientes caracterizados por um fluxo intenso e contínuo de passageiros. No nível operacional, os operadores de câmeras utilizam o sistema em salas de controle para acompanhar imagens em tempo real e responder a situações de segurança. Já no nível analítico e gerencial, analistas de dados e administradores acessam dashboards, relatórios e históricos em ambientes administrativos para planejar recursos, organizar escalas e otimizar a operação do transporte. Esse contexto envolve fatores sociais, econômicos e culturais complexos: o metrô atende milhões de pessoas diariamente, em sua maioria trabalhadores e estudantes de classes média e baixa. Além disso, existe uma forte preocupação com eficiência operacional, redução de custos e aumento da segurança, tanto para proteger os passageiros quanto para monitorar e proibir certas atividades ilegais dentro das estações. Antes de iniciar a interação, o sistema precisa guardar informações cruciais do ambiente, como a configuração das câmeras (identificador, localização e estação), credenciais e permissões dos usuários e dados de históricos de ações anteriores no sistema e dados. Durante a interação, o ambiente está em constante movimento, com milhares de passageiros circulando pelas estações a cada hora. Enquanto isso, os operadores monitoram eventos em tempo real com os logs de captura de passageiros, os analistas de dados transformam dados em relatórios e administradores utilizam esses resultados para embasar decisões estratégicas.

A idealização do projeto (somente o sistema distribuído em larga escala, e a geração de dados para análise futura) não necessita de uma inteface, então inicialmente não prevemos o desenvolvimento de uma interface.

## Desenvolvimento
- [Análise de Concorência](docs/2_concorencia.md)
- [Personas](docs/3_personas.md)
- [Cenário de Análise/Problema](docs/4_cenarios.md)
- [Análide de Tarefas](docs/5_analise_tarefas.md)
- [Prototipação em Papel](docs/6_prototipacao.md)
- [Coleta de Dados](docs/7_coleta_dados.md)
- [Ciclo de vida da engenharia de usabilidade](docs/8_ciclo_vida.md)
- [Modelo Conceitual](docs/9_modelo_conceitual.md) 
- [MOLIC]()
- [FIGMA]()
- [Planejamento da Avaliação]()
- [Avaliação de IHC através de Inspeção Heurística]()
- [Avaliação de Usabilidade baseado em Observação do Usuário]()
