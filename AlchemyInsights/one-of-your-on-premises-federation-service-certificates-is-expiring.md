---
title: Um dos seus certificados de serviço de federação local estiver prestes a expirar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543576"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Um dos seus certificados de serviço de federação local estiver prestes a expirar

Para resolver este problema, siga estes passos:
  
- Instale o Microsoft Azure Active Directory módulo para o Windows PowerShell no computador (se o módulo já não estiver instalado). Para tal, vá para [Azure Active Directory PowerShell para gráfico](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Siga os passos das "cenário 1: O certificado de assinatura de tokens do AD FS expirado" secção de [erro "Ocorreu um problema ao aceder ao site" do AD FS quando um utilizador federado inicia sessão no Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Siga os passos no t[como actualizar ou reparar as definições de um domínio federada no Office 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Para mais informações sobre como renovar certificados de Federação, consulte a [renovação de certificados para O365 e Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

