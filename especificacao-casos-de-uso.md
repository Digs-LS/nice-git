# 📝 Especificação de Caso de Uso

## 1. Introdução
O objetivo da especificação é definir as espeficiações de cada caso de uso do sistema para implementação.

## 2. Casos de uso


| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Realizar Login |
| **Ator Principal**    | Usuário |
| **Pré-condições**     | Usuário já cadastrado no sistema |
| **Fluxo Principal**   | 1. Usuário insere login e senha <br> 2. Sistema valida credenciais <br> 3. Sistema libera acesso |
| **Fluxos Alternativos** | Senha incorreta → Sistema exibe mensagem de erro |
| **Pós-condições**     | Usuário autenticado no sistema |
| **Regras de negócio** | Senha deve ter no mínimo 8 caracteres |

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Acessar questionário |
| **Ator Principal**    | Colaborador |
| **Pré-condições**     | Colaborador já cadastrado no sistema e logado no sistema |
| **Fluxo Principal**   | 1. Sistema abre mostrando a opção de responder questionário <br> 2. Colaborador clica em "Abrir Questionário" <br> 3. Sistema abre o questionário |
| **Pós-condições**     | Colaborador com o questionário aberto no sistema |
| **Regras de negócio** | |

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Preencher questionário |
| **Ator Principal**    | Colaborador |
| **Pré-condições**     | 1. Colaborador já logado no sistema <br> 2. Questionário aberto no sistema |
| **Fluxo Principal**   | 1. Sistema mostra questões que devem  <br> 2. Colaborador responde questões presentes no questionário |
| **Fluxos Alternativos** | Questão sem resposta → Sistema exibe mensagem de pergunta obrigatória necessita resposta |
| **Pós-condições**     | Questionário com perguntas preenchidas com respostas |
| **Regras de negócio** | Todas as questões do questionário preenchidas; publicação anônima |

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Publicar Sugestão sobre dinâmica da empresa  |
| **Ator Principal**    | Colaborador |
| **Pré-condições**     | Colaborador já cadastrado e autenticado no sistema com o tipo ‘Colaborador’ |
| **Fluxo Principal**   | 1. Colaborador seleciona a opção ‘Enviar sugestões’ <br> 2. Colaborador preenche campo de texto com suas sugestões <br> 3. Colaborador envia o texto de sugestão <br> 4. Sistema armazena sugestões e alerta o Psicólogo e Gestor da Equipe sobre nova sugestão |
| **Fluxos Alternativos** | Campo vazio → Sistema não permite envio e expõe alerta com indicação do problema |
| **Pós-condições**     | Nova sugestões sobre dinâmica da empresa armazenada no sistema |
| **Regras de negócio** | Sugestão deve conter no mínimo 10 caracteres |


| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Publicar feedback |
| **Ator Principal**    | Colaborador |
| **Pré-condições**     | Colaborador já cadastrado e autenticado no sistema como ‘Colaborador’ |
| **Fluxo Principal**   | 1. Colaborador seleciona a opção ‘Enviar feedback’ <br> 2. Colaborador preenche o campo de texto com sua experiência <br> 3. Colaborador envia o texto de feedback <br> 4. Sistema armazena novo feedback e alerta Administrador | 
| **Fluxos Alternativos** | Campo vazio → Sistema não permite o envio e exibe alerta com a indicação do problema |
| **Pós-condições**     | Novo feedback armazenado no sistema e mensagem enviada ao Administrador |
| **Regras de negócio** | Feedback deve conter no mínimo 10 caracteres |

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Reportar situações |
| **Ator Principal**    | Colaborador |
| **Pré-condições**     | Colaborador já cadastrado e autenticado no sistema como ‘Colaborador’ |
| **Fluxo Principal**   | 1. Colaborador seleciona a opção ‘Reportar situação’ <br> 2. Colaborador preenche o campo de texto com situação <br> 3. Colaborador envia o texto com situação <br> 4. Sistema armazena nova situação reportada e alerta Psicólogo e Gestor da Equipe | 
| **Fluxos Alternativos** | Campo vazio → Sistema não permite o envio e exibe alerta com a indicação do problema |
| **Pós-condições**     | Nova situação armazenada no sistema e mensagem enviada ao Psicólogo e ao Gestor da Equipe |
| **Regras de negócio** | Situação reportada deve conter no mínimo 10 caracteres; publicação anônima |

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Visualizar Questionário  | 
| **Ator Principal**  | Gestor de Equipe, Psicólogo |
| **Pré-condições**     | Usuário já cadastrado no seu sistema administrativo por meio de Login e Senha |
| **Fluxo Principal**   | 1. Usuário já cadastrado tem acesso a interface do sistema <br> 2. Por meio do botão “Visualizar Questionário” o usuário visualiza o questionário disponível no momento. | 
| **Pós-condições**     | Usuário já visualizou o questionário | 

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Gerar relatório dos questionários  | 
| **Ator Principal**  | Gestor de Equipe, Psicólogo |
| **Pré-condições**     | Usuário já cadastrado no sistema e tem acesso aos questionários preenchidos no último trimestre | 
| **Fluxo Principal**   | 1. O Sistema notifica o usuário da liberação de um novo relatório pronto. <br> 2. O usuário clica no botão ‘Gerar relatório’ <br> 3. O usuário libera o novo questionário para os usuários. | 
| **Fluxos Alternativos** | Não é possível enviar o questionário  → Sistema exibe mensagem de erro ao usuário quando alguma exigência  não é cumprida |
| **Pós-condições**     | Um relatório foi criado pelo usuário de Equipe | 

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Visualizar situações reportadas |
| **Ator Principal**    | Gestor de equipe, Psicólogo |
| **Pré-condições**     | Usuário já cadastrado no sistema |
| **Fluxo Principal**   | 1. Usuário faz o login no sistema administrativo com login e senha <br> 2. Usuário clica na aba situações reportadas <br> 3. Usuário consulta situações reportadas  |
| **Fluxos Alternativos** | Não é possível realizar a consulta → Sistema exibe mensagem de erro |
| **Pós-condições**     | Usuário autenticado no sistema |
| **Regras de negócio** | |

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Visualizar sugestões |
| **Ator Principal**    | Psicólogo, Gestor de equipe |
| **Pré-condições**     | Usuário já cadastrado no sistema |
| **Fluxo Principal**   | 1. Usuário faz o login no sistema administrativo com login e senha <br> 2. Usuário clica na aba sugestões publicadas <br> 3. Usuário consulta as sugestões publicadas  |
| **Fluxos Alternativos** | Não é possível realizar a consulta → Sistema exibe mensagem de erro |
| **Pós-condições**     | Usuário autenticado no sistema |
| **Regras de negócio** | |

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Criar o questionário |
| **Ator Principal**    | Psicólogo |
| **Pré-condições**     | Usuário já cadastrado no sistema |
| **Fluxo Principal**   | 1. Usuário faz o login no sistema administrativo com login e senha <br> 2. Usuário clica na aba Questionários <br> 3. Usuário clica no botão “Criar questionário” <br> 4. Usuário escreve questões. <br> 5. Usuário salva o questionário. |
| **Fluxos Alternativos** | Erro na criação do sistema → Sistema exibe mensagem de erro |
| **Pós-condições**     | Usuário autenticado no sistema e com autorização para criar questionários |
| **Regras de negócio** | 5 questões |

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Visualizar Feedback  |
| **Ator Principal**    | Administrador |
| **Pré-condições**     | 1. Sistema estar funcionando <br> 2. O administrador dever estar autenticado |
| **Fluxo Principal**   | 1. Administrador acessa o sistema <br> 2. Sistema valida credenciais <br> 3. Sistema libera acesso <br> 4. Administrador entra na página menu <br> 5. No menu lateral contém o botão “Feedbacks” <br> 6. Administrador clica no botão “Feedbacks”. <br> 7. Sistema abre interface de “Feedbacks”. <br> 8. Sistema exibe a lista de feedbacks enviados pelos colaboradores.   |
| **Fluxos Alternativos** | 1. Caso não existam feedbacks na lista, o sistema exibe a mensagem “Nenhum feedback disponível no momento”. <br> 2. Caso ocorra falha na conexão, o sistema exibe a mensagem “Erro de conexão. Tente novamente mais tarde” |
| **Pós-condições**     | 1. O administrador tem acesso ao histórico de feedbacks dos colaboradores. |
| **Regras de negócio** | 1. Feedback anônimos não podem exibir informações que identifiquem o colaborador. <br> 2. O sistema deve permitir filtragem de feedbacks por período (ex: mensal ou semanal) <br> Apenas usuários com perfil de Administrador podem acessar o módulo de feedbacks |


