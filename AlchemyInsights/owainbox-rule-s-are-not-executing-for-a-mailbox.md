---
title: 1332 OWA - regra (s) de pasta a receber é não execução de uma caixa de correio
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204071"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="dc69e-102">Uma regra de pasta a receber não funciona conforme esperado</span><span class="sxs-lookup"><span data-stu-id="dc69e-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="dc69e-103">Verifique se as seguintes definições:</span><span class="sxs-lookup"><span data-stu-id="dc69e-103">Verify the following settings:</span></span>

- <span data-ttu-id="dc69e-104">Uma mensagem pode ser redireccionada, reencaminhadas ou respondidas automaticamente com base nas regras da pasta a receber apenas uma vez.</span><span class="sxs-lookup"><span data-stu-id="dc69e-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="dc69e-105">Uma regra de redireccionamento (uma regra de pasta a receber ou uma regra de fluxo de correio, também conhecido como uma regra de transporte) pode adicionar um máximo de dez de reencaminhamento de destinatários para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="dc69e-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="dc69e-106">Para mais informações, consulte [os limites de regra de diário, o transporte e a receber](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="dc69e-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="dc69e-107">Regras da pasta a receber não funcionam com a caixa de correio do registo em diário alternativo.</span><span class="sxs-lookup"><span data-stu-id="dc69e-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="dc69e-108">Para mais informações sobre a caixa de correio do registo em diário alternativo, consulte a [caixa de correio do registo em diário alternativo](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="dc69e-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="dc69e-109">Para corrigir estes problemas, consulte [2829319 da KB](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="dc69e-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="dc69e-110">Se não aplicam os problemas anteriores, execute o relatório de diagnóstico de regra de pasta a receber antes de comunicar o problema à Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="dc69e-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="dc69e-111">Abrir a caixa de correio no Outlook na web e clique em</span><span class="sxs-lookup"><span data-stu-id="dc69e-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="dc69e-112">**Definições de** > **Ver todas as definições do Outlook** > **série** > **regras**.</span><span class="sxs-lookup"><span data-stu-id="dc69e-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="dc69e-113">Na parte inferior da página, clique em **se as regras não estão a funcionar em clique aqui para gerar um relatório de diagnóstico**.</span><span class="sxs-lookup"><span data-stu-id="dc69e-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
