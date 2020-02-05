---
title: Atrasos na receção de alertas SharePoint e OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771226"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Atrasos na receção de alertas SharePoint e OneDrive

- Primeiro, verifique a pasta Junk ou Spam no seu e-mail.
- Se **todos os alertas de vários ficheiros ou bibliotecas forem atrasados,** visite o painel de assistência ao [serviço](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) para verificar se existem avisos/incidentes que possam ocorrer com o SharePoint ou Exchange. O problema pode estar com a capacidade de alerta SharePoint ou atrasos em e-mails através do Exchange. Note também se outros e-mails estão a ser entregues — caso contrário, o problema é provável que seja com atrasos na Exchange.
- Se **um alerta individual de um ficheiro ou biblioteca específico não for entregue,** tente eliminá-lo e recriá-lo. Ver [Gerir, visualizar ou eliminar alertas sharePoint](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) para recriar o alerta.

> [!NOTE]
> - Os alertas não podem ser enviados para um Grupo de Distribuição. Apenas os grupos de Segurança e O365 são apoiados.
> - Não é possível personalizar modelos de e-mail de alerta. Tem de utilizar o Microsoft Flow ou o SharePoint Designer Workflow para os conseguir.
