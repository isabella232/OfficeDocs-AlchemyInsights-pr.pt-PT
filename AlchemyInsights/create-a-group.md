---
title: Criar um grupo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929316"
---
# <a name="create-a-group"></a>Criar um grupo

Este tópico descreve a criação de grupos.

**Permissão para Criar um Grupo**

Certifique-se de que está autorizado a criar um novo grupo. Os administradores globais podem desativar a criação de grupos no portal do Azure ou no Painel de Acesso. Poderá precisar que um administrador crie o novo grupo por si ou que lhe forneça as permissões adequadas.

**Gerir permissões de criação de Grupos**

1. Os administradores globais podem gerir as permissões de criação de grupos (por motivos de segurança) ou grupos do Office 365 criados no portal do Azure ou no Painel de Acesso, ao selecionando "Os utilizadores podem criar grupos de segurança nos portais do Azure" ou "Os utilizadores podem criar grupos Office 365 nos portais do Azure" em Todos os grupos Gerais   >  **(Definições).**
2. Também pode restringir a criação de grupos para selecionar um grupo de utilizadores se tiver uma Azure Active Directory P1 Premium licença.

**Desativar a notificação de boas-vindas para novos Office 365 membros do grupo**

A notificação de boas-vindas enviada aos utilizadores adicionados a grupos Office 365 pode ser desativada ao definir **UnifiedGroupWelcomeMessageEnabled** to False no PowerShell. Saiba mais sobre esta definição [aqui.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

