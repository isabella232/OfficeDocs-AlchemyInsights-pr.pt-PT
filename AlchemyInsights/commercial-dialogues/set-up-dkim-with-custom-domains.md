---
title: Configurar o DKIM com domínios personalizados
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332318"
---
# <a name="set-up-dkim-with-custom-domains"></a>Configurar o DKIM com domínios personalizados

Tem de publicar dois registos CNAME para cada domínio personalizado no DNS. Para fazê-lo, utilize o seguinte formato:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Nota:** **DomainGUID** é o texto à esquerda de **.mail.protection.outlook.com** no registo MX personalizado do domínio personalizado (por exemplo, contoso-com para o domínio **contoso.com**). **InitialDomain é** o domínio que usou quando se inscreveu no Office 365 (por exemplo, **contoso.onmicrosoft.com**).

Para obter mais informações sobre os registos DNS, consulte Criar registos DNS em qualquer fornecedor de [anfitrião DNS Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)