---
title: Problema de ativação - Não podemos nos conectar agora
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628253"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="ffdc4-102">Corrigindo os aplicativos do Office "Não podemos nos conectar agora" mensagem</span><span class="sxs-lookup"><span data-stu-id="ffdc4-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="ffdc4-103">Se você receber esta mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ffdc4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ffdc4-104">Verifique seu firewall, software antivírus e configurações de proxy para confirmar que eles não estão bloqueando o acesso à Internet aos aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="ffdc4-105">Veja [o Office 365 URLs e as faixas](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)de endereço IP.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ffdc4-106">Vá para **iniciar** > **a corrida,** e depois digite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ffdc4-107">Certifique-se de que os seguintes serviços estão todos em execução:</span><span class="sxs-lookup"><span data-stu-id="ffdc4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ffdc4-108">Configuração automática de dispositivos conectados à rede</span><span class="sxs-lookup"><span data-stu-id="ffdc4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ffdc4-109">Serviço de lista de rede</span><span class="sxs-lookup"><span data-stu-id="ffdc4-109">Network List Service</span></span>
    - <span data-ttu-id="ffdc4-110">Conscientização de localização da rede</span><span class="sxs-lookup"><span data-stu-id="ffdc4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ffdc4-111">Registro do evento de Windows</span><span class="sxs-lookup"><span data-stu-id="ffdc4-111">Windows Event Log</span></span>

<span data-ttu-id="ffdc4-112">Se um desses serviços não estiver funcionando, tente iniciá-lo.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ffdc4-113">Se você tiver um problema para iniciar o serviço, execute o comando a seguir, abrindo uma solicitação de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="ffdc4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ffdc4-114">**sfc /scannow Sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="ffdc4-114">**sfc /scannow**</span></span>

<span data-ttu-id="ffdc4-115">Após este comando terminar, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ffdc4-116">Para obter informações detalhadas, [consulte "Desculpe, não podemos nos conectar à sua conta. Por favor, tente novamente mais tarde" erro quando você ativar office do Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ffdc4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>