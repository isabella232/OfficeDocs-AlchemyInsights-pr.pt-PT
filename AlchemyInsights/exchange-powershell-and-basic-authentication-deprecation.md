---
title: PowerShell do Exchange e depreciação da autenticação básica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015700"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="b5ac1-102">PowerShell do Exchange e depreciação da autenticação básica</span><span class="sxs-lookup"><span data-stu-id="b5ac1-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="b5ac1-103">Para obter as mais recentes informações sobre como ligar à PowerShell do Exchange Online sem a utilização da Autenticação Básica, [aceda aqui](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="b5ac1-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="b5ac1-104">Tenha em atenção que a Autenticação Básica ainda precisa de ser ativada no computador cliente.</span><span class="sxs-lookup"><span data-stu-id="b5ac1-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="b5ac1-105">O novo módulo PowerShell V2 utiliza a Autenticação Moderna para estabelecer uma ligação que permita todos os Cmdlets V2 baseados em REST.</span><span class="sxs-lookup"><span data-stu-id="b5ac1-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="b5ac1-106">Para além dos cmdlets V2, também lhe permite aceder a Cmdlets da PowerShell Remota (RPS) mais antigos, os quais exigem a criação de uma sessão de PowerShell remota.</span><span class="sxs-lookup"><span data-stu-id="b5ac1-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="b5ac1-107">O estabelecimento de uma sessão de RPS no computador Windows requer a ativação do WinRM BasicAuth no computador cliente, mesmo que o módulo utilize o mecanismo de Autenticação Moderna para autenticar o serviço.</span><span class="sxs-lookup"><span data-stu-id="b5ac1-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="b5ac1-108">O pipeline de Autenticação Básica WinRM é utilizado para o transporte de tokens de Autenticação Moderna.</span><span class="sxs-lookup"><span data-stu-id="b5ac1-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="b5ac1-109">Se a Autenticação Básica WinRM estiver desativada no computador cliente, os novos cmdlets V2 continuarão a funcionar (mas os cmdlets RPS mais antigos não funcionarão).</span><span class="sxs-lookup"><span data-stu-id="b5ac1-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
