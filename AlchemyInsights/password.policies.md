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
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040841"
---
# <a name="password-policies"></a>Políticas de palavra-passe

**Estou a ter problemas com a política de palavras-passe de um utilizador**

- A política de palavras-passe de um utilizador depende de se o utilizador é apenas na nuvem ou no local.
- Apenas os utilizadores na nuvem têm de escolher uma palavra-passe que cumpre os requisitos neste artigo: Políticas de palavra-passe que só se aplicam a contas de [utilizador na nuvem](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Os utilizadores no local têm de selecionar uma palavra-passe que ender os requisitos no local. Se um utilizador no local não conseguir definir a palavra-passe, verifique os seus requisitos no local.

**Não sei como definir ou verificar políticas de expiração de palavras-passe**

- Pode definir e verificar a política de expiração para utilizadores na nuvem no seu inquilino através do PowerShell. Siga as instruções neste artigo: Definir ou [verificar as políticas de palavra-passe através do PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- A política de expiração de palavras-passe para utilizadores no local é definida no seu AD no local.

**Outras ligações úteis:**
- [Começar a Repor Palavra-passe](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Reposição de Palavras-passe iniciada por Administradores](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
