---
title: Configure LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885574"
---
# <a name="configure-ldap"></a>Configure LDAP

Para configurar o LDAP, faça o seguinte:

1. Verifique a saúde do seu domínio no [portal Azure](https://aka.ms/aadds-health).
1. Certifique-se de que está disponível uma subscrição AD Azure válida e que os Serviços de Domínio AD AZure foram ativados.
1. O certificado necessário para permitir a LDAP segura deve ser obtido a partir de uma autoridade de certificação pública de confiança ou ser um certificado auto-assinado.
1. Certifique-se de que o certificado segue as [orientações](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)exigidas.

**Certificado inválido**
1. Para renovar um certificado, siga os passos para criar um novo certificado e recarregar: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Para resolver problemas conhecidos com alertas Secure LDAP nos Serviços de Domínio do Diretório Azure Ative, consulte [os alertas Resolve LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
