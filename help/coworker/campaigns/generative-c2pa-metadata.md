---
description: Saiba como o Coworker Campaigns anexa e preserva automaticamente os metadados C2PA (Content Credentials) em imagens geradas e editadas por IA, nenhuma ação necessária.
title: Metadados do C2PA em campanhas de colegas de trabalho
hide: true
source-git-commit: cf96ff8bdb16708c6726854b92d0c2d6e681817a
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 5%

---

# Metadados do C2PA em campanhas de colegas de trabalho {#overview}

Novas leis estão surgindo em torno da transparência generativa da IA, e a Adobe está trabalhando para atender aos requisitos aplicáveis em todas as jurisdições. [Metadados C2PA](https://c2pa.org/) (também conhecidos como Content Credentials) são a ferramenta de origem que a Adobe usa para atender aos requisitos dessas leis.

Os metadados C2PA são metadados duráveis e invisíveis que registram como um conteúdo foi criado ou editado. Quando você gera ou edita uma imagem com ferramentas de IA gerativas em Campanhas do colega de trabalho, os metadados do C2PA são anexados automaticamente a essa imagem. Nenhuma ação é necessária da sua parte.

## Ações que anexam metadados C2PA {#cc-workflows}

A tabela a seguir resume quando os metadados C2PA são anexados, com base na ação de imagem executada na geração de imagem em Campanhas do colaborador.

| Ação | Descrição | Metadados C2PA anexados? | Exemplo de caso de uso |
| --- | --- | --- | --- |
| **Gerar uma imagem** | Crie uma nova imagem a partir de um prompt de texto ou de uma imagem de referência, ou gere uma imagem semelhante a partir de uma imagem existente. | Sempre. A imagem é gerada por IA gerativa, de modo que sempre transporta metadados C2PA novos. | Uma imagem de banner para uma campanha de email é gerada a partir de um prompt de texto que descreve o visual desejado. |

## Tipos de conteúdo e seu escopo {#cc-content-types}

* **Imagens**: Cobertas. Os metadados C2PA são anexados quando as imagens são geradas com IA gerativa e preservados por meio de operações de recorte, sobreposição de texto e sobreposição de imagem executadas pela geração de imagens em campanhas de colegas de trabalho.
* **Texto**: não aplicável. Saídas somente texto da geração de imagem em campanhas de colaboração, como geração de cópia, tradução e sugestões de alinhamento de marca, não exigem metadados C2PA.

## O que acontece quando o conteúdo se move {#cc-content-moves}

As Campanhas de colegas de trabalho preservam o Content Credentials associado aos ativos de imagem compatíveis. Se uma imagem contiver Content Credentials quando importada para Campanhas do colega de trabalho, essas credenciais serão mantidas quando o ativo for usado no conteúdo da campanha gerado e nas experiências de email de saída. [Saiba mais sobre metadados C2PA](https://helpx.adobe.com/br/firefly/using/content-credentials.html){target="_blank"}.

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

>[!MORELIKETHIS]
>
>[Diretrizes de usuário da IA gerada da Adobe Experience Cloud](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html?lang=pt-BR){target="_blank"}
