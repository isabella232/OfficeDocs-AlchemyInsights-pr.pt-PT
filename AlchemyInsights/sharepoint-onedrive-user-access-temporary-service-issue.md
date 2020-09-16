---
title: Questões de desempenho-SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771255"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ou OneDrive Lento, Inacessível ou Indisponível para Vários Utilizadores

Se um site OneDrive ou SharePoint não estiver disponível para vários utilizadores que tiveram acesso anteriormente, pode haver um problema de serviço temporário. [Verifique o painel de saúde do serviço.](https://portal.office.com/adminportal/home#/servicehealth)

**Adicionar e licenciar o utilizador**

Certifique-se de atribuir [licenças aos utilizadores da Microsoft 365 para negócios.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Atribuir permissões**

Se o utilizador tiver recebido uma licença Sharepoint e ainda estiver a receber uma mensagem de acesso negada, certifique-se de que tem o [nível de permissão adequado](https://docs.microsoft.com/sharepoint/understanding-permission-levels) atribuído.

**Considere usar a funcionalidade de pedido de acesso**

A [funcionalidade de pedido](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) de acesso permite que as pessoas solicitem acesso a conteúdos que não têm atualmente permissão para ver.

**Permitir scripts personalizados pode causar acesso a problemas negados**

Existem certos cenários em que a funcionalidade *de script personalizado Permitir* pode estar a apresentar um acesso negado. Para uma lista de funcionalidades afetadas, considerações de segurança e a capacidade de desativar a funcionalidade. Visite [o Allow ou evite scripts personalizados](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

