---
title: Rótulos de sensibilidade não aparecendo
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207236"
---
# <a name="sensitivity-labels-not-appearing"></a>Rótulos de sensibilidade não aparecendo

Os rótulos de sensibilidade permitem classificar e ajudar a proteger seu conteúdo confidencial. Eles podem ser criados no centro de conformidade da Microsoft 365, no centro de segurança da Microsoft 365 ou no Office 365 Security & Compliance Center em rótulos de classificação > sensibilidade. Para saber mais sobre esse recurso, consulte [visão geral dos rótulos de sensibilidade](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Se você configurou seus rótulos de sensibilidade, mas eles não estiverem aparecendo nos aplicativos do Office, verifique o seguinte:

- Confirme se o rótulo de sensibilidade foi [publicado](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) para os usuários e grupos que você deseja.

- Confirme se o usuário está usando um aplicativo que ofereça suporte a rótulos de sensibilidade-consulte [Rótulos de sensibilidade no documento](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Se você estiver [migrando rótulos de proteção de informações do Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), esteja ciente das considerações listadas [aqui](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Suporte a prevenção de perda de dados (DLP): atualmente, somente os rótulos de retenção podem ser usados como uma condição em políticas de DLP.  Suporte para rótulos de sensibilidade em uma política de DLP ainda não está disponível, mas estamos trabalhando nele.

- Quando a criptografia é habilitada em um rótulo de sensibilidade, você pode escolher:
    - Atribua permissões agora
    - Permitir que os usuários atribuam permissões


Para obter mais informações sobre possíveis problemas, consulte [problemas conhecidos com rótulos de sensibilidade](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).