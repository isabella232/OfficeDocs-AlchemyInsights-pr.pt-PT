---
title: Notificação AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037240"
---
# <a name="notification-aad-connect"></a>Notificação AAD Connect

- Certifique-se de que está autorizado a realizar a operação. Os Administradores Globais têm acesso por defeito. Além disso, pode utilizar [o Controlo de Acesso Baseado em Função](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) para delegar a permissão de registo ao Contribuinte.
- Certifique-se de que os pontos finais necessários estão ativados e não bloqueados devido à firewall. Para mais [informações, consulte os requisitos.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- O registo pode falhar devido à comunicação de saída ser submetida a inspeção SSL pela camada de rede.
- Certifique-se de que verificou as definições de notificação do Azure AD Connect Health e reveja a sua definição. Para entender como configurar as definições de notificação para notificações Azure AD Connect Health, consulte este [guia](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Para saber mais sobre o relatório de sincronização do AAD Connect Health e como descarregá-lo, consulte [o relatório de sincronização do nível de objeto](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Para resolver problemas, os alertas de saúde da AAD Connect seguem [o guia de resolução de problemas para alertas de frescura de dados AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) e para perguntas comumente colocadas, consulte [questões de instalação comuns da AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
