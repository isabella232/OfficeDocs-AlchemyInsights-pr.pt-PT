---
title: Um dos seus certificados de serviço da Federação está expirando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785314"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Um dos seus certificados de serviço da Federação está expirando

Para resolver esta questão, siga estes passos:
  
- Instale o Módulo de Diretório Ativo Microsoft Azure para windows PowerShell no computador (se o módulo ainda não estiver instalado). Para isso, vá ao [Azure Ative Directory PowerShell para graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Siga os passos na secção "Cenário 1: O certificado de assinatura de token AD caducou" da secção "Houve um problema de [acesso ao site" do erro da AD FS quando um utilizador federado insere na Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Siga os passos em [Como atualizar ou reparar as definições de um domínio federado no Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Para obter mais informações sobre a renovação dos certificados da Federação, consulte a renovação do [certificado para o O365 e a AD Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

