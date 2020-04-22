---
title: Corrigir aplicativos do Office Desculpe, estamos tendo mensagens temporárias de problemas de servidor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764128"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="271e7-102">Corrigir as aplicações do Office "Desculpe, estamos tendo problemas temporários de servidor" mensagem</span><span class="sxs-lookup"><span data-stu-id="271e7-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="271e7-103">Se receber esta mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="271e7-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="271e7-104">Verifique as definições de firewall, software antivírus e proxy para confirmar que não estão a bloquear o acesso à Internet às aplicações do Office.</span><span class="sxs-lookup"><span data-stu-id="271e7-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="271e7-105">Consulte [os intervalos urls e endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="271e7-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="271e7-106">Vá para **Iniciar** > **A Execução**, e, em seguida, digite **serviços.msc**.</span><span class="sxs-lookup"><span data-stu-id="271e7-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="271e7-107">Certifique-se de que os seguintes serviços estão em execução:</span><span class="sxs-lookup"><span data-stu-id="271e7-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="271e7-108">Configuração automática de dispositivos ligados à rede</span><span class="sxs-lookup"><span data-stu-id="271e7-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="271e7-109">Serviço de Lista de Rede</span><span class="sxs-lookup"><span data-stu-id="271e7-109">Network List Service</span></span>
    - <span data-ttu-id="271e7-110">Sensibilização para a localização da rede</span><span class="sxs-lookup"><span data-stu-id="271e7-110">Network Location Awareness</span></span>
    - <span data-ttu-id="271e7-111">Registo de Eventos do Windows</span><span class="sxs-lookup"><span data-stu-id="271e7-111">Windows Event Log</span></span>

<span data-ttu-id="271e7-112">Se um destes serviços não estiver a funcionar, tente iniciá-lo.</span><span class="sxs-lookup"><span data-stu-id="271e7-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="271e7-113">Se tiver algum problema em iniciar o serviço, faça o seguinte comando abrindo um pedido de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="271e7-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="271e7-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="271e7-114">**sfc /scannow**</span></span>

<span data-ttu-id="271e7-115">Depois deste comando terminar, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="271e7-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="271e7-116">Para obter informações detalhadas, consulte ["Desculpe, não podemos ligar-nos à sua conta. Tente novamente mais tarde" erro quando ativar](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="271e7-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>