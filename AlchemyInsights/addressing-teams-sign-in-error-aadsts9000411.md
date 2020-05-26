---
title: Endereçamento de equipas de erro de inscrição AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357873"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Endereçamento de equipas de erro de inscrição AADSTS9000411

Ao iniciar sessão no Microsoft Teams, pode receber o erro: **Desculpe, mas estamos com dificuldades em contratá-lo em AADSTS900411: O pedido não está devidamente formatado. O parâmetro "login_hint" é duplicado.**

Para resolver este problema, certifique-se de que os seus clientes da Microsoft Teams estão atualizados. Para obter mais informações sobre a atualização do seu cliente, consulte [Atualizar as Equipas microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Se não conseguir atualizar o seu cliente por alguma razão, o registo do cliente irá limpar a maioria dos dados em cache. No entanto, se ainda tiver problemas após o logoff/logon, desista das Equipas e, por favor, limpe a cache do seu cliente fazendo o seguinte:
1. Feche as equipas da Microsoft.
2. Vá a: %appdata%\microsoft\teams e delete todos os ficheiros.
3. Reabra as Equipas microsoft.
