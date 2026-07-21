---
title: Analisar dados do Customer Journey Analytics com o Chat do parceiro
description: Saiba como usar o Adobe CX Enterprise Co-worker Chat para analisar dados do Customer Journey Analytics, criar funis e descobrir onde os clientes chegam em sua jornada.
source-git-commit: 6e3ab12f1d9ec706e745749b7ca47b91a09ff8b3
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 4%

---

# Analisar dados do Customer Journey Analytics com o Chat do parceiro

>[!AVAILABILITY]
>
>A funcionalidade descrita neste artigo está na fase de Teste limitado da versão e pode ainda não estar disponível em seu ambiente. Essa nota será removida quando a funcionalidade estiver disponível no geral. Para obter informações sobre o processo de lançamento do Customer Journey Analytics, consulte [versões de recursos do Customer Journey Analytics](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/releases/latest).

O Adobe CX Enterprise Co-worker Chat pode executar análises avançadas de dados que anteriormente eram possíveis somente no Analysis Workspace. O Bate-papo com colegas de trabalho acessa os dados das visualizações de dados do Customer Journey Analytics, permitindo que você explore esses dados e obtenha respostas para prompts em linguagem natural.

Antes de começar a análise, saiba mais sobre a interface do Coworker Chat e as opções de configuração e, em seguida, verifique se o Coworker está conectado ao Customer Journey Analytics e à visualização de dados que contém os dados que você deseja usar.

## Introdução ao Chat do Colaborador

### Opções de interface e configuração

Antes de usar o Co-worker Chat com seus dados do Customer Journey Analytics, saiba como fazer logon e gerenciar as opções de configuração para os seguintes recursos:

* Entradas de chat

* Conversas

* Marketplaces

* Servidores MCP

* Memória

* Plug-ins

* Habilidades

* E muito mais

Para obter mais informações, consulte o [Guia de Interface de Chat do Colaborador](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/chat/ui-guide).

### Casos de uso do Customer Journey Analytics

Você pode ver casos de uso da Customer Journey Analytics e exemplos de prompts que os profissionais estão usando no Adobe CX Enterprise Coworker Chat. Cada prompt é criado para ser copiado, adaptado com seus próprios dados e contexto e refinado através da conversa.

Para obter mais informações, consulte [Casos de uso](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/chat/use-cases).

## Verifique se o Chat do colaborador está conectado ao Customer Journey Analytics

1. No Chat do colaborador, verifique se o colaborador está conectado ao Customer Journey Analytics:

1. Selecione o ícone MCP no painel à esquerda e verifique se [!UICONTROL **cja-mcp**] está disponível na lista de servidores MCP conectados.

   ![O ícone MCP realçado no painel esquerdo do Colaborador](assets/data-validation-aa-cja/coworker-mcp-cja.png)

1. (Condicional) Se o [!UICONTROL **cja-mcp**] ainda não estiver conectado, selecione [!UICONTROL **Adicionar Servidor MCP**], especifique o cja no campo [!UICONTROL **Nome do Servidor**] e selecione-o quando ele aparecer e selecione [!UICONTROL **Adicionar Servidor**].

## Conectar à visualização de dados direita

Uma visualização de dados é um container no Customer Journey Analytics que determina como os dados são interpretados.

Você pode ter acesso a várias visualizações de dados no Customer Journey Analytics, cada uma contendo diferentes dimensões e métricas que o Colaborador pode usar ao analisar dados.

### Decida quais visualizações de dados você deseja usar

Informe ao Coworker os tipos de perguntas que você deseja responder e pergunte a qual visualização de dados você tem acesso que seria melhor fornecer essas informações. Você também pode [definir sua visualização de dados como uma preferência na memória](#add-a-data-view-preference-in-memory).

**Você:**

>[!BEGINSHADEBOX]

Estou interessado em saber onde os clientes chegam na jornada do cliente. A quais visualizações de dados no Customer Journey Analytics tenho acesso que poderiam responder a essa pergunta para mim?

>[!ENDSHADEBOX]

**Resposta do Chat de Colaborador:**

>[!BEGINSHADEBOX]

Você tem acesso a três visualizações de dados. A visualização de dados do `Customer lifecycle` contém as seguintes dimensões e métricas, que seriam as melhores para responder à sua pergunta.

>[!ENDSHADEBOX]

**Você:**

>[!BEGINSHADEBOX]

Ótimo, vamos usar essa visualização de dados.

>[!ENDSHADEBOX]

**Resposta do Chat de Colaborador:**

>[!BEGINSHADEBOX]

OK, usarei a visualização de dados `Customer lifecycle` para responder a perguntas futuras nesta sessão de chat.

>[!ENDSHADEBOX]

### Adicionar uma preferência de visualização de dados na memória

O Chat do Colaborador contém um recurso de memória que permite fornecer a ele acesso a informações que se estendem por todos os chats. É uma boa prática adicionar suas visualizações de dados preferidas como preferências na memória do Colaborador.

1. No Bate-papo com colega, na navegação à esquerda, selecione o ícone Memória.

1. Na página Memória, na seção Preferências armazenadas, especifique uma ou mais visualizações de dados que você deseja que o Bate-papo de Colaborador use em seus chats.

   ![Seção Memória no painel esquerdo](assets/data-validation-aa-cja/coworker-memory.png)

## Analisar no Customer Journey Analytics

Depois que o Colaborador cria uma visualização, você pode abri-la no Analysis Workspace no Customer Journey Analytics para uma análise mais profunda com controle mais granular. A visualização é aberta em um novo projeto do Analysis Workspace no Customer Journey Analytics.

Para abrir uma visualização em um novo projeto do Analysis Workspace:

1. Selecione [!UICONTROL **Analisar no CJA**] ao lado de qualquer visualização criada no Co-worker.

1. Com a visualização aberta no Customer Journey Analytics, você pode usar a interface de navegador de arrastar e soltar do Analysis Workspace para fazer modificações, criar ainda mais sua análise, criar um público-alvo e muito mais. Você pode até mesmo compartilhar seu projeto do Workspace com qualquer pessoa que escolher.

   Para obter mais informações sobre o Analysis Workspace, consulte [visão geral do Analysis Workspace](https://experienceleague.adobe.com/pt-br/docs/analytics-platform/using/cja-workspace/home).

## Exemplo: descobrir onde os clientes chegam

Você pode pedir ao Bate-papo com colegas de trabalho que use seus dados para analisar qualquer questão comercial.

Por exemplo, como gerente de marketing, comerciante ou líder de crescimento, você pode querer entender onde os clientes abandonam o caminho para comprar, por que fizeram e o que pode ser feito para impulsionar taxas de conversão mais altas.

>[!NOTE]
>
>As figuras abaixo são dados de exemplo ilustrativos para uma retailer fictícia, [!DNL TechPulse Electronics], usada para mostrar a forma da conversa.

### Os tipos de perguntas que você pode fazer

Você não precisa saber o que é uma &quot;visualização de fallout&quot; ou qual métrica vai para qual slot. Em vez disso, descreva o resultado importante em linguagem simples:

* &quot;Onde estamos perdendo pessoas a caminho de comprar?&quot;
* &quot;Qual é o meu funnel de conversão completa, desde a visualização do produto até o check-out?&quot;
* &quot;Quais canais de marketing mais vazam entre o carrinho e a compra?&quot;
* &quot;O abandono do carrinho é pior em dispositivos móveis ou em desktops?&quot;
* &quot;As pessoas de redes sociais pagas convertem-se de forma diferente das pessoas de e-mail?&quot;

### A conversa

#### &#x200B;1. Comece com a pergunta comercial

**Você:**

>[!BEGINSHADEBOX]

Onde estamos perdendo pessoas a caminho de comprar?

>[!ENDSHADEBOX]

**Resposta do Chat de Colaborador:**

Observe que o Bate-papo com colegas de trabalho escolhe a visualização correta, faz a sequência dos pontos de contato e até adiciona as próximas etapas recomendadas.

>[!BEGINSHADEBOX]

![Resposta do Coworker funnel](assets/data-validation-aa-cja/coworker-funnel-response.png)

Esta é uma pergunta sobre o funnel — deixe-me executar o funnel de conversão para ver onde a entrega acontece no caminho da compra.

Aqui é onde você está perdendo pessoas:

| Etapa do funnel | Count | Conversão para o próximo | Drop-off |
| --- | --- | --- | --- |
| Sessions | 137,476 | 45% visualizam um produto | 55% de licenças sem navegar pelos produtos |
| Visualizações de produto | 61,845 | 55,0% de acréscimo ao carrinho | 45% navegam, mas não adicionam |
| Adições ao carrinho | 34,045 | 16,4% de compra | 83,6% abandonam o carrinho |
| Compras | 5,582 | — | — |

**A grande descoberta: o carrinho que você vai comprar é o seu maior vazamento**

28.463 pessoas adicionam itens ao carrinho, mas nunca concluem a compra. Essa é uma taxa de devolução de 83,6% do carrinho até a compra — de longe o maior ponto único de falha.

Para colocar em termos de dólares, converter apenas 10% mais desses adicionadores de carrinho adicionaria cerca de 2.846 compras. Na escala de dados atual, essa é uma receita potencialmente significativa deixada na mesa.

**O que isso informa sobre as prioridades:**

| Prioridade | Problema | Escala de oportunidade |
| --- | --- | --- |
| #1 | Abandono de carrinho para compra (queda de 83,6%) | 28.463 compradores perdidos |
| #2 | Sessão para visualização do produto (55% nunca navegam) | 75.631 sessões sem envolvimento com o produto |
| #3 | Exibição do produto ao carrinho (45% não adicionam) | 27.800 interessados, mas não comprometidos |

**Próximas etapas recomendadas:**

1. Detalhar o abandono do carrinho por canal de marketing: alguns canais estão trazendo tráfego de baixa intenção que aumenta o carrinho, mas nunca compra?
1. Observe o abandono do carrinho por tipo de dispositivo. O atrito do checkout móvel está matando as conversões?
1. Identifique quais produtos são mais abandonados — problema de preço? Surpresa no transporte?

**Quais destes itens você deseja que eu descubra a seguir?** O detalhamento do canal informaria diretamente quais ações de marketing estão trazendo a você &quot;quase compradores&quot; versus compradores reais.

>[!ENDSHADEBOX]

#### &#x200B;2. Perfurar o vazamento

**Você:**

>[!BEGINSHADEBOX]

Ok, vamos detalhar por canal de marketing

>[!ENDSHADEBOX]

**Resposta do Chat de Colaborador:**

>[!BEGINSHADEBOX]

![Resposta do Coworker funnel](assets/data-validation-aa-cja/coworker-funnel-response2.png)

Há uma dimensão personalizada de **Canal de marketing**. Deixem-me analisar a funnel e calcular as taxas de conversão por canal e identificar onde cada canal vaza.

**O veredicto: o vazamento não é específico do canal**

Esta é uma descoberta realmente reveladora. Este é o detalhamento do funnel por canal:

| Canal | Sessions | Para exibição do produto | Para adicionar carrinho | Para comprar | Conversão geral | Receita/sessão |
| --- | --- | --- | --- | --- | --- | --- |
| Pesquisa paga | 43,958 | 45.1% | 54.6% | 16.6% | 4.09% | $499.58 |
| Pesquisa orgânica | 31,492 | 44.9% | 54.9% | 16.9% | 4.17% | $494.76 |
| Direto | 25,661 | 43.6% | 55.4% | 15.8% | 3.82% | $497.29 |
| Email | 17,586 | 45.3% | 55.4% | 16.2% | 4.07% | $501.13 |
| Social pago | 12,684 | 45.4% | 55.7% | 16.0% | 4.03% | $512.17 |
| Exibir | 6,511 | 45.3% | 55.7% | 16.2% | 4.09% | $501.45 |

**Principais argumentos:**

1. A devolução do carrinho para compra é uniformemente incorreta em todos os canais (83-84%). Isso significa que o problema não está na qualidade do tráfego — cada canal fornece visitantes envolvidos de forma semelhante. O vazamento está na sua experiência de finalização em si, não no marketing.
1. Nenhum canal é significativamente melhor ou pior na conversão. As taxas de conversão gerais se agrupam perfeitamente entre 3,8% e 4,2%, e a receita por sessão é quase idêntica (US$ 495 a US$ 512).
1. Onde o impacto no volume é mais importante: a pesquisa paga perde mais pessoas em termos absolutos (9.015 abandonos de carrinho), seguida pela pesquisa orgânica (6.449 perdidos). Estas são as maiores oportunidades em valores de dólar porque elas geram mais tráfego.

**O que isso lhe diz estrategicamente**

Os canais de marketing estão fazendo seu trabalho — todos estão deixando as pessoas interessadas e adicionando ao carrinho em taxas semelhantes. O problema é downstream de marketing: seu checkout e fluxo de pagamento é onde o dinheiro está vazando.

**Próximas investigações recomendadas:**

1. Detalhar o abandono do carrinho por tipo de dispositivo — o checkout móvel é interrompido ou frustrante?
1. Veja quais produtos são mais abandonados — há uma surpresa de preços ou envio na finalização da compra?
1. Verifique se a campanha &quot;Holiday_flash_sale&quot; teve uma conversão melhor do checkout: campanhas orientadas por urgência podem superar o atrito do checkout

**Que ângulo você gostaria de explorar a seguir?**

>[!ENDSHADEBOX]

#### &#x200B;3. Continuar investigando

**Você:**

>[!BEGINSHADEBOX]

Interessante. Vamos tentar detalhar por tipo de dispositivo.

>[!ENDSHADEBOX]

**Resposta do Chat de Colaborador:**

>[!BEGINSHADEBOX]

![Resposta do Coworker funnel](assets/data-validation-aa-cja/coworker-funnel-response3.png)

**Encontrado: o check-out móvel foi desfeito**

O funnel é idêntico em todos os dispositivos até o check-out — depois, o dispositivo móvel cai de um penhasco:

| Dispositivo | Sessions | Para exibição do produto | Para adicionar carrinho | Para comprar | Conversão geral |
| --- | --- | --- | --- | --- | --- |
| Desktop | 70,172 | 44.9% | 54.8% | 23.2% | 5.70% |
| Tablet | 14,149 | 44.7% | 55.6% | 14.3% | 3.56% |
| Dispositivo móvel | 53,449 | 44.9% | 55.3% | 8.1% | 2.02% |

**A arma do cigarro**

| Métrica | Desktop | Dispositivo móvel | Lacuna |
| --- | --- | --- | --- |
| Taxa de compra do carrinho | 23.2% | 8.1% | 15 pontos percentuais |
| O dispositivo móvel é | — | 2,8x pior | — |
| Carrinhos abandonados | 13,274 | 12,178 | Quase o mesmo volume absoluto |

A experiência de navegação e de adição ao carrinho é boa em dispositivos móveis (taxa de navegação idêntica a ~45%, ~55% de taxa de adição ao carrinho). As pessoas estão igualmente interessadas e engajadas. Mas algo no fluxo de check-out móvel está matando as conversões.

**A oportunidade de receita**

Se o checkout móvel fosse convertido à mesma taxa do desktop, você ganharia ~1.991 compras adicionais — um aumento de 35% no volume total de compras com a correção de uma experiência.

**O que provavelmente está acontecendo**

O padrão de dados (engajamento igual, queda de check-out catastrófica) é um sinal clássico para:

* O atrito do formulário de pagamento em telas pequenas (problemas de preenchimento automático, layout de formulário)
* Custos inesperados revelados no checkout (envio, impostos) causando choque no adesivo
* Check-out de convidado não disponível ou um mural de logon em dispositivos móveis
* Problemas de carregamento de página ou tempo limite durante o processamento de pagamento em dispositivos móveis

**Próximas etapas recomendadas:**

1. Detalhar o abandono do carrinho móvel por categoria de produto — é pior para itens de alto preço (sugerindo problemas de confiança de pagamento móvel)?
1. Veja quais canais de marketing direcionam mais tráfego móvel: você está gastando dinheiro pago em mídia para enviar pessoas para uma funnel móvel quebrada?
1. Verifique se há um sinal de página ou seção do site. Podemos ver quais páginas de check-out os usuários móveis acessaram por último antes de abandonar?

**Qual você gostaria de explorar ou esta evidência é suficiente para levar para sua equipe de UX e check-out?**

>[!ENDSHADEBOX]

#### &#x200B;4. Transforme em uma decisão

**Você:**

>[!BEGINSHADEBOX]

Então, o que devo fazer?

>[!ENDSHADEBOX]

**Resposta do Chat de Colaborador:**

>[!BEGINSHADEBOX]

Com base no que os dados mostram, é aqui que eu me concentrarei:

* **Corrija o check-out móvel — não é um problema de canal.** Cada canal está convertendo pessoas no carrinho em uma taxa semelhante e saudável, então o gasto com anúncios está funcionando em todos os sentidos. A receita está sendo perdida especificamente no fluxo de check-out móvel, que é o lugar da correção.
* **Comece com pagamento e fricção de formulário.** Essas são as razões mais comuns para os compradores de dispositivos móveis de alta intenção abandonarem um carrinho. Oferecer opções de carteira móvel e encurtar o formulário geralmente são os ganhos mais rápidos.
* **Verificar novamente após a correção.** Depois que as alterações no checkout forem enviadas, observe se a taxa de carrinho-para-compra dos dispositivos móveis se move em direção à taxa de desktop de 23,2%.

Quer que eu salve como um projeto para que você possa rastreá-lo ou definir um alerta se o carrinho de compras de dispositivos móveis ficar abaixo de um limite?

>[!ENDSHADEBOX]

### O que aconteceu

Em quatro perguntas simples, Coworker nos ajudou a:

* Crie um funnel de conversão de várias etapas e sinalize o carrinho de compras como o maior vazamento
* Exclua o canal de marketing como causa — cada canal vazou quase na mesma taxa
* Isole o problema real para a finalização móvel e quantifique a correção em um aumento de 35% nas compras
* Saia com uma correção específica para priorizar: pagamento móvel e atrito de formulários. Isso é comparado com a taxa de conversão de 23,2% do desktop

<!--

## Example #2: Find which marketing efforts drive revenue

You can ask Coworker Chat to use your data to analyze any business question.

For example, as a marketing manager, demand generation lead, or CMO, you might want to know which marketing efforts actually deserve credit for revenue so you can confidently decide where to put your marketing spend, rather than rewarding whichever channel happened to get the last click.

>[!NOTE]
>
>The figures below are illustrative sample data for a fictional retailer, [!DNL TechPulse Electronics], used to show the shape of the conversation.

### The types of questions you can ask

You don't need to know what an "attribution model" is, or how to configure an Attribution panel. Instead, describe the outcome you care about in plain language:

* "Which channels actually drive our revenue, not just the last click?"
* "If I change how I give credit for a sale, does my best channel change?"
* "Which campaigns start customer journeys versus close them?"
* "Am I over-investing in paid search because it always gets the last click?"
* "What role does email play in conversions it never gets credit for?"

### The conversation

#### 1. Start with the business question

**You:**

>[!BEGINSHADEBOX]

Which marketing channels actually drive our revenue?

>[!ENDSHADEBOX]

**Coworker Chat response:**

Notice that Coworker Chat picks the right analysis, starts with the model most reports default to, and immediately flags what that model can't tell you.

>[!BEGINSHADEBOX]

![Coworker Chat showing attributed revenue by marketing channel under a last-touch model](assets/data-validation-aa-cja/coworker-attribution-response.png)

This is an attribution question — let me attribute revenue to your marketing channels so you can see who's earning it.

I'll start with **last-touch attribution**, since that's what most out-of-the-box reports show. It gives all the credit for a sale to the last channel a person used before purchasing.

| Marketing channel | Attributed revenue (last touch) | Share |
| --- | --- | --- |
| Paid search | $948,000 | 34% |
| Organic search | $614,000 | 22% |
| Direct | $474,000 | 17% |
| Email | $307,000 | 11% |
| Paid social | $251,000 | 9% |
| Display | $195,000 | 7% |

**The headline: paid search looks like your hero**

Under last touch, paid search earns a third of all revenue — more than any other channel. If this were the only view you had, you'd likely pour more budget into paid search.

**One important caveat before you do that**

Last touch only tells you who *closed* the sale. It says nothing about who *started* the journey or *assisted* along the way. A channel that introduces people to your brand weeks before they buy gets zero credit here, even if the purchase never would've happened without it.

To know whether paid search is really driving revenue — or just harvesting demand other channels created — you need to compare attribution models.

**Recommended next step:**

Compare the same channels across first-touch, last-touch, and linear models. If paid search stays on top across all of them, it's a genuine driver. If it shrinks under first touch, it's a closer, not a creator.

**Want me to run that comparison?**

>[!ENDSHADEBOX]

#### 2. Compare attribution models

**You:**

>[!BEGINSHADEBOX]

Yes, compare it across models.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat comparing channel revenue share across first-touch, last-touch, and linear attribution models](assets/data-validation-aa-cja/coworker-attribution-response2.png)

Here's each channel's share of revenue under three models. First touch credits the channel that started the journey, last touch credits the one that closed it, and linear splits credit evenly across every touch.

| Marketing channel | First touch | Last touch | Linear |
| --- | --- | --- | --- |
| Paid search | 19% | 34% | 26% |
| Organic search | 20% | 22% | 21% |
| Direct | 9% | 17% | 13% |
| Email | 18% | 11% | 15% |
| Paid social | 21% | 9% | 15% |
| Display | 13% | 7% | 10% |

**The verdict: your "best" channel depends entirely on how you count**

This is the finding that changes budget decisions.

1. **Paid search closes far more than it starts.** It jumps from 19% of first touches to 34% of last touches. That's the signature of a *harvester* — it captures people who are already ready to buy, often after another channel introduced them. Valuable, but it's finishing journeys, not creating them.
1. **Paid social and email are badly undercredited by last touch.** Paid social starts 21% of journeys but gets credit for only 9% of sales. Email starts 18% but closes 11%. These channels are doing the expensive work at the top of the funnel and handing warm prospects to paid search.
1. **Organic search is your steady workhorse.** It sits around 20% across every model — it both starts and closes journeys reliably.

**Why this matters for budget**

If you cut paid social or email based on their weak last-touch numbers, you'd starve the top of your funnel — and paid search would have far fewer ready-to-buy people to close. You'd likely see paid search revenue fall too, even though you didn't touch its budget.

**Recommended next step:**

Look at the campaign level to see exactly which efforts start journeys versus close them. That's where you can act — trimming or protecting specific campaigns rather than whole channels.

**Want me to break this down by campaign?**

>[!ENDSHADEBOX]

#### 3. Keep investigating

**You:**

>[!BEGINSHADEBOX]

Let's break it down by campaign.

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

![Coworker Chat showing top campaigns ranked by their role as initiators or closers of customer journeys](assets/data-validation-aa-cja/coworker-attribution-response3.png)

There's a **Campaign Name** dimension. Here are your highest-involvement campaigns, comparing the revenue they start (first touch) against the revenue they close (last touch).

| Campaign | Starts (first touch) | Closes (last touch) | Role |
| --- | --- | --- | --- |
| brand_awareness_q3 | $412,000 | $103,000 | Initiator |
| email_winback | $214,000 | $88,000 | Initiator |
| holiday_flash_sale | $268,000 | $249,000 | All-rounder |
| retargeting_dynamic | $71,000 | $339,000 | Closer |
| branded_search_always_on | $84,000 | $498,000 | Closer / harvester |

**The pattern: some of your "worst" campaigns are actually your best starters**

* **brand_awareness_q3** and **email_winback** start far more revenue than they close. On a last-touch ROI report, these look like underperformers you might cut. In reality, they're filling the top of your funnel — the journeys other campaigns finish.
* **retargeting_dynamic** and **branded_search_always_on** are the opposite. They close a lot but start almost nothing. They're efficient closers, but they can only close demand that already exists. Branded search, in particular, is largely capturing people who were going to search for you by name anyway.
* **holiday_flash_sale** does both — it introduces new shoppers and closes them, which is why urgency-driven promotions often look strong under any model.

**What this tells you strategically**

The campaigns you'd cut first on a last-touch report — the awareness and win-back efforts — are the ones creating the demand your closers depend on. Judge initiators on the journeys they start, and closers on the journeys they finish.

**Recommended next steps:**

1. Protect the initiator campaigns even though their last-touch ROI looks weak — they're feeding the funnel.
1. Right-size the branded search spend — test whether trimming it changes total revenue, since much of that demand may convert anyway.
1. Adopt a balanced model — like linear or a position-based model — as your default reporting view, so no channel gets systematically over- or under-rewarded.

**Want me to save this as a project, or is this enough to take into your budget planning?**

>[!ENDSHADEBOX]

#### 4. Turn it into a decision

**You:**

>[!BEGINSHADEBOX]

So how should I allocate budget?

>[!ENDSHADEBOX]

**Coworker Chat response:**

>[!BEGINSHADEBOX]

Based on what the data shows, here's where I'd focus:

* **Stop judging upper-funnel channels on last touch alone.** Paid social and email start about 20% of your revenue each, but last touch credits them for less than half of that. Protect their budgets — they're creating the demand paid search closes.
* **Treat branded search as a harvester, not a driver.** It closes a lot but starts almost nothing. Test trimming it, since much of that demand may convert through other paths anyway.
* **Make a balanced model your default.** Reporting on linear or a position-based model instead of last touch will stop you from over-rewarding closers and under-funding the channels that start journeys.
* **Re-check after you rebalance.** Watch whether total revenue holds steady as you shift spend toward initiators — that's the signal your funnel is healthier, not just your last-touch report.

Want me to save this as a project so you can track it, or build a calculated metric that reports revenue on a balanced attribution model going forward?

>[!ENDSHADEBOX]

### What just happened

In four plain-language questions, Coworker helped us:

* Attribute revenue to marketing channels and flag that the default last-touch view tells only part of the story
* Compare attribution models and reveal that the "best" channel changes completely depending on how credit is counted
* Discover that paid social and email start far more revenue than they ever get credit for closing
* Identify which campaigns initiate journeys versus close them, and walk away with a budget direction: protect the initiators, right-size the harvesters, and report on a balanced model

-->
