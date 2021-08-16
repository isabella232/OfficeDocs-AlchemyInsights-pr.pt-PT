---
title: DLP poderá necessitar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030805"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP poderá necessitar de um tipo personalizado

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**O DLP pode exigir um tipo de informações personalizado**

Com uma política de prevenção de perda de dados (DLP), pode identificar e proteger dados confidenciais na sua organização. Em alguns cenários, poderá ter de criar o seu **próprio** tipo de informações confidenciais personalizado para proteger os dados da sua organização.

Por exemplo, a sua organização poderá precisar de identificar e proteger IDs de colaboradores ou outros dados em algum formato específico da sua organização. Se for o caso, consulte os seguintes artigos para obter mais informações.
  
 **Personalizar um tipo de informação confidencial incorporado**
  
Se um tipo de informação confidencial incorporado se adeque às suas necessidades com apenas algumas otimizações, pode personalizar um tipo de informação [confidencial incorporado.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Por exemplo, pode adicionar ou remover palavras-chave ou adicionar ou remover provas de suporte, como uma data ou endereço.
  
 **Criar um tipo de informações confidenciais personalizado**
  
No entanto, se precisar de identificar e proteger um tipo [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) diferente de informações confidenciais, pode criar um tipo de informação confidencial personalizado na IU do Centro de Conformidade & segurança.
  
**Criar um tipo de informações confidenciais personalizado no PowerShell & Segurança**

Por fim, se a IU não fornecer todas as opções de que precisa, pode criar um tipo de informações confidenciais personalizado no [PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)do & de Conformidade. Ao começar com um ficheiro XML, pode utilizar todas as opções disponíveis.
