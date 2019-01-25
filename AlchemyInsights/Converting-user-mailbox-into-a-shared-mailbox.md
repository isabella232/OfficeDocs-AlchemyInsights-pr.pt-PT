---
title: Converter caixa de correio do utilizador para uma caixa de correio partilhada?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483870"
---
<span data-ttu-id="d9ccd-p101">Só pode converter uma caixa de correio do utilizador para uma caixa de correio partilhada, se o utilizador tiver uma licença de Exchange. Depois da caixa de correio é convertida, continuará a aparecer na lista de utilizadores do active uma vez que essa lista inclui caixas de correio partilhadas. No entanto, a caixa de correio convertida também aparecerá na lista de caixa de correio partilhada.</span><span class="sxs-lookup"><span data-stu-id="d9ccd-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="d9ccd-p102">Se tentar converter uma caixa de correio na consola de administração do Exchange e a conversão falha, limpar a cache do browser e os cookies e tente novamente. Se ainda não funcionar, tente converter a caixa de correio no Exchange Management Shell executando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="d9ccd-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="d9ccd-107">Mais informações de conversão de caixa de correio estão disponíveis no [converter uma caixa de correio do utilizador para uma caixa de correio partilhada](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="d9ccd-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
