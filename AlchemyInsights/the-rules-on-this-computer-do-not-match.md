---
title: 'Erro: As regras deste computador não coincidem'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782963"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="55c39-102">Erro: As regras deste computador não coincidem</span><span class="sxs-lookup"><span data-stu-id="55c39-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="55c39-103">Para ver o estado atualizado deste problema conhecido, consulte [as regras deste computador que não correspondem às regras da Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="55c39-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="55c39-104">A Equipa Outlook implementou uma correção na Build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="55c39-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="55c39-105">A correção já está no Insider Fast e irá para o Monthly Channel no final de junho de 2020.</span><span class="sxs-lookup"><span data-stu-id="55c39-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="55c39-106">Uma vez que tenha a construção fixa, poderá obter o pedido "Quais as regras que quer manter" uma última vez.</span><span class="sxs-lookup"><span data-stu-id="55c39-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="55c39-107">Escolha o Servidor quando solicitado e volte ao Outlook e volte a ativar quaisquer regras que foram desativadas.</span><span class="sxs-lookup"><span data-stu-id="55c39-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="55c39-108">Até que a correção esteja disponível, utilize a seguinte solução:</span><span class="sxs-lookup"><span data-stu-id="55c39-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="55c39-109">**Solução alternativa**: Em relatórios recentes, o problema ocorreu para aqueles que apenas criaram regras de clientes no ambiente de trabalho do Outlook.</span><span class="sxs-lookup"><span data-stu-id="55c39-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="55c39-110">Se continuar a deparar-se com o problema, considere eliminar as regras e, em seguida, criar e editar regras apenas na OWA (Outlook Web App) até que o problema seja resolvido.</span><span class="sxs-lookup"><span data-stu-id="55c39-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="55c39-111">Se não conseguir eliminar as regras manualmente, pode executar um comando Outlook quando iniciar o Outlook executando Outlook.exe /regras de limpeza.</span><span class="sxs-lookup"><span data-stu-id="55c39-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="55c39-112">Isto eliminará as regras do cliente e do servidor.</span><span class="sxs-lookup"><span data-stu-id="55c39-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="55c39-113">Eliminará todas as regras para todas as contas do Perfil outlook.</span><span class="sxs-lookup"><span data-stu-id="55c39-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="55c39-114">Este comando está ainda documentado no artigo de comutações da linha de comando.</span><span class="sxs-lookup"><span data-stu-id="55c39-114">This command is further documented in the Command-line switches article.</span></span>

