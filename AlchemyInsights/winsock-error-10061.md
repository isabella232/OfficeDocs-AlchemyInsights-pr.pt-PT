---
title: 1554 Winsock erro 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698873"
---
# <a name="winsock-error-10061"></a>Winsock error 10061

Este código de erro significa que a Microsoft não conseguiu estabelecer uma tomada TCP (ligação) com o anfitrião-alvo. A causa mais provável deste erro é um problema com a configuração da sua firewall. Para corrigir o problema, verifique estas definições:

- Verifique a sua configuração de firewall com as informações nos [intervalos de URLs e IP da Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Se o erro for específico da Exchange Online Protection (EOP), deveria ter sido previamente notificado para uma alteração dos [endereços IP da Proteção Online de Troca](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verifique se o seu Fornecedor de Serviços de Internet (ISP) não está a bloquear a porta.

- Verifique as definições do anfitrião inteligente e do servidor alvo nos seus conectores.

Note que o Microsoft 365 não bloqueia as ligações *de entrada* desta forma.
