---
title: Corrigindo aplicativos do Office Desculpe, estamos tendo mensagem temporária de problemas de servidor
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628001"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="4b036-102">Corrigindo os aplicativos do Office "Desculpe, estamos tendo problemas temporários de servidor" mensagem</span><span class="sxs-lookup"><span data-stu-id="4b036-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="4b036-103">Se você receber esta mensagem, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4b036-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4b036-104">Verifique seu firewall, software antivírus e configurações de proxy para confirmar que eles não estão bloqueando o acesso à Internet aos aplicativos do Office.</span><span class="sxs-lookup"><span data-stu-id="4b036-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="4b036-105">Veja [o Office 365 URLs e as faixas](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)de endereço IP.</span><span class="sxs-lookup"><span data-stu-id="4b036-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="4b036-106">Vá para **iniciar** > **a corrida,** e depois digite **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="4b036-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="4b036-107">Certifique-se de que os seguintes serviços estão todos em execução:</span><span class="sxs-lookup"><span data-stu-id="4b036-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="4b036-108">Configuração automática de dispositivos conectados à rede</span><span class="sxs-lookup"><span data-stu-id="4b036-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="4b036-109">Serviço de lista de rede</span><span class="sxs-lookup"><span data-stu-id="4b036-109">Network List Service</span></span>
    - <span data-ttu-id="4b036-110">Conscientização de localização da rede</span><span class="sxs-lookup"><span data-stu-id="4b036-110">Network Location Awareness</span></span>
    - <span data-ttu-id="4b036-111">Registro do evento de Windows</span><span class="sxs-lookup"><span data-stu-id="4b036-111">Windows Event Log</span></span>

<span data-ttu-id="4b036-112">Se um desses serviços não estiver funcionando, tente iniciá-lo.</span><span class="sxs-lookup"><span data-stu-id="4b036-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="4b036-113">Se você tiver um problema para iniciar o serviço, execute o comando a seguir, abrindo uma solicitação de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="4b036-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="4b036-114">**sfc /scannow Sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="4b036-114">**sfc /scannow**</span></span>

<span data-ttu-id="4b036-115">Após este comando terminar, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="4b036-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="4b036-116">Para obter informações detalhadas, [consulte "Desculpe, não podemos nos conectar à sua conta. Por favor, tente novamente mais tarde" erro quando você ativar office do Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="4b036-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>