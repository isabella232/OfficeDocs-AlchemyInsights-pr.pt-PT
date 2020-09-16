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
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="01bcf-102">Como enviar notificações personalizadas aos utilizadores de dispositivos geridos iOS e Android</span><span class="sxs-lookup"><span data-stu-id="01bcf-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="01bcf-103">As notificações personalizadas para o Intune são processadas pela aplicação Portal da Empresa no dispositivo de um utilizador.</span><span class="sxs-lookup"><span data-stu-id="01bcf-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="01bcf-104">A aplicação cria então a notificação push nesse dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01bcf-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="01bcf-105">Seguem-se os pré-requisitos do dispositivo para suportar a receção de notificações personalizadas e para que a aplicação crie a notificação push:</span><span class="sxs-lookup"><span data-stu-id="01bcf-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="01bcf-106">O dispositivo deve ter a aplicação Portal da Empresa instalada.</span><span class="sxs-lookup"><span data-stu-id="01bcf-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="01bcf-107">O dispositivo deve permitir que a aplicação Portal da Empresa envie notificações push.</span><span class="sxs-lookup"><span data-stu-id="01bcf-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="01bcf-108">Quando a aplicação for instalada ou atualizada, irá solicitar ao utilizador que permita notificações.</span><span class="sxs-lookup"><span data-stu-id="01bcf-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="01bcf-109">Os dispositivos Android devem ter os Serviços Google Play instalados.</span><span class="sxs-lookup"><span data-stu-id="01bcf-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="01bcf-110">O aparelho deve ser matriculado com o Intune.</span><span class="sxs-lookup"><span data-stu-id="01bcf-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="01bcf-111">Para obter mais informações, incluindo como enviar uma mensagem, consulte a [documentação](https://docs.microsoft.com/intune/custom-notifications)do recurso .</span><span class="sxs-lookup"><span data-stu-id="01bcf-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
