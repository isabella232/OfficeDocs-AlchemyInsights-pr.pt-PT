---
title: Sincronização de palavras-passe de resolução de problemas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387888"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="c3efb-102">Sincronização de palavras-passe de resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="c3efb-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="c3efb-103">Para resolver problemas de sincronização de palavras-passe, comece por utilizar esta tarefa de resolução de problemas do AAD Connect para determinar por que razão as palavras-passe não estão a sincronizar.</span><span class="sxs-lookup"><span data-stu-id="c3efb-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="c3efb-104">Para começar, vá para [Gerir a sincronização direta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="c3efb-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="c3efb-105">Abra uma nova sessão Windows PowerShell no seu servidor Azure AD Connect e selecione a opção **Executar como Administrador.**</span><span class="sxs-lookup"><span data-stu-id="c3efb-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="c3efb-106">Executar Set-ExecuçãoPolítica RemoteSigned ou Set-ExecutionPolicy Sem restrições.</span><span class="sxs-lookup"><span data-stu-id="c3efb-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="c3efb-107">Inicie o assistente Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c3efb-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="c3efb-108">Aceda à página Tarefas Adicionais > **Resolução de Problemas**  >  **Em seguida**.</span><span class="sxs-lookup"><span data-stu-id="c3efb-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="c3efb-109">Selecione **Lançamento** para abrir o menu de resolução de problemas powerShell.</span><span class="sxs-lookup"><span data-stu-id="c3efb-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="c3efb-110">Selecione **A sincronização da palavra-passe de resolução de problemas**.</span><span class="sxs-lookup"><span data-stu-id="c3efb-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="c3efb-111">O problema é que uma palavra-passe não é sincronizada para uma conta de utilizador específica.</span><span class="sxs-lookup"><span data-stu-id="c3efb-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="c3efb-112">**Notas** A sincronização da palavra-passe falha se a última sincronização de senhas bem sucedidas foi há algum tempo.</span><span class="sxs-lookup"><span data-stu-id="c3efb-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="c3efb-113">Para obter mais ajuda para resolver problemas na sincronização da palavra-passe, consulte [a sincronização de hash de resolução de palavras-passe com sincronização Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c3efb-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>