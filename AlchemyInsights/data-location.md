---
title: Localização dos dados
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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207272"
---
# <a name="data-location"></a>Localização dos dados

Você pode exibir o local do seu locatário do Office 365 no centro de administração ou conectando-se ao Exchange Online por meio do PowerShell.


**Centro de administração:**
1. Faça login no [centro de administração](https://admin.microsoft.com/Adminportal/Home).
2. Selecione **configurações** > **perfil da organização**.
3. Em **local de dados**, selecione **Exibir detalhes**.


**Powershell:**
1. Conecte-se ao Exchange Online usando o Windows PowerShell.
2. Execute o cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) para exibir uma lista das propriedades do locatário. 
3. Veja a propriedade OrganizationId.

Quando você tem o local de dados para EXO e SPO, você pode determinar o local de dados para outros serviços que você pode usar de [onde seus dados estão localizados](https://products.office.com/where-is-your-data-located).