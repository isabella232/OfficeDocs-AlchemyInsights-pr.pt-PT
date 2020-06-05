---
title: Problemas de sessão nas aplicações da Microsoft 365
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
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579876"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="7a309-102">Correção das aplicações Microsoft 365 "O módulo plataforma fidedigno do computador não está a funcionar corretamente"</span><span class="sxs-lookup"><span data-stu-id="7a309-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="7a309-103">Para corrigir este erro, experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="7a309-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7a309-104">Instale as atualizações mais recentes para [windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="7a309-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7a309-105">[Credenciais de Escritório Claro](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando Gestor credencial do Windows.</span><span class="sxs-lookup"><span data-stu-id="7a309-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7a309-106">**Nota:** Os percursos de registo do Office 2016 mudaram para 16,0.</span><span class="sxs-lookup"><span data-stu-id="7a309-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7a309-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identidade\)</span><span class="sxs-lookup"><span data-stu-id="7a309-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7a309-108">Experimente o [processo de recuperação](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) do utilizador para corrigir falhas no Módulo de Plataforma Fidedigna (TPM).</span><span class="sxs-lookup"><span data-stu-id="7a309-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="7a309-109">Desa estavido o EnableADAL = 0 utilizando os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="7a309-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="7a309-110">Clique com o botão Iniciar o Windows, escolha **Executar,** escreva **regedit**e, em seguida, escolha **OK**.</span><span class="sxs-lookup"><span data-stu-id="7a309-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="7a309-111">Selecione **Sim** para permitir que o Editor de Registo escora alterações no seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7a309-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7a309-112">No Editor de Registos, adicione um valor DWORD de **EnableADAL** com uma definição de **0** em HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identidade.</span><span class="sxs-lookup"><span data-stu-id="7a309-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="7a309-113">Para obter mais informações, consulte [os problemas de ligação no sôm-in após a atualização do Office 2016 construir 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="7a309-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>