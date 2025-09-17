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

## 2. Cadastro de Câmera

### HTA
<img width="1337" height="480" alt="image" src="https://github.com/user-attachments/assets/8eba7f6b-1787-407c-8d5d-bf59853ab1d4" />

### GOMS
GOAL 0: Cadastrar câmera
<br> GOAL 1: Inserir Identificador, localização e estação da câmera
<br> METHOD 1.A: Digitar ID e localização
<br> (SEL. RULE: O ID deve ser único para o sistema e a localização deve ser descrita de forma textual)
<br> METHOD 1.B: Selecionar estação
<br> (SEL. RULE: Estações são pré-definidas no sistema)
<br> GOAL 2: Enviar dados da câmera para o sistema
<br> METHOD 2.A: Salvar e enviar os dados da câmera
<br> (SEL. RULE: Os dados são submetidos para processamento e salvos no banco de dados)
<br> GOAL 3: Enviar mensagem confirmando sucesso no cadastramento
<br> METHOD 3.A: Exibir a mensagem de sucesso na tela
<br> (SEL. RULE: Os dados foram salvos com sucesso e o sistema confirma o cadastramento)
<br> METHOD 3.B: Exibir aviso de falha
<br> (SEL. RULE: O sistema não consegue salvar os dados devido a um erro, como ID duplicado ou falha de conexão com o banco de dados)

### CTT
