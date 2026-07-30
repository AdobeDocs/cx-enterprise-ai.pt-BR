---
title: IA em aplicativos corporativos do CX
description: Saiba como os aplicativos do CX Enterprise usam as ferramentas Gerative AI (GenAI), AI Assistant, Agentic AI, CX Enterprise Co-worker e MCP.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 325bdc7452557cf9a2b448b5e6afa613b87b4544
workflow-type: tm+mt
source-wordcount: 929
ht-degree: 2%

---

# IA na CX Enterprise

Este guia aborda os recursos de IA disponíveis nos aplicativos Adobe CX Enterprise: AI gerativa e AI Assistant para conhecimento do produto e insights operacionais, Agent Orchestrator e Experience Platform Agents para automatização de trabalhos, CX Enterprise Co-worker para uma experiência totalmente conversacional e de agente, e MCP para conectar suas próprias ferramentas de IA aos dados do CX Enterprise.

## Visão geral dos recursos de IA

Comece aqui para obter uma introdução sobre onde e como a IA é usada no CX Enterprise:

- [IA Gerativa](./overview/generative-ai.md) descreve quais aplicativos do CX Enterprise oferecem suporte ao AI e ao AI Assistant gerativos e como eles se comparam.
- [IA de agente](./overview/agentic-ai.md) explica como os Experience Platform Agents funcionam nos aplicativos CX Enterprise existentes e nos aplicativos AI-first, além de listar os agentes disponíveis em cada um.
- O [Monitoramento de IA de agente](./overview/monitoring.md) abrange os painéis que rastreiam a adoção, o uso, o feedback e o consumo de crédito de IA do agente.
- [Os trabalhos do agente e o consumo de crédito de IA](./overview/ai-credit-consumption.md) explica como os créditos de IA são consumidos pelos trabalhos do agente, com taxas de consumo estimadas por agente e tipo de trabalho.
- As [Ferramentas do CX Enterprise Agent](https://experienceleague.adobe.com/pt-br/docs/cx-enterprise-agentic-tools/using/overview) abordam habilidades e ferramentas adicionais de agente que ampliam os agentes do CX Enterprise.

## Assistente de IA

O [Assistente de IA](./ai-assistant/ai-assistant-ui.md) é uma ferramenta de IA conversacional e gerativa disponível em aplicativos baseados em Adobe Experience Platform. Use-o para obter conhecimento sobre o produto, solucionar problemas, encontrar insights operacionais e acessar agentes do Experience Platform, tudo por meio de prompts de linguagem natural em uma interface de exibição em tela cheia ou no painel.

Leia o [guia da interface do Assistente de IA](./ai-assistant/ai-assistant-ui.md) para saber como navegar na interface e a [biblioteca de prompts](./ai-assistant/prompt-library.md), por exemplo, os prompts do agente.

## Agentes do Agent Orchestrator e Experience Platform

[Agent Orchestrator](./agents/agent-orchestrator.md) é a camada de agente que habilita os Agentes Experience Platform. Quando você faz uma pergunta ao Assistente de IA, o Agent Orchestrator planeja o trabalho, chama os agentes especializados necessários para respondê-lo e retorna uma resposta unificada, tudo com supervisão humana.

Os seguintes agentes da Experience Platform estão documentados neste guia:

- [Audience Agent](./agents/audience.md)
- [Data Insights Agent](./agents/cja-data-insights-agent.md)
- [Experimentation Agent](./agents/agent-experiment.md)
- [Agente de descoberta de campo](./agents/field-discovery-agent.md)
- [Journey Agent](./agents/ajo-agent.md)
- [Agente de notificações](./agents/notifications.md)
- [Agente de suporte ao produto](./agents/product-support.md)
- [Adobe Marketing Agent for Microsoft 365 Copilot](./agents/ama-ms.md)
- [Validar seus dados](./agents/data-validation.md)

Para obter a lista completa de agentes, os aplicativos compatíveis e os requisitos de qualificação, consulte [IA de agente no CX Enterprise](./overview/agentic-ai.md).

## CX Enterprise Co-worker

O CX Enterprise Co-worker é uma evolução do assistente de IA realizada pelo agente, que automatiza a experiência do cliente e os fluxos de trabalho de marketing, para que sua equipe possa se concentrar em metas de negócios em vez de na execução de rotina. Em vez de fazer uma pergunta de cada vez, você descreve uma meta em linguagem natural e o Co-worker planeja o trabalho, executa-o no Adobe e nos sistemas conectados, valida os resultados e retorna o trabalho concluído para sua aprovação. O colega de trabalho inclui:

- **[Chat do Colaborador](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/chat/overview)**: uma interface conversacional para explorar seus dados, validar públicos e jornadas e concluir tarefas de várias etapas nos aplicativos do CX Enterprise.
- **[Campanhas com colegas de trabalho](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/campaigns/overview)**: um aplicativo nativo de IA que consolida instruções de campanha, a criação de públicos-alvo, a geração de conteúdo, o design de jornadas e a comprovação em uma única experiência de conversação, usando modelos internos, práticas recomendadas e orientações para que equipes pequenas e ágeis possam iniciar campanhas rapidamente.
- **Projetos de Colaborador** (em breve): um espaço de trabalho unificado para automatizar fluxos de trabalho completos de orquestração da experiência do cliente, ajudando as equipes a coordenar tarefas, aprovações e execução para impulsionar resultados da estratégia até a entrega. A documentação dos Projetos será disponibilizada em breve.

Os clientes qualificados estão sendo gradualmente migrados do Assistente de IA e Agentes do Experience Platform para o Chat de colaborador. Leia a [Avaliação do CX Enterprise Co-worker](./agents/trial.md) para saber mais sobre qualificação para a avaliação, uso de Crédito de IA e como obter acesso.

Para ver o Chat do Colaborador em ação, passe pelo [Chat do Colaborador no Playground](./coworker/playground-coworker-chat.md) ou leia casos de uso reais, como [Validar o AA para dados de migração do CJA](./coworker/data-validation-aa-cja.md) e [Analisar dados do CJA](./coworker/chat/analytics-chat.md).

Para obter a documentação completa do produto sobre bate-papo, campanhas e projetos do parceiro de trabalho, consulte [Colaborador corporativo do Adobe CX](./coworker/overview.md). Para replicação de objetos de sandbox para sandbox, consulte [Habilidades do agente de ferramentas de sandbox](./agents/sandbox-tooling.md).

## MCP

O [Adobe CX Co-worker Gateway](./mcp/overview.md) é o terminal MCP (Unified Model Context Protocol) do CX Enterprise. Ele oferece aos clientes compatíveis com MCP, como [!DNL Claude], [!DNL ChatGPT] e [!DNL Cursor], uma única conexão controlada com as ferramentas de produto que sua organização está autorizada a usar, incluindo Real-Time CDP, Experience Platform, Journey Optimizer, Customer Journey Analytics, Adobe Analytics e Workfront.

Novo no CX Co-worker Gateway? Consulte [Acessar as ferramentas do CX Coworker Gateway](./mcp/access.md) e [Instalar o CX Coworker Gateway](./mcp/install.md) para se conectar.

## Introdução

### Requisitos de acesso

Seu administrador do Adobe deve conceder as permissões apropriadas antes de usar o Assistente de IA e os Agentes da Experience Platform. Os requisitos variam de acordo com o aplicativo; consulte [Acesso](./agents/agent-orchestrator.md#access) no guia do Agent Orchestrator para obter detalhes.

### Privacidade e segurança

O Assistente de IA e os Agentes da Experience Platform são criados com privacidade, segurança e governança na vanguarda, incluindo isolamento de dados específico de sandbox e respeitando as políticas de controle de acesso existentes. Para obter detalhes completos, leia [Privacidade, segurança e governança no Assistente de IA](./ai-assistant/privacy.md).

## Práticas recomendadas

Para obter o máximo valor de sua experiência com o Assistente de IA ou Colaborador, siga estas práticas recomendadas:

- **Seja específico** em suas solicitações para obter insights relevantes e direcionados.
- **Verifique as respostas** examinando as citações de origem e as explicações de raciocínio fornecidas.
- **Use a configuração de contexto** para verificar se as fontes de dados mais relevantes são usadas para suas perguntas.
- **Forneça comentários** para ajudar a melhorar o desempenho e a precisão ao longo do tempo.
- **Combine insights** de vários agentes para obter uma análise mais abrangente.

## Considerações legais

O Assistente de IA atualmente suporta respostas somente em inglês e os modelos de idioma podem ocasionalmente cometer erros. Sempre verifique as informações fornecidas e use as etapas de raciocínio incluídas em cada resposta para entender como elas foram geradas. Para obter detalhes completos, leia o [aviso de isenção legal](./ai-assistant/legal-disclaimer.md).

