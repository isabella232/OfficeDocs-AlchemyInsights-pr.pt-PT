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
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configura definições de privacidade

Por predefinição, se o Microsoft Edge for implantado em plataformas não-Windows, os dados de diagnóstico e as informações do site não são enviados para a Microsoft. No entanto, se o Microsoft Edge for implantado no Windows 10, os dados de diagnóstico e as informações do site são enviados de acordo com as definições de [dados do Windows Diagnostic](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)dos utilizadores .

Para configurar como o Microsoft Edge lida com a recolha de dados para a sua organização, utilize as seguintes políticas de grupo:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Esta política permite a comunicação de dados de utilização e de acidentes.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Esta política envia informações do site que são usadas para melhorar os serviços da Microsoft.

Para saber mais, consulte [as definições de política](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)de configuração .