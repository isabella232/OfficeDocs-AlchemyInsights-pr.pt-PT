---
title: 646 Como configurar o AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722574"
---
# <a name="configure-sync-features"></a><span data-ttu-id="e554f-102">Configure as funcionalidades de sincronização</span><span class="sxs-lookup"><span data-stu-id="e554f-102">Configure sync features</span></span>

<span data-ttu-id="e554f-103">O Azure AD Connect inclui várias funcionalidades que são ativadas por padrão, ou que pode ativar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="e554f-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="e554f-104">Algumas funcionalidades requerem configuração adicional em ambientes específicos.</span><span class="sxs-lookup"><span data-stu-id="e554f-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="e554f-105">Os limites [de filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) dos objetos são sincronizados com o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e554f-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="e554f-106">Por padrão, todos os utilizadores, contactos, grupos e contas de computador do Windows 10 estão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="e554f-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="e554f-107">Pode incluir ou excluir objetos baseados em domínios, OUs ou outros atributos.</span><span class="sxs-lookup"><span data-stu-id="e554f-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="e554f-108">[A sincronização de hash de palavra-passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de senha do Diretório Ativo no local para O AD Azure.</span><span class="sxs-lookup"><span data-stu-id="e554f-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="e554f-109">Isto permite a gestão de passwords num local, mas a utilização da mesma senha tanto no local como em ambientes na nuvem.</span><span class="sxs-lookup"><span data-stu-id="e554f-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="e554f-110">Como o Diretório Ativo é a fonte autoritária, pode usar as suas próprias políticas de senha.</span><span class="sxs-lookup"><span data-stu-id="e554f-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="e554f-111">[O reset de palavra-passe self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que os utilizadores redefinirem as suas próprias palavras-passe na nuvem enquanto aplicam a sua política de senha no local.</span><span class="sxs-lookup"><span data-stu-id="e554f-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="e554f-112">[A reescrita](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) do dispositivo permite que os dispositivos registados em Azure AD sejam reescritos no Diretório Ativo no local para que possam ser utilizados para acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="e554f-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="e554f-113">[Evitar eliminações acidentais](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) é ativado por predefinição para ajudar a evitar demasiadas eliminações simultâneas de objetos (mais de 500 objetos por sincronização).</span><span class="sxs-lookup"><span data-stu-id="e554f-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="e554f-114">Pode alterar este cenário para atender às necessidades da sua organização.</span><span class="sxs-lookup"><span data-stu-id="e554f-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="e554f-115">[A atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está ativada por predefinição para instalações expressas e ajuda a garantir que a sua versão do Azure AD Connect está sempre atual.</span><span class="sxs-lookup"><span data-stu-id="e554f-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
