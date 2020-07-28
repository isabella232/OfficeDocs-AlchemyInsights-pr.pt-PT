---
title: Múltiplas sessões ativas para a mesma caixa de correio
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439717"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="f248d-102">Múltiplas sessões ativas para a mesma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="f248d-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="f248d-103">Para controlar o uso de recursos cambiais, uma caixa de correio tem um "orçamento".</span><span class="sxs-lookup"><span data-stu-id="f248d-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="f248d-104">A exceção sobre-orçamental pode ser desencadeada por, mas não se limita a, as seguintes circunstâncias:</span><span class="sxs-lookup"><span data-stu-id="f248d-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="f248d-105">Alguns separadores de navegador são abertos dentro da mesma sessão de Aplicação Web do Outlook.</span><span class="sxs-lookup"><span data-stu-id="f248d-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="f248d-106">Algumas sessões de Aplicação Web do Outlook ativo para a mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f248d-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="f248d-107">Algumas outras aplicações de clientes (Outlook, Outlook Mobile, uma aplicação de cliente de terceiros) acedem à caixa de correio ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="f248d-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="f248d-108">As operações de longa duração, como a execução de pedidos de pesquisa, são realizadas a partir de outra sessão de caixa de correio ativa.</span><span class="sxs-lookup"><span data-stu-id="f248d-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

