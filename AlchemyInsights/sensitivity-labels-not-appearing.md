---
title: Rótulos de sensibilidade que não aparecem
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048663"
---
# <a name="sensitivity-labels-not-appearing"></a>Rótulos de sensibilidade que não aparecem

Os rótulos de sensibilidade permitem que você classifique e ajude a proteger seu conteúdo sensível. Eles podem ser criados no centro de conformidade Microsoft 365, no centro de segurança Microsoft 365 ou no Office 365 Security & Compliance Center rótulos de classificação > sensibilidade. Para saber mais sobre esse recurso, consulte [a visão geral dos rótulos de sensibilidade.](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)

Se você configurou seus rótulos de sensibilidade, mas eles não estão aparecendo nos aplicativos do Office, verifique o seguinte:

- Confirme que o rótulo de sensibilidade foi [publicado](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) para os usuários e grupos que você deseja.

- Confirme que o usuário está usando um aplicativo que suporta rótulos de sensibilidade - veja rótulos de [sensibilidade em seu documento.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable)

- Se você está [migrando rótulos de Proteção de Informações Do Azure,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)esteja ciente das considerações listadas [aqui.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Suporte de prevenção de perdas de dados (DLP): Atualmente, apenas os rótulos de retenção podem ser usados como condição nas políticas de DLP.  O suporte para rótulos de sensibilidade em uma política de DLP ainda não está disponível, mas estamos trabalhando nisso.

- Quando a criptografia é ativada em um rótulo de sensibilidade, você pode escolher:
    - Atribuir permissões agora
    - Permitir que os usuários atribuam permissões


Para obter mais informações sobre possíveis problemas, consulte [problemas conhecidos com rótulos](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)de sensibilidade.