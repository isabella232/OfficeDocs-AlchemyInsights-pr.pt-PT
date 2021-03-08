---
title: Definir ClienteAccessServerEnabled a True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525965"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="0dfbd-102">Definir ClienteAccessServerEnabled a True</span><span class="sxs-lookup"><span data-stu-id="0dfbd-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="0dfbd-103">Se não conseguir abrir uma mensagem de correio eletrónico encriptada e, em vez disso, ver um anexo **rpmsg,** execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="0dfbd-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="0dfbd-104">Ligue-se a Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="0dfbd-105">Para se ligar ao Exchange Online PowerShell, tem de iniciar scontabilidade através de uma conta de administração global ou de administração Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="0dfbd-106">a.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-106">a.</span></span> <span data-ttu-id="0dfbd-107">Abra o Windows PowerShell e, em seguida, execute o seguinte comando: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="0dfbd-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="0dfbd-108">b.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-108">b.</span></span> <span data-ttu-id="0dfbd-109">Na caixa de diálogo **de pedido de pedido de procura do Windows PowerShell,** insira a sua conta de trabalho ou escola e a palavra-passe, c.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="0dfbd-110">Clique em **OK**.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-110">Click **OK**.</span></span> 

2. <span data-ttu-id="0dfbd-111">Executar o seguinte comando para criar uma nova sessão:</span><span class="sxs-lookup"><span data-stu-id="0dfbd-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="0dfbd-112">a.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-112">a.</span></span> <span data-ttu-id="0dfbd-113">Run the following command:</span><span class="sxs-lookup"><span data-stu-id="0dfbd-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="0dfbd-114">Executar `Get-IRMConfiguration` o comando.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="0dfbd-115">Verifique a definição **ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="0dfbd-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="0dfbd-116">a.</span><span class="sxs-lookup"><span data-stu-id="0dfbd-116">a.</span></span> <span data-ttu-id="0dfbd-117">Se a definição **DeServerEnabled do Cliente** estiver definida como **Falsa,** executar o seguinte cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="0dfbd-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="0dfbd-118">Feche sempre a sua sessão de powershell com o seguinte comando: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="0dfbd-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="0dfbd-119">Para mais informações, consulte [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="0dfbd-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

