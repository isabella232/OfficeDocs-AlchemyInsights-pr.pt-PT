---
title: Teams para Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582081"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="59ba6-102">Teams para Mac</span><span class="sxs-lookup"><span data-stu-id="59ba6-102">Teams add-in for Mac</span></span>

<span data-ttu-id="59ba6-103">Para somar problemas com um Teams de sistema operativo Mac para utilizadores do sistema operativo Mac, siga estes passos:</span><span class="sxs-lookup"><span data-stu-id="59ba6-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="59ba6-104">**Passo 1:** Se tiver o Exchange Híbrido no Local (2016 CU3 ou posterior), utilize a ferramenta Test-HMA.ps1 para confirmar que a Autenticação Moderna Híbrida está configurada corretamente.</span><span class="sxs-lookup"><span data-stu-id="59ba6-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="59ba6-105">Para mais informações, consulte Validar a [configuração da Autenticação Moderna Híbrida Outlook para iOS e Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="59ba6-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="59ba6-106">**Nota** Utilize o formato de endereço UPN (por exemplo, [username@contoso.com )](mailto:username@contoso.com)e não domínio \nome de utilizador.</span><span class="sxs-lookup"><span data-stu-id="59ba6-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="59ba6-107">Faça-o mesmo para utilizadores com caixas Exchange Online correio.</span><span class="sxs-lookup"><span data-stu-id="59ba6-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="59ba6-108">**Passo 2:** O utilizador pode ir para **Ferramentas**  >  **Contas...** no Outlook para Mac, localcione e selecione a conta.</span><span class="sxs-lookup"><span data-stu-id="59ba6-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="59ba6-109">Confirme que o nome de utilizador listado está no formato UPN (por exemplo, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="59ba6-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="59ba6-110">**Passo 3:** Confirme que o utilizador é um utilizador Microsoft Teams licença.</span><span class="sxs-lookup"><span data-stu-id="59ba6-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="59ba6-111">O utilizador tem de utilizar a subscrição Office 365 para Mac, versão de produto 16.24 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="59ba6-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>