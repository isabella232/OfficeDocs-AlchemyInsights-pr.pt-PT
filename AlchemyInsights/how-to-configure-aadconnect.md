---
title: 646 Como configurar a AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704500"
---
# <a name="configure-sync-features"></a><span data-ttu-id="6cdf6-102">Configure funcionalidades de sincronização</span><span class="sxs-lookup"><span data-stu-id="6cdf6-102">Configure sync features</span></span>

<span data-ttu-id="6cdf6-103">O Azure AD Connect inclui várias funcionalidades que são ativadas por predefinição ou que pode ativar mais tarde.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="6cdf6-104">Algumas funcionalidades requerem configuração adicional em ambientes específicos.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="6cdf6-105">[Limites de filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) os objetos são sincronizados com Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="6cdf6-106">Por padrão, todos os utilizadores, contactos, grupos e contas de computador do Windows 10 estão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="6cdf6-107">Pode incluir ou excluir objetos com base em domínios, OUs ou outros atributos.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="6cdf6-108">[A sincronização de hash de palavra-passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de palavra-passe do Diretório Ativo no local para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="6cdf6-109">Isto permite a gestão de passwords em um local, mas a utilização da mesma senha tanto no local como em ambientes em nuvem.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="6cdf6-110">Como o Ative Directory é a fonte autoritária, pode usar as suas próprias políticas de senha.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="6cdf6-111">[O reset da palavra-passe de autosserviço (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que os utilizadores republiquem as suas próprias palavras-passe na nuvem, aplicando ainda a sua política de senha no local.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="6cdf6-112">[O writeback do dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que os dispositivos registados em Azure AD sejam reencamidas para o Ative Directory no local para que possam ser utilizados para acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="6cdf6-113">[Evitar que as eliminações acidentais](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) sejam ativadas por padrão para ajudar a prevenir demasiadas eliminações simultâneas de objetos (mais de 500 objetos por sincronização).</span><span class="sxs-lookup"><span data-stu-id="6cdf6-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="6cdf6-114">Pode alterar esta definição para atender às necessidades da sua organização.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="6cdf6-115">[A atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) é ativada por padrão para instalações expressas e ajuda a garantir que a sua versão do Azure AD Connect está sempre atualizada.</span><span class="sxs-lookup"><span data-stu-id="6cdf6-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
