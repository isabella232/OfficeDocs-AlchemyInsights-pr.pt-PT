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
# <a name="configure-sync-features"></a>Configure as funcionalidades de sincronização

O Azure AD Connect inclui várias funcionalidades que são ativadas por padrão, ou que pode ativar mais tarde. Algumas funcionalidades requerem configuração adicional em ambientes específicos.

- Os limites [de filtragem](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) dos objetos são sincronizados com o Azure AD. Por padrão, todos os utilizadores, contactos, grupos e contas de computador do Windows 10 estão sincronizados. Pode incluir ou excluir objetos baseados em domínios, OUs ou outros atributos.

- [A sincronização de hash de palavra-passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sincroniza o hash de senha do Diretório Ativo no local para O AD Azure. Isto permite a gestão de passwords num local, mas a utilização da mesma senha tanto no local como em ambientes na nuvem. Como o Diretório Ativo é a fonte autoritária, pode usar as suas próprias políticas de senha.

- [O reset de palavra-passe self-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permite que os utilizadores redefinirem as suas próprias palavras-passe na nuvem enquanto aplicam a sua política de senha no local.

- [A reescrita](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) do dispositivo permite que os dispositivos registados em Azure AD sejam reescritos no Diretório Ativo no local para que possam ser utilizados para acesso condicional.

- [Evitar eliminações acidentais](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) é ativado por predefinição para ajudar a evitar demasiadas eliminações simultâneas de objetos (mais de 500 objetos por sincronização). Pode alterar este cenário para atender às necessidades da sua organização.

- [A atualização automática](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) está ativada por predefinição para instalações expressas e ajuda a garantir que a sua versão do Azure AD Connect está sempre atual.
