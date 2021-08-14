---
title: Certificado de Federação do AD FS a expirar
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952980"
---
# <a name="adfs-federation-certificate-expiring"></a>Certificado de Federação do AD FS a expirar

Para resolver este problema, siga estes passos:
  
1. Instale o Microsoft Azure Active Directory de Dados para Windows PowerShell no computador (se o módulo ainda não estiver instalado). Para o fazer, vá [a Gerir o Azure AD através do Windows PowerShell](https://aka.ms/aadposh).

2. Siga os passos na secção "Cenário 1: o certificado de assinatura de tokens do AD FS expirou" do erro "Ocorreu um problema ao aceder ao site" do AD FS quando um utilizador federado tem sessão de [Microsoft 365, Azure ou Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Siga os passos em Atualizar ou reparar as definições de um domínio [federado na Microsoft, no Azure ou no Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Para saber mais sobre como renovar os certificados de Federação, consulte Renovar os [certificados de federação Microsoft 365 e Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
