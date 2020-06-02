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
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507525"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP pode precisar de um tipo personalizado

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**DLP pode exigir um tipo de informação personalizada**

Com uma política de prevenção de perda de dados (DLP), pode identificar e proteger dados sensíveis na sua organização. Em alguns cenários, poderá ser necessário criar o seu próprio tipo **de** informação personalizada e sensível para proteger os dados da sua organização.

Por exemplo, a sua organização poderá necessitar de identificar e proteger iDs de funcionários ou outros dados em algum formato específico do seu org. Em caso afirmativo, consulte os seguintes artigos para obter mais informações.
  
 **Personalize um tipo de informação sensível incorporada**
  
Se um tipo de informação sensível incorporada satisfaça as suas necessidades com apenas alguns ajustes, pode [personalizar um tipo de informação sensível incorporada](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Por exemplo, pode adicionar ou remover palavras-chave, ou adicionar ou remover provas de suporte, como uma data ou endereço.
  
 **Criar um tipo de informação sensível personalizada**
  
Mas se precisar identificar e proteger um tipo diferente de informação sensível, pode [criar um tipo de informação sensível personalizada](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) na UI do Centro de Conformidade & de Segurança.
  
**Criar um tipo de informação sensível personalizada no Centro de Conformidade & Segurança PowerShell**

Finalmente, se a UI não fornecer todas as opções necessárias, pode [criar um tipo de informação sensível personalizada em Segurança & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Ao começar com um ficheiro XML, pode utilizar todas as opções disponíveis.
