---
title: Envie notificações personalizadas com a Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886868"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Como enviar notificações personalizadas para os usuários de dispositivos iOS e Android gerenciados

Notificações personalizadas para Intune são processadas pelo aplicativo Portal da Empresa no dispositivo de um usuário. O aplicativo, em seguida, cria a notificação por push nesse dispositivo.

A seguir estão os pré-requisitos do dispositivo para suportar o recebimento de notificações personalizadas e, para que o aplicativo crie a notificação por push:

- O dispositivo deve ter o aplicativo Portal da Empresa instalado.  

- O dispositivo deve permitir que o aplicativo Portal da Empresa envie notificações por push. Quando o aplicativo for instalado ou atualizado, ele solicitará ao usuário que permita notificações.

- Os dispositivos Android devem instalar o Google Play Services.

- O dispositivo deve ser inscrito com Intune.

Para obter mais informações, incluindo como enviar uma mensagem, consulte a documentação do [recurso.](https://docs.microsoft.com/intune/custom-notifications)
