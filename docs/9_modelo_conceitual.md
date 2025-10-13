1) **Cenários de Interação**
## Cenário de Interação A: Geração de Relatório de Fluxo (Analista Mariana)

Atores: Mariana (Analista de Dados)

Mariana precisa gerar o relatório sobre o fluxo de passageiros da Linha 3-Vermelha para a reunião com o Administrador Carlos. **Com o novo sistema, ela acessa a plataforma com seu login e vai diretamente para o módulo "Análise de Dados". Em vez de solicitar dados brutos, ela agora tem acesso a uma interface onde pode criar consultas diretamente [2]. Ela seleciona o período desejado (o último trimestre), filtra pela "Linha 3-Vermelha" e o sistema instantaneamente carrega os dados de fluxo já pré-processados.**

**Mariana utiliza a ferramenta de visualização integrada para gerar gráficos comparativos entre as estações, arrastando e soltando as métricas que deseja analisar [3]. O sistema permite que ela salve o conjunto de filtros e gráficos como um "Dashboard Personalizado" para futuras consultas. Ao identificar uma inconsistência, ela consegue detalhar os dados de um dia específico com apenas um clique, evitando a necessidade de refazer todo o processo manualmente [4]. Satisfeita com a análise, ela clica em "Exportar Relatório para Diretoria", e o sistema gera um PDF profissional, contendo os gráficos e um resumo dos insights, em menos de 10 minutos.**

## Cenário de Interação B: Monitoramento e Configuração (Operador João)

Atores: João (Operador de Câmeras)

João recebe a denúncia sobre vendedores ambulantes. **Ele acessa o painel de controle do novo sistema e abre a "Visão Unificada de Câmeras". Ele digita o nome da estação reportada e o sistema exibe um mosaico com o feed ao vivo de todas as câmeras daquela localidade [5]. Ele consegue acompanhar a movimentação e, ao identificar um suspeito, utiliza a ferramenta de "Rastreamento por IA" para seguir o indivíduo entre as diferentes câmeras, tudo na mesma tela.**

**Mais tarde, João precisa configurar uma nova câmera. Ele vai até a seção "Gerenciamento de Dispositivos" na interface. Em vez de usar linhas de comando, ele clica em "Adicionar Nova Câmera" [7]. Um formulário visual solicita o identificador, a localização e a estação. Após preencher, ele salva as informações. Imediatamente, o sistema exibe o status da câmera como "Online" e mostra uma miniatura do feed de vídeo como confirmação visual de que a configuração foi bem-sucedida [8].**

## Cenário de Interação C: Tomada de Decisão Estratégica (Administrador Carlos)

Atores: Carlos (Administrador)

Carlos precisa se preparar para a reunião de diretoria. **Ele abre o sistema em seu computador e acessa o "Dashboard Estratégico". Em vez de cobrar Mariana por e-mail [10], ele vê um card com o status do relatório dela, mostrando "Análise Concluída". Ele clica e visualiza o mesmo relatório que Mariana gerou.**

**Para justificar os investimentos em segurança, ele navega para a aba "Indicadores de Segurança". Lá, ele encontra gráficos consolidados que mostram o número de ocorrências de atividades ilegais detectadas pelo sistema por semana, o tempo médio de resposta da equipe de João e a eficácia das intervenções [11]. Com essas informações claras e visuais, ele tem todos os dados necessários para tomar decisões rápidas e embasar suas solicitações para a diretoria, tudo em uma única plataforma centralizada.**

2) **Design Centrado na Comunicação**

**Nome do Cenário: Geração de Relatório de Fluxo (Mariana)**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
| Criar análise de dados | U: Preciso analisar o fluxo de passageiros da Linha 3-Vermelha no último trimestre. |
| > Filtrar e visualizar dados | D: Aqui estão os dados consolidados para o período e linha solicitados. Você pode arrastar as métricas para criar seus gráficos. |
| > Exportar resultado | U: A análise está pronta. Quero exportar um relatório para a diretoria. <br> D: Relatório em PDF gerado com sucesso. O download está disponível. |


**Nome do Cenário: Monitoramento e Configuração (João)**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
| Monitorar estação | U: Preciso ver todas as câmeras da Estação Sé agora. |
| > Visualizar câmeras | D: Exibindo o feed ao vivo de todas as 12 câmeras da Estação Sé. |
| Adicionar dispositivo | U: Quero adicionar uma nova câmera ao sistema. |
| > Configurar câmera | D: Por favor, preencha o formulário com os dados da câmera. |
| > Confirmar configuração | U: Salvei as informações. <br> D: Câmera adicionada com sucesso. O status é "Online" e o feed está ativo.|

**Nome do Cenário: Tomada de Decisão Estratégica (Administrador Carlos)**

| tópico \> subtópico (diálogo) | falas e signos |
| :---- | :---- |
| Acompanhar desempenho e tomar decisões | U: (Ao fazer login) Preciso de uma visão geral do status da operação. |
| > Visualizar status geral  |D: Bem-vindo, Carlos. O relatório de fluxo da Linha 3-Vermelha está "Concluído". Os indicadores de segurança estão atualizados em tempo real no painel. |
| > Acessar relatório específico | U: Quero visualizar o relatório de fluxo que a Mariana preparou. <br> D: Exibindo o relatório "Comparativo de Fluxo - Sé vs. Paraíso", com todos os gráficos e análises. |
| > Analisar dados de segurança | U: Agora, mostre-me os resultados consolidados da equipe de segurança. <br> D: Aqui está o painel de segurança, com o número de ocorrências detectadas por estação e o tempo médio de resposta da equipe.  |
| > Concluir análise | U: Certo. As informações são suficientes para a reunião. |

3) **Mapa de Objetivos**
> **_NOTE:_**: cada um coloca seu mapa de objetivos e deverá ter um diagrama de consolidação

4) **Esquema Conceitual de Signos**

### 4) Esquema Conceitual de Signos

| Usuário do Sistema (US) - Credenciais e perfil de acesso ao sistema | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **signo** | **origem** | **observações** | **Tipo de conteúdo** | **restrição sobre conteúdo** | **valor default** | **prevenção** / **recuperação** |
| + id_usuario | aplicação | Identificador único no sistema. | texto | não pode ser nulo, único | gerado automaticamente | N/A |
| nome | domínio | Nome completo do funcionário. | texto | não pode ser nulo | — | **PP:** campo obrigatório / **RA** |
| email_login | domínio | E-mail corporativo usado para login. | texto | não pode ser nulo, formato de e-mail | — | **PP+PA:** validação de formato de e-mail / **RA** |
| perfil_acesso | domínio | Define as permissões do usuário. | seleção simples | {Administrador, Analista, Operador} | — | **PA:** botão "Salvar" desabilitado se não for selecionado / **RA** |
| senha | aplicação | Credencial de acesso criptografada. | texto | não pode ser nulo, mínimo 8 caracteres | — | **PP:** campo obrigatório com regras de complexidade / **RA** |

| Câmera (CAM) - Dispositivo de captura de imagem instalado nas estações | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **signo** | **origem** | **observações** | **Tipo de conteúdo** | **restrição sobre conteúdo** | **valor default** | **prevenção** / **recuperação** |
| + id_camera | domínio | Identificador único do equipamento. | texto | não pode ser nulo, único | — | **PP:** campo obrigatório / **RA:** informa se o ID já existe |
| localizacao | domínio | Descrição física da posição da câmera. | texto | não pode ser nulo | — | **PP:** campo obrigatório / **RA** |
| estacao | domínio | Estação do Metrô onde está instalada. | seleção simples | não pode ser nulo | — | **PA:** uma opção deve ser selecionada de uma lista pré-definida / **RA** |
| status | aplicação | Indica se a câmera está ativa e transmitindo. | texto | {Online, Offline, Em Manutenção} | Offline | **PA:** status é atualizado automaticamente pelo sistema |
| feed_video | aplicação | Fluxo de vídeo em tempo real. | vídeo | N/A | N/A | **CE:** exibe mensagem se o feed não puder ser carregado |

| Relatório de Fluxo (RF) - Análise de dados de fluxo de passageiros | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **signo** | **origem** | **observações** | **Tipo de conteúdo** | **restrição sobre conteúdo** | **valor default** | **prevenção** / **recuperação** |
| + id_relatorio | aplicação | Identificador único do relatório. | texto | não pode ser nulo, único | gerado automaticamente | N/A |
| titulo | domínio | Nome do relatório definido pelo analista. | texto | não pode ser nulo | "Relatório sem título" | **PP:** campo obrigatório / **RA** |
| data_inicio | domínio | Data de início do período de análise. | data | não pode ser nulo | data atual - 7 dias | **PP+PA:** seletor de calendário / **RA** |
| data_fim | domínio | Data de fim do período de análise. | data | não pode ser nulo, ≥ data_inicio | data atual | **PP+PA:** seletor de calendário / **RA** |
| filtros_aplicados | domínio | Lista de filtros (estações, linhas, horários). | lista de texto | deve conter ao menos uma estação/linha | — | **PA:** botão "Gerar" desabilitado se filtros essenciais não forem preenchidos / **RA** |
| status_geracao | aplicação | Indica o progresso da análise. | texto | {Em Andamento, Concluído, Falha} | — | **PA:** status atualizado automaticamente |




