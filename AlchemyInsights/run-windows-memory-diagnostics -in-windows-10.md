---
title: Executar diagnósticos de memória do Windows no Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357785"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="55627-102">Executar diagnósticos de memória do Windows no Windows 10</span><span class="sxs-lookup"><span data-stu-id="55627-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="55627-103">Se o Windows e as aplicações no seu PC estiverem a falhar, a congelar ou a agir de forma instável, poderá ter um problema com a memória do PC (RAM).</span><span class="sxs-lookup"><span data-stu-id="55627-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="55627-104">Pode executar o Diagnóstico de Memória do Windows para verificar se há problemas com a RAM do PC.</span><span class="sxs-lookup"><span data-stu-id="55627-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="55627-105">Na caixa de pesquisa na sua barra de tarefas, digite o diagnóstico de **memória**e, em seguida, selecione O Diagnóstico da **Memória do Windows**.</span><span class="sxs-lookup"><span data-stu-id="55627-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="55627-106">Para executar o diagnóstico, o PC precisa de reiniciar.</span><span class="sxs-lookup"><span data-stu-id="55627-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="55627-107">Tem a opção de reiniciar imediatamente (por favor, guarde o seu trabalho e feche primeiro documentos e e-mails abertos), ou agende o diagnóstico para ser executado automaticamente da próxima vez que o PC reiniciar:</span><span class="sxs-lookup"><span data-stu-id="55627-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnóstico da memória do Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="55627-109">Quando o PC reiniciar, a Ferramenta de **Diagnóstico da Memória do Windows** será executada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="55627-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="55627-110">O estado e o progresso serão apresentados à medida que os diagnósticos são executados, e você tem a opção de cancelar os diagnósticos atingindo a chave **ESC** no seu teclado.</span><span class="sxs-lookup"><span data-stu-id="55627-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="55627-111">Quando os diagnósticos estiverem completos, o Windows começará normalmente.</span><span class="sxs-lookup"><span data-stu-id="55627-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="55627-112">Imediatamente após o reinício, quando o Ambiente de Trabalho aparecer, aparecerá uma notificação (junto ao ícone do **Action Center** na barra de tarefas), para indicar se foram encontrados erros de memória.</span><span class="sxs-lookup"><span data-stu-id="55627-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="55627-113">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="55627-113">For example:</span></span>

<span data-ttu-id="55627-114">Aqui está o ícone do Centro de Ação:</span><span class="sxs-lookup"><span data-stu-id="55627-114">Here's the Action Center icon:</span></span> ![Ícone do centro de ação](media/action-center-icon.png) 

<span data-ttu-id="55627-116">E uma notificação de amostra:</span><span class="sxs-lookup"><span data-stu-id="55627-116">And a sample notification:</span></span> ![Sem erros de memória](media/no-memory-errors.png)

<span data-ttu-id="55627-118">Se perdeu a notificação, pode selecionar o ícone do **Action Center** na barra de tarefas para exibir o **Action Center** e ver uma lista de notificações perlocada.</span><span class="sxs-lookup"><span data-stu-id="55627-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="55627-119">Para rever informações detalhadas, digite **o evento** na caixa de pesquisa na sua barra de tarefas e, em seguida, selecione O Espectador **do Evento**.</span><span class="sxs-lookup"><span data-stu-id="55627-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="55627-120">No painel de mão esquerda do Espectador de **Eventos,** navegue para o Sistema > de **Registos do Windows**.</span><span class="sxs-lookup"><span data-stu-id="55627-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="55627-121">No painel da direita, analise a lista enquanto olha para a coluna **Fonte,** até ver eventos com valor fonte **MemóriaDiagnósticos-Resultados**.</span><span class="sxs-lookup"><span data-stu-id="55627-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="55627-122">Realce cada evento deste tipo e veja as informações de resultados na caixa sob o separador **Geral** abaixo da lista.</span><span class="sxs-lookup"><span data-stu-id="55627-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>