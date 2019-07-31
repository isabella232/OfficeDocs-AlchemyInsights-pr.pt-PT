---
title: DLP não funcionar conforme esperado
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
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941079"
---
# <a name="dlp-not-working-as-expected"></a>DLP não funcionar conforme esperado

Está a ter problemas com o **Data Loss Prevention (DLP)** no Office 365 não funcionar conforme esperado? Se assim for, certifique-se de que a **política do DLP** está configurado correctamente e que os seus dados contiverem que a **política do DLP** está à procura quando este está a ser avaliada.
  
 **Configurar DLP**
  
Políticas do DLP permite-lhe identificar e proteger informações confidenciais na sua organização. Para configurar as políticas do DLP, utilize as informações [aqui](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **O que procuram políticas DLP**
  
Quando utilizar os **tipos de informações sensíveis incorporada** no Centro de segurança do Office 365 e conformidade, as políticas do DLP procuram padrões específicos e elementos quando detectar estes tipos sensíveis.
  
- **Tipos de informações sensíveis incorporada**

    Para obter informações sobre os tipos de sensíveis incorporados e o que uma política do DLP procura quando detectar o tipo sensível, consulte: [procuram a que os tipos de informações sensíveis](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Tipos de informações sensíveis personalizadas**

    Se está a tentar criar tipos de informações sensíveis personalizadas, utilize o seguinte artigo para obter informações sobre como criar um tipo personalizado sensível: [criar um tipo de informações sensíveis personalizadas](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Teste uma política do DLP**

Para testar os seus dados com um tipo de informações sensíveis incorporados ou personalizados, utilize a opção de **tipo de teste** em **classificações** > **tipos de informações sensíveis**. Para mais informações, consulte [tipos de informações sensíveis personalizadas de ensaio](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Relatórios**
  
- Obter conhecimentos aprofundados de dados importantes com [relatórios do DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Ver detalhes do evento com um [Relatório de acidente](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
