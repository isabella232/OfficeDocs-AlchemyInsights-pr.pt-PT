---
title: PowerShell do Exchange e depreciação da autenticação básica
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813483"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="9d972-102">PowerShell do Exchange e depreciação da autenticação básica</span><span class="sxs-lookup"><span data-stu-id="9d972-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="9d972-103">Para obter as mais recentes informações sobre como ligar à PowerShell do Exchange Online sem a utilização da Autenticação Básica, [aceda aqui](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="9d972-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="9d972-104">O módulo PowerShell v2 não utiliza autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="9d972-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="9d972-105">Tenha em atenção que a Autenticação Básica ainda precisa de ser ativada no computador cliente.</span><span class="sxs-lookup"><span data-stu-id="9d972-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="9d972-106">O novo módulo PowerShell V2 utiliza a Autenticação Moderna para estabelecer uma ligação que permita todos os Cmdlets V2 baseados em REST.</span><span class="sxs-lookup"><span data-stu-id="9d972-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="9d972-107">Para além dos cmdlets V2, também lhe permite aceder a Cmdlets da PowerShell Remota (RPS) mais antigos, os quais exigem a criação de uma sessão de PowerShell remota.</span><span class="sxs-lookup"><span data-stu-id="9d972-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="9d972-108">O estabelecimento de uma sessão de RPS no computador Windows requer a ativação do WinRM BasicAuth no computador cliente, mesmo que o módulo utilize o mecanismo de Autenticação Moderna para autenticar o serviço.</span><span class="sxs-lookup"><span data-stu-id="9d972-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="9d972-109">O pipeline de Autenticação Básica WinRM é utilizado para o transporte de tokens de Autenticação Moderna.</span><span class="sxs-lookup"><span data-stu-id="9d972-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="9d972-110">Se a Autenticação Básica WinRM estiver desativada no computador cliente, os novos cmdlets V2 continuarão a funcionar (mas os cmdlets RPS mais antigos não funcionarão).</span><span class="sxs-lookup"><span data-stu-id="9d972-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
