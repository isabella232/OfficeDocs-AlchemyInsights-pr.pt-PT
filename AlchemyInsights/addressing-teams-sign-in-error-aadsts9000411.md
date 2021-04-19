---
title: Endereço de erro de inscrição das equipas AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821998"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Endereço de erro de inscrição das equipas AADSTS9000411

Ao iniciar sessão no Microsoft Teams, poderá receber o erro: **Desculpe, mas estamos com dificuldades em contratá-lo no AADSTS9000411: O pedido não está devidamente formatado. O parâmetro "login_hint" é duplicado.**

Para resolver este problema, certifique-se de que os seus clientes Microsoft Teams estão atualizados. Para obter mais informações sobre a atualização do seu cliente, consulte [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Se não conseguir atualizar o seu cliente por alguma razão, o registo do cliente limpará a maioria dos dados em cache. No entanto, se ainda tiver problemas após o logoff/início de são, saia das Equipas e, por favor, limpe a cache do seu cliente fazendo o seguinte:
1. Feche as equipas da Microsoft.
2. Aceda a: %appdata%\microsoft\microsoft\teams e elimine todos os ficheiros.
3. Reabrir equipas da Microsoft.
