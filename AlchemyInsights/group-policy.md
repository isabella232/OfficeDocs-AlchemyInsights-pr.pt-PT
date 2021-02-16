---
title: Política de grupo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256784"
---
# <a name="group-policy"></a><span data-ttu-id="00d2d-102">Política de grupo</span><span class="sxs-lookup"><span data-stu-id="00d2d-102">Group policy</span></span>

<span data-ttu-id="00d2d-103">As definições para objetos de utilizador e computador em Azure Ative Directory Domain Services (Azure AD DS) são frequentemente geridas usando objetos de política de grupo (GPOs).</span><span class="sxs-lookup"><span data-stu-id="00d2d-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="00d2d-104">O Azure AD DS inclui GPOs incorporados para os utilizadores da AADDC e recipientes de computadores AADDC.</span><span class="sxs-lookup"><span data-stu-id="00d2d-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="00d2d-105">Você pode personalizar estes GPOs incorporados para configurar a política de grupo conforme necessário para o seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="00d2d-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="00d2d-106">Membros do grupo de administradores AZure AD DC têm privilégios de administração de políticas de grupo no domínio Azure AD DS, e também podem criar GPOs personalizados e unidades organizacionais (OUs).</span><span class="sxs-lookup"><span data-stu-id="00d2d-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="00d2d-107">Para obter mais informações sobre o que é a política de grupo e como funciona, consulte [a visão geral da Política de Grupo.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="00d2d-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="00d2d-108">Num ambiente híbrido, as políticas de grupo configuradas num ambiente AD DS no local não são sincronizadas com a Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="00d2d-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="00d2d-109">Para definir definições de configuração para utilizadores ou computadores em Azure AD DS, edite um dos GPOs predefinidos ou crie um GPO personalizado.</span><span class="sxs-lookup"><span data-stu-id="00d2d-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="00d2d-110">Este artigo [Gerencie a Política de Grupo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) mostra-lhe como instalar as ferramentas de Gestão de Políticas de Grupo, como editar os GPOs incorporados e como criar GPOs personalizados.</span><span class="sxs-lookup"><span data-stu-id="00d2d-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



