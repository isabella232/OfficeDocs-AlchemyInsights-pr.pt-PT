---
title: Atrasos na receção de alertas SharePoint e OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742012"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Atrasos na receção de alertas SharePoint e OneDrive

- Primeiro, verifique a pasta Junk ou Spam no seu e-mail.
- Se **todos os alertas de vários ficheiros ou bibliotecas forem atrasados,** visite o painel de assistência ao [serviço](https://portal.office.com/adminportal/home?ref=/servicehealth) para verificar se existem avisos/incidentes que possam ocorrer com o SharePoint ou Exchange. O problema pode estar com a capacidade de alerta SharePoint ou atrasos em e-mails através do Exchange. Note também se outros e-mails estão a ser entregues — caso contrário, o problema é provável que seja com atrasos na Exchange.
- Se **um alerta individual de um ficheiro ou biblioteca específico não for entregue,** tente eliminá-lo e recriá-lo. Ver [Gerir, visualizar ou eliminar alertas sharePoint](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.

> [!NOTE]
> - Os alertas não podem ser enviados para um Grupo de Distribuição. Apenas os grupos de Segurança e O365 são apoiados.
> - Não é possível personalizar modelos de e-mail de alerta. Tem de utilizar o Microsoft Flow ou o SharePoint Designer Workflow para os conseguir.
