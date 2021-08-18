---
title: Enviar notificações personalizadas com o Intune
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
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086175"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Como enviar notificações personalizadas para os utilizadores de dispositivos Android e iOS geridos

As notificações personalizadas do Intune são processadas pela Portal da Empresa aplicação no dispositivo de um utilizador. Em seguida, a aplicação cria a notificação push nesse dispositivo.

Seguem-se os pré-requisitos do dispositivo para suportar o recibo de notificações personalizadas e para que a aplicação crie a notificação push:

- O dispositivo tem de ter a Portal da Empresa de dados instalada.  

- O dispositivo tem de permitir que Portal da Empresa aplicação envie notificações push. Quando a aplicação for instalada ou atualizada, irá pedir ao utilizador que permita notificações.

- Os dispositivos Android têm de ter o Google Play Services instalado.

- O dispositivo tem de estar inscrito com o Intune.

Para obter mais informações, incluindo como enviar uma mensagem, consulte a documentação [da funcionalidade.](https://docs.microsoft.com/intune/custom-notifications)
