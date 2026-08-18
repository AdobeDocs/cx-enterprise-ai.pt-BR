---
description: insira uma descrição aqui.
title: Iniciar uma campanha
feature_v2:
  - id: fdae8433-07cd-42e7-acce-738afe63f6bb
source-git-commit: 1c4f9585c04eae8693e38541084cead08412d192
workflow-type: tm+mt
source-wordcount: 757
ht-degree: 0%

---

# Iniciar uma campanha {#launch-campaign}

Iniciar uma campanha é a ação que a move do rascunho para o envio ativo. Antes que a caixa de diálogo de inicialização seja aberta, o Halo verifica se a campanha está pronta e bloqueia a inicialização até que a configuração necessária seja concluída. A caixa de diálogo de inicialização mostra uma pré-visualização do email e do público-alvo, permite que o usuário revise ou altere o agendamento de envio em linha e relata se a inicialização foi bem-sucedida. Esta seção aborda a experiência de inicialização de ponta a ponta; para as opções de agendamento oferecidas durante a inicialização, consulte [Agendar uma campanha](/help/coworker/campaigns/schedule-campaign.md).

## Pré-requisitos

- A campanha deve estar no status Rascunho. <!-- The Launch action isn't available once a campaign is already live. -->
<!-- - The campaign must pass a readiness check: sending settings configured, at least one test email sent, and a real (non-sample) audience uploaded. -->
- [PRECISA DE ENTRADA — para confirmar com o engenheiro: alguns usuários podem ver uma experiência &quot;em breve&quot; em vez de um botão Iniciar real, que oferece apenas o download da campanha ou o envio de um email de prova em vez da inicialização no aplicativo. Confirme o que determina qual experiência um determinado usuário ou campanha obtém.]

## O que este recurso faz

Quando um usuário inicia uma campanha, o Halo primeiro valida se a campanha está pronta. Se algo necessário estiver ausente, uma caixa de diálogo listará o que precisa ser corrigido para que a inicialização possa continuar. Depois que a validação é aprovada, a caixa de diálogo de inicialização mostra uma pré-visualização do email e do público-alvo/fluxo de trabalho, permite que o usuário revise ou edite a programação de envio sem sair do fluxo e, para envios grandes, mostra um aviso de volume de envio estimado. A confirmação aciona o lançamento, e o Halo relata um dos três resultados: iniciado, já iniciado ou com falha.

### Comportamentos principais

- O Launch só está disponível para campanhas com o status de Rascunho; uma campanha que já está ativa não pode ser iniciada novamente.
- Uma verificação de preparação é executada automaticamente antes da caixa de diálogo de inicialização ser aberta. Problemas não resolvidos bloqueiam a inicialização e são listados com uma maneira de resolver cada um.
- A caixa de diálogo de inicialização mostra uma visualização do email (assunto, pré-cabeçalho, remetente) e uma visualização do público-alvo/fluxo de trabalho.
- A programação de envio pode ser revisada ou alterada na caixa de diálogo de inicialização.
- Para envios grandes, a caixa de diálogo mostra um impacto estimado no volume de envio. [PRECISA DE ENTRADA — o texto exato deste aviso não estava disponível no código]
- No caso de sucesso, o status da campanha é atualizado para &quot;Programado&quot; ou &quot;Ao vivo&quot; (dependendo da programação escolhida), e uma mensagem de confirmação observa que os insights da campanha estarão disponíveis em 2 horas.
- Se a campanha já foi iniciada (por exemplo, a partir de um clique duplicado), o Halo mostra uma mensagem de &quot;já iniciado&quot; em vez de um erro.
- Se a inicialização falhar, uma mensagem de erro será exibida e a campanha permanecerá no Rascunho; o usuário pode tentar novamente.
- Uma vez interrompida a campanha <!--(see [Stop a live campaign](./stop-live-campaign.md))-->, ela não poderá ser reiniciada do mesmo registro de campanha — a interrupção é um estado separado e permanente.

## Como acessar o

**Para iniciar uma campanha:**

1. Na campanha, clique em **Iniciar** (mostrado como &quot;Pronto para iniciar&quot; ainda no rascunho).
2. Se algo estiver faltando, uma caixa de diálogo chamada &quot;Algumas coisas ainda precisam de atenção&quot; lista o que deve ser concluído:
   - **Definir configurações de email** — o envio de parâmetros (remetente/domínio) ainda não foi configurado.
   - **Emails não testados** — envie pelo menos um email de teste para revisar o email antes de iniciar.
   - **Público-alvo real necessário para o lançamento** — a campanha ainda está usando um público-alvo de exemplo; carregue um CSV de público-alvo real.
     Resolva cada item e tente iniciar novamente.
3. Depois que a campanha é aprovada na verificação de preparação, a caixa de diálogo de inicialização é aberta, mostrando uma pré-visualização do email e do público-alvo.
4. Revise o agendamento mostrado na caixa de diálogo. Para alterá-la, use as opções de agendamento descritas em [Agendar quando uma campanha for iniciada](/help/coworker/campaigns/schedule-campaign.md) e salve.
5. Confirme para iniciar. No caso de sucesso, uma mensagem de confirmação é exibida e o status da campanha é atualizado (para &quot;Agendado&quot; ou &quot;Ao vivo&quot;).

<!-- 
## Input fields / parameters

Not applicable beyond the schedule fields already documented in [Schedule when a campaign launches](/help/coworker/campaigns/schedule-campaign.md) — launching itself doesn't require any additional input. 
-->

## Chamadas de interface do usuário

> **Nota técnica do escritor**: Capturas de tela necessárias para o seguinte:

- [ ] O ponto de entrada/botão Iniciar no cabeçalho de detalhes da campanha
- [ ] A caixa de diálogo de preparação/validação listando itens incompletos
- [ ] A caixa de diálogo de inicialização mostrando a pré-visualização de email + público-alvo e a seção de programação
- [ ] O aviso de impacto estimado no volume de envio (para públicos grandes)
- [ ] A mensagem de confirmação de sucesso após a inicialização
- [ ] A mensagem &quot;já iniciado&quot;
- [ ] A mensagem de erro genérica de falha na inicialização

## O que este recurso não faz

- Ele não permite um lançamento de campanha com uma amostra de público (não real), emails não testados ou configurações de envio não definidas — todos os três devem ser resolvidos primeiro.
- O Launch não aceita um agendamento como parte da mesma ação; o agendamento é salvo separadamente (de dentro da mesma caixa de diálogo) antes ou como parte da confirmação do lançamento.
- Não há suporte para reiniciar uma campanha que foi interrompida — a interrupção é permanente <!--(see [Stop a live campaign](./stop-live-campaign.md))-->.
- [ENTRADA NECESSÁRIA — para confirmar com engenheiro/PM: para alguns usuários, o Launch pode ser substituído por uma experiência em &quot;breve&quot;, oferecendo apenas um download da campanha (PDF/DOCX) ou um email de prova enviado, sem inicialização de autoatendimento no aplicativo. Confirme o público ao qual isso se aplica antes da publicação, pois isso altera as etapas passo a passo desse coorte.]
