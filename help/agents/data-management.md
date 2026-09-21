---
title: Agente de gerenciamento de dados para Adobe Experience Platform
description: Saiba como usar o Agente de gerenciamento de dados no CX Coworker para localizar e analisar conjuntos de dados do Adobe Experience Platform e gerenciar políticas de retenção de data lake.
source-git-commit: 40f144c7a06592c78dccc6c17f19554b62f667c9
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 3%
---
# Agente de gerenciamento de dados

>[!AVAILABILITY]
>
>O Agente de gerenciamento de dados está disponível para todos os clientes com acesso ao Adobe CX Enterprise Coworker.

Para entender e gerenciar a retenção de data lake para seus conjuntos de dados de Evento de experiência, use o Agente de gerenciamento de dados na CX Coworker. À medida que os conjuntos de dados do evento de experiência em seu data lake da Adobe Experience Platform crescem, as consultas e os processos de downstream podem levar mais tempo para serem concluídos, enquanto os requisitos de retenção se tornam mais difíceis de gerenciar. Descreva o que você deseja realizar em linguagem natural. O Agente de gerenciamento de dados encontra os conjuntos de dados relevantes do Evento de experiência, analisa a atividade com que são usados e modela a quantidade de dados que um período de retenção proposto afetaria. Quando estiver pronto para agir, ele ajuda a definir, alterar ou remover uma política de retenção e solicita sua confirmação antes de qualquer alteração.

## O que o Agente de gerenciamento de dados pode fazer {#what-the-data-management-agent-can-do}

O Agente de gerenciamento de dados fornece quatro habilidades.

>[!NOTE]
>
>As habilidades de Listar conjuntos de dados, Analisar uso de conjunto de dados e Analisar retenção de conjunto de dados são somente leitura. Somente a habilidade Gerenciar retenção do conjunto de dados pode alterar uma política de retenção de data lake e requer sua confirmação explícita antes de aplicar qualquer alteração.

| Habilidade | Descrição |
|---|---|
| **Listar conjuntos de dados** | Use ao decidir onde iniciar uma revisão de retenção. Lista seus conjuntos de dados de Evento de experiência com tamanho do armazenamento, contagem de linhas, configurações de retenção existentes e ativação de perfil para que você possa identificar rapidamente os conjuntos de dados que podem ser candidatos a uma política de retenção de data lake |
| **Analisar uso do conjunto de dados** | Use antes de decidir se um conjunto de dados é um bom candidato para uma política de retenção do data lake. Classifica ativamente se um conjunto de dados específico é usado com base em sinais como assimilação recente, atividade de consulta e uso downstream de aplicativos. |
| **Analisar retenção de conjunto de dados** | Use antes de confirmar um período de retenção. Mostra as métricas de armazenamento de um conjunto de dados e a idade de seus dados e, em seguida, usa essa distribuição de idade para aproximar a quantidade de dados que um possível período de retenção manteria ou removeria. |
| **Gerenciar retenção do conjunto de dados** | Use quando estiver pronto para agir. Define, altera ou remove uma política de retenção de data lake em um conjunto de dados, com uma visualização de impacto e confirmação antes de qualquer alteração. |

## Escopo: retenção de data lake versus outras ferramentas de gerenciamento de dados {#scope}

Use o Agente de gerenciamento de dados quando precisar localizar e analisar conjuntos de dados de Evento de experiência e definir, alterar ou remover uma política de retenção de data lake.

Se você não tem certeza se uma política de retenção de data lake é a opção certa para sua meta, consulte [Escolher o recurso de gerenciamento do ciclo de vida dos dados](https://experienceleague.adobe.com/en/docs/experience-platform/data-lifecycle/choose-a-capability) correto para comparar as opções de retenção e exclusão disponíveis.

Essas habilidades não gerenciam os seguintes recursos relacionados:

- **Política de retenção de repositório de perfil.** Para gerenciar por quanto tempo os Eventos de experiência permanecem no armazenamento de Perfis, configure uma política de expiração de Evento de experiência em conjuntos de dados de Evento de experiência habilitados para perfil. Consulte [Expiração do evento de experiência](https://experienceleague.adobe.com/pt-br/docs/experience-platform/profile/event-expirations).
- **Expiração de dados de perfil pseudônimo em toda a sandbox.** Para excluir automaticamente dados de perfil pseudônimo em uma sandbox depois que ela atender às condições configuradas, consulte [Perfis pseudônimos](https://experienceleague.adobe.com/pt-br/docs/experience-platform/profile/pseudonymous-profiles).
- **Expiração do conjunto de dados.** Para agendar um conjunto de dados inteiro para exclusão em uma data futura, consulte [Expiração do conjunto de dados](https://experienceleague.adobe.com/en/docs/experience-platform/data-lifecycle/ui/dataset-expiration).
- **Exclusão de Registro.** Para remover registros de perfis individuais por motivos de privacidade ou higiene, consulte [Exclusão de registro](https://experienceleague.adobe.com/en/docs/experience-platform/data-lifecycle/ui/record-delete).

## Pré-requisitos {#prerequisites}

Antes de começar, verifique se você tem:

- Acesso ao Adobe Experience Platform e à sandbox que contém os conjuntos de dados que você deseja revisar.
- As permissões do Adobe Experience Platform necessárias para os conjuntos de dados e ações de retenção que você deseja usar. O Agente de gerenciamento de dados usa suas permissões existentes do Experience Platform e não concede acesso adicional. Consulte a [Visão geral do controle de acesso](https://experienceleague.adobe.com/pt-br/docs/experience-platform/access-control/home) para saber como as permissões e funções do Adobe Experience Platform funcionam.
- O plug-in CXO do Adobe instalado no CX Co-worker.

Para obter instruções sobre como instalar plug-ins, consulte o [Guia da Interface do Usuário do Coworker](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide).

## Usar o Agente de gerenciamento de dados {#use-the-data-management-agent}

Interaja com o Agente de gerenciamento de dados por meio do CX Coworker usando a linguagem natural. Descreva sua meta e refine os resultados com perguntas de acompanhamento.

>[!NOTE]
>
>Antes de começar, verifique se você está trabalhando na sandbox que contém os conjuntos de dados que deseja revisar.

Para usar o Agente de Gerenciamento de Dados:

1. Navegue até **[!UICONTROL CX Coworker]**. Para obter detalhes de acesso, consulte o [Guia da Interface do Usuário do Colaborador](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide).
1. Insira uma solicitação que descreva o que você deseja realizar.
1. Revise os resultados e use perguntas de acompanhamento para continuar sua investigação.

Se uma solicitação alterar uma política de retenção de data lake, o Agente de gerenciamento de dados mostrará o impacto proposto e solicitará sua confirmação antes de aplicar a alteração.

Para um fluxo de trabalho completo para identificação de conjuntos de dados, análise do impacto de uso e retenção e gerenciamento de políticas de retenção de data lake, consulte [Gerenciar retenção de data lake](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md).

## Como o Agente de gerenciamento de dados funciona {#how-the-data-management-agent-works}

O Agente de gerenciamento de dados usa cálculos determinísticos para analisar o uso do conjunto de dados, de modo que as mesmas entradas produzem a mesma camada de uso. Também calcula o impacto de retenção de forma programática, em vez de depender de estimativas geradas por IA. O impacto da retenção continua sendo uma aproximação, pois se baseia na distribuição por idade dos dados. O agente recupera dados diretamente dos serviços da Adobe Experience Platform para fornecer informações atuais sobre seus conjuntos de dados.

## Limitações {#limitations}

O Agente de gerenciamento de dados pode identificar conjuntos de dados que podem ser bons candidatos para uma política de retenção de data lake, mas não decide se um conjunto de dados requer uma. Ela não aplica, altera ou remove uma política de retenção sem a sua confirmação explícita.

## Próximas etapas {#next-steps}

Para obter orientação sobre como usar cada habilidade para localizar, analisar e gerenciar a retenção de data lake em seus conjuntos de dados de Evento de experiência, consulte [Gerenciar a retenção de data lake](../coworker/chat/use-cases/data-management/manage-data-lake-retention.md).

Para obter mais informações sobre como as políticas de retenção de data lake funcionam no Adobe Experience Platform, incluindo comportamento e configuração de retenção, consulte [Guia de retenção do conjunto de dados (TTL) de evento de experiência](https://experienceleague.adobe.com/en/docs/experience-platform/catalog/datasets/experience-event-dataset-retention-ttl-guide).
