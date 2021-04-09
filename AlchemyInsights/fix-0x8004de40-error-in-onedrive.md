---
title: Corrigir erro de 0x8004de40 no OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649759"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="8a7d2-102">Corrigir erro de 0x8004de40 no OneDrive</span><span class="sxs-lookup"><span data-stu-id="8a7d2-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="8a7d2-103">Se estiver a executar o Windows 7 e receber este erro, [atualize para ativar o TLS 1.1 e o TLS 1.2 como protocolos seguros predefinidos no WinHTTP no Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="8a7d2-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="8a7d2-104">Se estiver a executar o Windows 10 e receber um erro 0x8004de40 com o OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8a7d2-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="8a7d2-105">Reinicie o computador afetado enquanto estiver ligado ao seu domínio acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="8a7d2-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="8a7d2-106">Se um reboot não corrigir o problema, un un unin e rejoine o seu dispositivo a partir de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a7d2-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="8a7d2-107">**Nota:** Deve estar na sua rede corporativa durante a realização destes passos.</span><span class="sxs-lookup"><span data-stu-id="8a7d2-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="8a7d2-108">Não execute estes passos quando não estiver ligado à sua infraestrutura corporativa (por exemplo, durante a viagem).</span><span class="sxs-lookup"><span data-stu-id="8a7d2-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="8a7d2-109">Abra uma solicitação de comando elevada selecionando **Iniciar**, clique com o botão direito **Command Prompt** e, em seguida, selecione Executar **como administrador**.</span><span class="sxs-lookup"><span data-stu-id="8a7d2-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="8a7d2-110">Tipo *dsregcmd /leave* and press **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8a7d2-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="8a7d2-111">Quando estiver concluído, *escreva /junte-se* e prima **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8a7d2-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="8a7d2-112">Quando estiver completo, feche o aviso de comando.</span><span class="sxs-lookup"><span data-stu-id="8a7d2-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="8a7d2-113">Reinicie o computador e inicie sessão no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8a7d2-113">Reboot the computer, and log into OneDrive.</span></span>