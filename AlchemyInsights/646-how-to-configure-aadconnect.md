---
title: 646 como configurar AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499681"
---
# <a name="configure-sync-features"></a><span data-ttu-id="b4a1d-102">Configurar funcionalidades de sincronização</span><span class="sxs-lookup"><span data-stu-id="b4a1d-102">Configure sync features</span></span>

<span data-ttu-id="b4a1d-p101">Ligar de AD Azure inclui várias funcionalidades que estão activadas por predefinição, ou que pode activar mais tarde. Algumas funcionalidades requerem configuração adicional em ambientes específicos.</span><span class="sxs-lookup"><span data-stu-id="b4a1d-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="b4a1d-p102">Limites de [filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) os objectos são sincronizados para Azure AD. Por predefinição, todos os utilizadores, contactos, grupos e Windows 10 contas de computador são sincronizadas. Pode incluir ou excluir objectos baseados em domínios, UO ou outros atributos.</span><span class="sxs-lookup"><span data-stu-id="b4a1d-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="b4a1d-p103">[Sincronização de hash de palavra-passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de palavra-passe do Active Directory no local para Azure AD. Isto permite a gestão de palavra-passe numa localização, mas utilize a mesma palavra-passe em ambas as instalações e ambientes de nuvem. Uma vez que o Active Directory é a origem autoritária, pode utilizar as suas próprias políticas de palavra-passe.</span><span class="sxs-lookup"><span data-stu-id="b4a1d-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="b4a1d-111">[Reposição de palavra-passe self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite aos utilizadores para repor as respectivas palavras-passe na nuvem enquanto ainda a aplicar a política de palavra-passe no local.</span><span class="sxs-lookup"><span data-stu-id="b4a1d-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="b4a1d-112">[Repetição de escrita do dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que os dispositivos registados no AD Azure a ser escrito novamente ao Active Directory no local para que possam ser utilizados para acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="b4a1d-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="b4a1d-p104">[Acidental impedir eliminações](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) está activada por predefinição para ajudar a impedir eliminações de objecto simultâneas demasiados (mais de 500 objectos por sincronização). Pode alterar esta definição para satisfazer as necessidades da organização.</span><span class="sxs-lookup"><span data-stu-id="b4a1d-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="b4a1d-115">[Actualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está activada por predefinição para instalações express e ajuda a garantir a que sua versão do Azure AD ligar está sempre actual.</span><span class="sxs-lookup"><span data-stu-id="b4a1d-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

