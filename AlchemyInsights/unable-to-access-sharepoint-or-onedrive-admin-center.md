---
title: Não é possível aceder ao SharePoint ou OneDrive de administração
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020455"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Não é possível aceder ao SharePoint ou OneDrive de administração

- Se o seu site do Centro de administração do SharePoint ou do OneDrive estiver inacessível ou indisponível, poderá haver um problema de serviço temporário em que os utilizadores se deparam com atrasos intermitentes ou erros de navegação ao aceder a sites do SharePoint ou OneDrive conteúdo. Consulte o [dashboard Estado de saúde do](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) serviço para ver se a sua organização é afetada.

- É necessário atribuir uma licença do Microsoft Office SharePoint Online aos administradores globais e do SharePoint. As novas contas criadas apenas com uma licença do Microsoft Office SharePoint Online ou uma função de administrador podem ter problemas em aceder ao Microsoft Office SharePoint Online, como "acesso negado" ou "utilizador não encontrado". Aguarde pelo menos 24 horas para que a sincronização seja concluída em todos os sistemas. Compreendemos que 24 horas pode parecer muito tempo. Em muitos casos, estamos a trabalhar numa solução.

- Privileged Identity Management[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)os utilizadores podem receber acesso negado se a janela de tempo de acesso permitido for muito pequena. Consulte Acesso negado a contas [PIM.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)