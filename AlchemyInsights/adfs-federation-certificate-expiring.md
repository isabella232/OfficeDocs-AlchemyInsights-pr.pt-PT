---
title: Certificado de Federação do ADFS expirando
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737200"
---
# <a name="adfs-federation-certificate-expiring"></a>Certificado de Federação do ADFS expirando

Para resolver este problema, siga estes passos:
  
1. Instale o módulo do Active Directory do Microsoft Azure para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para fazer isso, vá para [gerenciar o Azure ad usando o Windows PowerShell](https://aka.ms/aadposh).

2. Siga as etapas na seção "cenário 1: o certificado de assinatura de token do AD FS expirou" do [erro "ocorreu um problema ao acessar o site" do AD FS quando um usuário federado entra no Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Siga as etapas em [atualizar ou reparar as configurações de um domínio federado no Office 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Para saber mais sobre como renovar certificados de Federação, consulte [renovar certificados de Federação para o Office 365 e o Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
