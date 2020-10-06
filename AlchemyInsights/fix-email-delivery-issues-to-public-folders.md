---
title: Corrija problemas de entrega de e-mail para pastas públicas via correio
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366475"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="de844-102">Corrija problemas de entrega de e-mail para pastas públicas via correio</span><span class="sxs-lookup"><span data-stu-id="de844-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="de844-103">Se os remetentes externos não puderem enviar mensagens para as suas pastas públicas ativadas por correio e os remetentes receberem o erro: **não foi possível encontrar (550 5.4.1)**, verifique se o domínio de e-mail da pasta pública está configurado como um domínio de retransmissão interno em vez de um domínio autoritário:</span><span class="sxs-lookup"><span data-stu-id="de844-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="de844-104">Abra o [Centro de Administração Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="de844-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="de844-105">Ir para **o fluxo de correio** \> **Domínios aceitos,** selecione o domínio aceite e, em seguida, clique em **Editar**.</span><span class="sxs-lookup"><span data-stu-id="de844-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="de844-106">Na página de propriedades que abre, se o tipo de domínio estiver definido como **Autoritário,** altere o valor para **relé Interno** e, em seguida, clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="de844-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="de844-107">Se os remetentes externos receberem o **erro, não tem permissão (550 5.7.13)**, executar o seguinte comando no [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver as permissões para utilizadores anónimos na pasta pública:</span><span class="sxs-lookup"><span data-stu-id="de844-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="de844-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Por exemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="de844-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="de844-109">Para permitir que utilizadores externos enviem e-mails para esta pasta pública, adicione o acesso createItems ao utilizador Anonymous.</span><span class="sxs-lookup"><span data-stu-id="de844-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="de844-110">Por exemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="de844-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
