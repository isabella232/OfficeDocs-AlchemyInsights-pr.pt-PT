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
# <a name="winsock-error-10061"></a>Erro winsock 10061

Este código de erro significa que a Microsoft não conseguiu estabelecer uma tomada TCP (ligação) com o anfitrião alvo. A causa mais provável deste erro é um problema com a configuração da firewall. Para corrigir o problema, verifique estas definições:

- Verifique a configuração da sua firewall com as informações nas [gamas Microsoft 365 URLs e IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Se o erro for específico para a Troca de Proteção Online (EOP), deverá ter sido previamente notificado para uma alteração aos endereços IP de [Proteção Online de Troca](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verifique se o seu Fornecedor de Serviços de Internet (ISP) não está a bloquear a porta.

- Verifique as definições do anfitrião inteligente e do servidor de destino nos seus conectores.

Note que o Microsoft 365 não bloqueia as ligações de *entrada* desta forma.
