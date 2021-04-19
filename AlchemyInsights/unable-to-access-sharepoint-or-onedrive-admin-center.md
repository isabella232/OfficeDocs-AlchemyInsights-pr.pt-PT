---
title: Não é possível aceder ao SharePoint ou ao centro de administração OneDrive
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
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824446"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Não é possível aceder ao SharePoint ou ao centro de administração OneDrive

- Se o seu site do Centro De Admin SharePoint ou OneDrive estiver inacessível ou indisponível, pode haver um problema de serviço temporário em que os utilizadores experimentem atrasos intermitentes ou erros de navegação ao aceder a sites SharePoint ou conteúdo OneDrive. Consulte o [painel de saúde do Serviço](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) para ver se a sua organização está com impacto.

- É necessário atribuir uma licença do Microsoft Office SharePoint Online aos administradores globais e do SharePoint. As novas contas criadas apenas com uma licença do Microsoft Office SharePoint Online ou uma função de administrador podem ter problemas em aceder ao Microsoft Office SharePoint Online, como "acesso negado" ou "utilizador não encontrado". Aguarde pelo menos 24 horas para que a sincronização seja concluída em todos os sistemas. Compreendemos que 24 horas pode parecer muito tempo. Em muitos casos, estamos a trabalhar numa solução.

- Os utilizadores privilegiados de Gestão de Identidade[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)podem ter acesso negado se a janela de tempo de acesso permitida for muito pequena, ver  [Acesso negado às contas PIM](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).