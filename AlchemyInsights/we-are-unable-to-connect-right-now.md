---
title: Problema de Ativação - Não podemos nos conectar agora
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725994"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="ef822-102">Correção da mensagem das aplicações Microsoft 365 "Não conseguimos ligar-nos agora"</span><span class="sxs-lookup"><span data-stu-id="ef822-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="ef822-103">Se receber esta mensagem, experimente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ef822-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ef822-104">Verifique as definições de firewall, antivírus e proxy para confirmar que não estão a bloquear o acesso à Internet às aplicações da Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ef822-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="ef822-105">Consulte [os intervalos de endereços Microsoft URLs e IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ef822-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ef822-106">Ir para **start**  >  **run**e, em seguida, escrever **serviços.msc**.</span><span class="sxs-lookup"><span data-stu-id="ef822-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ef822-107">Certifique-se de que todos os seguintes serviços estão em funcionamento:</span><span class="sxs-lookup"><span data-stu-id="ef822-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ef822-108">Configuração automática de dispositivos ligados à rede</span><span class="sxs-lookup"><span data-stu-id="ef822-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ef822-109">Serviço de Lista de Rede</span><span class="sxs-lookup"><span data-stu-id="ef822-109">Network List Service</span></span>
    - <span data-ttu-id="ef822-110">Consciência de localização da rede</span><span class="sxs-lookup"><span data-stu-id="ef822-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ef822-111">Registo de eventos do Windows</span><span class="sxs-lookup"><span data-stu-id="ef822-111">Windows Event Log</span></span>

<span data-ttu-id="ef822-112">Se um destes serviços não estiver a funcionar, tente iniciá-lo.</span><span class="sxs-lookup"><span data-stu-id="ef822-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ef822-113">Se tiver algum problema em iniciar o serviço, executar o seguinte comando abrindo um pedido de comando com permissões elevadas:</span><span class="sxs-lookup"><span data-stu-id="ef822-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ef822-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="ef822-114">**sfc /scannow**</span></span>

<span data-ttu-id="ef822-115">Depois de terminar este comando, reinicie o computador.</span><span class="sxs-lookup"><span data-stu-id="ef822-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ef822-116">Para obter informações detalhadas, consulte ["Desculpe, não podemos ligar-nos à sua conta. Tente novamente mais tarde" erro quando ativar o Office a partir do Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ef822-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>