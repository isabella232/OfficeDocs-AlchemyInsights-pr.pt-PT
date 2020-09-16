---
title: Corrigir aplicações da Microsoft 365 Desculpe, estamos tendo mensagem temporária de problemas de servidor
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758256"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="9f672-102">Correção das aplicações microsoft 365 "Desculpe, estamos tendo problemas temporários de servidor"</span><span class="sxs-lookup"><span data-stu-id="9f672-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="9f672-103">Se receber esta mensagem, experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="9f672-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9f672-104">Verifique as definições de firewall, antivírus e proxy para confirmar que não estão a bloquear o acesso à Internet às aplicações da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9f672-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9f672-105">Consulte [os intervalos de endereços URLs e IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9f672-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="9f672-106">Ir para **start**  >  **run**e, em seguida, escrever **serviços.msc**.</span><span class="sxs-lookup"><span data-stu-id="9f672-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="9f672-107">Certifique-se de que todos os seguintes serviços estão em funcionamento:</span><span class="sxs-lookup"><span data-stu-id="9f672-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="9f672-108">Configuração automática de dispositivos ligados à rede</span><span class="sxs-lookup"><span data-stu-id="9f672-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="9f672-109">Serviço de Lista de Rede</span><span class="sxs-lookup"><span data-stu-id="9f672-109">Network List Service</span></span>
    - <span data-ttu-id="9f672-110">Consciência de localização da rede</span><span class="sxs-lookup"><span data-stu-id="9f672-110">Network Location Awareness</span></span>
    - <span data-ttu-id="9f672-111">Registo de eventos do Windows</span><span class="sxs-lookup"><span data-stu-id="9f672-111">Windows Event Log</span></span>

<span data-ttu-id="9f672-112">Se um destes serviços não estiver a funcionar, tente iniciá-lo.</span><span class="sxs-lookup"><span data-stu-id="9f672-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="9f672-113">Se tiver algum problema em iniciar o serviço, executar o seguinte comando abrindo um pedido de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="9f672-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="9f672-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="9f672-114">**sfc /scannow**</span></span>

<span data-ttu-id="9f672-115">Depois de terminar este comando, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="9f672-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="9f672-116">Para obter informações detalhadas, consulte ["Desculpe, não podemos ligar-nos à sua conta. Por favor, tente novamente mais tarde" erro quando ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="9f672-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>