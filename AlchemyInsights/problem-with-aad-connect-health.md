---
title: Problema com a AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482074"
---
# <a name="problem-with-aad-connect-health"></a>Problema com a AAD Connect Health

- Certifique-se de que está autorizado a realizar a operação. Os Administradores Globais têm acesso por defeito. Além disso, pode utilizar [o Controlo de Acesso Baseado em Função](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) para delegar a permissão de registo ao Contribuinte.
- Certifique-se de que os pontos finais necessários estão ativados e não bloqueados devido à firewall. Para mais [informações, consulte os requisitos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- O registo pode falhar devido à comunicação de saída ser submetida a inspeção SSL pela camada de rede.
- Certifique-se de que verificou as definições de notificação para Azure AD Connect Health. Por favor, reveja a sua configuração. Este [guia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) pode ajudá-lo a entender como configurar as definições de notificação para notificações de saúde Azure AD Connect.
- Para saber mais sobre o relatório de sincronização do AAD Connect Health e como descarregá-lo, consulte [o relatório de sincronização do nível de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Para resolver os alertas de problemas da AAD Connect Health, siga [o guia de resolução de problemas para alertas de frescura de dados AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e para perguntas comumente feitas, consulte [questões de instalação de instalação Common AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
