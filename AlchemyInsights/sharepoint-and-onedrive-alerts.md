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
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="0ae1a-102">Atrasos na receção de alertas SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="0ae1a-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="0ae1a-103">Primeiro, verifique a pasta Junk ou Spam no seu e-mail.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="0ae1a-104">Se **todos os alertas de vários ficheiros ou bibliotecas forem atrasados,** visite o painel de assistência ao [serviço](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) para verificar se existem avisos/incidentes que possam ocorrer com o SharePoint ou Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="0ae1a-105">O problema pode estar com a capacidade de alerta SharePoint ou atrasos em e-mails através do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="0ae1a-106">Note também se outros e-mails estão a ser entregues — caso contrário, o problema é provável que seja com atrasos na Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="0ae1a-107">Se **um alerta individual de um ficheiro ou biblioteca específico não for entregue,** tente eliminá-lo e recriá-lo.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="0ae1a-108">Ver [Gerir, visualizar ou eliminar alertas sharePoint](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) para recriar o alerta.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="0ae1a-109">Os alertas não podem ser enviados para um Grupo de Distribuição.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="0ae1a-110">Apenas os grupos de Segurança e O365 são apoiados.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="0ae1a-111">Não é possível personalizar modelos de e-mail de alerta.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="0ae1a-112">Tem de utilizar o Microsoft Flow ou o SharePoint Designer Workflow para os conseguir.</span><span class="sxs-lookup"><span data-stu-id="0ae1a-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
