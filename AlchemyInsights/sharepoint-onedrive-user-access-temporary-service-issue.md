---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2db0a9442b9fdf1752b654f7c188e641e0a274cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053812"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive lento, inacessível ou indisponível para vários usuários

Se um site OneDrive ou SharePoint não estiver disponível para vários usuários que tiveram acesso anteriormente, pode haver um problema de serviço temporário. [Verifique o painel de saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).

**Adicionar e licenciar o usuário**

Certifique-se de atribuir [licenças aos usuários no Office 365 para negócios.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)


**Atribuir permissões**

Se o usuário tiver sido atribuído uma licença Sharepoint e ainda estiver recebendo uma mensagem negada de acesso, certifique-se de que eles tenham o [nível de permissão adequado](https://docs.microsoft.com/sharepoint/understanding-permission-levels) atribuído.

**Considere usar o recurso de solicitação de acesso**

O recurso de [solicitação](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) de acesso permite que as pessoas solicitem acesso a conteúdo que atualmente não têm permissão para ver.

**Permitir que o script personalizado pode causar problemas negados de acesso**

Há certos cenários em que o recurso *de script personalizado Permitir* pode estar apresentando um acesso negado. Para obter uma lista de recursos afetados, considerações de segurança e a capacidade de desativar o recurso. Visite [Permitir ou evitar script personalizado](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

