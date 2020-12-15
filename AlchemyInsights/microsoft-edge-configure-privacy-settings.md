---
title: Microsoft Edge configura definições de privacidade
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678856"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="08684-102">Microsoft Edge configura definições de privacidade</span><span class="sxs-lookup"><span data-stu-id="08684-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="08684-103">Por predefinição, se o Microsoft Edge for implantado em plataformas não-Windows, os dados de diagnóstico e as informações do site não são enviados para a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="08684-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="08684-104">No entanto, se o Microsoft Edge for implantado no Windows 10, os dados de diagnóstico e as informações do site são enviados de acordo com as definições de [dados do Windows Diagnostic](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)dos utilizadores .</span><span class="sxs-lookup"><span data-stu-id="08684-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="08684-105">Para configurar como o Microsoft Edge lida com a recolha de dados para a sua organização, utilize as seguintes políticas de grupo:</span><span class="sxs-lookup"><span data-stu-id="08684-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="08684-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Esta política permite a comunicação de dados de utilização e de acidentes.</span><span class="sxs-lookup"><span data-stu-id="08684-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="08684-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Esta política envia informações do site que são usadas para melhorar os serviços da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="08684-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="08684-108">Para saber mais, consulte [as definições de política](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)de configuração .</span><span class="sxs-lookup"><span data-stu-id="08684-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>