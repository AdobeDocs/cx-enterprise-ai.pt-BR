---
description: Procure casos de uso do Chat de colaborador e prompts de amostra, organizados por área entre insights de dados, públicos, jornadas e operações da plataforma.
title: Casos de uso
source-git-commit: ad1e50aa70822ba764b417d2559417c9a235422e
workflow-type: tm+mt
source-wordcount: '1232'
ht-degree: 3%

---

# Casos de uso {#use-cases}

Abaixo estão casos de uso e prompts de amostra que os profissionais estão usando no Adobe Co-worker Chat, organizado por área de trabalho. Cada prompt é criado para ser copiado, adaptado com seus próprios dados e contexto e refinado através da conversa.

## Insights de dados

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Obter relatórios e métricas do CJA | Consulta o CJA em tempo real para obter métricas, dimensões, segmentos e visualizações de dados | `cja` | Customer Journey Analytics (CJA) | &quot;Mostrar as exibições de página dos últimos 30 dias&quot; · &quot;Listar os principais segmentos na exibição de dados mestres&quot; |
| Análise comparativa | Comparar métricas entre canais, períodos ou segmentos lado a lado | `cja` | Customer Journey Analytics (CJA) | &quot;Compare a receita por canal, mês a mês&quot; · &quot;Como está a conversão móvel vs desktop neste trimestre?&quot; |
| Análise do funnel | Analise os funis de conversão de várias etapas com devolução em cada estágio | `cja` | Customer Journey Analytics (CJA) | &quot;Mostre-me o funnel de check-out&quot; · &quot;Mostrar o funnel de conversão do PDP para a compra&quot; |
| Previsão | Projetar valores de métricas futuras com base em dados históricos do CJA | `cja` | Customer Journey Analytics (CJA) | &quot;Sessões de previsão para os próximos 30 dias&quot; · &quot;Estamos no caminho certo para atingir nossa meta de receita?&quot; |
| Análise da causa principal | Investigar por que uma métrica mudou: diagnosticar quedas, picos e anomalias | `cja-root-cause-analysis` | Customer Journey Analytics (CJA) | &quot;Por que as conversões caíram na semana passada?&quot; · &quot;O que causou o pico de receita em 15 de janeiro?&quot; |
| Resumos executivos e resumos de KPI | Produzir resumos de desempenho prontos para as partes interessadas, recomendações prescritivas e descrições do conjunto de slides | `cja-executive-summary` | Customer Journey Analytics (CJA) | &quot;Dê-me um resumo executivo do mês passado&quot; · &quot;Criar um esboço do conjunto de slides a partir dos dados deste trimestre&quot; |
| Validação de dados do CJA AA | Comparar, auditar e reconciliar dados entre o Adobe Analytics e o Customer Journey Analytics | `aa-cja-validation` | ADOBE ANALYTICS + CJA | &quot;Comparar meu conjunto de relatórios do AA com minha visualização de dados do CJA&quot; · &quot;Validar visualizações de página entre o AA e o CJA&quot; |
| Séries cronológicas operacionais e análise causal | Consultar e analisar dados históricos de séries temporais para públicos, conjuntos de dados e jornadas com atribuição causal | `operational-stats-causal-analysis` | Todos os aplicativos qualificados | &quot;Mostre-me as tendências de tamanho de público nos últimos 90 dias&quot; · &quot;Por que minha contagem de linhas do conjunto de dados aumentou em 3 de março?&quot; |
| Criar habilidades personalizadas do CJA | Transformar padrões analíticos em habilidades reutilizáveis e repetíveis que persistem entre as sessões | `cja-skill-creator` | Customer Journey Analytics (CJA) | &quot;Transformar esta análise semanal de receita em uma habilidade reutilizável&quot; · &quot;Salvar isso como uma habilidade para relatórios mensais do funnel&quot; |

## Públicos-alvo

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Criar públicos-alvo a partir da linguagem natural | Orquestrar a criação passo a passo de público-alvo com a aprovação do usuário em cada fase | `audience-creation-flow` | Real-Time CDP (RTCDP) | &quot;Crie um público-alvo de usuários que compraram nos últimos 30 dias&quot; · &quot;Crie um segmento para membros de fidelidade de alto valor na Califórnia&quot; |
| Criar definições do PQL | Reunir definições de público-alvo de propriedades XDM, eventos comportamentais ou públicos-alvo existentes; oferecer suporte à agregação e janelas de tempo | `segment-definition-assembly` | Real-Time CDP (RTCDP) | &quot;Crie uma PQL para pessoas que visualizaram mais de 3 produtos, mas não compraram&quot; · &quot;Adicione uma janela de tempo de 7 dias à minha condição de evento&quot; |
| Pesquisar e encontrar públicos-alvo | Encontre públicos-alvo por ID, nome, pesquisa semântica; detecte duplicatas e analise a sobreposição | `audience-search` | Real-Time CDP (RTCDP) | &quot;Encontre todos os públicos-alvo de fidelidade&quot; · &quot;Há uma duplicata do meu segmento &quot;Compradores de Natal&quot;?&quot; |
| Estimar tamanho do público | Estimar o alcance do perfil para uma expressão do PQL usando a API de visualização do AEP com sondagem | `audience-size-estimate` | Real-Time CDP (RTCDP) | &quot;Qual é o tamanho desse público?&quot; · &quot;Estimativa de alcance para essa expressão do PQL&quot; |
| Cascata de tamanho do público | Decompor uma PQL em subpredicados e mostrar como cada condição contribui para o tamanho final do público | `audience-size-waterfall` | Real-Time CDP (RTCDP) | &quot;Mostre-me a cascata para esta PQL&quot; · &quot;Detalhe como cada condição reduz o público-alvo&quot; |
| Descobrir campos XDM para direcionamento | Pesquisar campos por nome, descrição ou valor de dados; veja onde eles residem e onde já são usados | `field-discovery` | Real-Time CDP (RTCDP) | &quot;Quais campos posso usar para direcionar clientes do programa de fidelidade?&quot; · &quot;Encontrar campos relacionados ao histórico de compras&quot; |
| Publicar/salvar públicos | Manter as definições de público-alvo para o Serviço de segmentação da AEP com convenções de nomenclatura e verificações de conformidade | `audience-publish` | Real-Time CDP (RTCDP) | &quot;Salvar como rascunho&quot; · &quot;Publicar o público-alvo com o nome &#39;Compradores de Vendas da primavera&#39;&quot; |

## Jornadas

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Criar jornadas a partir do idioma natural | Orquestrar a criação de jornadas no AJO a partir de um prompt de texto ou de uma imagem/fluxograma carregado | `journey-create` | Adobe Journey Optimizer (AJO) | &quot;Criar uma jornada de boas-vindas que envia um email após a inscrição, aguarda 3 dias e envia um acompanhamento&quot; · &quot;Criar uma jornada a partir desta imagem de fluxograma carregada&quot; |
| Analisar conflitos de jornada | Detectar sobreposição de público, agendamento de colisões e problemas de desduplicação entre jornadas ativas | `journey-analyze-conflict` | Adobe Journey Optimizer (AJO) | &quot;A jornada de abandono do carrinho entra em conflito com outras jornadas?&quot; · &quot;Verificar se há sobreposição de público-alvo entre minhas jornadas ativas&quot; |
| Analisar fallout de jornada | Identifique onde e por que os clientes caem durante uma jornada e detecte padrões de comportamento que levam à desvinculação | `journey-analyze-fallout` | Adobe Journey Optimizer (AJO) | &quot;Onde as pessoas estão caindo na minha jornada de reengajamento?&quot; · &quot;Quais nós na jornada X têm o fallout mais alto?&quot; |
| Analisar erros de ação personalizados | Identifique quando as ações personalizadas estão falhando ou as taxas de erro sobem em uma jornada e diagnostique as causas básicas antes que as falhas evoluam para uma interrupção mais ampla | `journey-analyze-custom-action` | Adobe Journey Optimizer (AJO) | &quot;Por que as ações personalizadas estão falhando na minha jornada de Inscrição de Fidelidade?&quot; · &quot;Mostrar a taxa de erro para a ação personalizada ExternalPush na minha jornada de boas-vindas&quot;. |

## Elementos fundamentais

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Conhecimento e documentação do produto | Responda perguntas práticas, conceituais, de solução de problemas e de práticas recomendadas dos documentos oficiais do Adobe | `product-knowledge` | Todos os aplicativos qualificados | &quot;Como configurar um destino de transmissão?&quot; · &quot;Qual é a diferença entre a segmentação em lote e por transmissão?&quot; |
| Consultar entidades do AEP/AJO | Servir como ponto de entrada principal para dúvidas sobre entidades da plataforma; rotear para KG, descoberta de campo ou APIs, conforme necessário | `operational-insights` | Todos os aplicativos qualificados | &quot;Quantos conjuntos de dados eu tenho?&quot; · &quot;Mostrar todas as jornadas ativas&quot; · &quot;Listar meus destinos&quot; |
| Consultas do gráfico de conhecimento | Contagens agregadas, junções entre entidades, pesquisas de relacionamento e exploração de metadados por meio de consultas SQL únicas | `knowledge-graph` | Todos os aplicativos qualificados | &quot;Quais públicos-alvo usam esse conjunto de dados?&quot; · &quot;Mostre-me as relações entre esquemas e conjuntos de dados&quot; |
| Operações de API do AEP/AJO/CJA | Fornecer um gateway de API direto para mutações, verificações de estado em tempo real e tipos de entidade que não estão no Gráfico de conhecimento | `cxo-api` | Todos os aplicativos qualificados | &quot;Excluir conjunto de dados X&quot; · &quot;Verificar o status do meu trabalho de assimilação em lote&quot; |
| Resolução e vinculação da entidade | Use a pesquisa semântica e léxica para resolver menções de entidade a entidades reais do AEP e descobrir campos XDM | `entity-linking` | Adobe Experience Platform (AEP) | &quot;Resolver &#39;Compradores de Férias&#39; para um público real&quot; · &quot;Encontre-me campos relacionados ao histórico de compras&quot; |
| Criar contexto pessoal | Gerar um perfil de usuário personalizado a partir dos logs de atividades do AEP, CJA e/ou Workfront | `build-my-context` | Todos os aplicativos qualificados | &quot;Criar meu contexto a partir da atividade do AEP e do CJA&quot; · &quot;Quem sou eu nesta organização?&quot; |
| Contexto da organização de destilação | Extrair conhecimento de toda a organização de um documento para o wiki compartilhado de contexto da organização | `distill-org-context` | Todos os aplicativos qualificados | &quot;Destilar este documento no wiki da organização&quot; · &quot;Adicionar este arquivo ao contexto da organização&quot; |
| Contexto de usuário do Distil | Extrair o contexto de trabalho pessoal de um documento para seu wiki de contexto de usuário | `distill-user-context` | Todos os aplicativos qualificados | &quot;Adicionar este arquivo ao meu contexto de usuário&quot; · &quot;Extrair meu contexto de trabalho deste documento&quot; |
| Gerenciar habilidades personalizadas | Salvar, modificar ou excluir habilidades reutilizáveis de propriedade do usuário que persistem entre as sessões | `manage-skill` | Todos os aplicativos qualificados | &quot;Salvar esse fluxo de trabalho como uma habilidade&quot; · &quot;Excluir minha habilidade semanal de relatório&quot; · &quot;Transformar isso em uma habilidade reutilizável&quot; |

## Ferramentas de sandbox

| Caso de uso | Descrição | Habilidade(s) | Aplicativo | Exemplos de Prompts |
| --- | --- | --- | --- | --- |
| Mover metadados de objetos em sandboxes | Migrar esquemas, públicos-alvo e outras configurações de objeto facilmente entre sandboxes, com dependências resolvidas automaticamente | `sandbox-tooling-workflow` | Adobe Experience Platform (AEP) | &quot;Mover Platina de Membros de Fidelidade Luma do esquema da sandbox atual para a sandbox de produção&quot; · &quot;Promover o público-alvo dos Membros de Fidelidade Gold dos EUA para o estágio&quot; |
