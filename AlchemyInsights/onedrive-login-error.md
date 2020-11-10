---
title: Erro de login oneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982542"
---
# <a name="onedrive-login-error-aadsts50011"></a>Erro de login oneDrive AADSTS50011

Se receber um erro "AADSTS50011: O URL de resposta especificado no pedido não corresponde à resposta" ao assinar na aplicação OneDrive, verifique o seguinte:

A sua versão OneDrive tem de ser igual ou superior à versão 20.052.XXXX. XXXX. Para verificar a sua versão, clique no ícone OneDrive azul na área de notificação, selecione **'Definições &' > Definições > Sobre**.

A sua rede pode bloquear o tráfego para **g.live.com** e **oneclient.sfx.ms**. Se o tráfego estiver bloqueado, o OneDrive não pode atualizar-se sozinho. Trabalhe com o seu administrador de rede para garantir que tem acesso a esses URLs. [Estes pontos finais](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) devem ser alcançáveis para os clientes que usam os planos da Microsoft 365.

Se precisar de obter manualmente uma versão atual do OneDrive, visite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
