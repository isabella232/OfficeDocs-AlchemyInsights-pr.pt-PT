---
title: 1554 Winsock erro 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766180"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="9b4f4-102">Erro winsock 10061</span><span class="sxs-lookup"><span data-stu-id="9b4f4-102">Winsock error 10061</span></span>

<span data-ttu-id="9b4f4-103">Este código de erro significa que a Microsoft não conseguiu estabelecer uma tomada TCP (ligação) com o anfitrião alvo.</span><span class="sxs-lookup"><span data-stu-id="9b4f4-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="9b4f4-104">A causa mais provável deste erro é um problema com a configuração da firewall.</span><span class="sxs-lookup"><span data-stu-id="9b4f4-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="9b4f4-105">Para corrigir o problema, verifique estas definições:</span><span class="sxs-lookup"><span data-stu-id="9b4f4-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="9b4f4-106">Verifique a configuração da sua firewall com as informações nas [gamas Microsoft 365 URLs e IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="9b4f4-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="9b4f4-107">Se o erro for específico para a Troca de Proteção Online (EOP), deverá ter sido previamente notificado para uma alteração aos endereços IP de [Proteção Online de Troca](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9b4f4-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="9b4f4-108">Verifique se o seu Fornecedor de Serviços de Internet (ISP) não está a bloquear a porta.</span><span class="sxs-lookup"><span data-stu-id="9b4f4-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="9b4f4-109">Verifique as definições do anfitrião inteligente e do servidor de destino nos seus conectores.</span><span class="sxs-lookup"><span data-stu-id="9b4f4-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="9b4f4-110">Note que o Microsoft 365 não bloqueia as ligações de *entrada* desta forma.</span><span class="sxs-lookup"><span data-stu-id="9b4f4-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
