---
title: Consumo de crédito de IA
description: Saiba mais sobre o consumo de créditos de IA em aplicativos do CX Enterprise.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
last-update: '2026-05-21T00:00:00.000Z'
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
source-git-commit: 34a3227d726a6249a6dedea420828b84ad1547a7
workflow-type: tm+mt
source-wordcount: 966
ht-degree: 4%

---

# Consumo de créditos de IA

Saiba mais sobre o consumo de créditos de IA em aplicativos do CX Enterprise.

## Créditos de IA

Um _crédito de IA_ é uma métrica baseada no uso que quantifica a execução de ações ou trabalhos.

## Serviços elegíveis que consomem créditos de IA

* [CX Enterprise Coworker](#cx-enterprise-coworker-credit-rate)
* [Agentes da AEP](#aep-agents-credit-rate)

### Taxa de crédito do CX Enterprise Co-worker

Por um período introdutório limitado, as entradas de Colaborador consomem créditos de IA a uma taxa de 25 créditos de IA por Entrada. Essa taxa está disponível por um período limitado e está sujeita a alterações.

### Taxa de crédito de Agentes AEP

Um _trabalho de agente_ é uma série de tarefas e ações que um agente do AEP executa para atingir um resultado específico, conforme determinado pelas entradas do cliente.

Usando prompts de linguagem natural por meio do Assistente de IA, você pode solicitar que os agentes realizem tarefas específicas. Com base nessas entradas, a Agent Orchestrator coordena os agentes apropriados para executar cada etapa nos aplicativos CX Enterprise relevantes.

O uso do crédito de IA pode variar dependendo da complexidade e do valor do trabalho executado:

* Tarefas simples (geralmente de etapa única) consomem menos créditos
* Tarefas complexas (geralmente de várias etapas) consomem mais créditos
* Tarefas que envolvem raciocínio avançado, validação, coordenação de vários agentes ou integração consomem mais créditos

Para ver quais agentes da AEP e trabalhos de agentes estão disponíveis nos aplicativos licenciados do CX Enterprise, consulte o [Catálogo de recursos do CX Enterprise Agentic AI](https://agentic-capability-explorer.entapp.adproto.com/).

#### Taxas de crédito de trabalho de agente estimadas

| Agente | Trabalho | Aplicativos compatíveis | Créditos de IA estimados | Exemplos de prompts |
| ------ | ----- | ------------------------ | ----------------------- | ----------------- |
| Audience Agent | Público-alvo/ideação da conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 50 | <ul><li><em>Mostre-me campos para compradores ricos</em></li><li><em>Localizar todos os campos relacionados às preferências do cliente</em></li></ul> |
| Audience Agent | Gerenciamento de público-alvo/conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li><em>Tenho públicos-alvo duplicados?</em></li><li><em>Mostre-me os cinco maiores públicos-alvo.</em></li><li><em>Mostre-me públicos que não estão ativados para nenhum destino</em></li><li><em>Listar todos os públicos-alvo usados em jornadas ao vivo</em></li></ul> |
| Audience Agent | Análise de público-alvo/conta | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li><em>Quais públicos-alvo aumentaram de tamanho em mais de 20% na última semana?</em></li><li><em>Quanto o público-alvo &quot;Platina Fiel&quot; mudou em comparação ao valor de 30 dias atrás?</em></li><li><em>Qual é o meu público que cresce mais rápido?</em></li></ul> |
| Audience Agent | Ideação de grupo de compra | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li><em>Quais contas estão mostrando a intenção para esses produtos?</em></li><li><em>Mostre-me as pessoas principais por intenção de produto para XYZ.</em></li><li><em>Quais grupos de compras têm mais de 5 membros?</em></li></ul> |
| Data Insights Agent | Análise e visualização de dados | <ul><li>Customer Journey Analytics (edições B2C e B2B)</li></ul> | 25 | <ul><li><em>Pedidos de tendência em julho</em></li><li><em>Mostrar receita por região.</em></li><li><em>Mostrar pedidos por gênero, de março a junho.</em></li><li><em>Quais foram minhas 10 principais SKUs por lucro em junho</em></li><li><em>Proporção de compras por mês do ano</em></li><li><em>Cota de receita por categoria de produto</em></li></ul> |
| Journey Agent | Jornada ideação | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li><em>Crie uma jornada para contas de espaço em branco com intenção para minha solução, focalizando pessoas envolvidas com conteúdo no site</em></li></ul> |
| Journey Agent | Análise de jornada | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> | 50 | <ul><li><em>Quero analisar o fallout por nó para a Campanha do jornada de 4 de julho.</em></li><li><em>Há conflitos de agendamento para a jornada X</em></li><li><em>Mostrar conflitos de sobreposição de público alvo para a jornada X</em></li></ul> |
| Journey Agent | Gerenciamento de jornadas | <ul><li>Adobe Journey Optimizer (edições B2B e B2C)</li></ul> | 25 | <ul><li><em>Quantas jornadas ativas eu tenho?</em></li><li><em>Listar todas as jornadas usando o público X.</em></li><li><em>Listar todas as jornadas atualmente no modo de teste</em></li></ul> |
| Agente de suporte ao produto | Solução de problemas com base no conhecimento | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (edições B2C e B2B)</li><li>Customer Journey Analytics (edições B2C e B2B)</li></ul> | 0 | <ul><li><em>Por que minha contagem de perfis é diferente no Painel de Uso da Licença e na home page do Experience Platform?</em></li><li><em>Quais são os motivos para uma jornada não ser acionada?</em></li><li><em>Como o Adobe Experience Platform cria experiências em tempo real?</em></li><li><em>Como você configura e usa alertas no Adobe Experience Platform?</em></li><li><em>Qual é o limite de riqueza média de perfis na Ativação do Adobe Experience Platform?</em></li></ul> |
| Agente de suporte ao produto | Criação e rastreamento de casos de suporte | <ul><li>Real-Time CDP (edições B2B, B2C e B2P)</li><li>Adobe Journey Optimizer (edições B2C e B2B)</li><li>Customer Journey Analytics (edições B2C e B2B)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li><em>Criar um novo tíquete de suporte para meu trabalho de segmentação com falha</em></li><li><em>Qual é o status do tíquete E-001772068?</em></li></ul> |
| Agente do Supervisor de Conteúdo | Descoberta de conteúdo | <ul><li>Adobe Experience Manager</li></ul> | 5 | <ul><li><em>Mostrar fragmentos de conteúdo para criar a campanha de oferta WKND.</em></li><li><em>Localizar imagens PNG da embalagem do produto.</em></li><li><em>Mostrar imagens com marcas de formatação do Office na pasta WKND.</em></li><li><em>Há svgs na pasta WKND?</em></li><li><em>Mostre-me todos os formulários de pedido de empréstimo.</em></li><li><em>Estou procurando formulários de integração de funcionários.</em></li></ul> |
| Agente do Supervisor de Conteúdo | <ul><li>Otimização de conteúdo</li></ul> | <ul><li>Adobe Experience Manager Assets e Dynamic Media</li></ul> | 10 | <ul><li><em>Crie uma representação 2000px como JPEG com 80% de qualidade.</em></li><li><em>Criar uma representação para uma história do Instagram.</em></li><li><em>Sobreponha a imagem com 30% de gráficos com desconto sobre o banner promocional, colocando-a a 100px do centro.</em></li><li><em>Alterar cor de fundo do PNG para #ff8932.</em></li></ul> |
| Agente de governança de marca | <ul><li>Verificações de política de marca</li></ul><ul><li>Permissões com o Content Hub</li></ul><ul><li>Expiração do ativo</li></ul> | <ul><li>Adobe Experience Manager Sites (Políticas da marca)</li></ul><ul><li>Adobe Experience Manager Assets</li></ul> | 25 | <ul><li><em>Esta página está alinhada à minha marca? `https://www.website/en.html`</em></li><li><em>Mostrar todas as regras ABAC existentes do Content Hub</em></li><li><em>Algum dos meus ativos vai expirar em breve?</em></li></ul> |
| Brand Experience Agent | <ul><li>Atualização de conteúdo</li><li>Criação de Forms</li><li>Solução de problemas de pipeline</li></ul> | <ul><li>Serviços em nuvem Adobe Experience Manager</li><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Forms</li></ul> | 50 | <ul><li><em>Em `URL`, atualize o título para Olá, mundo</em></li><li><em>Criar um formulário de contato com campos de nome, email e mensagem</em></li><li><em>Solucionar problemas do meu pipeline com falha</em></li><li><em>Listar meus pipelines com falha para o Programa Principal.</em></li></ul> |
| Brand Experience Agent | Modernização do site | Serviços em nuvem Adobe Experience Manager | 100 | <ul><li><em>Migrar a página `https://wknd-trendsetters.site`</em></li></ul> |

>[!NOTE]
>
>O consumo real de crédito de IA pode variar dependendo do número de etapas executadas e iterações por etapa.

## Mais ajuda sobre este tópico

* [GenAI no CX Enterprise](generative-ai.md)
* [IA agêntica na CX Enterprise](agentic-ai.md)
* [Avaliação vinculada ao uso dos Adobe Experience Platform Agents](https://experienceleague.adobe.com/pt-br/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)
