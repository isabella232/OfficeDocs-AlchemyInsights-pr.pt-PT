---
title: A minha aplicação não é mostrada na Governação da Aplicação
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454994"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>A minha aplicação não é mostrada na Governação da Aplicação

Se a sua aplicação não for apresentado na Governação da Aplicação, verifique o seguinte:

1. Vá para [o Azure AD](https://aad.portal.azure.com/) e procure o ID da aplicação para a sua aplicação ao procurar o nome da aplicação na barra superior, na página Visão Geral.

1. O Access Graph Explorer e procure o ID da aplicação no seu principal de serviço ao utilizar esta consulta e substituir pelo ID da aplicação <appId> relevante: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Se não for devolvido nenhum resultado, procure o ID da aplicação na aplicação utilizando esta consulta e substituindo pelo ID da aplicação <appId> relevante: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Se tiver problemas com a consulta, consulte Obter [suporte.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Para obter mais informações ou informações sobre as suas Aplicações na Governação da Aplicação, consulte Saber mais sobre [visibilidade e informações.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Para obter mais informações sobre como ver as suas aplicações, consulte [Ver as suas aplicações.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
