# Ideias para fazer o 5w2h

**How-much:** Custos relacionados a armazenagem de dados(seridores de banco de dados),valores estarão presos ao número de dados enviados/a serem armazenados. Em relação a entrega do projeto, pode-se dizer que terá uma duração de alguns meses ate a entrega definitiva.

**How:** O sistema sera feito em módulos.De primeira mão será entregue as partes que resolverão problemas diarios, como agendas e confirmação de presenças nas aulas,podendo desmarca-las. Depois, encaixamos o módulo de testes físicos e um bom layout de facil entendimento para os pais,alem de ter um bom entendimento para quem faz somente parte da "area de musculação", ambos precisam ter um bom entendimento visual. O sistema vai morar na nuvem, acessível por qualquer celular ou computador.Áreas relacionadas a metodos de pagamentos seriam de forma onde poderiam se pagar diretamente pelo whatsapp(caso prefira) ou diretamente no site via pix e cartões.

**What:** O desenvolvimento de uma plataforma web integrada de gestão esportiva, com banco de dados e área administrativa centralizados, mas ramificada em duas partes operacionais distintas:

            Módulo One to One (Estúdio de Personal & Musculação): Focado no público adulto com rotinas de treinamento físico. O sistema prioriza fluxos de preenchimento rápido para o professor no dia a dia (registrando intensidade, foco muscular, dores relatadas e conduta da próxima aula) e oferece uma interface onde o próprio aluno tem autonomia total para gerenciar sua agenda e créditos.



            Módulo PKZ (Desenvolvimento de Jovens Atletas): Focado em alta performance esportiva e prestação de contas para terceiros (pais e responsáveis). O sistema exige uma rotina complexa de avaliações (com mais de 16 testes físicos realizados por idade e esporte), alertas de prazos para retestes, geração de dashboards visuais de evolução histórica e infraestrutura de dados preparada para receber ferramentas de analises sobre os dados de partidas etc.

**When:** Não consegui ter um bom entendimento do que seria,visto que ja coloquei prazo no primeiro tópico, como recomendado anteriomente pelo superior(professor).

**Where:** Deve falar sobre aonde sera hospedado e implementado.
    
            Ambiente Físico (Operação do Negócio): O sistema será utilizado nas instalações físicas da empresa (Estúdios One to One e centros de treinamento PKZ)


            Ambiente Digital (Infraestrutura do Sistema): O software será hospedado na nuvem (Cloud Computing, como AWS ou Google Cloud), garantindo disponibilidade 24/7. O acesso ocorrerá de forma distribuída por meio de navegadores web (Web App), sendo majoritariamente mobile (celulares) para professores, alunos e pais, e desktop para a gestão administrativa e inserção de testes complexos.

**Who:** Deve ser informado quem fará e quem ira usar.

            Execução: Equipe de engenharia de software (arquitetura, front-end, back-end)

            "Usuários": Gestores (Henrique, Pedro, Dudu), professores (alimentação de dados em tempo real), alunos e pais (consumo de dashboards vitais e agendamento autônomo).

**Why:** automatizar processos manuais repetitivos (relatórios de testes físicos, cobranças) e estruturar a base de dados em um padrão limpo.

---
# Ideias sobre o AHT

O AHT na pratica seria sobre otimização de tempo.
      
        Módulo One to One (Estúdio de Personal & Musculação):Antes O professor perdia tempo buscando pastas no Drive e digitando relatórios longos pós-treino Na aula seguinte, 
        precisava caçar o histórico para saber o que foi feito. Apos o uso do sistema ja completo, seria possivel acessar rapidamente historicos com tags etc. O histórico do treino anterior aparece automaticamente na agenda do professor, zerando o tempo de busca.



       Módulo PKZ (Desenvolvimento de Jovens Atletas):Antes a coordenação controlava de forma manual os 16 testes físicos e os prazos de reteste em planilhas Excel. Os relatórios extensos em texto cansavam os pais que muitas vezes deveriam ler diversas paginas de relatórios. Apos o uso do sistema ja completo, O painel automatiza os alertas de retestes próximos e gera relatórios visuais baseados em métricas parametrizadas por idade e esporte. Isso entrega clareza imediata aos responsáveis e elimina o trabalho manual. 

---
# Doc de visao 

**Introdução:** O projeto visa criar um sistema web unificado para gerenciar as rotinas da PKZ (jovens atletas) e One to One (adultos). O objetivo é digitalizar processos manuais, reduzindo o tempo (AHT) e integrando agendamentos, pagamentos e avaliações físicas em uma única plataforma automatizada.

**Posicionamwnto:**

One to One (Adultos): Foco em conveniência e autonomia. O adulto gerencia sua própria agenda e pagamentos de forma rápida, sem precisar falar com a recepção.

PKZ (Jovens Atletas): Foco em performance. O sistema traduz os 16 testes físicos complexos em relatórios visuais claros, provando o valor do serviço aos pais.

**Descrição de Stackrolder:**

Gestores (Henrique, Pedro, Dudu): Monitoram o faturamento, ocupação das aulas e recebem alertas sobre alunos em risco de cancelar o plano (churn).

Professores: Operam o aplicativo na quadra. Precisam de telas ágeis para registrar o treino sem perder tempo digitando.

Alunos (One to One): Querem marcar aulas, fazer check-in por QR Code e pagar a mensalidade sem burocracia.

Pais (PKZ): São os pagantes do público jovem. Precisam de transparência financeira e gráficos fáceis de entender sobre a evolução física dos filhos.

**Visão geral do produto:** Uma aplicação que elimina atritos do dia a dia. Para o professor, a agenda inteligente já mostra se o aluno teve alguma dor na aula passada. Para a recepção, a fila de espera roda sozinha e as cobranças são automáticas. Para o cliente, o portal web funciona como uma central fácil para ver boletos, agendar treinos e acompanhar resultados.

**Requisitos de alto nível:** 

Front-end "Zero Digitação": Formulários baseados em cliques, sliders e botões rápidos. O professor fecha o relatório do treino usando apenas uma mão.

Relatórios Visuais (Sérgio Franco e Player Card): Para os pais, gráficos de evolução limpos. Para os jovens, as notas viram um "Player Card" (como atributos de jogador de videogame), gerando engajamento visual com as próprias métricas.

Agenda Inteligente e Waitlist: Fila de espera automática (se um aluno cancela, o sistema puxa o próximo e avisa por WhatsApp) e avisos automáticos de reteste físico vencido.

Financeiro Automatizado (Webhooks): Integração com Mercado Pago/Stripe. Se o pagamento atrasa, o agendamento é sutilmente bloqueado com um botão para pagar. Ao pagar, o sistema reconhece e libera a agenda na hora.

**Restrições e premissas:**

Premissa de Usabilidade: O sistema precisa ter portabilidade para desktops e disposivos móveis.

Restrição de Arquitetura e Dados: O código e o banco de dados devem isolar as informações da PKZ e da One to One.

**Riscos e dependências:**

Risco (Evasão de Alunos):Caso o aluno tenha muitas faltas, o professor e a coordenação podem e devem entrar em contato com o próprio para esclarecer duvidas ou insatisfações.

Dependência (APIs Externas): O disparo de lembretes e a aprovação instantânea de pagamentos dependem do WhatsApp e do Gateway de pagamento. Se caírem, a operação precisará usar controles manuais temporários.Além de que, caso o site caia, deverão ser usadas metodos manuáis.

**Prototipo da interface:**Divido em sessões,seguindo o modelo mostrado para o grupo, área sobre a empresa, avaliações e duvidas frequentes.
