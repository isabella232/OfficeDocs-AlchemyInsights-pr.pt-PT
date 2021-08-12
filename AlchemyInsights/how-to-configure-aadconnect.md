---
title: 646 Como configurar o AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963654"
---
# <a name="configure-sync-features"></a>Configurar funcionalidades de sincronização

O Azure AD Ligação inclui várias funcionalidades que estão ativadas por predefinição ou que pode ativar mais tarde. Algumas funcionalidades necessitam de configuração adicional em ambientes específicos.

- [A filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limita os objetos são sincronizados com o Azure AD. Por predefinição, todos os utilizadores, contactos, grupos e Windows 10 de computador são sincronizados. Pode incluir ou excluir objetos com base em domínios, OUs ou outros atributos.

- [A sincronização de hashes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) de palavras-passe sincroniza o hash de palavras-passe do Active Directory no local com o Azure AD. Isto permite a gestão de palavras-passe numa localização, mas utiliza a mesma palavra-passe em ambientes no local e na nuvem. Uma vez que o Active Directory é a origem autoritativa, pode utilizar as suas próprias políticas de palavra-passe.

- [A reposição de palavras-passe self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite aos utilizadores reporem as suas próprias palavras-passe na nuvem, ao mesmo tempo que aplicam a sua política de palavras-passe no local.

- [A escrita de](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) dispositivos permite que os dispositivos registados no Azure AD sejam de volta escritos no Active Directory no local para que possam ser utilizados para acesso condicional.

- A opção Impedir [eliminações acidentais](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) está ativada por predefinição para ajudar a impedir demasiadas eliminações de objetos em simultâneo (mais de 500 objetos por sincronização). Pode alterar esta definição para satisfazer as necessidades da sua organização.

- [A atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está ativada por predefinição para instalações rápidas e ajuda a garantir que a sua versão do Azure AD Ligação está sempre atualizada.
