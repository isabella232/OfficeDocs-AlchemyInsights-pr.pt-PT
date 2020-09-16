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
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="f769c-102">Atrasos na receção de alertas SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="f769c-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="f769c-103">Verifique primeiro a pasta Junk ou Spam no seu e-mail.</span><span class="sxs-lookup"><span data-stu-id="f769c-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="f769c-104">Se **todos os alertas de vários ficheiros ou bibliotecas estiverem atrasados,** visite o painel de [instrumentos de saúde](https://portal.office.com/adminportal/home?ref=/servicehealth) do serviço para verificar quaisquer avisos/incidentes que possam ocorrer com SharePoint ou Exchange.</span><span class="sxs-lookup"><span data-stu-id="f769c-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="f769c-105">O problema pode estar com a capacidade de alerta do SharePoint ou com atrasos nos e-mails através do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f769c-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="f769c-106">Note também se outro e-mail está a ser entregue - se não, o problema é provável com atrasos de Troca.</span><span class="sxs-lookup"><span data-stu-id="f769c-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="f769c-107">Se **um alerta individual de um ficheiro ou biblioteca específico não for entregue,** tente eliminá-lo e recriá-lo.</span><span class="sxs-lookup"><span data-stu-id="f769c-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="f769c-108">Consulte [Gerir, ver ou eliminar os alertas do SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) para recriar o alerta.</span><span class="sxs-lookup"><span data-stu-id="f769c-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="f769c-109">Os alertas não podem ser enviados para um Grupo de Distribuição.</span><span class="sxs-lookup"><span data-stu-id="f769c-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="f769c-110">Apenas os grupos de segurança e O365 são apoiados.</span><span class="sxs-lookup"><span data-stu-id="f769c-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="f769c-111">Não é possível personalizar modelos de e-mail de alerta.</span><span class="sxs-lookup"><span data-stu-id="f769c-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="f769c-112">Tem de utilizar o Microsoft Flow ou o SharePoint Designer Workflow para os conseguir.</span><span class="sxs-lookup"><span data-stu-id="f769c-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
