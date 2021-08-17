---
title: Enviar Como Pasta Pública Com Ativação de Correio no EXO
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
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052577"
---
# <a name="sendas-mail-enabled-public-folder"></a>Enviar Como Pasta Pública Ativada por Correio

O exemplo seguinte atribui permissões "Enviar Como" para a pasta pública com correio ativado em NewPF1 ao utilizador Jason.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Para obter informações detalhadas sobre a sintaxe e os parâmetros, consulte Atribuir permissões "Enviar Como" ou "Enviar em Nome De" para pastas públicas com correio [ativado.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

