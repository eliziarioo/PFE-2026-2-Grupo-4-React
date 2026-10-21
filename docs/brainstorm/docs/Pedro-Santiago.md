# Brainstorming do Projeto: One to One & PKZ

## 1. Visão Geral do Projeto
Desenvolvimento de uma plataforma integrada (Web e App) para unificar e automatizar a gestão de dois centros de treinamento esportivo: **One to One** (treinamento de performance para adultos/não atletas) e **Playmakers - PKZ** (desenvolvimento e avaliação física de alto rendimento para crianças e adolescentes). O sistema visa centralizar cadastros, agendamentos, relatórios de treino, testes físicos parametrizados por idade/modalidade, dashboards evolutivos e controle financeiro, otimizando o tempo dos professores sem perder o vínculo de proximidade com os clientes e responsáveis.

---

## 2. 5W2H

* **What (O quê):** Sistema integrado (Web e App) para gestão de treinos, agendamentos, testes físicos parametrizados, relatórios visuais/dashboards e controle financeiro de duas marcas esportivas (One to One e PKZ).
* **Who (Quem):** Desenvolvedores de software (Scrum Team) do Ibmec RJ, proprietários (Henrique, Thiago), coordenadores (Pedro), professores/avaliadores, alunos e responsáveis/pais.
* **Where (Onde):** Unidades físicas no Rio de Janeiro (Barra da Tijuca, Recreio, Vogue Square, Oasis) e ambiente digital acessível via web e aplicativo mobile.
* **When (Quando):** Cronograma estruturado em sprints ágeis, com entregas incrementais divididas entre módulos essenciais e avançados. Prazo previsto para entrega: 15/11.
* **Why (Por quê):** Eliminar processos manuais (planilhas e Google Drive), automatizar a geração de relatórios complexos em formatos visuais intuitivos para os pais, otimizar o tempo operacional da equipe e melhorar a retenção dos clientes.
* **How (Como):** Utilizando metodologias ágeis (Scrum), arquitetura web moderna, banco de dados relacional, integração com IA para tratamento de métricas e automação de notificações via WhatsApp/email.
* **How Much (Quanto):** Custos baseados em infraestrutura de hospedagem em nuvem, ferramentas de desenvolvimento, APIs de IA e horas de desenvolvimento da equipe técnica.

---

## 3. AHT (Análise Hierárquica de Tarefas)

* **0. Gestão Integrada de Treinamento Esportivo**
    * **1. Gerenciar Alunos e Cadastros**
        * 1.1 Cadastrar novo aluno (vínculo com One to One ou PKZ)
        * 1.2 Atualizar créditos semanais de atendimento
        * 1.3 Anexar documentos externos (ex: laudos de fisioterapia)
    * **2. Executar Agendamentos e Frequência**
        * 2.1 Aluno agendar ou remarcar horário autonomamente
        * 2.2 Receber lembrete automatizado via WhatsApp
        * 2.3 Professor confirmar presença e liberar o registro do treino
    * **3. Realizar Avaliações e Testes Físicos**
        * 3.1 Inserir métricas dos +16 testes físicos parametrizados por idade/modalidade
        * 3.2 Gerar automaticamente relatório/dashboard evolutivo comparativo
    * **4. Emitir Relatórios de Treino**
        * 4.1 Professor preencher checklist pós-treino (materiais, valências, intensidade)
        * 4.2 Aluno/Responsável visualizar histórico e evolução de treinos
    * **5. Gestão Financeira e Administrativa**
        * 5.1 Controlar mensalidades, vencimentos e status de pagamento
        * 5.2 Permitir alteração de forma de pagamento pelo próprio usuário

---

## 4. Documento de Visão

### Escopo do Sistema
O sistema será uma plataforma unificada composta por um **Website institucional/portfólio** (com páginas dedicadas à One to One e ao PKZ, galeria de fotos/vídeos e captação de leads) e uma **Aplicação Web/Mobile** funcional para gestão interna e portal do aluno/responsável.

### Requisitos Funcionais (RF)
* **RF01:** Cadastro diferenciado de usuários segmentado por perfil (Admin, Professor, Aluno, Responsável).
* **RF02:** Módulo de agendamento autônomo com controle de vagas por horário e professor.
* **RF03:** Inserção e armazenamento de métricas dos testes físicos com parametrização automática por faixa etária e modalidade.
* **RF04:** Geração automática de dashboards visuais e gráficos evolutivos com base nas reavaliações periódicas.
* **RF05:** Registro de fichas de treino pós-aula pelos professores (vinculado obrigatoriamente à chamada realizada).
* **RF06:** Módulo de pagamentos e controle de mensalidades com opção de alteração de dados de cobrança.

### Requisitos Não Funcionais (RNF)
* **RNF01:** Interface intuitiva e de fácil navegação para colaboradores com pouca afinidade tecnológica.
* **RNF02:** Resposta rápida no carregamento de agendamentos e relatórios (otimização de tempo entre turnos de atendimento).
* **RNF03:** Segurança e criptografia de dados sensíveis de menores de idade e informações financeiras.

---

## 5. Protótipo da Interface da Página Web (Wireframe Textual) - Home Hub

```text
+-----------------------------------------------------------------------+
|  [LOGO]    Início    Sobre Nós    FAQ & Suporte    Professores  [Entrar]|
+-----------------------------------------------------------------------+

=========================================================================
SECTION 1: HERO / APRESENTAÇÃO
[ IMAGEM / VÍDEO DE FUNDO: Centro de Treinamento Esportivo ]
+-----------------------------------------------------------------------+
|                                                                       |
|                     EXCELÊNCIA EM MOVIMENTO E PERFORMANCE             |
|          Unindo o treinamento adulto (One to One) e o desenvolvimento |
|             de alto rendimento infantojuvenil (PKZ) em um só lugar.   |
|                                                                       |
|                     [ Agende sua Aula ]  [ Conheça os Planos ]        |
|                                                                       |
+-----------------------------------------------------------------------+

=========================================================================
SECTION 2: NOSSAS MARCAS (Dois Cards Lado a Lado)
+-----------------------------------+  +--------------------------------+
| [ Imagem: One to One ]            |  | [ Imagem: PKZ Playmakers ]     |
| ## One to One                     |  | ## Playmakers - PKZ            |
| Foco: Treinamento de performance  |  | Foco: Avaliação física e       |
| para adultos e não atletas.       |  | alto rendimento para crianças  |
| Evolua no esporte que você ama,   |  | e adolescentes com testes      |
| seja futevôlei, corrida ou força. |  | parametrizados por idade.      |
|                                   |  |                                |
| [ Acessar One to One ]            |  | [ Acessar PKZ ]                |
+-----------------------------------+  +--------------------------------+

=========================================================================
SECTION 3: FAQ & SUPORTE
+-----------------------------------------------------------------------+
| ## Dúvidas Frequentes (FAQ)                                           |
|                                                                       |
| > [ + ] Como funcionam os créditos semanais de treino?               |
| > [ + ] Os testes físicos do PKZ são reavaliados com que frequência?   |
| > [ + ] Como os pais acompanham a evolução dos relatórios?            |
| > [ + ] Posso alterar minha forma de pagamento direto pelo app?       |
|                                                                       |
| --------------------------------------------------------------------- |
| ## Precisa de Ajuda?                                                  |
| [ Envie sua mensagem para o Suporte via WhatsApp ou Chat ]            |
| [ Nome: ____________ ] [ E-mail/Tel: ____________ ] [ Enviar Dúvida ] |
+-----------------------------------------------------------------------+

=========================================================================
SECTION 4: CORPO DOCENTE (Cards de Professores)
+-------------------+  +-------------------+  +-------------------+
| [ Foto Prof. 1 ]  |  | [ Foto Prof. 2 ]  |  | [ Foto Prof. 3 ]  |
| ### Henrique      |  | ### Pedro         |  | ### Eduardo       |
| Esp: Alto Rend.   |  | Esp: Coordenação  |  | Esp: Hipertrofia  |
| Form: Ed. Física  |  | Form: Fisiologia  |  | Form: Treinamento |
+-------------------+  +-------------------+  +-------------------+

+-----------------------------------------------------------------------+
| Rodapé: Contato | Unidades (Barra, Recreio, Vogue Square, Oasis)       |
+-----------------------------------------------------------------------+