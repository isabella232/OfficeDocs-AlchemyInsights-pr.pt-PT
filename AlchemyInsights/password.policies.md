---
title: Políticas de palavra-passe
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747049"
---
# <a name="password-policies"></a>Políticas de palavra-passe

**Estou tendo problemas com a política de senha para um utilizador**

- A política de palavra-passe para um utilizador depende se o utilizador é apenas na nuvem ou no local.
- Apenas os utilizadores da Cloud devem escolher uma palavra-passe que cumpra os requisitos deste artigo: [Políticas de palavra-passe que se aplicam apenas às contas de utilizadores na nuvem](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- No local, os utilizadores devem escolher uma palavra-passe que satisfaça os requisitos no local. Se um utilizador no local não conseguir definir a sua palavra-passe, verifique os seus requisitos no local.

**Não sei como definir ou verificar as políticas de validade da palavra-passe**

- Pode definir e verificar a política de expiração para utilizadores de nuvem no seu inquilino utilizando o PowerShell. Siga as instruções deste artigo: [Desa estalhe ou verifique as políticas de palavra-passe utilizando o PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- A política de expiração da palavra-passe para utilizadores no local está definida no seu AD no local.

**Outros links úteis:**
- [Começar com reset de palavra-passe](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Reset de senha iniciado por resolução de problemas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
