---
title: Atrasos na receção de alertas SharePoint e OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785676"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Atrasos na receção de alertas SharePoint e OneDrive

- Verifique primeiro a pasta Junk ou Spam no seu e-mail.
- Se **todos os alertas de vários ficheiros ou bibliotecas estiverem atrasados,** visite o painel de [instrumentos de saúde](https://portal.office.com/adminportal/home?ref=/servicehealth) do serviço para verificar quaisquer avisos/incidentes que possam ocorrer com SharePoint ou Exchange. O problema pode estar com a capacidade de alerta do SharePoint ou com atrasos nos e-mails através do Exchange. Note também se outro e-mail está a ser entregue - se não, o problema é provável com atrasos de Troca.
- Se **um alerta individual de um ficheiro ou biblioteca específico não for entregue,** tente eliminá-lo e recriá-lo. Consulte [Gerir, ver ou eliminar os alertas do SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.

> [!NOTE]
> - Os alertas não podem ser enviados para um Grupo de Distribuição. Apenas os grupos de segurança e O365 são apoiados.
> - Não é possível personalizar modelos de e-mail de alerta. Tem de utilizar o Microsoft Flow ou o SharePoint Designer Workflow para os conseguir.
