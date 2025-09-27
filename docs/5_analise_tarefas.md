# Análise de Tarefas

> **_NOTE:_**: A equipe deve descrever as funcionalidades mais importantes da interface/produto. A equipe deve modelar pelo menos 1 HTA, 1 GOMS e 1 CTT (de pelo menos 4 funcionalidades diferentes). Cada diagrama deve ter um texto explicando a funcionalidade.

## 1. Cadastro de Usuário

### HTA
<img width="1337" height="480" alt="image" src="https://github.com/user-attachments/assets/e7775ce4-bacc-416f-bf4e-1f2920efb55d" />

### GOMS
GOAL 0: Cadastrar novo usuário
<br> GOAL 1: Inserir dados do usuário
<br> METHOD 1.A: Digitar nome, e-mail
<br> (SEL. RULE: Nome tem que ter apenas letras e e-mail tem que ser no formato de e-mail)
<br> METHOD 1.B: Selecionar estação
<br> (SEL. RULE: Estações são pré-definidas no sistema)
<br> METHOD 1.C: Selecionar perfil de acesso
<br> (SEL. RULE: Usuário escolhe entre admin, analista ou operador)
<br> GOAL 2: Enviar e-mail com senha
<br> METHOD 2.A: Gerar senha automática e enviar por e-mail
<br> (SEL. RULE: política padrão do sistema)
<br> GOAL 3: Confirmar sucesso do cadastro
<br> METHOD 3.A: Mostrar mensagem de sucesso na tela
<br> (SEL. RULE: dados salvos e e-mail enviado)
<br> METHOD 3.B: Mostrar aviso parcial (sem e-mail enviado)
<br> (SEL. RULE: falha no envio mas sistema permite cadastro mesmo assim)

### CTT
<img width="1299" height="690" alt="image" src="https://github.com/user-attachments/assets/caaeaaaa-17b2-43e3-90e4-d59d2be36890" />

## 2. Cadastro de Câmera

### HTA
<img width="1337" height="480" alt="image" src="https://github.com/user-attachments/assets/8eba7f6b-1787-407c-8d5d-bf59853ab1d4" />
<br>
### 0. Cadastrar Câmera
* **Input:** O usuário inicia a tarefa ao acessar o formulário de cadastro de câmeras.
* **Feedback:** A câmera cadastrada é adicionada à lista de equipamentos do sistema.
* **Plano:** Realizar a operação 1, depois a 2 e, em seguida, a 3.
* **Recomendação:** O sistema deve oferecer um fluxo de navegação simples para que o usuário possa seguir as etapas de cadastro sem confusão.

### 1. Informar identificador, localização e estação da câmera
* **Problema:** Um usuário pode inserir um ID que já existe no sistema, ou a descrição da localização ser ambígua.
* **Recomendação:** Implementar uma validação em tempo real para o ID da câmera e utilizar campos de preenchimento automático para a estação.

### 2. Enviar dados da câmera para o sistema
* **Problema:** O envio dos dados pode falhar devido a problemas de conexão ou do servidor.
* **Recomendação:** O sistema deve exibir mensagens de erro claras e informativas, orientando o usuário sobre o que fazer em caso de falha.

### 3. Enviar mensagem informando sucesso no cadastramento
* **Problema:** A mensagem de confirmação pode ser facilmente ignorada se for muito discreta ou temporária.
* **Recomendação:** A mensagem de sucesso deve ser visualmente destacada e persistir na tela por tempo suficiente para garantir que o usuário a veja.

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
Essa funcionalidade permite que administradores visualizem um log completo das atividades dos usuários no sistema, como quem fez login ou ativou uma câmera e quando isso ocorreu. A análise abaixo demonstra o fluxo que o administrador segue para encontrar, filtrar e exportar essas informações para fins de segurança e auditoria.


![hta-gian](https://github.com/user-attachments/assets/ad8d5562-4e32-4f57-83c3-515c157c69b4)

### GOMS
GOAL 0: Consultar o histórico de ações de um usuário
<br> GOAL 1: Acessar a tela de histórico
<br> METHOD 1.A: Navegar pelo menu principal e clicar na opção "Logs"
<br>(SEL. RULE: O usuário deve ter permissão de administrador para acessar esta área do sistema)
<br> GOAL 2: Filtrar os resultados da busca
<br> METHOD 2.A: Definir um intervalo de datas e acionar o filtro
<br> (SEL. RULE: O usuário informa uma data de início e fim para limitar os registros a um período específico)
<br> GOAL 3: Analisar os dados apresentados
<br> METHOD 3.A: Ler a lista de ações na tela
<br> (SEL. RULE: O sistema exibe a lista de eventos em ordem cronológica)
<br> METHOD 3.B: Clicar em uma entrada para ver mais detalhes
<br> (SEL. RULE: SE uma ação específica precisar de investigação, o usuário clica para obter informações adicionais como endereço IP)
<br> GOAL 4: Exportar o relatório de histórico
<br> METHOD 4.A: Acionar a exportação dos dados
<br> (SEL. RULE: O arquivo com os dados atualmente exibidos na tela é gerado e salvo no computador do usuário)
 
### CTT
O diagrama abaixo detalha o fluxo de interação, mostrando a sequência obrigatória de acessar os dados para depois habilitar as demais ações. Em seguida, o modelo ilustra a flexibilidade que o usuário possui para filtrar, analisar e exportar as informações, tarefas que podem ser executadas de forma independente e em qualquer ordem.

![ctt](https://github.com/user-attachments/assets/f7ef8300-a79b-40de-b317-7db0dfbe6e5e)

