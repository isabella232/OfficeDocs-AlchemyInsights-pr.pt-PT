---
title: Corrigir problemas de entrega de e-mail para pastas públicas via correio
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716363"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="8bda9-102">Corrigir problemas de entrega de e-mail para pastas públicas via correio</span><span class="sxs-lookup"><span data-stu-id="8bda9-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="8bda9-103">Se os remetentes externos não puderem enviar mensagens para as suas pastas públicas ativadas por correio, e os remetentes receberem o erro: **não puderam ser encontrados (550 5.4.1),** verifique se o domínio de e-mail da pasta pública está configurado como um domínio interno de retransmissão em vez de um domínio autoritário:</span><span class="sxs-lookup"><span data-stu-id="8bda9-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="8bda9-104">Abra o centro de [administração exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="8bda9-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="8bda9-105">Vá ao **fluxo** \> de correio **Domínios aceitos,** selecione o domínio aceite e, em seguida, clique em **Editar**.</span><span class="sxs-lookup"><span data-stu-id="8bda9-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="8bda9-106">Na página de propriedades que se abre, se o tipo de domínio for definido para **Authoritativo,** altere o valor para **retransmissão interna** e, em seguida, clique em **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="8bda9-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="8bda9-107">Se os remetentes externos receberem o erro, **não tem permissão (550 5.7.13)**, executar o seguinte comando no [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) para ver as permissões para utilizadores anónimos na pasta pública:</span><span class="sxs-lookup"><span data-stu-id="8bda9-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="8bda9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Por exemplo, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="8bda9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="8bda9-109">Para permitir que utilizadores externos enviem e-mail para esta pasta pública, adicione o acesso do CreateItems ao utilizador Anónimo.</span><span class="sxs-lookup"><span data-stu-id="8bda9-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="8bda9-110">Por exemplo, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="8bda9-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
