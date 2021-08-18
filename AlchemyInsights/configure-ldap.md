---
title: Configurar LDAP
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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090423"
---
# <a name="configure-ldap"></a>Configurar LDAP

Para configurar o LDAP, faça o seguinte:

1. Verifique o estado de saúde do seu domínio no [portal do Azure.](https://aka.ms/aadds-health)
1. Certifique-se de que está disponível uma subscrição válida do Azure AD e de que os Serviços de Domínio do Azure AD foram ativados.
1. O certificado necessário para ativar o LDAP seguro tem de ser obtido a partir de uma autoridade de certificação pública de confiança ou ser um certificado autoassinado.
1. Certifique-se de que o certificado segue as diretrizes [necessárias.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Certificado Inválido**
1. Para renovar um certificado, siga os passos para criar um novo certificado e recarregar: [Configurar o LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Para resolver um problema conhecido com alertas LDAP Seguros nos Serviços de Domínio do Azure Active Directory, consulte [Resolver alertas LDAP.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
