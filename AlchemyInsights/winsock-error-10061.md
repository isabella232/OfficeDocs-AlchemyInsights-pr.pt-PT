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
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772452"
---
# <a name="winsock-error-10061"></a>Erro de Winsock 10061

Este código de erro significa que o Office 365 não foi possível estabelecer um socket TCP (ligação) com o anfitrião de destino. A causa mais provável deste erro é um problema com a configuração do firewall. Para corrigir o problema, verifique estas definições:
  
- Verifique a configuração de firewall com as informações no [Office 365 URLs e intervalos de endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Se o erro é específico para Exchange Online protecção (EOP), deve tiver sido previamente notificado a uma alteração para os [endereços IP de protecção Online do Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Certifique-se de que o fornecedor de serviços Internet (ISP) não está a bloquear a porta.
    
- Verifique as definições de servidor de anfitrião e de destino inteligentes os conectores.
    
Tenha em atenção que o Office 365 não bloquear ligações a *receber* desta forma. 
  

