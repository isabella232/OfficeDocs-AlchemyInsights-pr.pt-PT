---
title: Um dos seus Certificados de Serviço de Federação no local está a expirar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985228"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Um dos seus Certificados de Serviço de Federação no local está a expirar

Para resolver este problema, siga estes passos:
  
- Instale o Microsoft Azure Active Directory de Dados para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para o fazer, vá a [Azure Active Directory PowerShell para Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Siga os passos na secção "Cenário 1: o certificado de assinatura de tokens do AD FS expirou" do erro "Ocorreu um problema ao aceder ao site" do AD FS quando um utilizador federado tem sessão de [Microsoft 365, Azure ou Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Siga os passos em Como atualizar ou reparar as definições de um domínio [federado no Microsoft 365, no Azure ou no Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)
    
Para obter mais informações sobre como renovar os certificados de Federação, consulte Renovação de certificados para [o O365 e para o Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
  

