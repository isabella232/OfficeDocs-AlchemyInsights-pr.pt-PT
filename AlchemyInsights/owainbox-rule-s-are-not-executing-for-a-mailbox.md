---
title: 1332 OWA - regra (s) de pasta a receber é não execução de uma caixa de correio
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858755"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="6f6bf-102">Uma regra de pasta a receber não funciona conforme esperado</span><span class="sxs-lookup"><span data-stu-id="6f6bf-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="6f6bf-103">Verifique se as seguintes definições:</span><span class="sxs-lookup"><span data-stu-id="6f6bf-103">Verify the following settings:</span></span>

- <span data-ttu-id="6f6bf-104">Uma mensagem pode ser redireccionada, reencaminhadas ou respondidas automaticamente com base nas regras da pasta a receber apenas uma vez.</span><span class="sxs-lookup"><span data-stu-id="6f6bf-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="6f6bf-105">Uma regra de redireccionamento (uma regra de pasta a receber ou uma regra de fluxo de correio, também conhecido como uma regra de transporte) pode adicionar um máximo de dez de reencaminhamento de destinatários para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="6f6bf-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="6f6bf-106">Para mais informações, consulte [os limites de regra de diário, o transporte e a receber](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="6f6bf-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="6f6bf-107">Regras da pasta a receber não funcionam com a caixa de correio do registo em diário alternativo.</span><span class="sxs-lookup"><span data-stu-id="6f6bf-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="6f6bf-108">Para mais informações sobre a caixa de correio do registo em diário alternativo, consulte a [caixa de correio do registo em diário alternativo](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="6f6bf-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="6f6bf-109">Para corrigir estes problemas, consulte [2829319 da KB](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="6f6bf-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="6f6bf-110">Se não aplicam os problemas anteriores, execute o relatório de diagnóstico de regra de pasta a receber antes de comunicar o problema à Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="6f6bf-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="6f6bf-111">Abrir a caixa de correio no Outlook na web e clique em **Definições** \> **Opções** \> **mensagem de correio electrónico organizar** \> **regras da pasta a receber**.</span><span class="sxs-lookup"><span data-stu-id="6f6bf-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="6f6bf-112">Na parte inferior da página, clique em **se as regras não estão a funcionar em clique aqui para gerar um relatório de diagnóstico**.</span><span class="sxs-lookup"><span data-stu-id="6f6bf-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
