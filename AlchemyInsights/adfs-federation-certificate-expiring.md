---
title: Certificado da Federação ADFS expirando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686760"
---
# <a name="adfs-federation-certificate-expiring"></a>Certificado da Federação ADFS expirando

Para resolver esta questão, siga estes passos:
  
1. Instale o Módulo de Diretório Ativo Microsoft Azure para o Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para isso, vá a [Manage AD azure usando o Windows PowerShell](https://aka.ms/aadposh).

2. Siga os passos na secção "Cenário 1: O certificado de assinatura de fichas AD FS expirou" da secção ["Houve um problema de acesso ao site" de AD FS quando um utilizador federado assina a Microsoft 365, Azure ou Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Siga os passos em [Update ou repare as definições de um domínio federado na Microsoft, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Para saber mais sobre a renovação dos certificados da Federação, consulte [os certificados da federação Renovar para o Microsoft 365 e o Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
