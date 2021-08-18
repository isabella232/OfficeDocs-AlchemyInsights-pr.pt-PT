---
title: OneDrive de início de sessão AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112923"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive de início de sessão AADSTS50011

Se receber uma mensagem de erro "AADSTS50011: O URL de resposta especificado no pedido não corresponde à resposta" ao entrar na aplicação OneDrive, verifique o seguinte:

A OneDrive sua versão tem de ser igual ou superior à versão 20.052.XXXX.XXXX. Para verificar a sua versão, clique no ícone de OneDrive azul na área de notificação, selecione **Ajuda & Definições > Definições > Acerca de**.

A sua rede pode bloquear o **tráfego para g.live.com** e **oneclient.sfx.ms**. Se esse tráfego estiver bloqueado, a OneDrive não pode atualizar-se. Trabalhe com o seu administrador de rede para garantir que tem acesso a esses URLs. [Estes pontos finais devem](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) estar acessíveis para clientes que utilizam Microsoft 365 planos.

Se precisar de obter manualmente uma versão atual do OneDrive, visite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
