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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446702"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP poderá necessitar de um tipo personalizado

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

**O DLP pode exigir um tipo de informações personalizado**

Com uma política de prevenção de perda de dados (DLP), pode identificar e proteger dados confidenciais na sua organização. Em alguns cenários, poderá ter de criar o seu próprio tipo de informações confidenciais personalizado para proteger os dados da sua organização. Para obter mais informações, consulte Obter [informações sobre tipos de informações confidenciais](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) e [Definições de entidades](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)de tipo de informação sensível.

Para obter mais informações sobre como criar políticas e tipos de informação confidenciais personalizados, consulte: 

**Personalizar um tipo de informação confidencial incorporado**

Se um tipo de informação confidencial incorporado se adeque às suas necessidades com apenas algumas otimizações, consulte Personalizar um tipo de informação [confidencial incorporado.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Por exemplo, pode adicionar ou remover palavras-chave ou adicionar ou remover provas de suporte, como uma data ou endereço.

**Criar um tipo de informações confidenciais personalizado**

No entanto, se precisar de identificar e proteger um tipo diferente de informações confidenciais, pode criar um tipo de informação confidencial personalizado no Centro de Conformidade do Microsoft 365. Para obter mais informações, consulte [Começar a trabalhar com tipos de informação confidenciais personalizados.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Criar um tipo de informações confidenciais personalizado no PowerShell do & de Conformidade e Segurança**

Por fim, se a interface de utilizador não fornecer todas as opções de que precisa, pode criar um tipo de informações confidenciais personalizado no PowerShell do centro de & de Conformidade. Ao começar com um ficheiro XML, pode utilizar todas as opções disponíveis. Para obter mais informações, consulte [Criar um tipo de informação confidencial personalizado com o PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Para primeiro testar a sua política no modo de teste, consulte [Implementar](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) política no modo de teste e Criar, testar e [ajustar uma política DLP.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 