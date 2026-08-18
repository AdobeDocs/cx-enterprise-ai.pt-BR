---
description: Saiba como o Coworker Campaigns anexa e preserva automaticamente os metadados C2PA (Content Credentials) em imagens geradas e editadas por IA, nenhuma ação necessária.
title: Metadados do C2PA em campanhas de colegas de trabalho
hide: true
source-git-commit: 785b5d106cb029d68506c90385786cbdae164991
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 2%

---

# Metadados do C2PA em campanhas de colegas de trabalho {#overview}

Novas leis estão surgindo em torno da transparência generativa da IA, e a Adobe está trabalhando para atender aos requisitos aplicáveis em todas as jurisdições. [Metadados C2PA](https://c2pa.org/) (também conhecidos como Content Credentials) são a ferramenta de origem que a Adobe usa para atender aos requisitos dessas leis.

Os metadados C2PA são metadados duráveis e invisíveis que registram como um conteúdo foi criado ou editado. Quando você gera ou edita uma imagem com ferramentas de IA gerativas em Campanhas do colega de trabalho, os metadados do C2PA são anexados automaticamente a essa imagem. Nenhuma ação é necessária da sua parte.

## Ações que anexam metadados C2PA {#cc-workflows}

A tabela a seguir resume quando os metadados C2PA são anexados, com base na ação de imagem executada na geração de imagem em Campanhas do colaborador.

| Ação | Descrição | Metadados C2PA anexados? | Exemplo de caso de uso |
| --- | --- | --- | --- |
| **Gerar uma imagem** | Crie uma nova imagem a partir de um prompt de texto ou de uma imagem de referência, ou gere uma imagem semelhante a partir de uma imagem existente. | Sempre. A imagem é gerada por IA gerativa, de modo que sempre transporta metadados C2PA novos. | Uma imagem de banner para uma campanha de email é gerada a partir de um prompt de texto que descreve o visual desejado. |
| **Cortar uma imagem** (recorte central ou inteligente) | Ajustar uma imagem às dimensões solicitadas | Somente se a imagem de origem já tiver metadados C2PA. O corte recria os pixels da imagem, o que normalmente apagaria esses metadados do C2PA. Portanto, a geração de imagens nas Campanhas do colaborador os lê da imagem de origem antes do corte, e depois os recria e anexa novamente ao resultado cortado. O corte em si não adiciona uma nova ação de IA gerativa; ele preserva a existente. | Uma imagem de banner gerada é cortada para caber em uma página da Web: os metadados C2PA são preservados por meio do corte. <br> Uma foto do stock carregada usada como um plano de fundo de notificação por push é cortada para caber na tela: como a foto do stock não carrega nenhuma ação de IA gerativa, nenhum metadado C2PA é criado. |
| **Adicionar uma sobreposição de texto** | Renderizar texto gerado sobre uma imagem de plano de fundo | Somente se a imagem de fundo já tiver metadados C2PA. A renderização da sobreposição produz uma nova imagem do plano de fundo mais o texto, o que normalmente apagaria esses metadados C2PA. Portanto, a geração de imagens em Campanhas do colaborador lê previamente a imagem do plano de fundo, então reconstrói e reanexa ao resultado. A etapa de sobreposição não adiciona uma nova ação de IA gerativa. | Um título promocional é renderizado como uma sobreposição de texto em uma imagem de fundo gerada para uma landing page: os metadados C2PA da imagem de fundo são preservados. |
| **Sobrepor imagens** | Compor duas ou mais imagens | Se qualquer uma das imagens de origem tiver metadados C2PA, a imagem combinada carregará tudo isso, mesclado em um único conjunto de metadados C2PA. A composição produz uma nova imagem a partir das fontes, o que normalmente apagaria esses metadados C2PA, de modo que a geração de imagens em Campanhas de colegas de trabalho lê cada uma antes da composição e, em seguida, cria um registro de metadados C2PA combinado listando cada fonte que contribuiu para uma ação de IA geradora. | Uma imagem de produto gerada é composta por um plano de fundo gerado para um cabeçalho de email: o resultado carrega metadados C2PA que refletem ambas as fontes de IA geradoras. <br> Duas fotos de marca carregadas são compostas em uma única colagem: como nenhuma fonte carrega uma ação de IA gerativa, nenhum metadado C2PA é criado. |

## Tipos de conteúdo e seu escopo {#cc-content-types}

* **Imagens**: Cobertas. Os metadados C2PA são anexados quando as imagens são geradas com IA gerativa e preservados por meio de operações de recorte, sobreposição de texto e sobreposição de imagem executadas pela geração de imagens em campanhas de colegas de trabalho.
* **Texto**: não aplicável. Saídas somente texto da geração de imagem em campanhas de colaboração, como geração de cópia, tradução e sugestões de alinhamento de marca, não exigem metadados C2PA.

## O que acontece quando o conteúdo se move {#cc-content-moves}

As Campanhas de colegas de trabalho preservam o Content Credentials associado aos ativos de imagem compatíveis. Se uma imagem contiver Content Credentials quando importada para Campanhas do colega de trabalho, essas credenciais serão mantidas quando o ativo for usado no conteúdo da campanha gerado e nas experiências de email de saída. [Saiba mais sobre metadados C2PA](https://helpx.adobe.com/firefly/using/content-credentials.html){target="_blank"}.

<!-- Some ways of bringing images into your content, such as extracting an image from a PDF or from an embedded (base64) source, may not preserve the original C2PA metadata. In these cases, no C2PA metadata can be read from the source, and none is created for the result. -->

>[!MORELIKETHIS]
>
>[Diretrizes de usuário da IA gerada da Adobe Experience Cloud](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html?lang=pt-BR){target="_blank"}
