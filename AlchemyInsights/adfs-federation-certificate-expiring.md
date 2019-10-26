---
title: Certificado da Federação ADFS expirando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737200"
---
# <a name="adfs-federation-certificate-expiring"></a>Certificado da Federação ADFS expirando

Para resolver este problema, siga estas etapas:
  
1. Instale o Módulo de Diretório Ativo do Microsoft Azure para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para fazer isso, acesse [o AD do Azure usando o Windows PowerShell.](https://aka.ms/aadposh)

2. Siga os passos na seção "Cenário 1: O certificado de assinatura de tokens AD FS expirou" de "Houve um problema de [acesso ao site" erro de AD FS quando um usuário federado assina para o Office 365, Azure, ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Siga as [etapas em Atualização ou repare as configurações de um domínio federado no Office 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Para saber mais sobre a renovação de certificados da Federação, consulte os certificados da federação Renew para o [Office 365 e o Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
