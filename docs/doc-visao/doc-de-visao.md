# Documento de Visão: Plataforma Integrada One to One & PKZ

## 1. Introdução
* **Objetivo do documento:** Consolidar a visão geral, escopo, requisitos de alto nível, restrições e riscos do projeto de desenvolvimento da plataforma web integrada para a gestão das operações *One to One* e *Playmakers / PKZ*.
* **Público-alvo:** Gestores (Henrique, Pedro, Thiago, Dudu), corpo docente (professores), alunos (adultos/jovens) e pais ou responsáveis.
* **Escopo do sistema:** Plataforma web integrada com *Mobile* para clientes e professores, e interface desktop dedicada à gestão administrativa e inserção de testes complexos. O sistema abrange módulos de agendamento autônomo, controle de presença, gestão financeira automatizada, relatórios de evolução física e acompanhamento de mais de 16 testes físicos parametrizados.

## 2. Posicionamento
* **Oportunidade de mercado:** Atender à demanda por digitalização e eficiência no setor de treinamento personalizado e avaliação de alto rendimento infantil/juvenil, unificando duas frentes operacionais em uma única base tecnológica para otimizar o tempo de clientes e profissionais frente ao crescimento do negócio nas instalações físicas (Barra da Tijuca, Recreio, Vogue Square, Oasis).
* **Problema a ser resolvido:** Eliminação de processos manuais e controles descentralizados em planilhas do Excel e pastas do Google Drive. Redução do tempo gasto por profissionais buscando históricos operacionais e substituição de relatórios extensos em texto por entregas visuais e intuitivas para os clientes.
* **Proposta de solução:** Desenvolver uma plataforma digital integrada segmentada em duas frentes:
  * *One to One (Adultos):* Foco em conveniência, autonomia, preenchimento rápido de rotinas de musculação/personal, gestão de agenda, créditos e relatórios rápidos pós-treino.
  * *Playmakers / PKZ (Crianças/Adolescentes):* Foco em avaliação de alto rendimento e prestação de contas, controlando mais de 16 testes físicos parametrizados por idade e esporte, alertas de reteste e relatórios visuais gamificados para pais e responsáveis.

## 3. Descrição dos Stakeholders e Usuários
* **Quem são os envolvidos?** 
  * Gestores (Henrique, Pedro, Thiago, Dudu), Professores (Corpo Técnico), Alunos (adultos e jovens), Pais/Responsáveis, Equipe de Desenvolvimento (alunos do IBMEC), Professores IBMEC, faculdade IBMEC RJ, Sócios e investidores, Nutricionistas e Psicólogos.
* **Quais são suas necessidades e expectativas?**
  * *Gestores:* Monitorar faturamento, ocupação das aulas e receber alertas precoces sobre alunos com risco de cancelamento ou evasão.
  * *Professores:* Telas ágeis na quadra com conceito de "Zero Digitação" (uso de botões, sliders e preenchimento com uma mão) para registrar cargas, restrições e o treino executado, visualizando o histórico de dores da aula anterior de forma imediata.
  * *Alunos (One to One):* Central própria para gestão financeira, remarcação desburocratizada de aulas e check-in ágil via QR Code.
  * *Pais (PKZ):* Transparência financeira e leitura simplificada da evolução física dos filhos através de gráficos intuitivos e relatórios no estilo "Player Card".
  * *Equipe de alunos, professores e universidade:* Entregar um site de alta qualidade que atenda todos os requisitos do cliente e possua ferramentas para otimizar o trabalho da empresa.

## 4. Visão Geral do Produto
* **Principais funcionalidades:**
  * *Agenda Inteligente e Waitlist:* Agendamento autônomo com controle de vagas e fila de espera automática que notifica via WhatsApp o próximo da lista em caso de cancelamento.
  * *Notificações e Alertas:* Avisos automáticos de prazos vencidos para retestes físicos e alertas direcionados à coordenação para controle ativo de faltas.
  * *Módulo de Testes e Relatórios Visuais:* Inserção de métricas de mais de 16 testes físicos com geração de gráficos cronológicos e relatórios em formato de "Player Card" (estilo videogame) para engajamento dos jovens.
  * *Financeiro Automatizado:* Controle de mensalidades integrado por Webhooks (Mercado Pago/Stripe) com suporte a pagamento via PIX ou cartão (inclusive via WhatsApp) e bloqueio sutil de agendamentos em caso de inadimplência.
  * *Infográficos:* Controle da evolução, problemas físicos e acompanhamento costante por gráficos em tempo real.
* **Diferenciais em relação a soluções existentes:**
  * Unificação de duas operações distintas (público adulto e infanto-juvenil) em um ecossistema único.
  * Foco em usabilidade de campo (*Mobile First* para professores com preenchimento simplificado e sem digitação pesada).
  * Enfoque em engajamento visual de resultados para os clientes e responsáveis.
  * Transformação de processos manuais para atividades majoritariamente automatizadas

## 5. Requisitos de Alto Nível
* **Funcionais:**
  * Sistema de cadastro e gestão de perfis diferenciados para gestores, professores, alunos, pais, sócios, nutricionistas, psicólogos e investidores.
  * Módulo de agendamentos com controle de presença, lista de espera e integração com mensageria via WhatsApp.
  * Ferramenta de lançamento rápido de treinos e métricas de desempenho físico para o corpo docente.
  * Motor de relatórios evolutivos com exportação simplificada (ex: PDF para envio a médicos e nutricionistas).
  * Portal financeiro integrado com gateways de pagamento para automação de cobranças e liberação instantânea de acessos.
  * Sistemas infográficos e Player Cards para tornar as informações mais claras e objetivas.
* **Não funcionais:**
  * Arquitetura *Mobile First* responsiva e otimizada para uso em dispositivos móveis na quadra ou pelos clientes.
  * Isolamento estrito de dados e código entre os módulos *One to One* e *PKZ*.
  * Alta disponibilidade com hospedagem em nuvem (ex: AWS ou Google Cloud).
  * Usabilidade e Acessibilidade garantem que as telas sejam intuitivas, especialmente para os pais visualizarem os gráficos complexos (Player Card) e para os professores.

## 6. Restrições e Premissas
* **Restrições:**
  * Isolamento rígido de arquitetura de banco de dados e código para separar as informações das operações *One to One* e *PKZ*.
  * Prazos alinhados ao cronograma acadêmico, com entrega incremental prevista para a data da AP1 (ou limite até 15/11).
  * Alunos e responsáveis terão acesso apenas a contas de usuário simples, enquanto professores/gestores... terão acesso a modelos de administrador
* **Premissas:**
  * Utilização de ferramentas educacionais gratuitas e custo de desenvolvimento zerado pela equipe acadêmica do Ibmec.
  * Custos operacionais restritos à infraestrutura de nuvem e hospedagem (estimados entre R$ 40 e R$ 80/ano).
  * Dependência de integrações ativas com APIs de terceiros para disparo de mensagens (WhatsApp) e processamento de pagamentos (Gateways).
  * Acesso a internet e conhecimento das ferramentas disponibilizadas no site

## 7. Riscos e Dependências
* **Fatores críticos para o sucesso do projeto:**
  * *Risco de Evasão:* A necessidade de controle ativo de faltas pela coordenação para mitigar a evasão de alunos.
  * *Indisponibilidade de Rede/Sistema:* Risco de falhas na conexão de internet nas instalações físicas, exigindo a definição de um método manual temporário de contingência operacional na quadra.
  * *Resistência do Corpo Técnico:* Professores acostumados a métodos tradicionais (anotações em papel ou planilhas locais) podem resistir em adotar a interface mobile "Zero Digitação" na quadra.
  * *Conformidade e Segurança de Dados Sensíveis (LGPD):* O sistema lida com dados sensíveis de menores de idade (crianças e adolescentes do PKZ), histórico médico, restrições físicas, laudos e métricas de desempenho corporal. Vazamentos ou armazenamento inadequado dessas informações geram graves riscos jurídicos e reputacionais.
  * *Sobrecarga ou Concorrência no Agendamento (Concorrência de Banco de Dados):* Como o sistema possui uma Agenda Inteligente com Waitlist (fila de espera automática), existe o risco técnico de múltiplos usuários tentarem reservar a última vaga disponível para um mesmo horário exatamente ao mesmo tempo (condição de corrida / race condition). Se o banco de dados ou a regra de negócio falharem, o sistema pode acabar vendendo a mesma vaga para duas pessoas ou gerando conflitos na fila de espera.

* **Possíveis dependências ao longo do projeto:**
  * *Homologação de Contas de Pagamento e WhatsApp (APIs de Terceiros):* A automação financeira via Webhooks (Mercado Pago/Stripe) e os disparos de alertas e confirmações via WhatsApp dependem da aprovação de contas corporativas, chaves de API ativas e conformidade com as políticas de spam das plataformas de mensageria. Mudanças repentinas nos termos de uso ou quedas nas APIs podem bloquear cobranças e travar o fluxo de agendamento automático.
  * *Padronização dos Dados de Entrada (Testes Físicos):* Para que o sistema consiga gerar os relatórios gráficos/visuais gamificados ("Player Card") e comparar a evolução histórica de mais de 16 testes físicos, o sistema depende de que os professores insiram as métricas estritamente dentro do formato padrão esperado (ex: números decimais, unidades corretas de medida, sem campos em branco). Se o professor cadastrar dados corrompidos ou fora do padrão, o gráfico gerado para os pais pode quebrar ou exibir informações distorcidas.
