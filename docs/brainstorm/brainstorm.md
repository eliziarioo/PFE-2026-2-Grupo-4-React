# Brainstorm Consolidado - One to One & PKZ

## 1. Visão Geral do Produto e Posicionamento
O sistema será uma plataforma web integrada (com foco no uso mobile *Mobile First* pelos clientes e professores, e uso desktop para gestão/inserção de testes complexos) que gerencia duas operações distintas em uma única base:
* **One to One (Adultos):** Foco em conveniência, autonomia e preenchimento rápido (rotinas de musculação/personal). O adulto gerencia sua agenda, créditos e visualiza relatórios rápidos pós-treino.

* **Playmakers / PKZ (Crianças/Adolescentes):** Foco em avaliação de alto rendimento e prestação de contas. Envolve o controle de mais de 16 testes físicos parametrizados por idade e esporte, alertas de reteste e geração de relatórios complexos voltados para os pais/responsáveis.

**Objetivo Central:** Automatizar processos, zerar controles em planilhas/Drive, otimizar o tempo dos profissionais e entregar valor visual aos clientes (pais e alunos).

---

## 2. Ideias para o 5W2H

* **What (O quê):** 
  * Plataforma web integrada com área administrativa central e seções ramificadas para PKZ e One to One. 
  * Sistema entregue em módulos (primeiro agenda/presença, depois testes físicos e layouts visuais).
  * Site que atenda o máximo de demandas propostas pelo cliente para otimização de tempo.

* **Why (Por quê):** 
  * Automatizar rotinas operacionais manuais (relatórios e cobranças) e estruturar dados em um padrão limpo.
  * Ajudar a empresa a otimizar o tempo dos clientes e profissionais frente ao seu crescimento.
  * Sintomas visíveis atuais: perda de tempo buscando histórico em pastas do Drive, relatórios extensos em texto que cansam os pais, controle de +16 testes em planilhas Excel.
* **Where (Onde):** 
  * Operação nas instalações físicas (Barra da Tijuca, Recreio, Vogue Square, Oasis).
  * Infraestrutura Digital: Hospedado na nuvem (ex: AWS, Google Cloud) rodando via Web/App. Foco de entrada via mobile (maior volume de novos clientes), mas interface para desktop para gestão.
* **When (Quando):** 
  * Entregas incrementais com prazo final previsto para a data da AP1 (ou até 15/11).
* **Who (Quem):** 
  * **Desenvolvedores:** Alunos (Scrum Team) do Ibmec com apoio do Professor (PO).
  * **Usuários:** Gestores (Henrique, Pedro, Thiago, Dudu), Professores, Alunos (adultos/jovens) e Pais/Responsáveis.
* **How (Como):** 
  * Uso de metodologias ágeis (Scrum), ferramentas acessíveis/planos acadêmicos, arquitetura web e apoio de IA para otimização de desenvolvimento e análise de dados.
* **How Much (Quanto):** 
  * Custo de desenvolvimento zerado pela equipe acadêmica, usando ferramentas educacionais gratuitas.
  * Custos atrelados à hospedagem (estimativa de R$40 a R$80/ano) e armazenamento no banco de dados na nuvem.

---

## 3. Ideias para o Documento de Visão

**Stakeholders e Perfis de Usuário:**
* **Gestores:** Monitoram faturamento, ocupação das aulas e recebem alertas sobre alunos com risco de cancelamento.
* **Professores (Corpo Técnico):** Operam o sistema na quadra. Precisam de telas ágeis ("Zero Digitação") com botões, sliders e preenchimento rápido (com apenas uma mão) para registrar cargas, restrições e o treino executado. A agenda já deve mostrar o histórico de dores da aula passada.
* **Alunos (Adultos - One to One):** Central do cliente para gestão financeira, remarcação de aulas sem burocracia e check-in por QR Code.
* **Pais (PKZ):** Precisam de transparência financeira e leitura simplificada da evolução dos filhos (gráficos e relatórios).

**Requisitos Funcionais e Capacidades (Alto Nível):**
* **Agenda Inteligente e Waitlist:** Agendamento autônomo com controle de vagas. Fila de espera automática: se alguém cancela, puxa o próximo e avisa por WhatsApp.
* **Notificações e Alertas:** Alertas automáticos de prazos vencidos para retestes físicos.
* **Testes e Relatórios Visuais:** Inserção de métricas de +16 testes físicos. Geração de relatórios que lembram resultados do "Sérgio Franco" ou um "Player Card" (estilo videogame, para engajar os jovens com as próprias notas).
* **Financeiro Automatizado:** Módulo de controle de mensalidade com Webhooks (ex: Mercado Pago/Stripe). Pagamento via PIX/Cartão até pelo WhatsApp. Se atrasar, o agendamento é sutilmente bloqueado; se pagar, libera na hora.

**Restrições, Premissas e Riscos:**
* **Restrição de Arquitetura:** O código/banco de dados deve isolar estritamente as informações da One to One e do PKZ.
* **Dependências:** O disparo de mensagens e aprovação de pagamentos dependem de APIs externas (WhatsApp, Gateway).
* **Risco e Contingência:** Risco de evasão de alunos requer controle de faltas para o contato ativo da coordenação. Se o sistema/internet cair, a operação deve ter método manual temporário de contingência.
* **Regras do Documento (Estrutura):** O documento deve ser muito bem segmentado, numerado e estruturado para rápida leitura (Propósito, Posicionamento, Stakeholders, Visão Geral, Requisitos, Restrições e Riscos).

---

## 4. Ideias para o AHT (Análise Hierárquica de Tarefas)

**Foco Principal da AHT:** Otimização de tempo e eliminação de burocracia. A AHT deve focar na eficiência: número de passos, caminhos alternativos e em que ponto o usuário pode "travar" na interface.

**Fluxo Sugerido 1 - Consulta do Gráfico Evolutivo (Pelos Pais/Adultos):**
* **Objetivo:** Permitir visualizar a evolução física de forma simples, sem precisar interpretar dados brutos.
* **Passos:** 1. Acessa o portal do aluno. 2. Abre a aba de avaliações. 3. Clica no card da foto do aluno. 4. Navega até "Relatórios de teste físico". 5. Seleciona o treino/valência desejada (ex: Velocidade). 6. O sistema exibe o gráfico cronológico (barra/linha) cruzando dados do mês atual com os anteriores. 7. Opção final de Salvar ou Compartilhar (PDF) para envio a médicos e nutricionistas.

**Fluxo Sugerido 2 - Registro de Treino (Pelo Professor):**
* **Objetivo:** Eliminar o tempo de busca no histórico e a digitação de relatórios.
* **Passos:** 1. Professor acessa a agenda do dia no mobile. 2. O histórico do treino anterior e "dores relatadas" já aparecem automaticamente no card do aluno. 3. O professor executa o treino. 4. Preenche o checklist pós-treino usando formulários rápidos (sliders de intensidade, cliques em valências musculares, seleção de materiais) sem digitação pesada.

**Fluxos Adicionais Listados:**
* Gestão de Alunos: Cadastrar, atualizar créditos e anexar laudos.
* Agendamento e Presença: Aluno agenda; recebe lembrete no WhatsApp; professor confirma presença e libera o registro.
* Testes e Financeiro: Inserir métricas dos testes; controle e alteração de pagamentos.

---

## 5. Ideias para o Protótipo de Interface (Wireframes & UX)

**Layout e UX (Visão Geral):**
* Visual limpo ("clean"), focando em imagens, vídeos de fundo e pequenos textos impactantes.
* Layout responsivo (*Mobile First*), garantindo que o acesso pelo celular (maior volume de acessos) seja impecável.
* Foco em Funil de Conversão: A "Rota do Visitante até o Contato" deve ser clara. Ao rolar a página lendo as informações, deve haver um botão nítido chamando para o suporte.

**Estrutura da Página Principal (Landing Page):**
* **1. Hero / Apresentação (Primeira Dobra):** Fundo com imagem/vídeo do centro de treinamento. Frase de impacto unindo o conceito das duas marcas. Botões de Ação Rápida (CTA) visíveis, possivelmente inspirados em landing pages limpas (como Nubank), com link direto para agendamentos/planos.
* **2. Seção de Separação de Marcas (PKZ x One to One):** Dois "cards" ou blocos lado a lado evidenciando as características de cada negócio. A ideia é que o cliente clique na marca desejada e seja redirecionado para informações "nichadas" e vitrines de modalidades.
* **3. Prova Social e Resultados:** Seção para Mural de Resultados, Depoimentos e gráficos de dados ("Prova em Números", mostrando alunos ativos, evolução, anos de experiência).
* **4. Corpo Docente:** Apresentação dos profissionais que trabalham na empresa, mostrando foto, formação e qualidades (especialidades) para gerar confiança prévia no cliente.
* **5. FAQ e Contato / Suporte:** Dúvidas frequentes respondidas. Formulário inteligente de contato e botão flutuante/rápido para o WhatsApp, grande o suficiente para não passar despercebido.

**Ideias de Estratégia de Venda / Engajamento Visual na Interface:**
* **Redes Sociais:** Seção conectando o feed do Instagram no site para aproveitar o tráfego orgânico.