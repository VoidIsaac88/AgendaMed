AgendaMed — Entrega de Semana 5 (Documentação consolidada)
Documento preparado com base nas informações fornecidas (resumo do produto, visão,
público-alvo, personas, backlog MoSCoW, NFRs e tema). Estamos na quinta semana
do projeto.
1. Resumo do Projeto
O AgendaMed é uma plataforma web para gestão de clínicas e consultórios que
centraliza agendamentos, prontuários eletrônicos e relatórios administrativos. O sistema
facilita o trabalho de atendentes, médicos, pacientes e gestores, oferecendo uma
solução prática, eficiente e segura para o gerenciamento de consultas e dados médicos.
2. Visão
Simplificar a gestão de atendimentos médicos, garantindo agilidade, organização e
segurança das informações em clínicas e consultórios. O AgendaMed visa reduzir erros
de agendamento, otimizar o tempo dos profissionais e proporcionar uma experiência
melhor para os pacientes.
3. Público-Alvo e Personas
Público-Alvo:
- Atendentes de clı́nicas (organizar consultas).
- Médicos (acesso a prontuários e histó rico).
- Pacientes (agendar/remarcar/cancelar consultas).
- Gestores (relató rios administrativos).
Personas:
- João Silva — Paciente, 35 anos: quer agendar e cancelar consultas pelo celular com
rapidez.
- Ana Souza — Atendente, 28 anos: precisa evitar conϐlitos de horários e organizar a agenda
dos médicos.
- Carlos Mendes — Médico, 45 anos: acessa prontuários e mantém histó rico atualizado.
- Maria Oliveira — Gestora, 50 anos: monitora relató rios administrativos e controle da
clı́nica.
4. Escopo do Projeto
Incluído (escopo inicial):
- Cadastro e autenticação de usuá rios (pacientes, médicos, atendentes, gestores).
- Agendamento, cancelamento e remarcaçã o de consultas.
- Visualização de agenda por proϐissional (dia/semana).
- Controle de prontuá rios eletrô nicos com acesso restrito.
- Relató rios administrativos básicos.
- Notiϐicaçõ es de conϐirmaçã o e cancelamento.
Não incluído (fora do escopo inicial):
- Pagamento online integrado.
- Telemedicina (vı́deo).
- Integraçã o com Google Agenda / Outlook / convênios.
- Relató rios ϐinanceiros avançados.
5. Principais Funcionalidades (Resumo)
- Cadastro/gerenciamento de usuários e perϐis.
- Agenda por proϐissional (visualizaçã o e bloqueio de horá rios).
- Agendamento pelo paciente (sujeito a aprovação) e por recepçã o.
- Conϐirmação automá tica (e manual) e cancelamento.
- Prontuá rio eletrô nico simples com campos para anotaçõ es, alergias e histó rico de
consultas.
- Notiϐicaçõ es por e-mail/SMS (conϐirmaçã o, lembrete, cancelamento).
- Relató rios administrativos (quantidade de consultas, cancelamentos, ocupaçã o por
perı́odo).
6. Backlog Priorizado — MoSCoW (versão Semana 5)
Must Have (M) — imprescindível (MVP):
- M1: Cadastro e autenticaçã o de usuá rios (pacientes, médicos, atendentes, gestores).
- M2: Agendamento, cancelamento e remarcação de consultas.
- M3: Visualização da agenda por proϐissional (dia/semana) e gestão de conϐlitos de
horários.
- M4: Acesso restrito a prontuá rios (somente proϐissionais autorizados).
- M5: Notiϐicaçõ es (conϐirmaçã o/cancelamento/reminder).
Should Have (S) — importante, mas pode ficar para próximo ciclo:
- S1: Relató rios administrativos básicos (agenda por perı́odo, taxa de comparecimento).
- S2: Busca por médico, especialidade e ϐiltro por data.
Could Have (C) — desejável / nice-to-have:
- C1: Histó rico detalhado de agendamentos para pacientes (acesso na conta).
- C2: Filtros avançados na visualizaçã o da agenda (por sala, convênio, etc.).
Won’t Have (W) — fora do escopo agora:
- W1: Pagamento online integrado.
- W2: Telemedicina (vı́deo).
- W3: Integração com agendas externas (Google/Outlook).
7. Histórias de Usuário (exemplos)
1. Agendamento de Consulta (Paciente): Como paciente, quero agendar uma consulta em
horário disponı́vel para receber atendimento.
2. Cancelamento/Remarcaçã o (Paciente): Como paciente, quero cancelar ou remarcar
consultas para reorganizar meus compromissos.
3. Cadastro de Prontuário (Médico): Como médico, quero registrar informaçõ es do paciente
para manter o histó rico atualizado.
4. Controle de Agenda (Atendente): Como atendente, quero visualizar e organizar os
agendamentos para evitar conϐlitos.
5. Relató rios Administrativos (Gestor): Como gestor, quero gerar relató rios bá sicos para
acompanhar o desempenho da clı́nica.
8. Requisitos Não-Funcionais (NFRs)
Usabilidade:
- Treinamento do atendente ≤ 40 minutos.
- Interface responsiva para desktop e tablet; UX simples para telas de recepçã o.
Desempenho:
- Agenda (lista diá ria) deve carregar em ≤ 3 segundos sob carga normal.
- Suportar ao menos 100 usuários simultâneos no sistema (meta inicial).
Segurança:
- Autenticação por usuário/senha; perϐis e permissõ es (roles) distintos.
- Dados sensı́veis (prontuá rios) armazenados de forma criptografada em descanso;
comunicação TLS.
- Logs de auditoria para acesso e edição de prontuá rios (quem fez o quê e quando).
Confiabilidade / Disponibilidade:
- Disponibilidade mı́nima de 99% no horá rio comercial.
- Backups automáticos diá rios e plano de restore documentado.
Escalabilidade:
- Arquitetura preparada para expansã o (API REST/GraphQL; separaçã o de camadas)
9. Diagrama de Casos de Uso (placeholder)

<img width="523" height="723" alt="Captura de tela 2025-09-03 194626" src="https://github.com/user-attachments/assets/26db521c-ddd4-44a0-92f1-ca2fbeb49440" />


10. Recomendação para MVP e Sprints (sugerido)
Definição de MVP (mínimo produto viável): MVP = todas as histórias Must-Have (M1–
M5) entregues de forma que uma clínica possa operar agendamentos,
confirmar/cancelar e manter prontuários básicos com notificações.
Sugestão de divisão em 2 sprints curtos (ex.: 2 ou 3 semanas cada):
- Sprint 1: Cadastro/autenticação (M1); Visualização de agenda e ló gica de bloqueio de
horários (M3); Agendamento bá sico pelo atendente (parte de M2).
- Sprint 2: Agendamento pelo paciente (M2), conϐirmaçõ es e cancelamentos (M5); Controle
de acesso a prontuá rios e interface de médico para adicionar anotaçõ es (M4); Ajustes ϐinos
nos NFRs e relató rios básicos (S1 se houver tempo).
Critérios de aceitação do MVP:
- Usuá rio atendente consegue registrar/agendar/cancelar sem erros.
- Médico consegue visualizar e editar prontuário com registro de auditoria.
- Notiϐicaçõ es enviadas ao paciente em eventos (conϐirmaçã o/cancelamento).


-link- https://trello.com/b/7HXFcI3R/meu-quadro-do-trello
