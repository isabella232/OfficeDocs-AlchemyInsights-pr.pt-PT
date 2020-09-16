---
title: Enviar notificações personalizadas com a Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720657"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Como enviar notificações personalizadas aos utilizadores de dispositivos geridos iOS e Android

As notificações personalizadas para o Intune são processadas pela aplicação Portal da Empresa no dispositivo de um utilizador. A aplicação cria então a notificação push nesse dispositivo.

Seguem-se os pré-requisitos do dispositivo para suportar a receção de notificações personalizadas e para que a aplicação crie a notificação push:

- O dispositivo deve ter a aplicação Portal da Empresa instalada.  

- O dispositivo deve permitir que a aplicação Portal da Empresa envie notificações push. Quando a aplicação for instalada ou atualizada, irá solicitar ao utilizador que permita notificações.

- Os dispositivos Android devem ter os Serviços Google Play instalados.

- O aparelho deve ser matriculado com o Intune.

Para obter mais informações, incluindo como enviar uma mensagem, consulte a [documentação](https://docs.microsoft.com/intune/custom-notifications)do recurso .
