---
title: Microsoft Edge configurar definições de privacidade
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114183"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configurar definições de privacidade

Por predefinição, Microsoft Edge estiver implementado em plataformas que não sejam Windows, os dados de diagnóstico e as informações do site não são enviados para a Microsoft. No entanto, se Microsoft Edge implementado no Windows 10, os dados de diagnóstico e as informações do site são enviados de acordo com as definições de dados de Windows [diagnóstico dos utilizadores.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Para configurar a forma como Microsoft Edge a recolha de dados para a sua organização, utilize as seguintes políticas de grupo:
- [MétricasReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): esta política permite a comunicação de dados relacionados com falhas e utilização.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)esta política envia informações do site que são utilizadas para melhorar serviços Microsoft.

Para saber mais, consulte [Configurar definições de política.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)