---
title: Problemas de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: ec378981d4f24837b037e18214cbeba2f2b657c5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692704"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive Slow, Inacessível ou Indisponível para Vários Utilizadores

Se um site oneDrive ou SharePoint não estiver disponível para vários utilizadores que anteriormente tiveram acesso, pode haver um problema de serviço temporário. [Verifique o painel de saúde do serviço.](https://portal.office.com/adminportal/home#/servicehealth)

**Adicionar e licenciar o utilizador**

Certifique-se de que [atribui licenças aos utilizadores no Microsoft 365 para negócios](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**Permissões de atribuição**

Se o utilizador tiver recebido uma licença sharepoint e ainda estiver a receber uma mensagem de acesso negada, certifique-se de que tem o nível de [permissão adequado](https://docs.microsoft.com/sharepoint/understanding-permission-levels) atribuído.

**Considere usar a funcionalidade de pedido de acesso**

A funcionalidade de [pedido de acesso](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) permite que as pessoas solicitem acesso a conteúdos que não têm atualmente autorização para ver.

**Permitir script personalizado pode causar problemas de acesso negados**

Existem certos cenários em que a funcionalidade de *script personalizada Permitir* pode estar a apresentar um acesso negado. Para uma lista de funcionalidades afetadas, considerações de segurança e a capacidade de desativar a funcionalidade. Visite [Permitir ou evitar scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

