---
title: Corrigir problemas de entrega de correio electrónico correio nas pastas públicas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752683"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="7e7fd-102">Corrigir problemas de entrega de correio electrónico correio nas pastas públicas</span><span class="sxs-lookup"><span data-stu-id="7e7fd-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="7e7fd-103">Se remetentes externos não é possível enviar mensagens para as pastas públicas com correio electrónico e os remetentes recebem o erro: **não foi possível localizar (550 5.4.1)**, verifique o domínio de correio electrónico para a pasta pública está configurada como um domínio de retransmissão interno, em vez de um domínio autoritário:</span><span class="sxs-lookup"><span data-stu-id="7e7fd-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="7e7fd-104">Abra o [Centro de administração do Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="7e7fd-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="7e7fd-105">Vá para **o fluxo de correio** \> **aceites domínios**, seleccione o domínio aceite e, em seguida, clique em **Editar**.</span><span class="sxs-lookup"><span data-stu-id="7e7fd-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="7e7fd-106">Nas propriedades da página que abre, se o tipo de domínio estiver definido como **autoritários**, altere o valor para **reencaminhamento interno** e, em seguida, clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="7e7fd-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="7e7fd-107">Se os remetentes externos recebem o erro **que não tem permissão (550 5.7.13)**, execute o seguinte comando no [PowerShell Online do Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver as permissões para utilizadores anónimos na pasta pública:</span><span class="sxs-lookup"><span data-stu-id="7e7fd-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="7e7fd-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Por exemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="7e7fd-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="7e7fd-109">Para permitir que os utilizadores externos enviar correio electrónico para esta pasta pública, adicione o acesso de CreateItems para a direita para o utilizador anónimo.</span><span class="sxs-lookup"><span data-stu-id="7e7fd-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="7e7fd-110">Por exemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="7e7fd-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
