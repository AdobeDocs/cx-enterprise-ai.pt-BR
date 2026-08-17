---
description: insira uma descrição aqui.
title: Interromper uma campanha
feature_v2: id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 410
ht-degree: 0%

---

# Interromper uma campanha {#stop-campaign}

Os usuários agora podem interromper uma campanha que está enviando ativamente (uma campanha &quot;em tempo real&quot;) diretamente da página de detalhes da campanha. Interromper uma campanha é permanente: os recipients param de progredir pela campanha imediatamente e a campanha não pode ser retomada ou reiniciada posteriormente.

## Pré-requisitos

- A campanha deve estar em um estado ativo (envio ativo). A ação Parar não está disponível para campanhas de rascunho, programadas ou que já foram interrompidas.
- [PRECISA DE ENTRADA — para confirmar com o engenheiro: parar uma campanha requer uma função ou permissão específica, ou qualquer usuário com acesso à campanha pode fazer isso?]

## O que este recurso faz

Uma ação &quot;Interromper campanha&quot; é exibida no cabeçalho de detalhes da campanha sempre que uma campanha está ativa. Selecionar essa opção abre um aviso de caixa de diálogo de confirmação de que a ação é permanente. A confirmação chama o backend para interromper a campanha; se a campanha for bem-sucedida, o status muda para &quot;Interrompida&quot; e uma mensagem de confirmação é exibida.

### Comportamentos principais

- A ação Interromper campanha só é exibida enquanto uma campanha está ativa (enviando ativamente).
- A interrupção é permanente: os recipients param de progredir na campanha e ela não pode ser retomada.
- Uma caixa de diálogo de confirmação exige que o usuário confirme explicitamente antes que a campanha seja interrompida.
- Depois de parar, o emblema de status da campanha é atualizado para &quot;Parado&quot;.
- Se a solicitação de interrupção falhar, uma mensagem de erro será exibida e a campanha permanecerá ativa.

## Como usá-lo

1. Abrir uma campanha que esteja ativa (enviando ativamente).
2. No cabeçalho de detalhes da campanha, clique em **Parar Campanha**.
3. Na caixa de diálogo de confirmação, revise o aviso: &quot;Interromper a campanha é permanente. Todos os recipients pararão de avançar e a campanha não poderá ser retomada.&quot;
4. Clique em **Parar** para confirmar.
5. Uma &quot;Campanha interrompida.&quot; será exibida e o status da campanha será atualizado para &quot;Parado&quot;.

### Campos/parâmetros de entrada

Not applicable — este recurso é uma única ação de confirmação sem campos de entrada.

## Chamadas de interface do usuário

> **Nota técnica do escritor**: Capturas de tela necessárias para o seguinte:

- [ ] O botão &quot;Interromper campanha&quot; no cabeçalho de detalhes da campanha, exibido em uma campanha ao vivo
- [ ] A caixa de diálogo de confirmação com o aviso de permanência
- [ ] O selo de status &quot;Parado&quot; após uma interrupção bem-sucedida
- [ ] A mensagem de erro exibida se a interrupção falhar

## O que este recurso não faz

- Não pausa uma campanha temporariamente. Não há como retomar uma campanha interrompida; parar é uma ação unidirecional.
- Não há suporte para reiniciar ou reiniciar uma campanha interrompida do mesmo registro de campanha.
- [PRECISA DE ENTRADA — para confirmar com o engenheiro: há um recurso separado de &quot;pausar e retomar&quot; planejado ou é Parar a única ação de controle de estado enviada nesta versão?]
