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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655293"
---
# <a name="data-location"></a>Localização de dados

Pode ver a localização do seu inquilino no centro de administração ou ligando-se ao Exchange Online via PowerShell.


**Centro de administração:**
1. Faça login no [centro de administração](https://admin.microsoft.com/Adminportal/Home).
2. Selecione o perfil da**Organização** **de Definições** > .
3. Em **termos de localização de Dados,** selecione Ver **detalhes**.


**PowerShell:**
1. Ligue-se ao Exchange Online utilizando o Windows PowerShell.
2. Execute o cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) para apresentar uma lista das propriedades do seu inquilino. 
3. Olhe para a propriedade OrganizationId.

Quando tiver a localização dos dados para EXO e SPO, pode determinar a localização dos dados para outros serviços que poderá utilizar a partir de [onde os seus dados estão localizados](https://products.office.com/where-is-your-data-located).