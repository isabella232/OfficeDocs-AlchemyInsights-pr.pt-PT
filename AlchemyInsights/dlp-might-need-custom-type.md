---
title: DLP pode precisar de um tipo personalizado
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704500"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP pode precisar de um tipo personalizado

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**DLP pode requerer um tipo de informação personalizada**

Com uma política de prevenção de perdas de dados (DLP), pode identificar e proteger dados sensíveis na sua organização. Em alguns cenários, poderá ser necessário criar o seu **próprio** tipo de informação personalizada e sensível para proteger os dados da sua organização.

Por exemplo, a sua organização pode precisar de identificar e proteger iDs ou outros dados de funcionários em algum formato específico do seu org. Em caso afirmativo, consulte os seguintes artigos para obter mais informações.
  
 **Personalize um tipo de informação sensível incorporada**
  
Se um tipo de informação sensível incorporado atender às suas necessidades com apenas alguns ajustes, pode [personalizar um tipo de informação sensível incorporado](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Por exemplo, pode adicionar ou remover palavras-chave, ou adicionar ou remover provas de apoio, como uma data ou endereço.
  
 **Criar um tipo de informação sensível personalizado**
  
Mas se precisar de identificar e proteger completamente um tipo diferente de informação sensível, pode criar um tipo de [informação sensível personalizado](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) na UI do Centro de Conformidade & Segurança.
  
**Criar um tipo de informação sensível personalizado em Security & Compliance Center PowerShell**

Finalmente, se o UI não fornecer todas as opções de que necessita, pode criar um tipo de [informação sensível personalizado em Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Ao começar com um ficheiro XML, pode utilizar todas as opções disponíveis.
