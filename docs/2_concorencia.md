# Análise de Concorrência

## 1. Principais Concorrentes

- **Digifort:** Empresa brasileira consolidada que oferece uma plataforma VMS (Video Management System) robusta e modular.
- **Amazon Rekognition:** Serviço da Amazon Web Services (AWS) que oferece APIs de visão computacional prontas para uso.
- **Irisity:** Empresa sueca especializada em análise de vídeo de alta performance baseada em Inteligência Artificial.

---

## 2. Informações sobre os Concorrentes

### Digifort
- **Site:** [https://www.digifort.com.br](https://www.digifort.com.br)
- **Características:**
    - **Plataforma Integrada:** Oferece um ecossistema completo para gerenciamento de câmeras, compatível com múltiplos fabricantes e integrável a sistemas de alarme e controle de acesso.
    - **Módulos Analíticos:** As funcionalidades de inteligência são comercializadas como módulos adicionais, incluindo contagem de pessoas, detecção de aglomerações e reconhecimento facial.
- **Preços:**
    - Modelo de licenciamento por câmera e por módulo analítico. Os preços não são públicos e a venda é feita por distribuidores certificados, variando conforme a escala do projeto.
- **Público-alvo:**
    - Grandes corporações, governo, cidades, aeroportos e transporte público.
- **Materiais de Marketing:**
    - Focada em demonstrar a confiabilidade e a aplicação prática da solução através de estudos de caso ("Notícias") e demonstrações técnicas em seu canal no YouTube.
- **Interface:**
    <img width="1919" height="1043" alt="digifort" src="https://github.com/user-attachments/assets/853f8960-191b-4c93-9ede-218cbeb0fe54" />

### Amazon Rekognition
- **Site:** [https://aws.amazon.com/rekognition/](https://aws.amazon.com/rekognition/)
- **Características:**
    - **Person Tracking:** API StartPersonTracking que rastreia pessoas em um vídeo, atribuindo um ID único para cada indivíduo detectado.
    - **Face Detection and Analysis:** Detecta faces e atributos (gênero, idade aproximada, emoções).
    - **Face Search:** Permite buscar uma face detectada em um banco de faces previamente cadastradas, o que possibilita a reidentificação.
- **Preços:**
    - Modelo "Pay-as-you-go" (pague pelo que usar), com custos baseados no volume de dados processados (ex: minutos de vídeo ou número de imagens).
- **Público-alvo:**
    - Desenvolvedores e equipes de TI que precisam adicionar capacidades de visão computacional a seus próprios sistemas e produtos.
- **Materiais de Marketing:**
    - A comunicação é voltada para o público técnico, destacando a facilidade de uso (simples chamadas de API), a precisão dos modelos de IA e a escalabilidade.
- **Interface:**
  <img width="1912" height="1057" alt="amaz" src="https://github.com/user-attachments/assets/7bf00170-f808-46e7-ae05-2719f2c8214a" />

### Irisity
- **Site:** [https://irisity.com](https://irisity.com)
- **Características:**
    - **Foco em IA Proativa:** A plataforma é projetada para aprender o comportamento padrão de um ambiente e detectar anomalias e desvios em tempo real.
    - **Rastreamento Inter-câmeras (Re-ID):** Sua principal tecnologia permite rastrear um mesmo indivíduo ou objeto de forma contínua através de múltiplas câmeras.
    - **Análise Comportamental:** Gera insights avançados como mapas de calor (heatmaps) e análise de filas, focados na otimização de operações.
- **Preços:**
    - O modelo tende a ser de assinatura (SaaS), sem preços públicos. Oferecem um período de teste gratuito ("30-Day Trial") para demonstração de valor.
- **Público-alvo:**
    - Cidades inteligentes, transporte, grandes varejistas e escolas.
- **Materiais de Marketing:**
    - Centrada nos benefícios da IA, como precisão, automação e otimização de recursos, comunicados através de vídeos e artigos no site.
- **Interface:**
  <img width="1919" height="1079" alt="irisity" src="https://github.com/user-attachments/assets/4cd0a867-5be0-4a8e-a79a-17918ec52dac" />
---

## 3. Análise de Características e Funcionalidades

### Concorrente 1: Digifort
- **Pontos Fortes:**
    - **Maturidade:** É um produto comercial consolidado, testado em milhares de cenários reais, o que garante alta confiabilidade.
    - **Suporte e Rede:** Possui uma rede de distribuidores e suporte técnico estabelecida em todo o Brasil.
- **Pontos Fracos:**
    - **Foco Generalista:** O Digifort possui funcionalidades genéricas, enquanto nosso projeto é totalmente focado no problema complexo de reidentificação de pessoas entre estações para gerar dados de fluxo, algo que não é a função principal dos módulos do Digifort.
    - **Custo:** O modelo de licenças por câmera/módulo pode gerar um alto custo inicial. Nossa arquitetura tem um custo operacional mais flexível e escalável.

### Concorrente 2: Amazon Rekognition
- **Pontos Fortes:**
    - **Custo-Benefício:** Usar a API é mais barato e rápido do que desenvolver, treinar e manter um algoritmo de Re-ID próprio do zero.
- **Pontos Fracos:**
    - **Ferramenta vs. Solução Completa:** Ele não oferece backend, banco de dados, regras de negócio, sistema distribuído de coleta ou interface de relatórios. Entrega a ferramenta, não a solução.

### Concorrente 3: Irisity
- **Pontos Fortes:**
    - **Superioridade Tecnológica em IA:** Sendo especialistas em IA, seus algoritmos de Re-ID são provavelmente mais precisos e maduros que o algoritmo pré-desenvolvido que utilizaremos.
- **Pontos Fracos:**
    - **Foco na Solução, não no Cliente:** A Irisity vende um produto poderoso que o cliente precisa adaptar aos seus processos. Em contrapartida, nosso projeto parte do problema do Metrô para criar uma solução sob medida, garantindo que o resultado final seja exatamente o que o usuário final precisa.

---

## 4. Avaliação de Experiência do Usuário (UX)

### Concorrente 1: Digifort
- **Pontos Positivos:**
    - A plataforma permite alta capacidade de personalização da área de trabalho através de mosaicos de câmeras configuráveis.
    - Por ser uma aplicação desktop nativa, a velocidade de resposta a cliques e interações é fluida e satisfatória.
- **Pontos Negativos:**
    - A interface apresenta uma alta densidade informacional, o que pode sobrecarregar usuários iniciantes.
    - O design funcional, porém esteticamente datado, exige um período de treinamento para o uso eficiente da ferramenta.

### Concorrente 2: Irisity
- **Pontos Positivos:**
    - A interface possui um design limpo e moderno, que prioriza a hierarquia visual e facilita a absorção das informações.
    - A experiência é guiada por um paradigma de "monitoramento por exceção", onde alertas proativos guiam o usuário diretamente aos eventos de interesse.
- **Pontos Negativos:**
    - Por ser uma plataforma web, a fluidez da interação está diretamente atrelada à qualidade da conexão de rede e à latência do backend.

### Concorrente 3: Amazon Rekognition
- **Pontos Positivos:**
    - O console oferece uma interface minimalista com um fluxo de trabalho objetivo, permitindo ao desenvolvedor testar e validar as funcionalidades rapidamente.
    - A velocidade de processamento para análise de imagens é quase instantânea, agilizando o ciclo de desenvolvimento e prova de conceito.
- **Pontos Negativos:**
    - Atualizações forçadas nos modelos de IA pela AWS, sem controle do usuário, podem alterar o comportamento do algoritmo. Isso cria um risco de inconsistência nos dados ao comparar relatórios de fluxo entre diferentes períodos.

---

## 5. Análise de Preços e Modelos de Negócio

### Concorrente 1: Digifort
- **Modelo de Negócio:**
    - O modelo principal é a venda de licenças de software permanentes.
    - Exige o pagamento de uma taxa anual de manutenção para acesso a atualizações e suporte.
    - A precificação é granular e modular (licença base + licenças por câmera + licenças por módulo analítico).
    - Oferece diferentes edições do software (Explorer, Standard) com diferentes limites e funcionalidades.
- **Suporte:**
    - O suporte primário é fornecido pela rede de distribuidores e integradores certificados.
- **Impacto na Aquisição e Retenção:**
    - **Aquisição:** O alto custo inicial pode ser uma barreira, mas a modularidade ajuda a começar pequeno.
    - **Retenção:** A retenção é extremamente alta, garantida pelo grande investimento inicial e pelo alto custo de troca.

### Concorrente 2: Irisity
- **Modelo de Negócio:**
    - O modelo é baseado em assinaturas recorrentes.
    - O preço é calculado por câmera conectada e pelo nível de análise de IA contratado.
    - Oferece planos em níveis ("Professional", "Enterprise") com diferentes funcionalidades e níveis de serviço.
- **Suporte:**
    - O suporte técnico está incluído na assinatura e é fornecido diretamente pela Irisity.
- **Impacto na Aquisição e Retenção:**
    - **Aquisição:** O baixo custo inicial e a oferta de **"trial" gratuito** removem a barreira financeira e facilitam a adoção.
    - **Retenção:** É baseada no valor contínuo percebido, exigindo inovação constante e qualidade de serviço para evitar o cancelamento.

### Concorrente 3: Amazon Rekognition
- **Modelo de Negócio:**
    - Pagamento por uso (Pay-as-you-go), sem contratos ou taxas mínimas. O cliente paga exatamente pelo que consome.
    - Oferece um nível gratuito por 12 meses para novos clientes, que funciona como uma poderosa ferramenta de aquisição.
    - A precificação é granular por chamada de API, com descontos por volume para grandes clientes.
- **Suporte:**
    - O suporte é para a conta AWS como um todo e não específico para o Rekognition, com planos pagos (Developer, Business).
- **Impacto na Aquisição e Retenção:**
    - **Aquisição:** A barreira de entrada é praticamente zero, incentivando a experimentação e a adoção em pequenos projetos.
    - **Retenção:** É garantida pela integração com o ecossistema AWS. Uma vez que a aplicação é construída em torno dos serviços, o esforço para migrar se torna imenso.

---

## 6. Padrões e Tendências de Mercado

### Inovações Tecnológicas
- **Inteligência Artificial e Análise Preditiva:** A mudança de monitoramento passivo (apenas gravar) para análise ativa (extrair insights e prever eventos).
- **Computação na Borda (Edge Computing):** Processar o vídeo localmente (na câmera ou na estação) para economizar banda e aumentar a velocidade de resposta.
- **Integração de Dados (Data Fusion):** Unificar dados de vídeo com outras fontes (bilhetagem, horários) para uma visão operacional completa.

### Mudanças nas Preferências do Usuário
- **Dashboards Interativos:** A expectativa por dashboards dinâmicos (como Power BI) onde o próprio usuário pode explorar os dados, em vez de relatórios estáticos.
- **Privacidade por Design (Privacy-by-Design):** Com a LGPD, a crescente demanda por sistemas que anonimizam dados e protegem a privacidade desde sua concepção.

### Novos Modelos de Negócios
- **Migração para Assinaturas (SaaS):** A substituição de licenças caras (CAPEX) por pagamentos recorrentes e mais acessíveis (OPEX) como o modelo dominante no mercado de software.

---

## 7. Relatórios e resultados

### Sumário

A presente análise investigou três concorrentes chave — **Digifort**, **Irisity** e **Amazon Rekognition** — que representam as principais abordagens do mercado de monitoramento e análise de vídeo: a plataforma VMS tradicional, a solução especialista em IA e a tecnologia como serviço (PaaS), respectivamente.
A análise revelou um mercado maduro, com soluções robustas para segurança e análise genérica. Contudo, foi identificado um claro gap de mercado para uma solução especialista, customizável e focada em resolver problemas de negócio específicos, como a análise de fluxo de passageiros.
Nosso projeto se posiciona estrategicamente nesta lacuna, oferecendo não uma ferramenta genérica, mas uma solução fim-a-fim sob medida, com uma arquitetura moderna e um modelo de custos potencialmente mais eficiente, alinhado às principais tendências tecnológicas e às necessidades do cliente final.

---

### Tabela Comparativa Geral de Concorrentes

| Concorrente | Perfil | Principal Ponto Forte | Principal Ponto Fraco (vs. Nosso Projeto) |
| :--- | :--- | :--- | :--- |
| **Digifort** | Plataforma VMS completa e modular | Ecossistema maduro, robusto e com ampla rede de suporte no Brasil. | Foco generalista; alto custo inicial (CAPEX) e baixa customização para problemas de negócio específicos. |
| **Irisity** | Solução especialista em IA (SaaS) | Superioridade tecnológica em algoritmos de Re-ID e análise comportamental. | Alto custo (solução premium); vende um produto fechado que o cliente deve se adaptar. |
| **Amazon Rekognition**| Plataforma de APIs (PaaS) | Baixíssima barreira de entrada e custo-benefício para o componente de IA. | Entrega a "ferramenta", não a "solução completa".|
| **Nosso Projeto**| **Solução Especialista** | Foco total no problema de análise de fluxo; 100% customizável às necessidades do Metrô. | Produto em desenvolvimento; sem a maturidade e a escala dos concorrentes comerciais. |

---

### Análise Comparativa de Modelos de Negócio

A forma como cada concorrente gera receita impacta diretamente os clientes. A tabela abaixo resume os modelos:

| Característica | Digifort | Irisity | Amazon Rekognition |
| :--- | :--- | :--- | :--- |
| **Tipo de Custo** | CAPEX (Alto Custo Inicial) | OPEX (Custo Recorrente) | OPEX (Custo Variável) |
| **Modelo Principal** | Licença Perpétua + Manutenção| Assinatura (SaaS) | Pagamento por Uso |
| **Vantagem p/ Aquisição**| Orçamentos de capital; modularidade| Baixo custo inicial; teste gratuito| Barreira de entrada zero; nível gratuito|
| **Fator de Retenção**| Alto Custo de Troca (inércia)| Valor Contínuo (serviço) | Integração no Ecossistema (lock-in)|

**Conclusão:** Nosso projeto, com sua arquitetura em nuvem, se alinha ao modelo OPEX, preferido pelo mercado moderno por sua flexibilidade e baixo custo inicial, similar ao da Irisity e Amazon Rekognition.

---

## 8. Pontos positivos e recomendações

### Oportunidades de Melhoria para o Projeto

Enquanto concorrentes oferecem ferramentas genéricas, a maior oportunidade do nosso projeto é nos aprofundarmos nos KPIs que realmente importam para o Metrô-SP. Perguntas como *"Qual o tempo médio de deslocamento entre a estação A e B no horário de pico?"* ou *"Qual a rota de fluxo mais comum após um grande evento no Anhangabaú?"* são diferenciais que apenas uma solução sob medida pode responder com precisão.

### Recomendações

Podemos acelerar nosso desenvolvimento adotando as melhores práticas dos concorrentes e, ao mesmo tempo, evitando seus erros mais comuns.

**Aproveitando os Pontos Fortes dos Concorrentes:**
- Pensando no Digifort poderiamos implementar uma dashboard customizável. A interface principal deve permitir que o usuário final (gestor) crie sua própria visão, arrastando e configurando widgets com os gráficos e KPIs mais relevantes para sua função.

**Evitando os Pontos Fracos dos Concorrentes:**
-  Pensando no Digifort deveriamos focar na simplicidade e intuitividade. Devemos resistir à tentação de adicionar todas as funcionalidades possíveis. Nosso objetivo é criar uma ferramenta que seja poderosa para sua finalidade específica e que exija o mínimo de treinamento.

---

### Estratégias de Diferenciação para o Mercado

Para se destacar, nosso software deve adotar uma estratégia de hiperfoco no problema do cliente, posicionando-se como uma solução especialista. Nossa principal mensagem de marketing e desenvolvimento não é ser "mais um software de análise de vídeo", mas sim:

> **"A plataforma de inteligência de fluxo de passageiros para o Metrô de São Paulo."**

Esse diferencial, embora segmente o mercado inicial, cria um caso de sucesso com potencial para despertar o interesse de outras concessionárias (como a ViaMobilidade), demonstrando valor claro e efetivo na otimização da operação metroviária.
