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
# <a name="configure-sync-features"></a>Configure funcionalidades de sincronização

O Azure AD Connect inclui várias funcionalidades que são ativadas por predefinição ou que pode ativar mais tarde. Algumas funcionalidades requerem configuração adicional em ambientes específicos.

- [Limites de filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) os objetos são sincronizados com Azure AD. Por padrão, todos os utilizadores, contactos, grupos e contas de computador do Windows 10 estão sincronizados. Pode incluir ou excluir objetos com base em domínios, OUs ou outros atributos.

- [A sincronização de hash de palavra-passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de palavra-passe do Diretório Ativo no local para o Azure AD. Isto permite a gestão de passwords em um local, mas a utilização da mesma senha tanto no local como em ambientes em nuvem. Como o Ative Directory é a fonte autoritária, pode usar as suas próprias políticas de senha.

- [O reset da palavra-passe de autosserviço (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que os utilizadores republiquem as suas próprias palavras-passe na nuvem, aplicando ainda a sua política de senha no local.

- [O writeback do dispositivo](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permite que os dispositivos registados em Azure AD sejam reencamidas para o Ative Directory no local para que possam ser utilizados para acesso condicional.

- [Evitar que as eliminações acidentais](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) sejam ativadas por padrão para ajudar a prevenir demasiadas eliminações simultâneas de objetos (mais de 500 objetos por sincronização). Pode alterar esta definição para atender às necessidades da sua organização.

- [A atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) é ativada por padrão para instalações expressas e ajuda a garantir que a sua versão do Azure AD Connect está sempre atualizada.
