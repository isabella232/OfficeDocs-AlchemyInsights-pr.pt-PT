---
title: Criar um grupo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088911"
---
# <a name="create-a-group"></a>Criar um grupo

Este tópico descreve a criação de grupo.

**Permissão para criar um grupo**

Certifique-se de que está autorizado a criar um novo grupo. Os administradores globais podem desativar a criação de grupos no portal Azure ou no Painel de Acesso. Pode precisar de um administrador para criar o novo grupo para si, ou para lhe dar permissões apropriadas.

**Gerir permissões de criação de grupo**

1. Os administradores globais podem gerir permissões de criação de grupos (por razões relacionadas com a segurança) ou grupos do Office 365 criados no portal Azure ou painel de acesso, escolhendo "Os utilizadores podem criar grupos de segurança em portais Azure" ou "Os utilizadores podem criar grupos office 365 em portais Azure" opções em **todos os**  >  **grupos Gerais (Definições)**.
2. Também pode restringir a criação de grupo para selecionar um grupo de utilizadores se tiver uma licença Azure Ative Directory P1 Premium.

**Notificação de boas-vindas incapacitante para novos membros do grupo Office 365**

A notificação de boas-vindas enviada aos utilizadores adicionados aos grupos Office 365 pode ser desativada através da definição **de UnifiedGroupWelcomeMessageEnabled** to False in Powershell. Saiba mais sobre este cenário [aqui.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

