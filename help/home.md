---
title: IA nos aplicativos do CX Enterprise
description: Saiba como os aplicativos do CX Enterprise usam as ferramentas Gerative AI (GenAI), AI Assistant, Agentic AI, CX Enterprise Co-worker e MCP.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 543c62ff56886213b9212864e6ff6ad02dc0f742
workflow-type: tm+mt
source-wordcount: 862
ht-degree: 3%

---

# IA no CX Enterprise

Este guia aborda os recursos de IA do Adobe CX Enterprise: IA gerativa, AI Assistant, Agent Orchestrator, Experience Platform Agents, CX Enterprise Co-worker e MCP.

## Visão geral dos recursos de IA

Comece aqui para obter uma introdução sobre onde e como a IA é usada no CX Enterprise:

- [Sobre a IA gerativa](./overview/generative-ai.md) descreve quais aplicativos do CX Enterprise oferecem suporte à IA gerativa e ao Assistente de IA e como eles se comparam.
- [Sobre IA de agente](./overview/agentic-ai.md) explica como os Agentes da Experience Platform funcionam nos aplicativos CX Enterprise existentes e nos aplicativos AI-first, além de listar os agentes disponíveis em cada um.
- O [monitoramento de IA](./overview/monitoring.md) abrange os painéis que rastreiam a adoção, o uso, o feedback e o consumo de crédito de IA do agente.
- [Consumo de créditos de IA](./overview/ai-credit-consumption.md) explica como os trabalhos de agente consomem créditos de IA, com taxas de consumo estimadas por agente e tipo de trabalho.
- As [ferramentas do CX Enterprise Agent](https://experienceleague.adobe.com/pt-br/docs/cx-enterprise-agentic-tools/using/overview) abrangem habilidades e ferramentas adicionais de agente que ampliam os CX Enterprise agents (tutoriais em vídeo).

## Assistente de IA

O [Assistente de IA](./ai-assistant/ai-assistant-ui.md) é uma ferramenta de IA conversacional e gerativa disponível em aplicativos baseados em Adobe Experience Platform. Use-o para obter conhecimento sobre o produto, solucionar problemas, encontrar insights operacionais e acessar agentes do Experience Platform, tudo por meio de prompts de linguagem natural em uma interface de exibição em tela cheia ou no painel.

Para saber como navegar na interface, leia o [guia da interface do assistente do AI](./ai-assistant/ai-assistant-ui.md). Para ver exemplos de prompts por agente, consulte a [biblioteca de prompts](./ai-assistant/prompt-library.md).

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

## Colaborador

O Colaborador é uma evolução do Assistente de IA realizada por um agente que automatiza a experiência do cliente e os fluxos de trabalho de marketing, para que sua equipe possa se concentrar nas metas de negócios em vez da execução de rotina. Em vez de fazer uma pergunta por vez, você descreve uma meta. O colega de trabalho planeja, executa, valida e retorna o trabalho concluído para sua aprovação. O colega de trabalho inclui:

- **[Chat do Colaborador](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/overview)**: uma interface conversacional para explorar seus dados, validar públicos e jornadas e concluir tarefas de várias etapas nos aplicativos do CX Enterprise.
- **[Campanhas de colega](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/overview)**: um aplicativo nativo de IA que consolida informações de campanha, criação de público, geração de conteúdo, design de jornada e provas em uma única experiência de conversação. Ele usa modelos integrados, práticas recomendadas e orientação de solicitação para ajudar equipes pequenas e ágeis a iniciar campanhas rapidamente.
- **Projetos de Colaborador** (em breve): um espaço de trabalho unificado para automatizar fluxos de trabalho completos de orquestração da experiência do cliente, ajudando as equipes a coordenar tarefas, aprovações e execução para impulsionar resultados da estratégia até a entrega. A documentação dos Projetos será disponibilizada em breve.

Os clientes qualificados estão sendo gradualmente migrados do Assistente de IA e Agentes do Experience Platform para o Chat de colaborador. Leia [Avaliação de colaborador](./agents/trial.md) para saber mais sobre qualificação de avaliação, uso de Crédito de IA e como obter acesso.

Para ver o Chat do Colaborador em ação, passe pelo [Chat do Colaborador no Playground](./coworker/playground-coworker-chat.md) ou leia casos de uso reais, como [Validar o AA para dados de migração do CJA](./coworker/chat/use-cases/data-insights/data-validation-aa-cja.md) e [Analisar dados do CJA](./coworker/chat/use-cases/data-insights/analytics-chat.md).

Para obter a documentação completa do produto sobre Chat, Campanhas e Projetos do Colaborador, consulte [Colaborador](./coworker/overview.md). Para replicação de objetos de sandbox para sandbox, consulte [Habilidades do agente de ferramentas de sandbox](./agents/sandbox-tooling.md).

## MCP

O [Adobe CX Co-worker Gateway](./mcp/overview.md) é o terminal MCP (Unified Model Context Protocol) do CX Enterprise. Ele fornece aos clientes compatíveis com MCP, como [!DNL Claude], [!DNL ChatGPT] e [!DNL Cursor], uma única conexão controlada com as ferramentas de produto que sua organização está autorizada a usar. Essas ferramentas incluem [!DNL Real-Time CDP], [!DNL Experience Platform], [!DNL Journey Optimizer], [!DNL Customer Journey Analytics], [!DNL Adobe Analytics] e [!DNL Workfront].

Novo no CX Co-worker Gateway? Consulte [Acessar as ferramentas do CX Coworker Gateway](./mcp/access.md) e [Instalar o CX Coworker Gateway](./mcp/install.md) para se conectar.

## Introdução

### Requisitos de acesso

Seu administrador do Adobe deve conceder as permissões apropriadas antes de usar o Assistente de IA e os Agentes da Experience Platform. Os requisitos variam de acordo com o aplicativo; consulte [Acesso](./agents/agent-orchestrator.md#access) no guia do Agent Orchestrator para obter detalhes.

### Privacidade e segurança

O Assistente de IA e os Agentes da Experience Platform priorizam a privacidade, a segurança e o controle, incluindo o isolamento de dados específico da sandbox e suas políticas de controle de acesso existentes. Para obter detalhes completos, leia [Privacidade, segurança e governança no Assistente de IA](./ai-assistant/privacy.md).

## Práticas recomendadas

Para obter o máximo valor de sua experiência com o Assistente de IA ou Colaborador, siga estas práticas recomendadas:

- **Seja específico** em suas solicitações para obter insights relevantes e direcionados.
- **Verifique as respostas** examinando as citações de origem e as explicações de raciocínio fornecidas.
- **Use a configuração de contexto** para verificar se as fontes de dados mais relevantes são usadas para suas perguntas.
- **Forneça comentários** para ajudar a melhorar o desempenho e a precisão ao longo do tempo.
- **Combine insights** de vários agentes para obter uma análise mais abrangente.

## Considerações legais

O Assistente de IA atualmente suporta respostas somente em inglês e os modelos de idioma ocasionalmente cometem erros. Sempre verifique as informações fornecidas e use as etapas de raciocínio incluídas em cada resposta para entender como elas foram geradas. Para obter detalhes completos, leia o [aviso de isenção legal](./ai-assistant/legal-disclaimer.md).

