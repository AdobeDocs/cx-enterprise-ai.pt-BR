---
description: insira uma descrição aqui.
title: Programar uma campanha
source-git-commit: 500932a1e705af1682a71ce460b6fa62e4ffd4ac
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# Programar uma campanha {#schedule-campaign}

Ao iniciar uma campanha, os usuários agora podem escolher exatamente quando ela sai: imediatamente, em uma data e hora futuras específicas ou em um cronograma repetitivo (recorrente). Os usuários também podem voltar mais tarde e alterar a programação de uma campanha que já foi iniciada ou programada.

> **O que mudou**: anteriormente, só era possível iniciar campanhas imediatamente. Esta versão adiciona programação futura única, programações recorrentes e a capacidade de editar uma programação após a inicialização.

## Pré-requisitos

- A campanha deve estar pronta para ser iniciada (todas as configurações necessárias foram concluídas).
- Nenhum pré-requisito necessário além de ter uma campanha em um estado inicializável.

## O que este recurso faz

Quando um usuário inicia uma campanha, ele escolhe um dos três modos de agendamento e confirma. O agendamento escolhido determina quando a campanha começa a enviar e, para campanhas recorrentes, com que frequência ela se repete e quando (ou se) termina. Depois que uma campanha é agendada ou ativada, sua programação pode ser editada nas configurações da campanha.

### Comportamentos principais

- Três modos de agendamento estão disponíveis ao iniciar: **Agora**, **Agendar uma vez** e **Recorrente**.
- Uma campanha programada para o futuro mostra um status &quot;Programado&quot; até chegar a hora de início e, em seguida, alterna automaticamente para &quot;Ativo&quot;.
- Uma campanha recorrente que começou mostra &quot;Ao vivo&quot; junto com um resumo de sua recorrência (por exemplo, &quot;Semanalmente na terça-feira, quinta às 9h&quot;).
- As campanhas recorrentes podem ser definidas para serem executadas indefinidamente (fim &quot;Nunca&quot;) ou até uma data final específica. Campanhas únicas e imediatas não têm uma opção de data de término, pois são executadas uma vez.
- Os usuários podem editar o agendamento de uma campanha que já foi iniciada ou agendada, usando as mesmas opções de agendamento, nas configurações da campanha.

## Como usá-lo

**Para agendar uma campanha no lançamento:**

1. Na campanha, clique em **Pronto para iniciar**.
2. Na caixa de diálogo de inicialização, escolha uma opção de programação:
   - **Agora** — a campanha começa a ser enviada imediatamente após o lançamento.
   - **Agendar uma vez** — escolha uma **Data de início** futura (data e hora juntas).
   - **Recorrente** — escolha uma **Frequência** (Diariamente, Semanalmente ou Mensalmente) e uma hora de início, depois defina o padrão de recorrência (consulte os campos abaixo).
3. Se a opção Recorrente estiver selecionada, escolha se a campanha termina **Nunca** ou **Em uma data** e escolha uma data final, se aplicável.
4. Confirme para iniciar a campanha com a programação selecionada.

**Para editar um agendamento existente:**

1. Abra a campanha e vá para as configurações.
2. Localize a seção programação e selecione o resumo da programação atual.
3. Atualize a programação usando as mesmas opções descritas acima.
4. Salve a alteração.

### Campos/parâmetros de entrada

| Campo | Descrição | Obrigatório? |
| --- | --- | --- |
| Modo de agendamento | Opção de Agora, Agendar uma vez ou Recorrente | Sim |
| Data inicial | Data e hora em que a campanha começa (modo Agendar uma vez) | Sim, para Agendar uma vez |
| Frequência | Diariamente, Semanalmente ou Mensalmente (modo Recorrente) | Sim, para Recorrente |
| Hora de início | Hora do dia que a campanha recorrente envia | Sim, para Recorrente |
| Dias da semana | Em quais dias a campanha se repete | Sim, para a frequência Semanal |
| Dia do mês | Em qual dia do mês a campanha se repete | Sim, para frequência Mensal |
| Encerrar campanha | Nunca ou em uma data final específica | Sim, para Recorrente |

## Chamadas de interface do usuário

> **Nota técnica do escritor**: Capturas de tela necessárias para o seguinte:

- [ ] A caixa de diálogo de inicialização mostrando as opções Agora / Agendar uma vez / Recorrente
- [ ] O seletor de data e hora Agendar uma vez
- [ ] As opções Recorrentes: seletor de frequência, alternância semanal de dia, grade mensal de dia do mês
- [ ] A &quot;Campanha final&quot; Nunca / Em uma data escolhida
- [ ] O selo de status &quot;Agendado&quot; em uma campanha aguardando sua hora de início
- [ ] O selo de status &quot;Ao vivo&quot; com um resumo de recorrência (por exemplo, &quot;Semanalmente na Terça, quinta às 9h)
- [ ] A seção de agendamento nas configurações da campanha, mostrando o ponto de entrada de edição

## O que este recurso não faz

- Ele não aceita intervalos de repetição personalizados, como &quot;a cada 2 semanas&quot; ou &quot;a cada 3 dias&quot; — somente as frequências padrão Diário, Semanal ou Mensal estão disponíveis.
- Não há suporte para recorrência mensal relativa, como &quot;a segunda segunda-feira do mês&quot; — somente a seleção específica do dia do mês está disponível para Mensalmente.
- Não oferece uma data de término para campanhas **Agora** ou **Agendar uma vez** — uma data de término só está disponível quando a opção Recorrente está selecionada, uma vez que campanhas únicas são executadas uma vez por definição.
