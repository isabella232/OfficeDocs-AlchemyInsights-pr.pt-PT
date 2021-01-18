---
title: Emissão juntando VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885665"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="50c1c-102">Emissão juntando VMs</span><span class="sxs-lookup"><span data-stu-id="50c1c-102">Issue joining VMs</span></span>

<span data-ttu-id="50c1c-103">Para resolver problemas que ocorrem ao tentar juntar VMs, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="50c1c-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="50c1c-104">Tente iniciar sação utilizando o formato **UPN** (por exemplo, 'joeuser@contoso.com') em vez do formato **SAMAccountName** ('CONTOSO\joeuser').</span><span class="sxs-lookup"><span data-stu-id="50c1c-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="50c1c-105">Certifique-se de que ativou a sincronização da palavra-passe de acordo com os passos descritos no guia *'Iniciar'.*</span><span class="sxs-lookup"><span data-stu-id="50c1c-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="50c1c-106">Certifique-se de que a conta de utilizador afetada não é uma conta externa no inquilino AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="50c1c-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="50c1c-107">Os utilizadores externos não podem entrar no domínio gerido, uma vez que os Serviços de Domínio AD Azure não têm credenciais para essas contas de utilizador.</span><span class="sxs-lookup"><span data-stu-id="50c1c-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="50c1c-108">Se a conta de utilizador afetada for uma conta de utilizador exclusivamente na nuvem, certifique-se de que os utilizadores alteraram a sua palavra-passe depois de ter ativado os Serviços de Domínio Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50c1c-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="50c1c-109">Este passo faz com que os haques credenciais necessários para que os Serviços de Domínio AD AD do Azure sejam gerados.</span><span class="sxs-lookup"><span data-stu-id="50c1c-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="50c1c-110">Se as contas de utilizador afetadas forem sincronizadas a partir de um diretório no local, verifique se a libertação recomendada do Azure AD Connect foi configurada para realizar uma sincronização completa.</span><span class="sxs-lookup"><span data-stu-id="50c1c-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="50c1c-111">Se os problemas persistirem após confirmar o Passo 4, execute os seguintes comandos da sua máquina de sincronização:</span><span class="sxs-lookup"><span data-stu-id="50c1c-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="50c1c-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="50c1c-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>