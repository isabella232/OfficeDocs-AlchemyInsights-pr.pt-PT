---
title: Problemas de início de sessão em aplicações do Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938304"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="16026-102">Corrigir a mensagem de "módulo de plataforma fidedigna do computador não está a funcionar correctamente" de aplicações do Office</span><span class="sxs-lookup"><span data-stu-id="16026-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="16026-103">Para corrigir este erro, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="16026-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="16026-104">Instale as actualizações mais recentes para o [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="16026-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="16026-105">[Office Limpar credenciais](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizando o Gestor de credenciais do Windows.</span><span class="sxs-lookup"><span data-stu-id="16026-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="16026-106">**Nota:** Os caminhos de registo para o Office 2016 foram alterados para 16,0.</span><span class="sxs-lookup"><span data-stu-id="16026-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="16026-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="16026-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="16026-108">Tente o [processo de recuperação de utilizador](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) para corrigir falhas de Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="16026-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="16026-109">Definir o EnableADAL = 0, utilizando os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="16026-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="16026-110">Botão direito do rato no botão Iniciar do Windows, seleccione **Executar**, escreva **regedit**e, em seguida, escolha **' OK '**.</span><span class="sxs-lookup"><span data-stu-id="16026-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="16026-111">Seleccione **Sim** para permitir que o Editor de registo para efectuar alterações ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="16026-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="16026-112">No Editor de registo, adicione um valor DWORD de **EnableADAL** com uma definição de **0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="16026-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="16026-113">Para mais informações, consulte [problemas de ligação no início de sessão-in após a actualização do Office de 2016 compilação 16.0.7967 10 do Windows](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="16026-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>