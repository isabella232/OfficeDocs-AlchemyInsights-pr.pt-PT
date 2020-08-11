---
title: Complemento de equipas para Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629799"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="c7978-102">Complemento de equipas para Mac</span><span class="sxs-lookup"><span data-stu-id="c7978-102">Teams add-in for Mac</span></span>

<span data-ttu-id="c7978-103">Para resolver um suplemento de equipas em falta para os utilizadores do sistema operativo Mac, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="c7978-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="c7978-104">**Passo 1:** Se tiver As Instalações de Intercâmbio Híbrido (2016 CU3 ou posteriormente necessária), utilize a ferramenta Test-HMA.ps1 para confirmar que a Autenticação Moderna Híbrida está corretamente configurada.</span><span class="sxs-lookup"><span data-stu-id="c7978-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="c7978-105">Para obter mais informações, consulte [a configuração de autenticação moderna híbrida para Outlook para iOS e Android.](https://aka.ms/AA980zq)</span><span class="sxs-lookup"><span data-stu-id="c7978-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="c7978-106">**Nota** Utilize o formato de endereço UPN (por exemplo, [username@contoso.com),](mailto:username@contoso.com)não domínio\username.</span><span class="sxs-lookup"><span data-stu-id="c7978-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="c7978-107">Faça isto mesmo para utilizadores com caixas de correio Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c7978-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="c7978-108">**Passo 2:** Que o utilizador **Tools**vá às  >  **Contas Ferramentas...** no Outlook for Mac, e encontrar e selecionar a conta.</span><span class="sxs-lookup"><span data-stu-id="c7978-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="c7978-109">Confirme que o nome de utilizador listado está no formato UPN (por exemplo, [username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="c7978-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="c7978-110">**Passo 3:** Confirme que o utilizador é um utilizador licenciado da Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c7978-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="c7978-111">O utilizador deve estar a utilizar o Office 365 para a subscrição do Mac, versão do produto 16.24 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="c7978-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>