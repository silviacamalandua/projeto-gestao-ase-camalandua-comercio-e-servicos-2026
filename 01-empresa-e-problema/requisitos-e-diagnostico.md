# Diagnóstico da Empresa 

A ASE Camalandua Comércio e Serviços apresenta dificuldades relacionadas à organização e à distribuição das tarefas internas entre os funcionários.

Considerando o cenário analisado, foi identificado que uma das principais causas desse problema é a falta de comunicação eficiente entre os colaboradores e a ausência de uma definição clara de responsabilidades para determinadas atividades.

Essa situação pode gerar a duplicação de tarefas, uma vez que mais de um funcionário pode executar a mesma atividade sem ter conhecimento de que ela já foi atribuída ou iniciada por outra pessoa. Também pode ocorrer o problema inverso, no qual determinadas tarefas deixam de ser realizadas por não haver um reponsável claramente definido.

A falta de organização das atividades e de acompanhamento do andamento das tarefas pode dificultar na execução dos serviços e aumentar o tempo necessário para a sua conclusão.

Como consequência, ocorre uma redução da eficiência operacional, dificuldade no acompanhamento das responsabilidades e menor controle sobre o fluxo das atividades e prejuízos no atendimento aos clientes, que podem enfrentar maior tempo de espera para a conclusão dos serviços solicitados.

Diante desse diagnóstico, foi definida como proposta de solução a futura implementação de um sistema para cadastro, atribuição e acompanhamento das tarefas dos funcionários, permitindo uma distribuição mais organizada das responsabilidades e maior controle sobre o andamento das atividades.

Nesta etapa, o projeto será direcionado ao planejamento e à especificação da solução proposta, incluindo a definição das funcionalidades, regras de negócio e requisitos de segurança, além da realização de análise de dados e de modelos de otimização que contribuam para compreender os problemas operacionais e apoiar a tomada de decisões.

# Requisitos do Sistema 

# Requisitos Funcionais 

RF01 - Cadastro de Funcionários 

O sistema deve permitir o cadastro dos funcionários da empresa.

RF02 - Restrição do Cadastro dos Funcionários 

Somente o usuário com o perfil de administrador deve possuir a permissão para cadastrar, alterar, eliminar ou desativar funcionários no sistema.

RF03 - Cadastro de Tarefas 

O sistema deve permirtir que o administrador e o gerente cadastrem as tarefas que serão executadas pelos funcionários.

RF04 - Resgistro do Tipo de Atividade

O sistema deve permitir identificar o tipo de atividade relacionada à tarefa, como venda, manutenção, reparo ou administrativa.

RF05 - Atribuição de Tarefas 

O sistema deve exigir a atribuição de cada tarefa a um funcionário responsável pela sua execução.

RF06 - Restrição da Atribuição de Tarefas 

Somente usuários autorizados, com perfil de gerente ou administrador, devem possuir permissão para atribuir tarefas aos demais funcionários.

RF07 - Consulta e Acompanhameno das Tarefas

O sistema deve permitir a consulta e o acompanhamento das tarefas de dos seus respectivos status.

Cada funcionário deverá visualizar as tarefas atríbuidas a ele, enquanto o gerente e o administrador poderão visualizar as tarefas de todos os funcionários.Os status previstos são:
- Pendente;
- Em andamento;
- Aguardando validação;
- Finalizada 

RF08 - Execução das Tarefas 

O sistema não deve permitir que um funcionário realize mais de uma tarefa, ou seja, ele não deve permitir que o funcionário mantenha mais de uma tarefa com status "Em andamento" simultaneamente.
O funcionário poderá possuir várias tarefas atribuídas, porém somente uma poderá ser executada por vez.

RF9 - Solicitação de Conclusão 

Após a conclusão de uma tarefa, o sistema deve permitir que o funcionário responsável altere o status da tarefa para "aguardando validação".

RF10 - Validação da Conclusão da Tarefa

O sistema deve permitir que somente usuários com perfil de gerente ou administrador validem a conclusão das tarefas.
Após a validação, o sistema deverá alterar o status da tarefa de "Aguardando validação" para "Finalizada".


# Requisitos Não Funcionais 

RNF01 - Autenticação

O sistema deve exigir a autenticação por usuário e senha para permitir o acesso às funcionalidades.

RNF02 - Disponibilidade

O sistema deve permanecer disponível durante o horário de funcionamento da empresa.

RNF03 - Controle de Acesso 

O sistema deve restringir o acesso às funcionalidades de acordo com o perfil do usuário, diferencioando as permissões de funcionários, gerente e administrador.

RNF04 - Confidencilidade dos Dados 

O sistema deve proteger os dados dos funcionários e dos clientes contra acessos não autorizados.