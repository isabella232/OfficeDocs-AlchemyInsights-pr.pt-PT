---
title: Federação ADFS certificado expirar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 518261787b1b0df99ee7b3dc3e51dec70e4373bc
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398351"
---
# <a name="adfs-federation-certificate-expiring"></a>Federação ADFS certificado expirar

Para resolver este problema, siga estes passos:
  
1. Instale o Microsoft Azure Active Directory módulo para o Windows PowerShell no computador (se o módulo já não estiver instalado). Para efectuar este procedimento, vá para [Gerir os AD Azure utilizando o Windows PowerShell](https://aka.ms/aadposh).
    
2. Siga os passos das "cenário 1: O certificado de assinatura de tokens do AD FS expirado" secção de [erro "Ocorreu um problema ao aceder ao site" do AD FS quando um utilizador federado inicia sessão no Office 365, Azure ou Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Siga os passos de [como actualizar ou reparar as definições de um domínio federada no Office 365, Azure ou Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Para mais informações sobre como renovar certificados de Federação, consulte [renovar certificados de Federação para o Office 365 e Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

