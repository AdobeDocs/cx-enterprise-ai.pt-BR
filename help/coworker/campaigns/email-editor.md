---
description: descrição.
title: Entender o editor de email
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 707
ht-degree: 0%

---

# Entender o editor de email {#email-editor}

O editor de email permite refinar um email gerado por IA diretamente no quadro da campanha. Edite a linha de assunto e o pré-cabeçalho, formate o texto e as imagens em linha ou troque em um modelo diferente. <!-- It's an inline editor over the email's actual HTML, not a drag-and-drop block builder. -->

>[!PREREQUISITES]
>
>Crie uma campanha com um email gerado.

## O que este recurso faz

Clicar em um cartão de email no quadro de campanha abre o editor de email como um painel lateral. A partir daí, o usuário pode editar o assunto e o pré-cabeçalho (com alternativas sugeridas pela IA), clicar no corpo do email para selecionar e formatar texto ou imagens, alternar entre variantes geradas pela IA, trocar o modelo do HTML, verificar a compatibilidade do cliente de email e enviar um email de teste para sua própria caixa de entrada. As alterações são salvas automaticamente e as versões anteriores podem ser revisadas e restauradas.

### Comportamentos principais

- Clicar em qualquer texto ou imagem no corpo do email seleciona-o e revela uma barra de ferramentas de formatação flutuante.
- Opções de formatação de texto: Negrito, Itálico, Sublinhado, fonte e tamanho da fonte.
- Opções de imagem: Substituir, Excluir, Vincular, Editar com Expresso, Gerar imagem (AI), Fazer upload do computador.
- Os uploads de imagem são limitados a 10 MB; imagens com mais ou menos 3 MB são compactadas automaticamente, com uma nota de qualidade recomendando imagens com menos de 3 MB.
- Os campos de assunto e pré-cabeçalho têm uma opção &quot;Sugestões inteligentes&quot; para alternativas geradas por IA.
- Altera o salvamento automático (no desfoque e logo após as ações de formatação) — um indicador de status mostra Alterações não salvas, Salvando..., Salvas, Salvas automaticamente ou Não é possível salvar (com uma opção Repetir).
- Desfazer/refazer está disponível para a sessão de edição atual.
- As versões salvas anteriores podem ser visualizadas e restauradas a partir de um painel de histórico de versões.
- Se houver várias variantes geradas por IA, o usuário poderá alternar entre elas em um painel de miniaturas.
- O modelo HTML do email pode ser trocado usando a opção &quot;Alternar modelo HTML&quot;.
- &quot;Enviar email de teste&quot; envia uma visualização real para a caixa de entrada do próprio usuário usando dados de amostra; não afeta os relatórios da campanha.
- Uma verificação de compatibilidade de cliente de email está disponível em alguns ambientes, que abrangem Gmail, Outlook, Apple Mail, Yahoo Mail, Samsung Email e Thunderbird. [PRECISA DE ENTRADA — isto está atrás de um sinalizador de recurso; confirme se ele está habilitado para o público-alvo antes de documentá-lo como geralmente disponível]

## Como acessar o

1. Abra a campanha desejada e clique em Open editor no cartão de email.

CAPTURA DE TELA

1. Edite os campos **Assunto** e **Pré-cabeçalho** diretamente ou clique em **Sugestões inteligentes** ao lado de qualquer uma das alternativas geradas pela IA.
1. Clique no corpo do email para selecionar um bloco de texto ou uma imagem e, em seguida, use a barra de ferramentas flutuante exibida para formatar o texto ou gerenciar a imagem.
1. Use **Alternar Modelo do HTML** para substituir o corpo do email por um modelo diferente.
1. Use **Enviar email de teste**, insira um endereço de destinatário e clique em **Enviar** para enviar uma visualização ao vivo por email para esse endereço.
1. Use o ícone de histórico da versão para visualizar e restaurar uma versão salva anteriormente.
1. Salvar alterações automaticamente — nenhuma etapa de salvamento manual é necessária.

### Campos/parâmetros de entrada

| Campo | Descrição | Obrigatório? |
| --- | --- | --- |
| Assunto | A linha de assunto do email | Não (pode ser deixado em branco; não está sendo aplicado no momento) |
| Pré-cabeçalho | O texto de visualização mostrado ao lado do assunto em uma caixa de entrada | Não |
| Endereço de email do destinatário | Para onde enviar um email de teste | Sim, para Enviar email de teste |

## Chamadas de interface do usuário

> **Nota técnica do escritor**: Capturas de tela necessárias para o seguinte:

- [ ] O painel lateral do editor de email (campos de assunto/pré-cabeçalho mais corpo do email)
- [ ] A barra de ferramentas flutuante para seleção de texto
- [ ] A barra de ferramentas flutuante para seleção de imagem
- [ ] O painel de miniaturas da variante de IA
- [ ] O painel do histórico de versões
- [ ] A caixa de diálogo &quot;Alternar modelo do HTML&quot;
- [ ] A caixa de diálogo Enviar email de teste
- [ ] O verificador de compatibilidade de email-cliente (se habilitado no ambiente de destino)

## O que este recurso não faz

- Não é um construtor de blocos de arrastar e soltar — não há biblioteca de blocos e os blocos de conteúdo não podem ser adicionados, removidos ou reordenados; a edição acontece diretamente no HTML de email existente.
- No momento, não há suporte para a inserção de tags de personalização/mesclagem.
- Ele não fornece um campo de texto alternativo para imagens.
- Ele não impõe uma linha de assunto, pré-cabeçalho ou outras verificações de nível de conteúdo antes que um email seja considerado &quot;pronto&quot;. As únicas verificações de pré-lançamento são no nível da campanha (configuração de envio, um email de teste enviado, um público real), não verifica o conteúdo do email em si.
- A alternância de visualização de desktop/dispositivo móvel não está disponível na visualização padrão de edição de email da campanha. [PRECISA DE ENTRADA para confirmar o escopo]
- [NEEDS INPUT — para confirmar com o engenheiro: se o editor se torna totalmente somente leitura (não apenas o campo do remetente) depois que uma campanha é ativada/iniciada.]
