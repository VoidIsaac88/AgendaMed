Documento de Visão e Escopo do Projeto
AgendaMed - Gestão de Clínicas e Consultórios
Equipe de Produto: Amanda, Carlos André Gama Santos Silva, Gabriel Alcantara Ribeiro, Isaac Silva
Morais, Jose Marcio Silva Pinho e Marcos Vinícius Cardoso de Araújo
Product Owner: Isaac Silva Morais
Sumário
1. Introdução
2. Personas e Público-Alvo
3. Requisitos Funcionais
4. Requisitos Não Funcionais
5. Recomendações para a Equipe de Desenvolvimento
1. Introdução
1.1. Visão Geral do Projeto
O projeto AgendaMed visa desenvolver uma plataforma web para modernizar a gestão de
clínicas e consultórios, substituindo processos manuais e descentralizados por uma
operação digital, eficiente e segura. O sistema centraliza agendamentos, prontuários
eletrônicos e relatórios administrativos, com o objetivo de otimizar o tempo dos
profissionais, reduzir erros operacionais e melhorar a experiência de agendamento para os
pacientes.
1.2. Escopo do Projeto
Funcionalidades DENTRO do Escopo:
Cadastro e autenticação de usuários.
Agendamento, cancelamento e remarcação.
Visualização de agenda por profissional.
Controle de prontuários eletrônicos.
Relatórios administrativos básicos.
Notificações de confirmação e lembrete.
Funcionalidades FORA do Escopо:
Sistema de pagamento online integrado.
Funcionalidade de Telemedicina.
Integração com agendas externas (Google/Outlook).
Relatórios financeiros avançados.
1.3. Glossário de Termos
Prontuário Eletrônico (PEP): Registro digital das informações de saúde do paciente.
Perfil de Acesso (Role): Conjunto de permissões que define o que cada tipo de usuário
pode fazer.
Conflito de Horário: Agendamento de duas ou mais consultas no mesmo horário para o
mesmo profissional.
Log de Auditoria: Registro de atividades em dados sensíveis para fins de segurança.
2. Personas e Público-Alvo
João Silva - Paciente, 35 anos: Quer agendar e gerenciar suas consultas de forma
rápida pelo celular.
Ana Souza - Atendente, 28 anos: Precisa de uma ferramenta para organizar as
agendas e evitar erros.
Dr. Carlos Mendes - Médico, 45 anos: Necessita de acesso rápido e seguro aos
prontuários.
Maria Oliveira - Gestora, 50 anos: Busca relatórios para monitorar o desempenho da
clínica.
3. Requisitos Funcionais
3.1. Diagrama de Casos de Uso
AgendaMed
Marcar Consulta Checar Disponibilidade
Check-in
Cliente
Cadastrar Cliente
Cancelar Consulta Enviar Avisos
Confirmar Consulta Verificar Conflito
Registrar Pagamento
Atendente
Consultar Agenda
Organizar Agenda Bloquear Horários
Medico
Login
Anotar no Prontuário Genenciar Acessos
Gestor
Cadastrar Médico
Notificador
3.2. Product Backlog Priorizado (MoSCoW)
ID HISTÓRIA DE USUÁRIO (RESUMIDA) PRIORIDADE
M1 Realizar cadastro e login com perfis distintos Must-Have
M2 Agendar, cancelar e remarcar consultas Must-Have
M3 Visualizar agenda e gerenciar conflitos Must-Have
M4 Acessar e editar prontuários com acesso restrito Must-Have
M5 Enviar notificações de confirmação e lembrete Must-Have
S1 Gerar relatórios administrativos básicos Should-Have
S2 Buscar médicos por especialidade e filtrar datas Should-Have
C1 Visualizar histórico de agendamentos na sua conta Could-Have
C2 Usar filtros avançados na agenda (sala, convênio) Could-Have
W1 Realizar pagamento online integrado Won't Have
W2 Realizar consulta por vídeo (telemedicina) Won't Have
W3 Integrar com agendas externas (Google/Outlook) Won't Have
4. Requisitos Não Funcionais
Usabilidade (USAB-01): O tempo de treinamento para um novo atendente deve ser inferior
a 40 minutos.
Desempenho (DESEM-01): A agenda diária deve carregar em menos de 3 segundos sob
carga normal.
Segurança (SEG-01): O acesso aos prontuários dos pacientes deve ser restrito apenas a
usuários com perfil de "Médico".
Disponibilidade (DISP-01): O sistema deve ter uma disponibilidade mínima de 99% em
horário comercial.
5. Recomendações para a Equipe de Desenvolvimento
Esta seção finaliza a fase de especificação e serve como um guia para a equipe de
desenvolvimento. Nossas sugestões visam alinhar o desenvolvimento com as prioridades
do produto e antecipar possíveis desafios.
5.1. Sugestão para o Mínimo Produto Viável (MVP)
Recomendamos que o primeiro ciclo de desenvolvimento (Sprint 1) se concentre em
entregar o fluxo operacional essencial para uma clínica. O objetivo é criar a versão mais
simples do AgendaMed que já entrega valor real para os usuários principais (atendentes e
médicos).
Definição do MVP: O MVP deve permitir que uma clínica cadastre seus profissionais,
gerencie a agenda, agende pacientes, realize confirmações/cancelamentos e mantenha
um prontuário eletrônico básico. Essencialmente, são todas as histórias classificadas como
"Must-Have" (M1 a M5) em nosso backlog.
Plano Sugerido para Sprints:
Sprint 1- O Coração da Agenda: O objetivo principal é "Permitir que uma atendente
gerencie a agenda de um médico de forma 100% digital e funcional".
Foco em: Cadastro e autenticação de usuários (M1).
Visualização da agenda por profissional e gestão de conflitos (M3).
Funcionalidades de agendamento, cancelamento e remarcação pela atendente (parte de M2).
Acesso restrito a um prontuário simples para o médico (M4).
Sprint 2 - Empoderando o Paciente e o Gestor: O foco seria expandir o sistema com
as funcionalidades restantes do MVP e as mais importantes do "Should-Have".
Foco em: Agendamento realizado pelo próprio paciente (restante de M2).
Implementação robusta do sistema de notificações automáticas (M5).
Desenvolvimento dos relatórios administrativos básicos para o gestor (S1).
Implementação da busca por médico/especialidade (S2).
Essa abordagem garante que, ao final do Sprint 1, já teremos um produto funcional que
resolve a maior dor da clínica, mesmo que funcionalidades complementares ainda não
estejam prontas.
5.2. Principais Desafios Técnicos Previstos
Acreditamos que os maiores desafios no desenvolvimento deste projeto serão:
Lógica de Conflitos e Concorrência: Garantir que dois usuários (ex: dois atendentes ou
um atendente e um paciente) não consigam agendar o mesmo horário
simultaneamente. Isso exige um tratamento cuidadoso de transações no banco de
dados para evitar condições de corrida (race conditions).
Controle de Acesso: Implementar um sistema de perfis de usuário (roles) que garanta
de forma segura que apenas médicos e assistentes possam visualizar e editar os
prontuários dos pacientes.
Desempenho da Agenda em Tempo Real: A visualização da agenda precisa ser
atualizada para múltiplos usuários (médicos, atendentes) em tempo real. A solução
deve ser performática para não sobrecarregar o sistema, especialmente em clínicas
com muitos profissionais.
5.3. Pontos de Atenção
• Usabilidade da Tela da Atendente: A interface de agendamento é o coração do sistema
e será usada intensivamente. Ela precisa ser extremamente ágil, clara e otimizada para
minimizar cliques. Cada segundo economizado nesta tela impacta diretamente a
produtividade da recepção.
Consistência dos Dados do Prontuário: É fundamental garantir que todas as operações
relacionadas a um prontuário (novas anotações, histórico de consultas) sejam atômicas e
consistentes. A perda ou corrupção de dados médicos é um risco inaceitável.
Confiança nas Notificações: O sistema de lembretes e confirmações por e-mail/SMS é
vital para reduzir a taxa de não comparecimento (no-show). A integração com o serviço de
envio deve ser robusta e possuir monitoramento para garantir que as mensagens estão
sendo entregues.
