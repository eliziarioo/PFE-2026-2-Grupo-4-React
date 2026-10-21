# Demandas — PKZ / One to One

## Stack e arquitetura

| Prioridade | Demanda |
|---|---|
| Alta | Centralizar em um único sistema as informações atualmente espalhadas em Drive, Excel, aplicativo atual e WhatsApp. |
| Alta | Atender PKZ e One to One na mesma plataforma, com identidades, públicos e fluxos diferentes. |
| Alta | Permitir personalização de campos, duração dos treinos, relatórios, logotipos e fluxos. |
| Alta | Suportar múltiplas unidades, como Cosquare e Ase. |
| Alta | Implementar perfis e permissões para administração, coordenação, recepção, professores, alunos, responsáveis, fisioterapeutas e nutricionistas. |
| Alta | Integrar a plataforma com WhatsApp, serviços de pagamento e, futuramente, análise de vídeos. |
| Média | Disponibilizar aplicação responsiva ou mobile para professores, alunos e responsáveis. |
| Média | Garantir segurança e privacidade dos dados de crianças, adolescentes, responsáveis, avaliações físicas, informações de saúde e documentos. |
| Média | Manter histórico e auditoria de agendamentos, presenças, relatórios, avaliações e pagamentos. |

## Front-end e experiência do usuário

| Prioridade | Demanda |
|---|---|
| Alta | Fazer um redesign visual completo do aplicativo, com aparência mais profissional, coesa e alinhada à marca. |
| Alta | Criar dashboard operacional com alunos ativos, atividades do mês, testes realizados, relatórios pendentes e alunos atrasados. |
| Alta | Criar dashboard individual do aluno com cadastro, créditos, agenda, frequência, arquivos, avaliações e relatórios. |
| Alta | Substituir relatórios extensos por relatórios visuais com gráficos, indicadores e linguagem mais acessível. |
| Alta | Exibir gráficos de evolução das métricas ao longo do tempo. |
| Alta | Criar formulário simples para lançamento dos mais de 16 testes físicos. |
| Alta | Permitir abrir testes e relatórios com poucos cliques, sem navegação desnecessária. |
| Alta | Melhorar a agenda, exibindo horários, vagas, unidade, estúdio, professor, modalidade e status do agendamento. |
| Alta | Exibir, diretamente na agenda, o relatório e as observações do treino anterior do aluno. |
| Alta | Criar fluxo rápido para professores preencherem relatórios durante o expediente. |
| Média | Criar área do aluno e do responsável para consulta de treinos, relatórios, evolução, agenda, créditos, arquivos e pagamentos. |
| Média | Criar website institucional para PKZ e One to One, com serviços, portfólio, fotos, vídeos e canais de contato. |
| Média | Permitir cadastro de interessados pelo website e geração de login e senha. |
| Média | Permitir configurar logotipos, cores e identidade visual das duas marcas. |
| Média | Permitir que o aluno marque, cancele e remarque horários de forma autônoma. |
| Baixa/Futuro | Criar interface para carregar jogos, selecionar atletas e revisar eventos e indicadores de scout. |

## Dados e regras de negócio

| Prioridade | Demanda |
|---|---|
| Alta | Cadastrar alunos, responsáveis, contatos, idade, categoria, modalidade, unidade e plano. |
| Alta | Parametrizar avaliações conforme a idade e a modalidade do atleta. |
| Alta | Modelar os mais de 16 testes físicos, incluindo salto, velocidade, agilidade, reação, foco e demais métricas. |
| Alta | Armazenar o histórico de avaliações e permitir comparações entre períodos. |
| Alta | Registrar microciclo, mesociclo, cronograma mensal e treinos previstos. |
| Alta | Registrar materiais, tecnologias, capacidades, intensidade, desempenho, dores, desconfortos, conduta da próxima aula e observações. |
| Alta | Registrar o relatório do professor e a avaliação do aluno sobre o treino. |
| Alta | Controlar créditos semanais, com renovação periódica e sem acúmulo. |
| Alta | Registrar frequência, presença, aula realizada, professor responsável e status do relatório. |
| Alta | Controlar a data do próximo reteste e identificar avaliações vencidas ou próximas do vencimento. |
| Alta | Permitir anexar testes da fisioterapeuta e outros documentos externos. |
| Média | Controlar vagas e capacidade dos horários conforme a disponibilidade de professores e alunos. |
| Média | Cadastrar serviços como musculação, fisioterapia, nutrição e treinamento esportivo. |
| Média | Calcular evolução, tendências e faixas adequadas ou não adequadas. |
| Média | Armazenar mensalidades, vencimentos, formas de pagamento, situação da cobrança e histórico financeiro. |
| Baixa/Futuro | Estruturar jogos, atletas, categorias, eventos e indicadores de scout. |

## Back-end e automações

| Prioridade | Demanda |
|---|---|
| Alta | Gerar automaticamente o dashboard do aluno a partir dos dados inseridos. |
| Alta | Gerar automaticamente relatórios de treino e de teste a partir de formulários estruturados. |
| Alta | Criar alertas para avaliações vencidas ou próximas do vencimento. |
| Alta | Vincular automaticamente o agendamento ao relatório e às observações do treino anterior. |
| Alta | Liberar o relatório do professor somente após o registro da presença ou da aula realizada. |
| Alta | Renovar automaticamente os créditos semanais conforme as regras do plano. |
| Alta | Enviar lembretes e solicitações de confirmação de agendamento via WhatsApp. |
| Média | Automatizar avisos de vencimento e situação financeira por um canal institucional. |
| Média | Criar portal para consulta de vencimentos, pagamentos e formas de pagamento. |
| Média | Permitir alteração da forma de pagamento pelo aluno, quando autorizado. |
| Média | Integrar o website ao aplicativo para cadastro, login e agendamento. |
| Média | Utilizar IA para organizar métricas e textos dos relatórios, com validação contra erros de nomes, imagens e dados. |
| Média | Automatizar mensagens operacionais sem eliminar o contato humano com os clientes. |
| Baixa/Futuro | Criar scout assistido por vídeo, identificando eventos por atleta e gerando análises de desempenho. |

## Priorização das entregas

### MVP operacional

- Cadastro e perfis de acesso.
- Gestão de unidades e estúdios.
- Agenda com vagas e disponibilidade.
- Registro de presença.
- Controle de créditos.
- Relatório rápido de treino.
- Dashboard operacional.
- Histórico básico do aluno.

### MVP de avaliação

- Formulário dos testes físicos.
- Parametrização por idade e modalidade.
- Controle automático de retestes.
- Relatório visual.
- Gráficos de evolução.
- Upload de anexos.

### Experiência do cliente

- Área do aluno e do responsável.
- Consulta de relatórios e evolução.
- Feedback do aluno.
- Lembretes de agenda.
- Cancelamento e remarcação autônomos.

### Presença digital

- Website institucional.
- Páginas de PKZ e One to One.
- Portfólio de serviços.
- Cadastro e geração de acesso.
- Integração com WhatsApp.

### Financeiro

- Cobranças.
- Vencimentos.
- Histórico de pagamentos.
- Formas de pagamento.
- Alteração do meio de pagamento.

### Produto avançado

- IA validada para geração de relatórios.
- Scout de vídeos.
- Análise automática de eventos.
- Indicadores de desempenho por atleta.
