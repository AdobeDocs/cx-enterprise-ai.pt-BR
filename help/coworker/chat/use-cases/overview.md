---
description: Procure casos de uso do Chat de colaborador e prompts de amostra, organizados por área entre insights de dados, públicos, jornadas e operações da plataforma.
title: Casos de uso do chat com colegas de trabalho
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: c5535d1d559f65b78ccc20a5b4c867f1bd2613e7
workflow-type: tm+mt
source-wordcount: 3344
ht-degree: 7%

---

# Casos de uso do chat do colaborador{#use-cases}

O Chat do Colaborador permite consultar, analisar e agir nos dados do [!DNL Experience Platform] usando linguagem natural em vez de navegar em várias interfaces do usuário ou gravar consultas manualmente. Esta página cataloga os casos de uso dos quais os profissionais mais dependem, organizados por área de trabalho: insights de dados, públicos, jornadas, elementos fundamentais e ferramentas de sandbox. Cada entrada inclui a habilidade que ele chama, os aplicativos com os quais ele funciona e avisos de amostra que você pode copiar, adaptar aos seus próprios dados e refinar através da conversa.

>[!NOTE]
>
>Em breve:
>
>Novos recursos do AEM Agentic por meio do CX Enterprise Co-worker, criado para ajudá-lo a fazer mais, de modo mais rápido.
>
>Todos os clientes qualificados terão acesso aos recursos de agentes da Adobe Experience Manager no Colaborador continuamente.
>
>Consulte também [IA no AEM - Visão geral dos recursos de agente no AEM](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/overview).

## Experiência da marca

### Produção de experiência - Casos de uso de sites

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Atualizar páginas do AEM | Execute ações como atualizar, remover, substituir ou adicionar elementos de conteúdo para manter as experiências precisas e atuais. As entradas podem ser linguagem natural ou anotações visuais como PDFs ou capturas de tela. | `aem-sites-pages-update` | Adobe Experience Manager (AEM) | Em &lt;URL> atualize o título para Olá, mundo<br><br>em &lt;URL> altere o botão &quot;Faça nosso questionário do café&quot; para uma versão mais envolvente<br><br>Atualize &lt;URL> com base no anexo<br><br>em &lt;URL> Quero adicionar uma nova seção de teaser ao final da página sobre uma promoção que estamos executando no mês de agosto, que é comprar uma máquina de café e obter 2 sacos de café gratuitamente. Encontre também imagens de amigos bebendo café e use-as no teaser |
| Atualizar o AEM em massa | Execute ações em massa em várias páginas ao mesmo tempo, como remover, substituir ou adicionar elementos de conteúdo para manter as experiências precisas e atuais. | `aem-sites-pages-bulkreplace` | Adobe Experience Manager (AEM) | em &lt;aem path>, atualize todas as páginas que contenham a cópia &quot;MyBarista\&quot; para &quot;BrewPass&quot; |
| Ir do Figma para o Fragmento de conteúdo visual | Importe designs diretamente do Figma para o Adobe Experience Manager usando a linguagem natural. A habilidade cria automaticamente o modelo de conteúdo, o fragmento de conteúdo, os ativos e o modelo de visualização necessários, permitindo que os usuários empresariais migrem do design para o conteúdo pronto para a Web em minutos sem configuração manual. | `aem-sites-visualcontentfragments-create` | Adobe Experience Manager (AEM) | Importar de &lt;Figma_URL> |

**Informações relacionadas**

* [Recursos de agente no AEM: Experiência da marca - Produção de experiência - Sites](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-sites)

### Produção de experiência - Casos de uso do Forms

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Criar formulário | Gerar um novo Formulário adaptável a partir de uma descrição em linguagem simples, um resumo anexado, uma imagem ou um PDF | `aem-forms-adaptiveform-create` | Adobe Experience Manager (AEM) | &quot;Criar um formulário de integração de funcionário&quot;<br><br>&quot;Criar um formulário usando o resumo anexado (imagem ou pdf)&quot;<br><br>&quot;Criar um formulário adaptável &lt;tipo de formulário>&quot; |
| Editar/atualizar formulário | Modificar um formulário existente — adicionar/editar campos, ajustar layout simples, configurar ações de envio ou aplicar alterações de um documento de diretrizes anexado | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) | &quot;Adicionar campo Nome do Meio abaixo do campo Nome&quot;<br><br>&quot;Coloque os campos Nome e Sobrenome em um layout de 2 colunas, 50/50&quot;<br><br>&quot;Configurar o formulário para enviar dados a um ponto de extremidade REST&quot;<br><br>&quot;Atualizar este formulário para corresponder ao documento de diretrizes anexado&quot;<br><br>&quot;Adicionar campo &lt;nome do campo> abaixo do campo &lt;campo existente>&quot; |
| Adicionar lógica de negócios | Criar regras simples, como mostrar ou ocultar um campo com base no valor de outro campo | `aem-forms-adaptiveform-edit` | Adobe Experience Manager (AEM) | &quot;Mostrar o campo Empresa somente quando o Tipo de Funcionário for Contratante&quot;<br><br>&quot;Mostrar o campo &lt;campo> somente quando &lt;outro campo> for &lt;valor>&quot; |
| Formulário incorporado | Coloque um formulário existente ou recém-criado em uma página do AEM Sites designada (compatível somente com páginas do Edge Delivery Services) | `aem-forms-adaptiveform-embed` | Adobe Experience Manager (AEM) | &quot;Incorporar este formulário na página inicial do nosso site&quot;<br><br>&quot;Incorporar este formulário no &lt;caminho da página>&quot; |

**Informações relacionadas**

* [Recursos de agente no AEM: Experiência da marca - Produção de experiência - Forms](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/experience-production/use-cases#use-cases-forms)

### Desenvolvimento

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Diagnosticar e corrigir falhas em pipelines do Cloud Manager | Investigue uma execução de pipeline com falha, identifique a causa raiz e gere uma correção (com uma comparação) para revisão | `cloud-manager-pipeline-troubleshooting` | Adobe Experience Manager (AEM) | &quot;Por que houve falha no pipeline de compilação?&quot;<br><br>&quot;Sugira uma correção para o pipeline de produção com falha&quot; |
| Gerenciar pipelines do Cloud Manager | Crie, execute e monitore pipelines do AEM Cloud Manager, incluindo logs, artefatos, variáveis e configurações | `cloud-manager-pipeline-management` | Adobe Experience Manager (AEM) | &quot;Listar pipelines para o programa 12345&quot;<br><br>&quot;Por que a execução do meu Pipeline de Desenvolvimento falhou?&quot; |
| Gerenciar ambientes do Cloud Manager | Criar, configurar e manter ambientes AEM Cloud Manager, inclusive RDEs, variáveis de ambiente, logs e backups | `cloud-manager-environment-management` | Adobe Experience Manager (AEM) | &quot;Listar meus ambientes para o programa 12345&quot;<br><br>&quot;Redefinir meu RDE&quot; |
| Gerenciar programas do Cloud Manager | Listar, inspecionar e excluir programas do AEM Cloud Manager, incluindo seus pipelines e ambientes | `cloud-manager-program-management` | Adobe Experience Manager (AEM) | &quot;Listar meus programas do Cloud Manager&quot;<br><br>&quot;Obter detalhes do programa 12345&quot; |
| Gerenciar agendamentos de atualização de versão do AEM | Configure o Quiet Hours diário e os Períodos de ausência de atualização para manutenção automatizada e visualize as janelas globais de Congelamento de código do Adobe | `cloud-manager-release-management` | Adobe Experience Manager (AEM) | &quot;Qual é a minha janela atual de Período de Silêncio?&quot;<br><br>&quot;Agende um período sem atualizações de 20 de dezembro a 2 de janeiro&quot; |

**Informações relacionadas**

* [Recursos de agente no AEM: experiência da marca - desenvolvimento](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/development/use-cases)

### Integração - Casos de uso do AEM Assets

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Integração guiada de ponta a ponta | Orquestra o ciclo de vida de integração completo, a seleção do repositório, a delegação à pasta, a tag, os metadados, a importação e a pesquisa de sub-habilidades, se você não souber a tarefa de integração específica necessária. | `aem-onboarding-workflow` | Adobe Experience Manager (AEM) Assets | &quot;Integre nossa equipe ao AEM Assets&quot;<br><br>&quot;Mostre-me a integração com o AEM DAM&quot; |
| Projetar e criar hierarquias de pastas | Recomenda e cria estruturas de pastas escaláveis no AEM Assets (em `/content/dam`) com base nas necessidades comerciais ou entradas de CSV. | `aem-folder-management` | Adobe Experience Manager (AEM) Assets | &quot;Recomendamos uma estrutura de pastas para nossos ativos de marketing de estilo de vida&quot;<br><br>&quot;Criar pastas com base neste arquivo CSV&quot; |
| Criar e criar tags | Cria e cria vocabulários de marcas controladas em `/content/cq:tags` — namespaces, marcas hierárquicas e operações de marcas em lote. | `aem-tag-taxonomy` | Adobe Experience Manager (AEM) Assets | &quot;Projetar uma taxonomia de marcas com namespaces para nossas categorias de produto&quot;<br><br>&quot;Importar marcas deste CSV&quot;<br><br>&quot;Criar essas marcas hierárquicas na AEM&quot; |
| Criar e atribuir formulários de metadados | Projeta e cria formulários de metadados personalizados, a interface de criação que os autores de conteúdo usam, de um CSV, tabela, documento de requisitos ou descrição e, opcionalmente, os atribui a pastas. | `aem-metadata-form` | Adobe Experience Manager (AEM) Assets | &quot;Criar um formulário de metadados a partir desta lista de campos&quot;<br><br>&quot;Atribuir este formulário à pasta `campaigns`&quot; |

**Informações relacionadas**

* [Recursos de agente no AEM: experiência da marca - integração](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-experience/onboarding/use-cases)

## Supervisor de conteúdo - Casos de uso do AEM Assets

### Descoberta de conteúdo

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Pesquisar por tema semântico | Encontre ativos por conceito, humor ou tema visual usando a correspondência semântica habilitada por IA. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | &quot;Encontre-me imagens matinais do estilo de vida do café&quot; |
| Pesquisar por metadados personalizados | Filtre ativos por campos de metadados personalizados (por exemplo, Mistura de café, Marca, Nível de assado). | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | &quot;Localizar ativos em que `Coffee Blend` é `Morning Muse`&quot;<br><br>&quot;Obter ativos cuja licença não expirou&quot;<br><br>&quot;Localizar ativos em mim cujo Nome da Campanha não está definido (a propriedade deve ser indexada para resultados apropriados).&quot; |
| Pesquisar por status de aprovação | Filtrar ativos com base no status de aprovação. Por exemplo, status aprovado, em revisão, rejeitado ou ausente. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | &quot;Mostrar todos os ativos aprovados na pasta `Campaign`&quot; |
| Pesquisar por pasta/caminho | Identifique ativos interpretando prompts de idioma natural que fazem referência a nomes de pastas no AEM. Você pode simplesmente mencionar a pasta no prompt, sem navegar manualmente pelo repositório, reduzindo significativamente o número de cliques necessários para localizar o conteúdo correto. | `aem-assets-discovery` | Adobe Experience Manager (AEM) Assets | &quot;Há algum svgs na pasta `WKND`&quot;?<br><br>&quot;Mostrar ativos modificados após 1º de novembro de 2025 na pasta `WKND`&quot; |

**Informações relacionadas**

* [Recursos de agente no AEM: Supervisor de conteúdo - Detecção de conteúdo](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/discovery/use-cases)

### Otimização de conteúdo

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Criação de representações de alta resolução e representações otimizadas por canal | Gerar novas representações de um ativo em uma resolução e um nível de qualidade especificados, facilitando a preparação de variações prontas para canais sem edição manual. Você também pode produzir representações personalizadas para requisitos específicos da plataforma, como o Instagram Stories, garantindo que os ativos atendam automaticamente às diretrizes de formato, proporção e qualidade. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | &quot;Criar uma representação de `2000px` como `JPEG` com `80% quality`&quot;<br><br>&quot;Criar uma representação para uma história do Instagram&quot; |
| Sobreposições de marca e geração composta | Aplique gráficos promocionais, sobreposições ou selos aos ativos existentes com posicionamento preciso, apoiando a criação rápida de compostos prontos para campanha. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | &quot;Sobreponha a imagem com `30%` gráficos de desconto sobre o banner promocional, colocando-a `100px` do centro&quot; |
| Aprimoramentos de imagem, ajustes de cor de fundo, transformações de orientação | Aplique melhorias visuais (nitidez da imagem), substitua cores de fundo e execute transformações de orientação. | `aem-assets-content-optimisation` | Adobe Experience Manager (AEM) Assets | &quot;Alterar a cor de plano de fundo de `PNG` para `#ff8932`&quot;<br><br>&quot;Nitidez da imagem&quot;<br><br>&quot;Espelhar a imagem horizontalmente&quot; |

**Informações relacionadas**

* [Recursos de agente no AEM: Supervisor de conteúdo - Otimização de conteúdo](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/content-advisor/content-optimization/use-cases)

## Governança da marca

| Caso de uso | Descrição | Habilidades | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Pesquisa de diretriz e segmento | Recuperar diretrizes detalhadas da marca, com escopo por segmento, mercado ou categoria | enterprise-context | Adobe Experience Manager (AEM) | &quot;Quais são as diretrizes de tom de voz desta marca?&quot;<br>&quot;Listar as categorias de declaração usadas no vertical de integridade&quot; |
| Avaliar o conteúdo em relação às diretrizes da marca | Avaliar uma página publicada/criada, bloco de texto ou imagem em relação às verificações de marca configuradas | aem-governance | Adobe Experience Manager (AEM) | &quot;Avaliar esta página de aterrissagem em relação às diretrizes do SecurBank&quot;<br>&quot;Esse slogan passa pelas nossas verificações de tom de voz?&quot; |
| Depurar permissões do AEM | Depurar/entender políticas de permissão, ACLs e regras de herança. | aem-governance | Adobe Experience Manager (AEM) | &quot;Por que o administrador principal pode gravar `/content/folder/us` em `https://author/` ?&quot;<br>&quot;Por que o autor de amostra não pode gravar em `/content/dam` em `https://author`&quot; |

**Informações relacionadas**

* [Recursos de agente no AEM: governança da marca](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/ai-in-aem/agentic-capabilities/brand-governance/use-cases)

## Insights de dados

| Caso de uso | Descrição | Habilidades | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| [Obter relatórios e métricas do CJA](data-insights/analytics-chat.md) | Consulta o CJA em tempo real para obter métricas, dimensões, segmentos e visualizações de dados | `cja` | Customer Journey Analytics (CJA) | &quot;Mostrar as exibições de página dos últimos 30 dias&quot; · &quot;Listar os principais segmentos na exibição de dados mestres&quot; |
| Análise comparativa | Comparar métricas entre canais, períodos ou segmentos lado a lado | `cja-root-cause-analysis`, `cja`, `dx-api`, `knowledge-graph` | Customer Journey Analytics (CJA) | &quot;Compare a receita por canal, mês a mês&quot; · &quot;Como está a conversão móvel vs desktop neste trimestre?&quot; |
| Desempenho da campanha | Meça o desempenho de campanhas, canais e propriedades da Web em um determinado período. | `cja`, `dx-api`, `knowledge-graph` | | &quot;Como nossas campanhas da Web do Acrobat se saíram no mês passado?&quot; |
| Análise do funnel | Analise os funis de conversão de várias etapas com devolução em cada estágio | `cja` | Customer Journey Analytics (CJA) | &quot;Mostre-me o funnel de check-out&quot; · &quot;Mostrar o funnel de conversão do PDP para a compra&quot; |
| Previsão | Projetar valores de métricas futuras com base em dados históricos do CJA | `cja` | Customer Journey Analytics (CJA) | &quot;Sessões de previsão para os próximos 30 dias&quot; · &quot;Estamos no caminho certo para atingir nossa meta de receita?&quot; |
| [Análise da causa principal](data-insights/root-cause-analysis.md) | Investigar por que uma métrica mudou: diagnosticar quedas, picos e anomalias | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | &quot;Por que as conversões caíram na semana passada?&quot; · &quot;O que causou o pico de receita em 15 de janeiro?&quot; |
| Resumos executivos e resumos de KPI | Produzir resumos de desempenho prontos para as partes interessadas, recomendações prescritivas e descrições do conjunto de slides | `cja-executive-summary`, `cja-bacom-anomaly-tracker-v2`, `cja-cno-weekly-pulse`, `cja-reporting`, `cja`, `dx-api` | Customer Journey Analytics (CJA) | &quot;Dê-me um resumo executivo do mês passado&quot; · &quot;Criar um esboço do conjunto de slides a partir dos dados deste trimestre&quot; |
| [Validação de dados do CJA considerada pelo AA](data-insights/data-validation-aa-cja.md) | Comparar, auditar e reconciliar dados entre o Adobe Analytics e o Customer Journey Analytics, especialmente ao atualizar do Adobe Analytics para o Customer Journey Analytics | `aa-cja-validation`, `cja`, `dx-api` | ADOBE ANALYTICS + CJA | &quot;Comparar meu conjunto de relatórios do AA com minha visualização de dados do CJA&quot; · &quot;Validar visualizações de página entre o AA e o CJA&quot; |
| Séries cronológicas operacionais e análise causal | Consultar e analisar dados históricos de séries temporais para públicos, conjuntos de dados e jornadas com atribuição causal | `operational-stats-causal-analysis` | Todos os aplicativos qualificados | &quot;Mostre-me as tendências de tamanho de público nos últimos 90 dias&quot; · &quot;Por que minha contagem de linhas do conjunto de dados aumentou em 3 de março?&quot; |
| Criar habilidades personalizadas do CJA | Transformar padrões analíticos em habilidades reutilizáveis e repetíveis que persistem entre as sessões | `cja-skill-creator` | Customer Journey Analytics (CJA) | &quot;Transformar esta análise semanal de receita em uma habilidade reutilizável&quot; · &quot;Salvar isso como uma habilidade para relatórios mensais do funnel&quot; |

## Públicos-alvo

| Caso de uso | Descrição | Habilidades | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| [Criar públicos-alvo da linguagem natural](audiences/create-audience-from-natural-language.md) | Orquestrar a criação passo a passo de público-alvo com a aprovação do usuário em cada fase | `audience-creation-flow` | Real-Time CDP (RTCDP) | &quot;Crie um público-alvo de usuários que compraram nos últimos 30 dias&quot; · &quot;Crie um segmento para membros de fidelidade de alto valor na Califórnia&quot; |
| Criar definições do PQL | Reunir definições de público-alvo de propriedades XDM, eventos comportamentais ou públicos-alvo existentes; oferecer suporte à agregação e janelas de tempo | `segment-definition-assembly` | Real-Time CDP (RTCDP) | &quot;Crie uma PQL para pessoas que visualizaram mais de 3 produtos, mas não compraram&quot; · &quot;Adicione uma janela de tempo de 7 dias à minha condição de evento&quot; |
| Pesquisar e encontrar públicos-alvo | Encontre públicos-alvo por ID, nome, pesquisa semântica; detecte duplicatas e analise a sobreposição | `audience-search` | Real-Time CDP (RTCDP) | &quot;Encontre todos os públicos-alvo de fidelidade&quot; · &quot;Há uma duplicata do meu segmento &quot;Compradores de Natal&quot;?&quot; |
| Estimar tamanho do público | Estimar o alcance do perfil para uma expressão do PQL usando a API de visualização do Adobe Experience Platform com sondagem | `audience-size-estimate` | Real-Time CDP (RTCDP) | &quot;Qual é o tamanho desse público?&quot; · &quot;Estimativa de alcance para essa expressão do PQL&quot; |
| Cascata de tamanho do público | Decompor uma PQL em subpredicados e mostrar como cada condição contribui para o tamanho final do público | `audience-size-waterfall` | Real-Time CDP (RTCDP) | &quot;Mostre-me a cascata para esta PQL&quot; · &quot;Detalhe como cada condição reduz o público-alvo&quot; |
| Descobrir campos XDM para direcionamento | Pesquisar campos por nome, descrição ou valor de dados; veja onde eles residem e onde já são usados | `field-discovery` | Real-Time CDP (RTCDP) | &quot;Quais campos posso usar para direcionar clientes do programa de fidelidade?&quot; · &quot;Encontrar campos relacionados ao histórico de compras&quot; |
| Publicar/salvar públicos | Manter as definições de público-alvo para o Serviço de segmentação da Experience Platform com convenções de nomenclatura e verificações de conformidade | `audience-publish` | Real-Time CDP (RTCDP) | &quot;Salvar como rascunho&quot; · &quot;Publicar o público-alvo com o nome &#39;Compradores de Vendas da primavera&#39;&quot; |

## Jornadas

| Caso de uso | Descrição | Habilidades | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| [Criar jornadas do idioma natural](journeys/create-journey-from-natural-language.md) | Orquestrar a criação de jornadas no AJO a partir de um prompt de texto ou de uma imagem/fluxograma carregado | `journey-create` | Adobe Journey Optimizer (AJO) | &quot;Criar uma jornada de boas-vindas que envia um email após a inscrição, aguarda 3 dias e envia um acompanhamento&quot; · &quot;Criar uma jornada a partir desta imagem de fluxograma carregada&quot; |
| Analisar conflitos de jornada | Detectar sobreposição de público, agendamento de colisões e problemas de desduplicação entre jornadas ativas | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | &quot;A jornada de abandono do carrinho entra em conflito com outras jornadas?&quot; · &quot;Verificar se há sobreposição de público-alvo entre minhas jornadas ativas&quot; |
| Analisar fallout de jornada | Identifique onde e por que os clientes caem durante uma jornada e detecte padrões de comportamento que levam à desvinculação | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | &quot;Onde as pessoas estão caindo na minha jornada de reengajamento?&quot; · &quot;Quais nós na jornada X têm o fallout mais alto?&quot; |
| Analisar erros de ação personalizados | Identifique quando as ações personalizadas estão falhando ou as taxas de erro sobem em uma jornada e diagnostique as causas básicas antes que as falhas evoluam para uma interrupção mais ampla | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | &quot;Por que as ações personalizadas estão falhando na minha jornada de Inscrição de Fidelidade?&quot; · &quot;Mostrar a taxa de erro para a ação personalizada ExternalPush na minha jornada de boas-vindas&quot;. |
| [Criar, editar e gerenciar desafios de fidelidade](journeys/create-loyalty-challenge.md) | Simplifique e acelere o gerenciamento do programa de fidelidade | `loyalty` | Adobe Journey Optimizer (AJO) | &quot;Crie um desafio incentivando os membros a experimentar uma nova bebida sazonal&quot; · &quot;Mostre-me os desafios de fidelidade com as taxas mais altas de devolução de membros.&quot; |

## Elementos fundamentais

| Caso de uso | Descrição | Habilidades | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Conhecimento e documentação do produto | Responda perguntas práticas, conceituais, de solução de problemas e de práticas recomendadas dos documentos oficiais do Adobe | `product-knowledge` | Todos os aplicativos qualificados | &quot;Como configurar um destino de transmissão?&quot; · &quot;Qual é a diferença entre a segmentação em lote e por transmissão?&quot; |
| Consultar entidades do Experience Platform/Journey Optimizer | Servir como ponto de entrada principal para dúvidas sobre entidades da plataforma; rotear para KG, descoberta de campo ou APIs, conforme necessário | `operational-insights` | Todos os aplicativos qualificados | &quot;Quantos conjuntos de dados eu tenho?&quot; · &quot;Mostrar todas as jornadas ativas&quot; · &quot;Listar meus destinos&quot; |
| Consultas do gráfico de conhecimento | Contagens agregadas, junções entre entidades, pesquisas de relacionamento e exploração de metadados por meio de consultas SQL únicas | `knowledge-graph` | Todos os aplicativos qualificados | &quot;Quais públicos-alvo usam esse conjunto de dados?&quot; · &quot;Mostre-me as relações entre esquemas e conjuntos de dados&quot; |
| Operações de API do Experience Platform / Journey Optimizer / Customer Journey Analytics | Fornecer um gateway de API direto para mutações, verificações de estado em tempo real e tipos de entidade que não estão no Gráfico de conhecimento | `cxo-api` | Todos os aplicativos qualificados | &quot;Excluir conjunto de dados X&quot; · &quot;Verificar o status do meu trabalho de assimilação em lote&quot; |
| Resolução e vinculação da entidade | Use a pesquisa semântica e léxica para resolver menções de entidade a entidades reais do Experience Platform e descobrir campos XDM | `entity-linking` | Adobe Experience Platform | &quot;Resolver &#39;Compradores de Férias&#39; para um público real&quot; · &quot;Encontre-me campos relacionados ao histórico de compras&quot; |
| Gerenciar habilidades personalizadas | Salvar, modificar ou excluir habilidades reutilizáveis de propriedade do usuário que persistem entre as sessões | `manage-skill` | Todos os aplicativos qualificados | &quot;Salvar esse fluxo de trabalho como uma habilidade&quot; · &quot;Excluir minha habilidade semanal de relatório&quot; · &quot;Transformar isso em uma habilidade reutilizável&quot; |
| Monitorar a capacidade de transmissão e as violações | Verificar o uso atual e histórico da transmissão, a capacidade e o status de violação em sandboxes | `observability-streaming-capacity`, `observability-streaming-usage`, `observability-capacity-breaches` | Adobe Experience Platform | &quot;Qual é minha capacidade de transmissão atual na minha sandbox atual?&quot; · &quot;Minha sandbox atual está excedendo os limites de capacidade na última semana?&quot; |
| [Exibir resultados da avaliação de verificação de integridade](https://experienceleague.adobe.com/pt-br/docs/experience-platform/run-and-operate/health-checks/overview) | Visualize a avaliação de verificação de integridade mais recente para sua sandbox, examine uma verificação de falha e veja as entidades afetadas | `rao-view-latest-health-checks-assessment` | Adobe Experience Platform | &quot;O que há de errado com minha sandbox?&quot; · &quot;Conte-me sobre minha última avaliação de verificação de integridade&quot; · &quot;Quais são os problemas da verificação de descrição do namespace personalizado?&quot; |
| Corrigir problemas de verificação de integridade | Corrija problemas de namespace de identidade, política de mesclagem e esquema sinalizados diretamente do chat, com sua aprovação antes que qualquer alteração seja feita | `rao-remediate-identity-namespace-description`, `rao-remediate-merge-policy-duplicate-name`, `rao-remediate-missing-audit-field-group`, `rao-remediate-default-merge-policy-naming` | Adobe Experience Platform | &quot;Corrigir descrições de namespace de identidade&quot; · &quot;Corrigir nomes de política de mesclagem duplicados&quot; · &quot;Corrigir esquemas que não têm o grupo de campos de auditoria&quot; · &quot;Corrigir nomenclatura de política de mesclagem padrão&quot; |

## Ferramentas de sandbox

| Caso de uso | Descrição | Habilidades | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| [Mover objetos entre sandboxes](/help/agents/sandbox-tooling.md) | Migrar esquemas, públicos-alvo e outras configurações de objeto facilmente entre sandboxes, com dependências resolvidas automaticamente | `sandbox-tooling-workflow` | Adobe Experience Platform | &quot;Mover Platina de Membros de Fidelidade Luma do esquema da sandbox atual para a sandbox de produção&quot; · &quot;Promover o público-alvo dos Membros de Fidelidade Gold dos EUA para o estágio&quot; |

## Alertas do cliente

| Caso de uso | Descrição | Habilidades | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Gerenciar assinaturas de alerta | Exiba e gerencie assinaturas de alerta por meio de conversas em idioma natural. | `alerts-subscribe` | Adobe Experience Platform | &quot;Em quais alertas estou inscrito?&quot;<br><br>&quot;Assinar este alerta.&quot;<br><br>&quot;Remover minha inscrição neste alerta.&quot; |
| Revisar atividade de alerta | Revise o status do alerta atual e a atividade de alerta histórica para um período de tempo especificado. | `alerts-list` | Adobe Experience Platform | &quot;O que aconteceu nas últimas 24 horas?&quot;<br><br>&quot;Quais alertas foram disparados nas últimas 24 horas?&quot;<br><br>&quot;Mostrar alertas ativos dos últimos sete dias.&quot; |
| Identificar padrões de alerta recorrentes | Analise o histórico de alertas para identificar tipos de alertas acionados com frequência e tendências operacionais. | `alerts-list` | Adobe Experience Platform | &quot;Mostrar os 3 principais tipos de alertas acionados.&quot;<br><br>&quot;Quais tipos de alertas ocorreram com mais frequência este mês?&quot;<br><br>&quot;Quais padrões de alertas você vê nos últimos sete dias?&quot; |
| Concentre-se em questões de alta prioridade | Filtre a atividade de alerta por gravidade para priorizar os esforços de investigação. | `alerts-list` | Adobe Experience Platform | &quot;Mostrar apenas alertas de alta severidade.&quot;<br><br>&quot;Quais alertas críticos foram disparados esta semana?&quot;<br><br>&quot;Mostrar alertas críticos dos últimos 30 dias.&quot; |
| Entender o raio de impacto dos alertas | Identifique os objetos mais afetados pelos alertas e determine onde a investigação deve começar. | `alerts-list` | Adobe Experience Platform | &quot;Quais são os 5 principais objetos afetados?&quot;<br><br>&quot;Quais objetos estão associados aos alertas de severidade mais alta?&quot; |
| Conectar tipos de alerta a objetos afetados | Analisar relações entre tipos de alertas e recursos afetados. | `alerts-list` | Adobe Experience Platform | &quot;Quais tipos de alerta afetaram este conjunto de dados com mais frequência?&quot;<br><br>&quot;Mostrar a relação entre os tipos de alerta e os objetos afetados.&quot;<br><br>&quot;Qual tipo de alerta afetou o objeto afetado com mais frequência?&quot; |
| Foco em Meus Alertas | Analise os alertas nos quais você se inscreve e que são responsáveis pelo monitoramento. | `alerts-list` | Adobe Experience Platform | &quot;Mostrar os alertas de alta severidade que eu assino.&quot;<br><br>&quot;Quais alertas dos Meus Alertas foram disparados esta semana?&quot;<br><br>&quot;Algum dos meus alertas que assinei requer atenção?&quot; |
