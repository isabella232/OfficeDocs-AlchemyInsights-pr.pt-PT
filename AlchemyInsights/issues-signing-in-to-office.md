---
title: Problemas de sessão nas aplicações da Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695298"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="ed935-102">Ecrã de sindução em branco nas aplicações da Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ed935-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="ed935-103">Para corrigir este problema, experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ed935-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="ed935-104">Instale as atualizações mais recentes para [windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="ed935-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="ed935-105">Redefinir as opções do Internet Explorer: Vá a **Ferramentas**  >  **Opções**de Internet  >  **Advanced**  >  **Versões avançadas do Internet Reset (note** que perderá as definições personalizadas) e tente iniciar novamente a sessão no Office.</span><span class="sxs-lookup"><span data-stu-id="ed935-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="ed935-106">Desative a Proteção de Aplicações do Windows Defender (WDAG) ou qualquer programa semelhante de firewall ou antivírus:</span><span class="sxs-lookup"><span data-stu-id="ed935-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="ed935-107">No Painel de Controlo, vá a Programas e, em seguida, escolha as **funcionalidades** **Turn Windows ligados ou desligados**.</span><span class="sxs-lookup"><span data-stu-id="ed935-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="ed935-108">Se o Windows Defender Application Guard estiver ativado, tente desativá-lo.</span><span class="sxs-lookup"><span data-stu-id="ed935-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="ed935-109">**Nota:** Pode ser necessário reiniciar o computador.</span><span class="sxs-lookup"><span data-stu-id="ed935-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="ed935-110">Certifique-se de que o plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) não está a ser bloqueado por qualquer aplicação ou programa de firewall/antivírus.</span><span class="sxs-lookup"><span data-stu-id="ed935-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="ed935-111">[Credenciais de Escritório Claro](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) usando Gestor credencial do Windows.</span><span class="sxs-lookup"><span data-stu-id="ed935-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ed935-112">**Nota:** Os percursos de registo do Office 2016 mudaram para 16,0.</span><span class="sxs-lookup"><span data-stu-id="ed935-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ed935-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identidade\)</span><span class="sxs-lookup"><span data-stu-id="ed935-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="ed935-114">Para obter mais informações, consulte [os problemas de ligação no sôm-in após a atualização do Office 2016 construir 16.0.7967 no Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="ed935-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>