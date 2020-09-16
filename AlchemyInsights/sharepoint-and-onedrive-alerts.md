---
title: Atrasos na receção de alertas SharePoint e OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727254"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Atrasos na receção de alertas SharePoint e OneDrive

- Verifique primeiro a pasta Junk ou Spam no seu e-mail.
- Se **todos os alertas de vários ficheiros ou bibliotecas estiverem atrasados,** visite o painel de [instrumentos de saúde](https://portal.office.com/adminportal/home?ref=/servicehealth) do serviço para verificar quaisquer avisos/incidentes que possam ocorrer com SharePoint ou Exchange. O problema pode estar com a capacidade de alerta do SharePoint ou com atrasos nos e-mails através do Exchange. Note também se outro e-mail está a ser entregue - se não, o problema é provável com atrasos de Troca.
- Se **um alerta individual de um ficheiro ou biblioteca específico não for entregue,** tente eliminá-lo e recriá-lo. Consulte [Gerir, ver ou eliminar os alertas do SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.

> [!NOTE]
> - Os alertas não podem ser enviados para um Grupo de Distribuição. Apenas os grupos de segurança e O365 são apoiados.
> - Não é possível personalizar modelos de e-mail de alerta. Tem de utilizar o Microsoft Flow ou o SharePoint Designer Workflow para os conseguir.
