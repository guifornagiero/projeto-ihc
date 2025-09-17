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
