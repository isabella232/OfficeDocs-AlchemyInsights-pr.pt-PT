---
title: Implementação do GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067851"
---
# <a name="gpo-deployment"></a>Implementação do GPO

Definições para objetos de utilizador e computador no Azure Active Directory Domain Services (Azure AD DS) são frequentemente geridos através de GPOs (Group Policy Objects). O Azure AD DS inclui GPOs incorporados para os contentores Utilizadores AADDC e Computadores AADDC. Pode personalizar estes GPOs incorporados para configurar a política de grupo conforme necessário para o seu ambiente. Os membros do grupo de administradores do Azure AD DC têm privilégios de administração de política de grupo no domínio Azure AD DS e também podem criar GPOs personalizados e unidades organizacionais (OUs). Para obter mais informações sobre o que é a política de grupo e como funciona, consulte a [Visão Geral da Política de Grupo.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Num ambiente híbrido, as políticas de grupo configuradas num ambiente AD DS no local não são sincronizadas com o Azure AD DS. Para definir as definições de configuração para utilizadores ou computadores no Azure AD DS, edite um dos GPOs predefinido ou crie um GPO personalizado.

Este artigo Gerir Política [de](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) Grupo mostra-lhe como instalar as ferramentas de Gestão da Política de Grupo, como editar os GPOs incorporados e como criar GPOs personalizados.
