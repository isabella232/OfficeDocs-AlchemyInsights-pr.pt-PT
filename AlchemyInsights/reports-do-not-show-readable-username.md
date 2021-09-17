---
title: Os relatórios no centro de administração do Microsoft 365 não mostram um nome de utilizador aceitável
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327825"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Os relatórios no centro de administração do Microsoft 365 não mostram um nome de utilizador aceitável

Os relatórios no centro de administração do Microsoft 365 não mostram nomes de utilizador, mas mostram valores alfanuméricos, como B2BC6C15BB9FCDEA71E5CD302D228CC8.

Este é o comportamento esperado e foi comunicado no Centro de Mensagens (MC275344, publicado a 3 de agosto de 2021). 

Os administradores globais podem reverter esta alteração para o seu inquilino e mostrar informações de utilizador identificáveis se as práticas de privacidade da organização o permitirem. Para reverter a alteração para o inquilino:

1. No centro de administração, vá para **Definições** > **Definições da organização** > [**Serviços**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) e selecione **Relatórios**. 
1. Em **Escolha como mostrar informações do utilizador**, selecione **Mostrar informações de utilizador identificáveis nos relatórios** e, em seguida, execute o relatório de novo.