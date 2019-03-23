---
title: 646 como configurar AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779522"
---
# <a name="configure-sync-features"></a>Configurar funcionalidades de sincronização

Ligar de AD Azure inclui várias funcionalidades que estão activadas por predefinição, ou que pode activar mais tarde. Algumas funcionalidades requerem configuração adicional em ambientes específicos.
  
- Limites de [filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) os objectos são sincronizados para Azure AD. Por predefinição, todos os utilizadores, contactos, grupos e Windows 10 contas de computador são sincronizadas. Pode incluir ou excluir objectos baseados em domínios, UO ou outros atributos. 
    
- [Sincronização de hash de palavra-passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de palavra-passe do Active Directory no local para Azure AD. Isto permite a gestão de palavra-passe numa localização, mas utilize a mesma palavra-passe em ambas as instalações e ambientes de nuvem. Uma vez que o Active Directory é a origem autoritária, pode utilizar as suas próprias políticas de palavra-passe. 
    
- [Reposição de palavra-passe self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite aos utilizadores para repor as respectivas palavras-passe na nuvem enquanto ainda a aplicar a política de palavra-passe no local. 
    
- [Repetição de escrita do dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que os dispositivos registados no AD Azure a ser escrito novamente ao Active Directory no local para que possam ser utilizados para acesso condicional. 
    
- [Acidental impedir eliminações](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) está activada por predefinição para ajudar a impedir eliminações de objecto simultâneas demasiados (mais de 500 objectos por sincronização). Pode alterar esta definição para satisfazer as necessidades da organização. 
    
- [Actualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está activada por predefinição para instalações express e ajuda a garantir a que sua versão do Azure AD ligar está sempre actual. 
    

