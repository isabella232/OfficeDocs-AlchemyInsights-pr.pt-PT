---
title: 1554 Erro 10061 do Winsock
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083241"
---
# <a name="winsock-error-10061"></a>Erro 10061 do Winsock

Este código de erro significa que a Microsoft não conseguiu estabelecer uma socket TCP (ligação) com o anfitrião de destino. A causa mais provável deste erro é um problema na sua configuração da firewall. Para corrigir o problema, verifique estas definições:

- Verificar a configuração da firewall com as informações nos [Microsoft 365 intervalos de URLs e endereços IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Se o erro for específico do Proteção do Exchange Online (EOP), deverá ter sido anteriormente notificado para uma alteração aos [endereços IP da Proteção do Exchange Online.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Verifique se o seu Fornecedor de Serviços Internet (ISP) não está a bloquear a porta.

- Verifique as definições de servidor de destino e anfitrião inteligentes nos seus conectores.

Tenha em atenção Microsoft 365 não *bloqueia as ligações* recebidas desta forma.
