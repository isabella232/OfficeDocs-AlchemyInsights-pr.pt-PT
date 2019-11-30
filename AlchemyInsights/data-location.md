---
title: Localização de dados
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627857"
---
# <a name="data-location"></a>Localização de dados

Você pode visualizar a localização do seu inquilino do Office 365 no centro de administração ou conectando-se ao Exchange Online via PowerShell.


**Centro de administração:**
1. Faça login no [centro de administração.](https://admin.microsoft.com/Adminportal/Home)
2. Selecione o perfil da**Organização**de **Configurações** > .
3. De acordo com **a localização**dos dados, selecione **detalhes de exibição.**


**Powershell:**
1. Conecte-se ao Intercâmbio On-line usando o Windows PowerShell.
2. Execute o cmdlet [get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) para exibir uma lista de propriedades do seu inquilino. 
3. Olhe para a propriedade OrganizationId.

Quando você tem o local de dados para EXO e SPO, você pode determinar a localização dos dados para outros serviços que você pode usar [de onde seus dados estão localizados.](https://products.office.com/where-is-your-data-located)