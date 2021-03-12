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
# <a name="password-policies"></a><span data-ttu-id="cd2d4-102">Políticas de palavra-passe</span><span class="sxs-lookup"><span data-stu-id="cd2d4-102">Password policies</span></span>

<span data-ttu-id="cd2d4-103">**Estou tendo problemas com a política de senha para um utilizador**</span><span class="sxs-lookup"><span data-stu-id="cd2d4-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="cd2d4-104">A política de palavra-passe para um utilizador depende se o utilizador é apenas na nuvem ou no local.</span><span class="sxs-lookup"><span data-stu-id="cd2d4-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="cd2d4-105">Apenas os utilizadores da Cloud devem escolher uma palavra-passe que cumpra os requisitos deste artigo: [Políticas de palavra-passe que se aplicam apenas às contas de utilizadores na nuvem](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="cd2d4-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="cd2d4-106">No local, os utilizadores devem escolher uma palavra-passe que satisfaça os requisitos no local.</span><span class="sxs-lookup"><span data-stu-id="cd2d4-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="cd2d4-107">Se um utilizador no local não conseguir definir a sua palavra-passe, verifique os seus requisitos no local.</span><span class="sxs-lookup"><span data-stu-id="cd2d4-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="cd2d4-108">**Não sei como definir ou verificar as políticas de validade da palavra-passe**</span><span class="sxs-lookup"><span data-stu-id="cd2d4-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="cd2d4-109">Pode definir e verificar a política de expiração para utilizadores de nuvem no seu inquilino utilizando o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cd2d4-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="cd2d4-110">Siga as instruções deste artigo: [Desa estalhe ou verifique as políticas de palavra-passe utilizando o PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="cd2d4-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="cd2d4-111">A política de expiração da palavra-passe para utilizadores no local está definida no seu AD no local.</span><span class="sxs-lookup"><span data-stu-id="cd2d4-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="cd2d4-112">**Outros links úteis:**</span><span class="sxs-lookup"><span data-stu-id="cd2d4-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="cd2d4-113">Começar com reset de palavra-passe</span><span class="sxs-lookup"><span data-stu-id="cd2d4-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="cd2d4-114">Reset de senha iniciado por resolução de problemas</span><span class="sxs-lookup"><span data-stu-id="cd2d4-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
