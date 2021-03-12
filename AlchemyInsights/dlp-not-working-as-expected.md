---
title: DLP não funciona como esperado
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707821"
---
# <a name="dlp-not-working-as-expected"></a>DLP não funciona como esperado

**Importante**: durante estes tempos sem precedentes, estamos a tomar medidas para garantir que os serviços SharePoint Online e OneDrive permaneçam com elevada disponibilidade. Para obter mais informações, visite [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) (Ajustes Temporários de Funcionalidades do SharePoint Online).

 **Criação de DLP**

Está a ter problemas com **a Prevenção de Perdas de Dados (DLP)** no Office 365 que não funciona como esperado? Em caso afirmativo, certifique-se de que a sua **política DLP** está corretamente configurada e que os seus dados contêm o que a **política de DLP** procura quando está a ser avaliada.
  
As políticas de DLP permitem identificar e proteger informações sensíveis na sua organização. Para configurar as políticas DLP, utilize a informação [aqui.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **O que as políticas de DLP procuram**
  
Ao utilizar os **tipos de informação sensível incorporados** nos centros de Segurança e Conformidade, as políticas DLP procuram padrões e elementos específicos ao detetar estes tipos sensíveis.
  
- **Tipos de informação sensível incorporados**

    Para obter informações sobre os tipos sensíveis incorporados e sobre o que uma política DLP procura ao detetar o tipo Sensível, consulte: [O que os tipos de informação sensíveis procuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipos de informação sensível personalizados**

    Se estiver a tentar criar tipos de informação sensíveis personalizados, utilize o seguinte artigo para obter informações sobre como criar um tipo de informação sensível personalizado: [Criar um tipo de informação sensível personalizado](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testar uma política de DLP**

Para testar os seus dados com um tipo de informação sensível incorporada ou personalizada, utilize a opção **tipo teste** em **classificações**  >  **Tipos de informação sensíveis**. Para obter mais informações, consulte [test tipos de informações sensíveis personalizadas.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Relatórios**
  
- Obtenha informações confidenciais de dados com [relatórios DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Consulte detalhes específicos do evento com um [Relatório de Incidentes.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
