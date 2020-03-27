---
title: DLP não funciona como esperado
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977449"
---
# <a name="dlp-not-working-as-expected"></a>DLP não funciona como esperado

**Importante**: Durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permanecem altamente disponíveis – Visite os Ajustes de [FuncionalidadeS Temporárias Online SharePoint](https://aka.ms/ODSPAdjustments) para obter mais informações.

 **Criação de DLP**

Está a ter problemas com a Prevenção de Perdas de **Dados (DLP)** no Office 365 que não está a funcionar como esperado? Em caso afirmativo, certifique-se de que a sua **política de DLP** está corretamente configurada e que os seus dados contêm o que a **política do DLP** procura quando está a ser avaliada.
  
As políticas de DLP permitem identificar e proteger informações sensíveis na sua organização. Para configurar políticas de DLP, use a informação [aqui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **O que as políticas do DLP procuram**
  
Ao utilizar os **tipos de informação sensível incorporados** no Office 365 Security and Compliance center, as políticas de DLP procuram padrões e elementos específicos ao detetar estes tipos sensíveis.
  
- **Tipos de informação sensível incorporados**

    Para obter informações sobre os tipos sensíveis incorporados e o que uma política de DLP procura ao detetar o tipo Sensível, consulte: O que os [tipos de informação sensíveis procuram](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Tipos de informação sensível personalizado**

    Se estiver a tentar criar tipos de informação sensíveis personalizados, utilize o seguinte artigo para obter informações sobre como criar um tipo de [informação sensível personalizada: Criar um tipo](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)de informação sensível personalizado .

**Teste uma política de DLP**

Para testar os seus dados com um tipo de informação sensível incorporada ou personalizada, utilize a opção **do tipo Teste** em tipos de**informação sensíveis**de **classificações** > . Para mais informações, consulte os tipos de [informação personalizadas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Relatórios**
  
- Obtenha informações confidenciais de dados com [relatórios DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Consulte detalhes específicos do evento com um Relatório de [Incidentes](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
