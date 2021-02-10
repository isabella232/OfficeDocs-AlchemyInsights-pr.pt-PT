---
title: Sincronização de hash de palavra-passe para o serviço de domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177625"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="a484c-102">Sincronização de hash de palavra-passe para o serviço de domínio</span><span class="sxs-lookup"><span data-stu-id="a484c-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="a484c-103">**Se a sua instância AD DS Azure estiver a pedir-lhe para ativar a sincronização de hash de palavra-passe**</span><span class="sxs-lookup"><span data-stu-id="a484c-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="a484c-104">Encontra-se um cenário em que está a executar um ambiente híbrido com os utilizadores a sincronizar-se a partir de um ambiente no local Azure Ative Directory Domain Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="a484c-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="a484c-105">Este cenário encontra-se apesar de ter sincronização de hash de palavra-passe do AD DS no local para o seu inquilino AZure AD.</span><span class="sxs-lookup"><span data-stu-id="a484c-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="a484c-106">**Causa**</span><span class="sxs-lookup"><span data-stu-id="a484c-106">**Cause**</span></span>

<span data-ttu-id="a484c-107">Isto acontece porque o Azure AD Connect por padrão não sincroniza o legado New Technology LAN Manager (NTLM) e os hashes de password Kerberos que são necessários para o Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="a484c-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="a484c-108">**Solução**</span><span class="sxs-lookup"><span data-stu-id="a484c-108">**Workaround**</span></span> 

<span data-ttu-id="a484c-109">Você precisaria configurar Azure AD Connect para sincronizar os hashes de palavra-passe necessários para a autenticação NTLM e Kerberos.</span><span class="sxs-lookup"><span data-stu-id="a484c-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="a484c-110">Depois de configurado O Azure AD Connect, um evento de criação de conta no local ou de mudança de palavra-passe também sincroniza a palavra-passe do legado hashes para Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a484c-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="a484c-111">Consulte [aqui](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) mais informações sobre este caso e para obter orientações sobre como permitir a sincronização de passwords em ambientes híbridos Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="a484c-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>