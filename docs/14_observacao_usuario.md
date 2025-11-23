1) **Fluxograma de Avaliação de Usabilidade por Observação do Usuário**
   <img width="1192" height="174" alt="image" src="https://github.com/user-attachments/assets/8b377246-b97f-499b-9cb4-b4245fd99a5f" />


3) **DESCRIÇÃO DO PROCEDIMENTO DE PREPARAÇÃO DO TESTE \[1 solução por equipe\]**

**Passo 1: Definir os objetivos e o escopo da avaliação (Validar os fluxos MOLIC, identificar problemas e medir a eficácia das tarefas).**  
**Passo 2: Definir o perfil dos participantes (Persona Analista, Operador e Administrador) e recrutar 6 usuários (2 de cada perfil).**  
**Passo 3: Definir as tarefas (cenários) que os participantes irão executar, com base nos diagramas MOLIC e no Mapa de Objetivos.**  
**Passo 4: Preparar e imprimir todos os instrumentos e materiais de apoio necessários.**
**Passo 5: Preparar o ambiente, hardware (computador com o protótipo) e software (para gravação de tela).**
**Passo 6: Realizar um teste-piloto (com um colega de equipe) para validar o roteiro, as tarefas e o tempo estimado.**

3) **RESULTADOS DO TESTE \[1 solução por equipe\]**

**Avaliação de cada Tarefa (para cada usuário)**

| Tarefa | Grau de Sucesso | Total de Erros cometidos | Tipos de Erros | Tempo Necessário | Grau de Satisfação |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1 (P01 - Analista)** | Sucesso Parcial | 2 | (1) Recuperação (erro de data), (1) Compreensão (botão exportar) | 3 min e 10 seg | Confusão Moderada |
| **2 (P02 - Operador)** | Sucesso Total | 1 | (1) Hesitação (procurou o botão 'Salvar' no lugar errado) | 1 min 25 seg | Satisfeito |
| **3 (P03 - Admin)** | Sucesso Total | 0 | N/A (Nenhum erro cometido) | 48 seg | Muito Satisfeito |
| **1 (P04 - Analista)** | Sucesso Total | 2 | (1) Recuperação (erro de data), (1) Compreensão (botão exportar) | 2 min 15 seg | Insatisfeito |
| **2 (P05 - Operador)** | Sucesso Parcial | 1 | (1) Falha (Tentou salvar com ID duplicado, erro [SR] 'ID já cadastrado') | 2 min 05 seg | Neutro |

**Links dos vídeos:** https://youtu.be/G2DB18q2k2Q 

**Respostas do Formulário do Usuário:**

### **Usuário P01 (Analista - Tarefa 1)**

* **Perfil (Pré-teste):**
    * **Função:** Analista de Dados
    * **Experiência:** 3 a 5 anos
    * **Conforto com novas ferramentas (1-5):** 4
* **Satisfação (Pós-teste):**
    * **Achei o sistema fácil de usar (1-5):** 3 (Neutro)
    * **As mensagens de erro me ajudaram (1-5):** 2 (Discordo)
    * **O que foi mais difícil?** "A mensagem de erro da data não foi clara. Não sabia se eu tinha digitado errado ou se a data final não podia ser antes da inicial. Também demorei para achar o botão de exportar."
    * **O que mudaria?** "Colocar o botão 'Exportar' em um lugar mais óbvio."

---

### **Usuário P02 (Operador - Tarefa 2)**

* **Perfil (Pré-teste):**
    * **Função:** Operador de Câmeras
    * **Experiência:** 1 a 3 anos
    * **Conforto com novas ferramentas (1-5):** 3
* **Satisfação (Pós-teste):**
    * **Achei o sistema fácil de usar (1-5):** 5 (Concordo Totalmente)
    * **Me senti confiante usando o sistema (1-5):** 5 (Concordo Totalmente)
    * **O que foi mais fácil?** "O formulário para adicionar a câmera. É muito melhor do que usar os comandos no terminal."
    * **O que mudaria?** "Nada, para essa tarefa foi ótimo."

---

### **Usuário P03 (Admin - Tarefa 3)**

* **Perfil (Pré-teste):**
    * **Função:** Administrador
    * **Experiência:** Mais de 5 anos
    * **Conforto com novas ferramentas (1-5):** 4
* **Satisfação (Pós-teste):**
    * **Achei o sistema fácil de usar (1-5):** 5 (Concordo Totalmente)
    * **As informações estavam claras e organizadas (1-5):** 5 (Concordo Totalmente)
    * **O que foi mais fácil?** "Achar o histórico. Foi muito rápido, os filtros são simples e a tabela de resultados é limpa."
    * **O que mudaria?** "Gostaria de poder salvar meus filtros mais usados."

---

### **Usuário P04 (Analista - Tarefa 1)**

* **Perfil (Pré-teste):**
    * **Função:** Analista de Dados
    * **Experiência:** 1 a 3 anos
    * **Conforto com novas ferramentas (1-5):** 5
* **Satisfação (Pós-teste):**
    * **Achei o sistema fácil de usar (1-5):** 2 (Discordo)
    * **As mensagens de erro me ajudaram (1-5):** 1 (Discordo Totalmente)
    * **O que foi mais difícil?** "Exatamente a mesma coisa do meu colega [P01]. O erro da data é péssimo e o botão de exportar está escondido. Eu me senti frustrado."
    * **O que mudaria?** "A mensagem de erro precisa dizer *o que* está errado. E o botão de exportar devia estar no topo da tela."

---

### **Usuário P05 (Operador - Tarefa 2)**

* **Perfil (Pré-teste):**
    * **Função:** Operador de Câmeras
    * **Experiência:** Mais de 5 anos
    * **Conforto com novas ferramentas (1-5):** 2
* **Satisfação (Pós-teste):**
    * **Achei o sistema fácil de usar (1-5):** 3 (Neutro)
    * **Me senti confiante usando o sistema (1-5):** 3 (Neutro)
    * **O que foi mais difícil?** "Eu tentei cadastrar um ID que já tinha, e o sistema deu um erro `[SR] d: Erro: ID já cadastrado`. Foi bom, mas eu tive que apagar tudo e começar de novo. Podia só limpar o campo do ID."
    * **O que mudaria?** "Quando der um erro, não limpar o formulário todo, só o campo que deu problema."
---

**Conclusão da avaliação por observação do usuário:**

**Pontos Positivos (Sucessos):**

* **Fluxos de Gerenciamento (Operador e Admin):** As tarefas de "Cadastro de Câmera" (Operador - P02 e P05) e "Consultar Histórico de Ações" (Admin - P03) foram validadas com sucesso.
* **Alta Satisfação:** Os usuários (P02, P03) classificaram essas tarefas como "fáceis" e "Muito Satisfatórias", destacando a superioridade da interface visual em relação aos seus métodos de trabalho atuais (linha de comando, e-mail).
* **Eficiência:** O Administrador (P03) completou sua tarefa em menos de 1 minuto e sem erros, demonstrando alta eficiência da interface.

**Pontos Críticos (Falhas):**

* **Fluxo de Análise de Dados (Analista):** A tarefa "Gerar Relatório de Fluxo" (Analista - P01 e P04) apresentou falhas graves de usabilidade, resultando em "Sucesso Parcial", confusão e insatisfação.
* **Principais Problemas Identificados:**
    1.  **Mensagens de Erro Ineficazes:** O erro `[SR] d: Erro: Datas são obrigatórias` no MOLIC `Gerar Relatório de Fluxo` se mostrou genérico e não ajudou os usuários (P01 e P04) a se recuperarem, violando o princípio de "Projeto para Erros".
    2.  **Baixa Visibilidade:** Ambos os analistas (P01 e P04) tiveram dificuldade em localizar o botão "Exportar Relatório" após a geração do gráfico, indicando uma falha no princípio de "Visibilidade e Reconhecimento".
    3.  **Recuperação de Erro Frustrante:** O Operador P05, ao receber o erro `[SR] d: Erro: ID já cadastrado`, teve o formulário inteiro limpo, aumentando seu retrabalho.


