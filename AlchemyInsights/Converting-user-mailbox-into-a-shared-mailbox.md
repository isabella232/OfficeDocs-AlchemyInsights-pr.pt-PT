---
title: Converter caixa de correio do utilizador para uma caixa de correio partilhada?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496446"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="5c1d1-102">Converter uma caixa de correio do utilizador uma caixa de correio partilhada</span><span class="sxs-lookup"><span data-stu-id="5c1d1-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="5c1d1-103">Só pode converter uma caixa de correio do utilizador para uma caixa de correio partilhada, se o utilizador tiver uma licença de Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c1d1-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="5c1d1-104">Depois da caixa de correio é convertida, continuará a aparecer na lista de utilizadores do active uma vez que essa lista inclui caixas de correio partilhadas.</span><span class="sxs-lookup"><span data-stu-id="5c1d1-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="5c1d1-105">No entanto, a caixa de correio convertida também aparecerá na lista de caixa de correio partilhada.</span><span class="sxs-lookup"><span data-stu-id="5c1d1-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="5c1d1-106">Se tentar converter uma caixa de correio na consola de administração do Exchange e a conversão falha, limpar a cache do browser e os cookies e tente novamente.</span><span class="sxs-lookup"><span data-stu-id="5c1d1-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="5c1d1-107">Se ainda não funcionar, tente converter a caixa de correio no Exchange Management Shell executando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="5c1d1-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="5c1d1-108">Mais informações de conversão de caixa de correio estão disponíveis no [converter uma caixa de correio do utilizador para uma caixa de correio partilhada](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="5c1d1-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
