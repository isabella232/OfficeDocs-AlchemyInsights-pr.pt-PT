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
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563521"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="81f8b-102">Atrasos na receção de alertas SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="81f8b-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="81f8b-103">Verifique primeiro a pasta Junk ou Spam no seu e-mail.</span><span class="sxs-lookup"><span data-stu-id="81f8b-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="81f8b-104">Se **todos os alertas de vários ficheiros ou bibliotecas estiverem atrasados,** visite o painel de [instrumentos de saúde](https://portal.office.com/adminportal/home?ref=/servicehealth) do serviço para verificar quaisquer avisos/incidentes que possam ocorrer com SharePoint ou Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f8b-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="81f8b-105">O problema pode estar com a capacidade de alerta do SharePoint ou com atrasos nos e-mails através do Exchange.</span><span class="sxs-lookup"><span data-stu-id="81f8b-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="81f8b-106">Note também se outro e-mail está a ser entregue - se não, o problema é provável com atrasos de Troca.</span><span class="sxs-lookup"><span data-stu-id="81f8b-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="81f8b-107">Se **um alerta individual de um ficheiro ou biblioteca específico não for entregue,** tente eliminá-lo e recriá-lo.</span><span class="sxs-lookup"><span data-stu-id="81f8b-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="81f8b-108">Consulte [Gerir, ver ou eliminar os alertas do SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.</span><span class="sxs-lookup"><span data-stu-id="81f8b-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="81f8b-109">Os alertas não podem ser enviados para um Grupo de Distribuição.</span><span class="sxs-lookup"><span data-stu-id="81f8b-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="81f8b-110">Apenas os grupos de segurança e O365 são apoiados.</span><span class="sxs-lookup"><span data-stu-id="81f8b-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="81f8b-111">Não é possível personalizar modelos de e-mail de alerta.</span><span class="sxs-lookup"><span data-stu-id="81f8b-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="81f8b-112">Tem de utilizar o Microsoft Flow ou o SharePoint Designer Workflow para os conseguir.</span><span class="sxs-lookup"><span data-stu-id="81f8b-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
