---
title: Notificações de alerta do SharePoint não entregues
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 05bd913098372a57d3061e8c516a6a6b4f0a9bdafde02acc930062d6281d06dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957912"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Notificações de alerta do SharePoint não entregues

Verifique a pasta LIXO no seu e-mail, uma vez que por vezes podem ser enviados alertas.

Determine se **todos os alertas não são entregues** ou **se não** é entregue um alerta individual de um ficheiro ou biblioteca específico.

- **Os alertas individuais não** são entregues: Se não for entregue um alerta individual de um ficheiro ou biblioteca específico, pode tentar eliminá-lo e recriá-lo. Consulte [Gerir, ver ou eliminar alertas do SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.
- Todos os alertas não são **entregues:** Se todos os alertas de múltiplos ficheiros ou bibliotecas não são entregues, visite o [dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) do Estado de Serviço para verificar se existem avisos/incidentes que possam estar a ocorrer no SharePoint ou no Exchange. O problema pode estar na capacidade de alerta ou atrasos nos e-mails através de Exchange. Também será importante ter em conta se os outros e-mails estão a ser entregues e, caso contrário, o problema está provavelmente Exchange entrega.

FAQ sobre alertas:

- Não é possível enviar alertas para o Grupo de Distribuição, apenas são suportados os grupos de Segurança e do O365.
- Não pode personalizar modelos de e-mail de alerta; tem de utilizar o Microsoft FLOW ou o Fluxo de Trabalho do SharePoint Designer para os conseguir.

## <a name="related-topics"></a>Tópicos Relacionados

Pretende experimentar o Microsoft Flow SharePoint Online?

- [Criar Flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint e Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
