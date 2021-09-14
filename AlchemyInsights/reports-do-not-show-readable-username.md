---
title: Os relatórios centro de administração do Microsoft 365 não mostram o nome de utilizador lido
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
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/04/2021
ms.locfileid: "59316195"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Os relatórios centro de administração do Microsoft 365 não mostram o nome de utilizador lido

Os relatórios no centro de administração do Microsoft 365 não mostram os nomes de utilizador, mas mostram valores numéricos alfa como B2BC6C15BB9FCDEA71E5CD302D228CC8.

Este é o comportamento esperado e foi comunicado no Centro de Mensagens (MC275344, publicado em 3 de agosto de 2021). 

Os administradores globais podem reverter esta alteração no seu inquilino e mostrar informações de utilizador identificáveis se as práticas de privacidade da organização o permitirem. Para reverter a alteração do inquilino:

1. No centro de administração, selecione Serviços **Definições** definições da Sua Empresa e  >    >  [](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)selecione **Relatórios**. 
1. Em **Escolha como mostrar as informações do utilizador**, selecione Mostrar informações **identificáveis do utilizador** nos relatórios e, em seguida, execute o relatório.