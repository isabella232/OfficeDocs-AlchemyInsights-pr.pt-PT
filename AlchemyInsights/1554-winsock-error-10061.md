---
title: Erro de Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903118"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="de129-102">Erro de Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="de129-102">Winsock error 10061</span></span>

<span data-ttu-id="de129-p101">Este código de erro significa que o Office 365 não foi possível estabelecer um socket TCP (ligação) com o anfitrião de destino. A causa mais provável deste erro é um problema com a configuração do firewall. Para corrigir o problema, verifique estas definições:</span><span class="sxs-lookup"><span data-stu-id="de129-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="de129-106">Verifique a configuração de firewall com as informações no [Office 365 URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="de129-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="de129-107">Se o erro é específico para Exchange Online protecção (EOP), deve tiver sido previamente notificado a uma alteração para os [endereços IP de protecção Online do Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="de129-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="de129-108">Certifique-se de que o fornecedor de serviços Internet (ISP) não está a bloquear a porta.</span><span class="sxs-lookup"><span data-stu-id="de129-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="de129-109">Verifique as definições de servidor de anfitrião e de destino inteligentes os conectores.</span><span class="sxs-lookup"><span data-stu-id="de129-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="de129-110">Tenha em atenção que o Office 365 não bloquear ligações a *receber* desta forma.</span><span class="sxs-lookup"><span data-stu-id="de129-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

