---
title: Transparência do conteúdo de IA gerativa
description: Saiba como o Adobe anexa automaticamente metadados C2PA a conteúdo gerado e editado por GenAI nos aplicativos corporativos do Adobe CX.
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
  - id: ec4263d9-bf7c-44c7-b3f1-3e664861c8f2
source-git-commit: 1ff44fcfab1a304b3640032d6c0985795f580e5e
workflow-type: tm+mt
source-wordcount: 1745
ht-degree: 2%

---


# Transparência do conteúdo de IA gerativa

Ao longo de agosto de 2026, a Adobe está lançando gradualmente o suporte a metadados C2PA em aplicativos Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly e Adobe CX Enterprise.

>[!NOTE]
>
>Após a implantação, os workflows futuros que envolverem conteúdo criado ou editado usando IA terão suporte automático aos metadados C2PA.

Esta página aborda detalhes sobre como o Adobe lida com a anexação automática de metadados C2PA nos aplicativos Adobe CX Enterprise.

As novas regulamentações exigem que os provedores de tecnologias de IA gerativa ofereçam suporte a divulgações duráveis e legíveis por máquina associadas a fluxos de trabalho de conteúdo gerados e editados pela GenAI para aumentar a transparência.

Como provedor de ferramentas, a Adobe anexa automaticamente metadados C2PA legíveis por máquina ao conteúdo gerado e editado por GenAI usando tecnologias da Adobe (incluindo modelos de IA gerativos de terceiros compatíveis nos fluxos de trabalho do Adobe). [Saiba mais sobre C2PA](https://c2pa.org/).

## O que está mudando

Lançamento em agosto de 2026, a Adobe introduzirá o suporte a metadados C2PA em aplicativos Adobe Creative Cloud, Adobe Document Cloud, Adobe Firefly e Adobe CX Enterprise.

Esta versão inclui:

* Anexação automática de metadados C2PA a conteúdo gerado e editado por GenAI com suporte.
* Suporte para tipos de conteúdo, incluindo imagens, vídeo, áudio e texto.
* Preservação de metadados C2PA em fluxos de trabalho do Adobe compatíveis.

Nenhuma ação adicional é necessária para anexar metadados C2PA ao conteúdo de IA gerativa qualificado.

>[!NOTE]
>
>Os metadados C2PA não afetarão a aparência do seu conteúdo. Os metadados C2PA e as marcas d&#39;água visíveis atendem a diferentes objetivos. Os metadados C2PA fornecem informações de origem legíveis por máquina, enquanto as marcas d&#39;água visíveis fornecem divulgação visual. Você pode optar por adicionar marcas d&#39;água visíveis ao seu conteúdo com base nas necessidades comerciais e nos requisitos legais de cada jurisdição aplicável.

## Quais detalhes são adicionados como parte dos metadados C2PA

Os metadados C2PA anexados automaticamente podem incluir informações como:

* Informações de nome e versão do sistema de IA usado (por exemplo, Adobe GenStudio, Adobe Firefly)
* Modelo de IA usado (por exemplo, Adobe Firefly)
* Uso: se foi gerado ou editado usando GenAI
* Hora e data da criação e/ou modificação do conteúdo com ferramentas de IA geradoras
* Identificador exclusivo (que pode ser usado para distinguir cada uso da IA gerativa)

## Metadados C2PA no supply chain de conteúdo

Os metadados C2PA foram projetados para permanecer associados ao conteúdo compatível à medida que se movem entre aplicativos Adobe e plataformas compatíveis de terceiros.

À medida que o conteúdo é publicado, distribuído ou compartilhado, as plataformas que suportam metadados C2PA ou tecnologias de origem relacionadas podem ler metadados anexados e exibir informações de transparência para os usuários.

O Adobe não controla como os serviços externos interpretam, exibem ou usam metadados C2PA depois que o conteúdo sai dos aplicativos Adobe. Os clientes devem consultar a documentação de plataformas de publicação individuais para entender como os metadados do C2PA são tratados.

## Marcação d&#39;água visível

Em algumas circunstâncias e em determinadas regiões, as organizações podem escolher ou ser solicitadas a identificar visivelmente o conteúdo gerado ou editado pela GenAI.

A Adobe fornece [orientação](https://helpx.adobe.com/br/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html) sobre como usar os recursos de marca d&#39;água existentes compatíveis com os aplicativos da Adobe. A visibilidade da marca d&#39;água depende dos requisitos de negócios de uma organização e das leis e regulamentos aplicáveis nas jurisdições onde o conteúdo é publicado.

>[!NOTE]
>
>Os metadados C2PA e as marcas d&#39;água visíveis atendem a diferentes objetivos. Os metadados do C2PA fornecem informações de origem legíveis por máquina, enquanto as marcas d&#39;água visíveis fornecem uma divulgação visual que as organizações podem optar por aplicar.

## Disponibilidade e versões

Esses recursos estão sendo lançados durante o **agosto de 2026** em todos os fluxos de trabalho corporativos do Adobe CX com suporte.

>[!NOTE]
>
>Após a implantação, os workflows futuros que envolverem conteúdo criado ou editado usando IA terão suporte automático aos metadados C2PA.

A versão inclui:

### Metadados automáticos do C2PA

Os metadados C2PA são anexados automaticamente ao conteúdo compatível gerado e editado por GenAI. Essa funcionalidade é habilitada por padrão e não pode ser desabilitada.

### Orientação de marca d&#39;água

A Adobe fornece a [documentação](https://helpx.adobe.com/br/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html) descrevendo como usar os recursos de marca d&#39;água existentes disponíveis em aplicativos compatíveis da Adobe para organizações que escolhem ou precisam aplicar rótulos visíveis.

## Aplicativos compatíveis com toda a Adobe CX Enterprise {#supported-applications}

Os seguintes aplicativos e serviços da Adobe fornecem informações adicionais sobre como e quando os metadados C2PA são anexados ao conteúdo qualificado em determinados aplicativos CX Enterprise.

No entanto, quando aplicável, todos os aplicativos corporativos Adobe CX continuam a preservar os metadados C2PA existentes, à medida que os ativos compatíveis passam pelos fluxos de trabalho do Adobe. Isso ajuda a manter a integridade das informações de origem em todo o conteúdo do supply chain.

>[!NOTE]
>
>As notas de versão ou orientações para cada um dos aplicativos listados abaixo serão disponibilizadas no Experience League nas respectivas seções da página de produtos do aplicativo. A tabela será atualizada com os links conforme eles se tornarem disponíveis. Consulte as seções mais recentes do produto no Experience League.

| Aplicativo/Solução | Notas de versão/Orientação |
|---|---|
| Adobe Advertising Cloud | [Documentação](https://experienceleague.adobe.com/pt-br/docs/advertising/creative/creative-studio/creative-studio-content-credentials) |
| Adobe Experience Manager (AEM) | [Documentação](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/c2pa-metadata-dynamic-media-openapi) |
| Assistente de IA para geração de conteúdo (recurso no Adobe Journey Optimizer/Adobe Campaign) | [Documentação](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/content-management/generate-content/generative-c2pa-metadata) |
| Ultimate B2B Adobe Journey Optimizer | [Documentação](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer-b2b/user/content-management/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2B Prime (também conhecido como Adobe Marketo Otimizer) | [Documentação](https://experienceleague.adobe.com/pt-br/docs/marketo-optimizer/user/content/assets/c2pa-metadata) |
| Adobe Journey Optimizer B2C | [Documentação](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/generate-content/c2pa/generative-c2pa-metadata) |
| Adobe Campaign | [Documentação](https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/content/ai-assistant/c2pa-metadata-email-designer) |
| Adobe Commerce | [Documentação](https://experienceleague.adobe.com/pt-br/docs/commerce/optimizer/manage-results/success-metrics#c2pa-metadata-on-exported-reports) |
| GenStudio para marketing de desempenho | [Documentação](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/content/content-credentials) |
| Adobe Marketo Engage | [Documentação](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/images-and-files/c2pa-metadata) |
| Adobe Workfront | [Documentação](https://experienceleague.adobe.com/pt-br/docs/workfront/using/documents/c2pa-metadata-overview) |
| Campanhas do CX Enterprise Co-worker (antigo HALO) | [Documentação](https://experienceleague.adobe.com/pt-br/docs/cx-enterprise-ai/experience-cloud-ai/coworker/campaigns/c2pa-metadata) |

## Links relacionados

* [Guia de marca d&#39;água visível](https://helpx.adobe.com/br/creative-cloud/apps/generative-ai/ai-content-watermarks-faq.html)
* [Adobe Inspect](https://contentauthenticity.adobe.com/inspect)
* [Visão geral da Iniciativa de conformidade de rotulagem da Adobe GenAI](https://helpx.adobe.com/br/creative-cloud/apps/generative-ai/ai-content-labeling-faq.html)

## Perguntas frequentes

**Quais aplicativos do Adobe aplicam metadados C2PA ao conteúdo editado ou criado de IA geradora?**

Os aplicativos corporativos Adobe CX compatíveis anexam automaticamente metadados C2PA ao conteúdo qualificado gerado e editado por GenAI. Consulte a seção [Aplicativos compatíveis](#supported-applications) para obter mais detalhes sobre os aplicativos corporativos do Adobe CX.

**A quais tipos de conteúdo o Adobe adiciona metadados C2PA?**

Em geral, imagens, áudio, vídeo, documentos e texto estão no escopo. No entanto, consulte a documentação na seção [Aplicativos compatíveis](#supported-applications) para descobrir como cada aplicativo suporta os metadados C2PA em diferentes produtos e tipos de conteúdo.

**Quais aplicativos do Adobe CX preservam os metadados C2PA durante a edição e a publicação?**

Todos os aplicativos corporativos Adobe CX foram projetados para preservar os metadados C2PA à medida que o conteúdo passa pelos fluxos de trabalho compatíveis do Adobe. A preservação fora dos aplicativos do Adobe depende de as plataformas externas oferecerem suporte aos metadados C2PA.

**O que acontece quando várias imagens geradas pela GenAI são combinadas em uma única imagem?**

Os metadados C2PA resultantes dependem do aplicativo e do fluxo de trabalho usados. Quando suportado, o Adobe preserva as informações de origem em todo o processo de edição. Consulte a seção [Aplicativos com suporte](#supported-applications-across-adobe-cx-enterprise) para obter a documentação sobre o comportamento específico do fluxo de trabalho em cada aplicativo.

**O que acontece quando imagens geradas pela GenAI de aplicativos Adobe e não Adobe são combinadas?**

O Adobe preserva metadados C2PA que estão disponíveis e são compatíveis com o fluxo de trabalho. Sempre que aplicável, o Adobe atualizará os metadados subjacentes com as informações mais recentes sempre que o conteúdo aplicável (imagem, áudio, vídeo, texto) for editado ou criado usando a GenAI nos fluxos de trabalho do Adobe. Ao combinar várias fontes em um novo ativo, os metadados subjacentes não são substituídos ou perdidos. Em vez disso, o novo ativo obtém seus próprios metadados C2PA e os detalhes de cada fonte são mantidos dentro dele. Se uma fonte já tiver seus próprios metadados C2PA — provenientes de uma ferramenta Adobe ou não-Adobe — esse histórico permanecerá anexado a ela. Isso significa que o ativo final carrega uma imagem completa: seu próprio registro de ser criado ou editado com a GenAI, além do histórico individual de cada peça que entrou nele.

**Os fluxos de trabalho editados e criados pela GenAI nos aplicativos do Adobe CX anexam automaticamente metadados C2PA?**

Sim. Para fluxos de trabalho de IA gerativa compatíveis, o Adobe anexa automaticamente metadados C2PA que identificam se o conteúdo foi gerado ou editado por GenAI junto com outras informações de origem, como carimbos de data e hora, informações do sistema de IA e identificadores exclusivos.

**Como os metadados C2PA são mantidos no supply chain de conteúdo?**

Os metadados C2PA são metadados duráveis projetados para permanecer associados ao conteúdo compatível, à medida que se movem entre aplicativos compatíveis do Adobe e plataformas de terceiros compatíveis. Os serviços externos determinam como as informações de origem anexadas são exibidas após a publicação.

**Como as organizações podem adicionar suas próprias informações autenticadas sem romper a cadeia de origem?**

Alguns aplicativos do Adobe permitem que criadores e organizações adicionem mais informações autenticadas aos metadados C2PA existentes, preservando a origem. A disponibilidade varia conforme o aplicativo.

**É possível desativar a anexação automática de metadados C2PA?**

Não. As novas leis de transparência da IA gerativa exigem que as empresas que fornecem ferramentas de IA gerativa, incluindo o Adobe, anexem metadados duráveis ao conteúdo qualificado gerado ou editado com IA gerativa. A anexação automática de metadados C2PA não pode ser desativada.

**O que acontece com o conteúdo criado/editado com IA gerativa antes da versão de agosto?**

O conteúdo criado ou editado com ferramentas de IA gerativas antes da versão de agosto de 2026 não tem metadados C2PA automáticos anexados. No entanto, o conteúdo criado na Web do Firefly e outros aplicativos nos quais os metadados C2PA foram aplicados anteriormente continuam a anexá-los.

**Como um cliente pode verificar se o conteúdo tem metadados C2PA anexados?**

Os clientes podem verificar se o conteúdo tem metadados C2PA anexados ao carregá-los na página [Adobe Inspect](https://contentauthenticity.adobe.com/inspect).

**Como as plataformas externas exibem metadados C2PA quando o conteúdo é publicado ou compartilhado?**

À medida que o conteúdo se move entre plataformas de publicação, canais de mídia social, serviços de email e outros ecossistemas digitais, os serviços downstream que oferecem suporte aos metadados C2PA ou às tecnologias de proveniência relacionadas podem ler os metadados anexados e optar por exibir divulgações ou indicadores com base nessas informações. A Adobe não controla como as plataformas externas exibem, interpretam ou aplicam as divulgações associadas aos metadados C2PA anexados. Para obter as informações mais atuais sobre como uma plataforma específica lida com informações de origem, os clientes devem verificar diretamente as diretrizes da plataforma.

**Essas alterações aumentam o custo dos produtos ou assinaturas da Adobe?**

Não. Os metadados C2PA não afetam o custo dos produtos da Adobe.
