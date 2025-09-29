# Análise de Tarefas

> **_NOTE:_**: A equipe deve descrever as funcionalidades mais importantes da interface/produto. A equipe deve modelar pelo menos 1 HTA, 1 GOMS e 1 CTT (de pelo menos 4 funcionalidades diferentes). Cada diagrama deve ter um texto explicando a funcionalidade.

## 1. Cadastro de Usuário

### HTA
<img width="1337" height="480" alt="image" src="https://github.com/user-attachments/assets/e7775ce4-bacc-416f-bf4e-1f2920efb55d" />

| Objetivos/Operações | Problemas e Recomendações |
| :--- | :--- |
| **Cadastrar Usuário** | **Input:** O administrador acessa a funcionalidade de gerenciamento de usuários para adicionar um novo membro. <br> **Feedback:** Um novo usuário é criado no sistema e um e-mail de boas-vindas com a senha é enviado. <br> **Plano:** Realizar a operação 1, depois a 2 e, por fim, a 3. <br> **Recomendação:** O formulário deve ser claro, objetivo e indicar quais campos são obrigatórios para agilizar o processo. |
| **1. Acessar o formulário de cadastro** | **Problema:** O botão para adicionar um novo usuário pode não ser facilmente localizável se a interface de gerenciamento de usuários for confusa. <br> **Recomendação:** O botão "Novo Usuário" deve ser um Call-to-Action (CTA) com destaque visual na tela principal de listagem de usuários. |
| **2. Preencher os dados do usuário** | **Problema:** O administrador pode inserir um e-mail em formato inválido ou já existente. A diferença entre os perfis de acesso (admin, analista, operador) pode não ser clara. <br> **Recomendação:** Implementar validação de e-mail em tempo real (formato e duplicidade). Fornecer textos de ajuda que expliquem as permissões de cada perfil de acesso. |
| **3. Salvar o cadastro** | **Problema:** O sistema pode falhar ao salvar ou ao enviar o e-mail, e o administrador pode não perceber o erro específico. <br> **Recomendação:** Exibir uma mensagem de sucesso clara. Em caso de falha (ex: no envio do e-mail), a mensagem deve informar o sucesso parcial e indicar os próximos passos (ex: "Usuário criado, mas falha ao enviar e-mail. Peça para o usuário usar a função 'Esqueci minha senha'"). |

### GOMS
* **GOAL 0: Cadastrar novo usuário**
    * **GOAL 1: Acessar o formulário de cadastro**
        * **METHOD 1.A:** Navegar e abrir o formulário
            * (SEL. RULE: O usuário precisa estar na área de gerenciamento de usuários)
            * OP. 1.A.1: Deslocar o cursor para o botão "Novo Usuário"
            * OP. 1.A.2: Clicar no botão
            * OP. 1.A.3: Aguardar o carregamento do formulário de cadastro
    * **GOAL 2: Inserir dados do usuário**
        * **METHOD 2.A:** Digitar nome e e-mail
            * (SEL. RULE: Nome tem que ter apenas letras e e-mail tem que ser no formato de e-mail)
            * OP. 2.A.1: Deslocar o cursor para o campo "Nome"
            * OP. 2.A.2: Clicar no campo
            * OP. 2.A.3: Digitar o nome do usuário
            * OP. 2.A.4: Deslocar o cursor para o campo "E-mail"
            * OP. 2.A.5: Clicar no campo
            * OP. 2.A.6: Digitar o e-mail do usuário
        * **METHOD 2.B:** Selecionar estação
            * (SEL. RULE: Estações são pré-definidas no sistema)
            * OP. 2.B.1: Deslocar o cursor para a lista suspensa "Estação"
            * OP. 2.B.2: Clicar para abrir a lista
            * OP. 2.B.3: Deslocar o cursor para a estação desejada
            * OP. 2.B.4: Clicar na estação
        * **METHOD 2.C:** Selecionar perfil de acesso
            * (SEL. RULE: Usuário escolhe entre admin, analista ou operador)
            * OP. 2.C.1: Deslocar o cursor para a lista suspensa "Perfil de Acesso"
            * OP. 2.C.2: Clicar para abrir a lista
            * OP. 2.C.3: Deslocar o cursor para o perfil desejado
            * OP. 2.C.4: Clicar no perfil
    * **GOAL 3: Salvar o cadastro e confirmar**
        * **METHOD 3.A:** Clicar para salvar
            * (SEL. RULE: Todos os campos obrigatórios foram preenchidos corretamente)
            * OP. 3.A.1: Deslocar o cursor para o botão "Salvar"
            * OP. 3.A.2: Clicar no botão
            * OP. 3.A.3: Aguardar a resposta do sistema
        * **METHOD 3.B:** Confirmar sucesso do cadastro
            * (SEL. RULE: Os dados foram salvos com sucesso e o e-mail foi enviado)
            * OP. 3.B.1: O sistema exibe a mensagem de sucesso na tela (ação do sistema)
            * OP. 3.B.2: O usuário lê a mensagem de confirmação

### CTT
<img width="1299" height="690" alt="image" src="https://github.com/user-attachments/assets/caaeaaaa-17b2-43e3-90e4-d59d2be36890" />

## 2. Cadastro de Câmera

### HTA
<img width="1337" height="480" alt="image" src="https://github.com/user-attachments/assets/8eba7f6b-1787-407c-8d5d-bf59853ab1d4" />

| Objetivos/Operações | Problemas e Recomendações |
| :--- | :--- |
| **Cadastrar Câmera** | **Input:** O usuário inicia a tarefa ao acessar o formulário de cadastro de câmeras. <br> **Feedback:** A câmera cadastrada é adicionada à lista de equipamentos do sistema. <br> **Plano:** Realizar a operação 1, depois a 2 e, em seguida, a 3. <br> **Recomendação:** O sistema deve oferecer um fluxo de navegação simples para que o usuário possa seguir as etapas de cadastro sem confusão. |
| **1. Informar identificador, localização e estação da câmera** | **Problema:** Um usuário pode inserir um ID que já existe no sistema, ou a descrição da localização ser ambígua. <br> **Recomendação:** Implementar uma validação em tempo real para o ID da câmera e utilizar campos de preenchimento automático para a estação. |
| **2. Enviar dados da câmera para o sistema** | **Problema:** O envio dos dados pode falhar devido a problemas de conexão ou do servidor. <br> **Recomendação:** O sistema deve exibir mensagens de erro claras e informativas, orientando o usuário sobre o que fazer em caso de falha. |
| **3. Enviar mensagem informando sucesso no cadastramento** | **Problema:** A mensagem de confirmação pode ser facilmente ignorada se for muito discreta ou temporária. <br> **Recomendação:** A mensagem de sucesso deve ser visualmente destacada e persistir na tela por tempo suficiente para garantir que o usuário a veja. |

### GOMS
* **GOAL 0: Cadastrar Câmera**
     * **GOAL 1: Inserir identificador, localização e estação da câmera**
         * **METHOD 1.A:** Digitar ID e localização
             * (SEL. RULE: O ID deve ser único para o sistema e a localização deve ser descrita de forma textual)
             * OP. 1.A.1: Deslocar o cursor do mouse para o campo de ID
             * OP. 1.A.2: Clicar no campo
             * OP. 1.A.3: Digitar o ID da câmera
             * OP. 1.A.4: Deslocar o cursor para o campo de localização
             * OP. 1.A.5: Clicar no campo
             * OP. 1.A.6: Digitar a localização
             * OP. 1.A.7: Preparação mental para a próxima ação
         * **METHOD 1.B:** Selecionar estação
             * (SEL. RULE: Estações são pré-definidas no sistema)
             * OP. 1.B.1: Deslocar o cursor para o campo de estação
             * OP. 1.B.2: Clicar no campo para abrir a lista suspensa
             * OP. 1.B.3: Deslocar o cursor para a estação desejada
             * OP. 1.B.4: Clicar na estação
             * OP. 1.B.5: Verificar se a estação selecionada está correta
     * **GOAL 2: Enviar dados da câmera para o sistema**
         * **METHOD 2.A:** Salvar e enviar os dados da câmera
             * (SEL. RULE: Os dados são submetidos para processamento e salvos no banco de dados)
             * OP. 2.A.1: Deslocar o cursor para o botão "Salvar" ou "Cadastrar"
             * OP. 2.A.2: Clicar no botão
             * OP. 2.A.3: Aguardar a resposta do sistema
     * **GOAL 3: Enviar mensagem confirmando sucesso no cadastramento**
         * **METHOD 3.A:** Exibir a mensagem de sucesso na tela
             * (SEL. RULE: Os dados foram salvos com sucesso e o sistema confirma o cadastramento)
             * OP. 3.A.1: O sistema exibe a mensagem (ação do sistema)
             * OP. 3.A.2: O usuário lê a mensagem
         * **METHOD 3.B:** Exibir aviso de falha
             * (SEL. RULE: O sistema não consegue salvar os dados devido a um erro, como ID duplicado ou falha de conexão com o banco de dados)
             * OP. 3.B.1: O sistema exibe a mensagem de erro (ação do sistema)
             * OP. 3.B.2: O usuário lê a mensagem e entende o problema

### CTT
<img width="1291" height="497" alt="image" src="https://github.com/user-attachments/assets/5c851192-e5af-41ea-bc7f-22fed32358ff" />


## 3. Gerar Relatório de Fluxo de Passageiros

### HTA
![cta3](https://github.com/user-attachments/assets/fff0fae6-d2ac-4ea2-ab4f-5178b2b7ab64)

### GOMS
GOAL 0: Gerar Relatório de Fluxo de Passageiros
<br> GOAL 1: Definir parâmetros para a consulta do relatório
<br> METHOD 1.A: Selecionar período da análise
<br> (SEL. RULE: O usuário deve informar uma data de início e uma data de fim para a consulta)
<br> METHOD 1.B: Selecionar estações de origem e destino
<br> (SEL. RULE: As estações devem ser selecionadas a partir de uma lista pré-definida no sistema)
<br> GOAL 2: Submeter consulta e visualizar o relatório
<br> METHOD 2.A: Acionar a geração do relatório
<br> (SEL. RULE: A consulta é enviada para o sistema e os dados são exibidos na tela após o processamento)
<br> GOAL 3: Receber confirmação da geração do relatório
<br> METHOD 3.A: Exibir relatório com os dados solicitados
<br> (SEL. RULE: O sistema encontrou e processou os dados com sucesso para os filtros informados)
<br> METHOD 3.B: Exibir aviso de erro ou ausência de dados
<br> (SEL. RULE: O sistema não encontrou dados para o período/trajeto solicitado ou ocorreu uma falha na consulta)
<br> GOAL 4: Exportar dados do relatório
<br> (SEL. RULE: O arquivo é exportado no computador do usuário)



### CTT
<img width="1337" height="480" alt="Screenshot 2025-09-20 at 8 16 49 PM" src="https://github.com/user-attachments/assets/c2f095b2-fb83-4c33-a71d-3365f5b4a3f1" />


## 4. Consultar histórico de ações de usuário

### HTA
![hta-gian](https://github.com/user-attachments/assets/ad8d5562-4e32-4f57-83c3-515c157c69b4)
| Objetivos/Operações | Problemas e Recomendações |
| :--- | :--- |
| **Consultar histórico de ações de usuário** | **Input:** O administrador acessa a área de logs do sistema. <br> **Feedback:** O sistema exibe o histórico de atividades dos usuários. <br> **Plano:** Realizar a operação 1, e então as operações 2, 3 e 4 ficam disponíveis para execução em qualquer ordem. <br> **Recomendação:** A interface deve ser clara e eficiente, permitindo que um administrador encontre rapidamente as informações necessárias para uma auditoria. |
| **1. Acessar tela de histórico de ações** | **Problema:** A funcionalidade de logs pode estar escondida em menus complexos, dificultando o acesso rápido em caso de uma investigação de segurança. <br> **Recomendação:** A opção "Logs" ou "Histórico de Ações" deve estar em um local de destaque no painel de administração. |
| **2. Aplicar filtros de busca** | **Problema:** A ausência de filtros detalhados (ex: por tipo de ação, por usuário específico) pode tornar a busca por um evento particular muito demorada. <br> **Recomendação:** Implementar múltiplos filtros, como campo de busca por nome de usuário, seletor de data/hora com atalhos ("Hoje", "Últimos 7 dias") e um dropdown para tipos de evento. |
| **3. Analisar os resultados apresentados** | **Problema:** Uma grande quantidade de logs apresentada sem formatação ou paginação pode sobrecarregar o usuário. <br> **Recomendação:** Exibir os resultados em uma tabela paginada e com colunas ordenáveis. Ações críticas (ex: falha de login, exclusão de dados) podem ser destacadas com cores para facilitar a identificação. |
| **4. Exportar o relatório de histórico**| **Problema:** O usuário pode precisar dos dados para análise externa ou para gerar relatórios de conformidade. <br> **Recomendação:** Oferecer a exportação dos dados filtrados em formatos comuns, como CSV e PDF, e exibir uma notificação de progresso durante a geração do arquivo. |

### GOMS
* **GOAL 0: Consultar o histórico de ações de um usuário**
    * **GOAL 1: Acessar a tela de histórico**
        * **METHOD 1.A:** Navegar pelo menu principal e clicar na opção "Logs"
            * (SEL. RULE: O usuário deve ter permissão de administrador para acessar esta área do sistema)
            * OP. 1.A.1: Deslocar o cursor para o menu de navegação principal (ex: "Administração")
            * OP. 1.A.2: Clicar no menu para expandir as opções
            * OP. 1.A.3: Deslocar o cursor para a opção "Logs" ou "Histórico"
            * OP. 1.A.4: Clicar na opção
            * OP. 1.A.5: Aguardar o carregamento da tela de histórico
    * **GOAL 2: Filtrar os resultados da busca**
        * **METHOD 2.A:** Definir um intervalo de datas e acionar o filtro
            * (SEL. RULE: O usuário informa uma data de início e fim para limitar os registros a um período específico)
            * OP. 2.A.1: Deslocar o cursor para o campo "Data de Início"
            * OP. 2.A.2: Clicar no campo para abrir o seletor de data
            * OP. 2.A.3: Selecionar a data de início desejada
            * OP. 2.A.4: Repetir os passos para o campo "Data de Fim"
            * OP. 2.A.5: Deslocar o cursor para o botão "Filtrar" ou "Buscar"
            * OP. 2.A.6: Clicar no botão
            * OP. 2.A.7: Aguardar a atualização dos resultados na tela
    * **GOAL 3: Analisar os dados apresentados**
        * **METHOD 3.A:** Ler a lista de ações na tela
            * (SEL. RULE: O sistema exibe a lista de eventos em ordem cronológica)
            * OP. 3.A.1: O sistema exibe a tabela de logs (ação do sistema)
            * OP. 3.A.2: O usuário lê e interpreta os dados exibidos
        * **METHOD 3.B:** Clicar em uma entrada para ver mais detalhes
            * (SEL. RULE: SE uma ação específica precisar de investigação, o usuário clica para obter informações adicionais como endereço IP)
            * OP. 3.B.1: Deslocar o cursor para a linha do log de interesse
            * OP. 3.B.2: Clicar na linha para expandir ou abrir uma janela de detalhes
            * OP. 3.B.3: Ler as informações detalhadas
    * **GOAL 4: Exportar o relatório de histórico**
        * **METHOD 4.A:** Acionar a exportação dos dados
            * (SEL. RULE: O arquivo com os dados atualmente exibidos na tela é gerado e salvo no computador do usuário)
            * OP. 4.A.1: Deslocar o cursor para o botão "Exportar"
            * OP. 4.A.2: Clicar no botão
            * OP. 4.A.3: Aguardar a geração e o download do arquivo
 
### CTT
O diagrama abaixo detalha o fluxo de interação, mostrando a sequência obrigatória de acessar os dados para depois habilitar as demais ações. Em seguida, o modelo ilustra a flexibilidade que o usuário possui para filtrar, analisar e exportar as informações, tarefas que podem ser executadas de forma independente e em qualquer ordem.

![ctt](https://github.com/user-attachments/assets/f7ef8300-a79b-40de-b317-7db0dfbe6e5e)

## 5. Consultar Logs de Câmera

### HTA
<img width="1303" height="444" alt="image" src="https://github.com/user-attachments/assets/b4906e26-5ae8-4258-bf38-df0c85b81314" />


| Objetivos/Operações | Problemas e Recomendações |
| :--- | :--- |
| **Consultar Logs de Câmera** | **Input:** O usuário acessa a interface de consulta de logs. <br> **Feedback:** Os logs de atividades da câmera são exibidos na tela. <br> **Plano:** Realizar a operação 1, depois a 2 e, em seguida, a 3. <br> **Recomendação:** O sistema deve oferecer um fluxo de navegação simples para que o usuário possa seguir as etapas da consulta. |
| **1. Informar critérios de busca** | **Plano:** Realizar a operação 1.1 e 1.2 em paralelo. <br> **Problema:** A seleção de múltiplos critérios pode ser confusa. <br> **Recomendação:** Use campos de autocompletar e seletores de data e hora para facilitar a entrada de dados. |
| **1.1 Informar identificador, localização e estação da câmera** | **Problema:** O usuário pode não saber o ID exato da câmera. <br> **Recomendação:** Permita que a busca seja feita por nome da estação ou localização. |
| **1.2 Informar data e hora do período a ser consultado** | **Problema:** A seleção de data e hora pode ser confusa. <br> **Recomendação:** Forneça opções de atalho, como "Últimas 24h", "Últimos 7 dias", ou "Último mês". |
| **2. Enviar critérios e requisição de consulta** | **Problema:** A consulta pode levar muito tempo para ser processada. <br> **Recomendação:** O sistema deve exibir um indicador de carregamento e um tempo estimado para a conclusão da busca. |
| **3. Visualizar o conteúdo da consulta** | **Plano:** O usuário pode exibir a lista de logs e realizar ações como filtrar e exportar. <br> **Recomendação:** Apresentar os resultados em uma tabela paginada com opções de filtro e ordenação. |
| **3.1 Exibir lista de logs** | **Problema:** A grande quantidade de logs pode dificultar a análise. <br> **Recomendação:** Apresente os resultados de forma clara, com colunas bem definidas para cada tipo de informação. |
| **3.2 Filtrar logs (ex: "Acessos", "Erros")** | **Problema:** O usuário precisa de uma forma eficiente para encontrar informações específicas. <br> **Recomendação:** Adicione filtros por tipo de evento e por nível de severidade. |
| **3.3 Exportar logs para um arquivo** | **Problema:** O usuário pode precisar dos dados para análise externa. <br> **Recomendação:** Forneça a opção de exportar os dados para formatos comuns como CSV ou Excel. |

### GOMS
* **GOAL 0: Consultar logs de câmera**
    * **GOAL 1: Informar os critérios de busca**
        * **METHOD 1.A:** Digitar ID e selecionar período
            * (SEL. RULE: O usuário sabe o ID exato da câmera e o período de interesse)
            * OP. 1.A.1: Deslocar o cursor para o campo de ID
            * OP. 1.A.2: Clicar no campo
            * OP. 1.A.3: Digitar o ID da câmera
            * OP. 1.A.4: Deslocar o cursor para o campo de período
            * OP. 1.A.5: Clicar no campo
            * OP. 1.A.6: Selecionar a data e hora de início e fim
    * **GOAL 2: Enviar a requisição de consulta**
        * **METHOD 2.A:** Clicar para consultar
            * (SEL. RULE: O usuário preencheu todos os campos necessários)
            * OP. 2.A.1: Deslocar o cursor para o botão "Consultar"
            * OP. 2.A.2: Clicar no botão
            * OP. 2.A.3: Aguardar a resposta do sistema
    * **GOAL 3: Visualizar os resultados da consulta**
        * **METHOD 3.A:** Exibir os logs na tela
            * (SEL. RULE: A consulta foi concluída com sucesso)
            * OP. 3.A.1: O sistema exibe os resultados (ação do sistema)
            * OP. 3.A.2: O usuário lê e interpreta os logs
        * **METHOD 3.B:** Exibir aviso de erro
            * (SEL. RULE: Nenhum log foi encontrado ou houve uma falha na consulta)
            * OP. 3.B.1: O sistema exibe a mensagem de erro (ação do sistema)
            * OP. 3.B.2: O usuário lê a mensagem e entende o problema

### CTT
<img width="1297" height="602" alt="image" src="https://github.com/user-attachments/assets/b0c98c8a-831b-49c3-9c90-13bb921bdc33" />
