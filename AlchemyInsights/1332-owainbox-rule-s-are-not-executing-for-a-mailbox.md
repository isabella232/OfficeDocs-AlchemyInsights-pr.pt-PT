---
title: 1332 OWA - regra (s) de pasta a receber é não execução de uma caixa de correio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28306146"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="13216-102">Uma regra de pasta a receber não funciona conforme esperado</span><span class="sxs-lookup"><span data-stu-id="13216-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="13216-103">Verifique se as seguintes definições:</span><span class="sxs-lookup"><span data-stu-id="13216-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="13216-p101">Uma mensagem pode ser redireccionada, reencaminhadas ou respondidas automaticamente com base nas regras da pasta a receber apenas uma vez. Uma regra de redireccionamento (uma regra de pasta a receber ou uma regra de fluxo de correio, também conhecido como uma regra de transporte) pode adicionar um máximo de dez de reencaminhamento de destinatários para uma mensagem. Para mais informações, consulte [os limites de regra de diário, o transporte e a receber](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="13216-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="13216-p102">Regras da pasta a receber não funcionam com a caixa de correio do registo em diário alternativo. Para mais informações sobre a caixa de correio do registo em diário alternativo, consulte a [caixa de correio do registo em diário alternativo](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="13216-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="13216-109">Para corrigir estes problemas, consulte [2829319 da KB](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="13216-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="13216-110">Se não aplicam os problemas anteriores, execute o relatório de diagnóstico de regra de pasta a receber antes de comunicar o problema à Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="13216-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="13216-111">Abrir a caixa de correio no Outlook na web e clique em **Definições** \> **Opções** \> **mensagem de correio electrónico organizar** \> **regras da pasta a receber**.</span><span class="sxs-lookup"><span data-stu-id="13216-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="13216-112">Na parte inferior da página, clique em **se as regras não estão a funcionar em clique aqui para gerar um relatório de diagnóstico**.</span><span class="sxs-lookup"><span data-stu-id="13216-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

