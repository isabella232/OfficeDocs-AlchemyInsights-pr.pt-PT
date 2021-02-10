---
title: Problema com grupos de segurança
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
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177629"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="8e77d-102">Problema com grupos de segurança</span><span class="sxs-lookup"><span data-stu-id="8e77d-102">Issue with security groups</span></span>

<span data-ttu-id="8e77d-103">**Se estiver a receber O Erro de Rede AADDS104**</span><span class="sxs-lookup"><span data-stu-id="8e77d-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="8e77d-104">As regras do grupo de segurança da rede inválidas são a causa mais comum de erros de rede para os Serviços de Domínio do Diretório Ativo Azure (DS AD).</span><span class="sxs-lookup"><span data-stu-id="8e77d-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="8e77d-105">O grupo de segurança da rede virtual deve permitir o acesso a portas e protocolos específicos.</span><span class="sxs-lookup"><span data-stu-id="8e77d-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="8e77d-106">Se estas portas estiverem bloqueadas, a plataforma Azure não pode monitorizar ou atualizar o domínio gerido.</span><span class="sxs-lookup"><span data-stu-id="8e77d-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="8e77d-107">A sincronização entre o Azure AD e o Azure AD DS também é impactada.</span><span class="sxs-lookup"><span data-stu-id="8e77d-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="8e77d-108">Certifique-se de que mantém as portas padrão abertas para evitar interrupções no serviço.</span><span class="sxs-lookup"><span data-stu-id="8e77d-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="8e77d-109">Para compreender e resolver alertas comuns para problemas de configuração do grupo de segurança de rede, consulte [Grupos de Segurança Adicionar e Verificar](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="8e77d-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
