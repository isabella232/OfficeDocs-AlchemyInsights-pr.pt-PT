---
title: Caducidade do certificado da Federação ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710418"
---
# <a name="adfs-federation-certificate-expiring"></a>Caducidade do certificado da Federação ADFS

Para resolver esta questão, siga estes passos:
  
1. Instale o Módulo de Diretório Ativo Microsoft Azure para windows PowerShell no computador (se o módulo ainda não estiver instalado). Para isso, vá para [a Manage Azure AD utilizando o Windows PowerShell](https://aka.ms/aadposh).

2. Siga os passos na secção "Cenário 1: O certificado de assinatura de token AD caducou" da secção "Houve um problema de [acesso ao site" do erro da AD FS quando um utilizador federado insere na Microsoft 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Siga os passos em [Atualizar ou repare as definições de um domínio federado na Microsoft, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Para saber mais sobre a renovação dos certificados da Federação, consulte Renovar os certificados da federação para o [Microsoft 365 e o Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
