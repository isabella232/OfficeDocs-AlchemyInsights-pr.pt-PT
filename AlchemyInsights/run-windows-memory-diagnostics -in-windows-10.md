---
title: Executar Windows Diagnóstico de Memória no Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922582"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Executar Windows Diagnóstico de Memória no Windows 10

Se Windows aplicações no seu PC estiverem a falhar, a congelar ou a agir de forma instável, poderá ter um problema com a memória do PC (RAM). Pode executar o diagnóstico Windows de memória para verificar a deteção de problemas com a RAM do PC.

Na caixa de pesquisa da barra de tarefas, escreva diagnóstico **de** memória e, em seguida, selecione **Windows Diagnóstico de Memória**. 

Para executar o diagnóstico, o PC tem de reiniciar. Tem a opção de reiniciar imediatamente (guarde primeiro o seu trabalho e feche os documentos e e-mails abertos) ou agende o diagnóstico para ser executado automaticamente da próxima vez que o PC reiniciar:

![Windows Diagnóstico de Memória](media/windows-memory-diagnostic.png)

Quando o PC é reiniciado, **a Windows de Diagnóstico de Memória será** executada automaticamente. O estado e o progresso serão apresentados à medida que os diagnósticos são executados e tem a opção de cancelar os diagnósticos ao atingir a tecla **Esc** no teclado.

Quando o diagnóstico for concluído, o Windows iniciará normalmente.
Imediatamente após reiniciar, quando o Ambiente de Trabalho aparecer, aparecerá uma notificação (junto ao ícone do Centro de Ação na barra de tarefas), para indicar se foram encontrados erros de memória.  Por exemplo:

Eis o ícone do Centro de Ação: ![Ícone do centro de ação](media/action-center-icon.png) 

E uma notificação de exemplo: ![Sem erros de memória](media/no-memory-errors.png)

Se perdeu a notificação, pode  selecionar o ícone do  Centro de Ação na barra de tarefas para apresentar o Centro de Ação e ver uma lista percorra as notificações.

Para rever informações detalhadas, escreva evento **na caixa** de pesquisa na barra de tarefas e, em seguida, selecione **Visualizador de Eventos**. No painel **do lado esquerdo** do Visualizador de Eventos, navegue até à Windows de > **Sistema.** No painel do lado direito, procure na lista  enquanto vê a coluna Origem até ver os eventos com o valor de **OrigemDiagnósticos-Resultados** da Memória. Realce cada um desses eventos e veja as informações de resultados na caixa no **separador** Geral abaixo da lista.
