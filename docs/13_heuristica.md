#  Avaliação Heurística

<div align="center">

| Heurística | Pedro | Gian | Paulo |
| :--- | :---: | :---: | :---: |
| 1. Visibilidade do status do sistema | 0 | 0 | 0 |
| 2. Compatibilidade com o mundo real | 2 | 0 | 0 |
| 3. Controle e liberdade do usuário | 3 | 0 | 2 |
| 4. Consistência e padrões | 1 | 0 | 0 |
| 5. Prevenção de erros | 0 | 0 | 0 |
| 6. Reconhecimento em vez de lembrança | 0 | 2 | 2 |
| 7. Flexibilidade e eficiência de uso | 2 | 2 | 2 |
| 8. Projeto minimalista e estético | 1 | 0 | 0 |
| 9. Diagnóstico e recuperação de erros | 0 | 3 | 0 |
| 10. Ajuda e documentação | 0 | 2 | 3 |

</div>

---

| # | Heurística | Descrição (Critério) | Problemas Identificados |
| :---: | :--- | :--- | :--- |
| **1** | **Visibilidade do status do sistema** | O sistema deve sempre manter os usuários informados sobre o que está acontecendo através de feedback apropriado, em um tempo razoável. | *Nenhum problema identificado.* |
| **2** | **Compatibilidade entre sistema e mundo real** | O sistema deve utilizar a linguagem do usuário, com palavras, frases e conceitos familiares. A informação deve aparecer em ordem lógica e natural. | *Nenhum problema identificado.* |
| **3** | **Controle e liberdade para o usuário** | Usuários precisam de uma "saída de emergência" (undo/redo) para sair de estados indesejados sem percorrer longos diálogos. | • **(Paulo):** Sistema rígido ("chumbado"), permitindo apenas o fluxo estrito disponível, sem liberdade.<br>• **(Pedro):** **[GRAVE]** Falha de permissão onde todos os usuários possuem acesso de Administrador. |
| **4** | **Consistência e padrões** | Os usuários não deveriam ter que se perguntar se palavras, situações ou ações diferentes significam a mesma coisa. | • **(Pedro):** Apontado como inconsistência "Cosmética" (Grau 1), sem detalhamento específico. |
| **5** | **Prevenção de erros** | Um design cuidadoso que previne a ocorrência de problemas é melhor que boas mensagens de erro. | *Nenhum problema identificado.* |
| **6** | **Reconhecimento em lugar de lembrança** | O usuário não deve ter que lembrar informações de uma parte do diálogo para outra. Instruções devem estar visíveis. | • **(Paulo):** Menus exigem memorização do caminho para serem acessados (ex: Logs de Usuário).<br>• **(Gian):** Na edição de dispositivos, campos como "ID da Câmera" aparecem em branco, forçando o usuário a lembrar os dados originais. |
| **7** | **Flexibilidade e eficiência de uso** | O sistema deve atender usuários inexperientes e experientes (uso de atalhos e aceleradores). | • **(Pedro):** Usuário forçado a sempre voltar ao Menu para qualquer ação.<br>• **(Paulo):** Navegação ineficiente em telas de logs, exigindo muitos passos.<br>• **(Gian):** Ausência total de atalhos, criando dependência do menu lateral. |
| **8** | **Projeto minimalista e estético** | Diálogos não devem conter informações irrelevantes que competem com a informação útil. | • **(Pedro):** Apontado como problema "Cosmético" (Grau 1), sem detalhamento específico. |
| **9** | **Auxiliar os usuários a reconhecer e recuperar erros** | Mensagens de erro devem ser em linguagem natural, precisas e sugerir solução. | • **(Gian):** **[GRAVE]** O sistema não apresenta mensagens de erro detalhadas, dificultando o diagnóstico. |
| **10** | **Ajuda e documentação** | Informações de ajuda devem ser fáceis de encontrar, focadas na tarefa e listar passos concretos. | • **(Paulo):** **[GRAVE]** Interface sem informações de ajuda para situar o usuário.<br>• **(Gian):** Inexistência de ícones de ajuda ou links para documentação/suporte. |

##  Exemplo – Heurística 6  
**Reconhecimento em vez de lembrança**

<p align="center">
  <img src="https://github.com/user-attachments/assets/7f84cc9a-fcda-49f8-8f05-92082ca79100" alt="Exemplo heurística 6" width="1280" height="720"/>
</p>

---

##  Exemplo – Heurística 7  
**Flexibilidade e eficiência de uso**

<p align="center">
  <img src="https://github.com/user-attachments/assets/d13993e9-afb9-46e5-9eb4-af29d363d77c" alt="Exemplo heurística 7" width="1280" height="720"/>
</p>

---

##  Exemplo – Heurística 9  
**Prevenção de erros**

<p align="center">
  <img src="https://github.com/user-attachments/assets/55957122-a980-4c3c-979e-8a321e378ccb" alt="Exemplo heurística 9" width="1280" height="720"/>
</p>

>  **Observação:** Poderia haver uma tela de erro ao cadastrar usuário por qualquer motivo inválido.

---

##  Exemplo – Heurística 10  
**Ajuda e documentação**

<p align="center">
  <img src="https://github.com/user-attachments/assets/440afc87-4295-43cc-9d9d-4688146ade86" alt="Exemplo heurística 9" width="1280" height="720"/>
</p>

>  **Observação:** A tela principal poderia exibir mensagens orientando o usuário sobre como utilizar o aplicativo.

---

## INDICAÇÃO DE BOAS PRÁTICAS DE HEURÍSTICA - HEURÍSTICAS NÃO VIOLADAS

> **Nota:** Abaixo estão listadas soluções completas onde a heurística foi atendida, baseando-se nas avaliações onde não foram detectados problemas de usabilidade (classificados como "Sem importância").

### 1. Visibilidade do status do sistema
* **Avaliador de referência:** Paulo (Heurística atendida).
* **Cenário do Sistema:** O usuário acessa a tela de monitoramento de câmeras que carrega um fluxo de vídeo pesado.
* **Boa Prática Aplicada:** Ao clicar em "Visualizar Câmera", o sistema exibe imediatamente um ícone de carregamento (*spinner*) girando com a mensagem "Carregando stream de vídeo...".
* **Por que funciona:** Isso informa ao usuário que a solicitação foi recebida e está sendo processada, evitando cliques repetidos por incerteza se o sistema travou.

### 2. Compatibilidade entre sistema e mundo real
* **Avaliador de referência:** Pedro (Heurística atendida).
* **Cenário do Sistema:** Configuração de permissões de acesso para um novo funcionário.
* **Boa Prática Aplicada:** O sistema utiliza cargos com permissões pré estabilecidas na criação do usuário, sem necessidade de utilizar outros termos complexos para seleção de permissões do usuário.
* **Por que funciona:** A linguagem segue as convenções do mundo real e a hierarquia da empresa, tornando a interface natural e lógica para quem não é da área de TI.

### 3. Prevenção de erros
* **Avaliador de referência:** Gian (Heurística atendida).
* **Cenário do Sistema:** O usuário clica acidentalmente no botão de "Excluir Dispositivo" na lista de câmeras.
* **Boa Prática Aplicada:** O sistema aciona um modal de confirmação: "Tem certeza que deseja remover esta câmera? Esta ação não pode ser desfeita", exigindo um segundo clique consciente.
* **Por que funciona:** O design previne a ocorrência de erros graves acidentais, garantindo que ações destrutivas sejam sempre intencionais.
  
##  Conclusão

As avaliações foram realizadas sobre **protótipos desenvolvidos no Figma**, ainda em uma versão inicial.  
A análise revelou que, embora haja consenso em algumas heurísticas — como **visibilidade do status do sistema** e **prevenção de erros** —, existem divergências relevantes em outras.

- **Rocha** destacou problemas de segurança e controle de acesso, atribuindo severidade alta à liberdade do usuário.  
- **Gian** foi mais crítico quanto à ausência de mensagens de erro detalhadas e à falta de documentação.  
- **Paulo** apontou limitações de navegação e ausência de suporte ao usuário.

###  Heurísticas mais problemáticas segundo os avaliadores:
- Controle e liberdade do usuário  
- Reconhecimento em vez de lembrança  
- Ajuda e documentação  

>  **Próximos passos:** Priorizar melhorias nessas áreas para aumentar a **usabilidade e a satisfação do usuário**.




