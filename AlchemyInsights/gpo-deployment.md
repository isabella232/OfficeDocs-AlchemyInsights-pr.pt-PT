---
title: Implantação de GPO
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
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427563"
---
# <a name="gpo-deployment"></a>Implantação de GPO

As definições para objetos de utilizador e computador em Azure Ative Directory Domain Services (Azure AD DS) são frequentemente geridas usando objetos de política de grupo (GPOs). O Azure AD DS inclui GPOs incorporados para os utilizadores da AADDC e recipientes de computadores AADDC. Você pode personalizar estes GPOs incorporados para configurar a política de grupo conforme necessário para o seu ambiente. Membros do grupo de administradores AZure AD DC têm privilégios de administração de políticas de grupo no domínio Azure AD DS, e também podem criar GPOs personalizados e unidades organizacionais (OUs). Para obter mais informações sobre o que é a política de grupo e como funciona, consulte [a Visão Geral da Política de Grupo](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Num ambiente híbrido, as políticas de grupo configuradas num ambiente AD DS no local não são sincronizadas com a Azure AD DS. Para definir definições de configuração para utilizadores ou computadores em Azure AD DS, edite um dos GPOs predefinidos ou crie um GPO personalizado.

Este artigo [Gerencie a Política de Grupo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) mostra-lhe como instalar as ferramentas de Gestão de Políticas de Grupo, como editar os GPOs incorporados e como criar GPOs personalizados.
