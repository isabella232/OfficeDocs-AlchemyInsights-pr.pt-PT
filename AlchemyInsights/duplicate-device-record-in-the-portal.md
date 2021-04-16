---
title: Registo de dispositivo duplicado no portal
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814527"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="7a11d-102">Registo de dispositivo duplicado no portal</span><span class="sxs-lookup"><span data-stu-id="7a11d-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="7a11d-103">É possível que veja 2 registos de um dispositivo no portal se o dispositivo não reportar corretamente o estado de cogestão ao site do Gestor de Configuração.</span><span class="sxs-lookup"><span data-stu-id="7a11d-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="7a11d-104">Para verificar o estado de cogestão de um dispositivo, consulte a coluna **Cogerido** do dispositivo na consola do Gestor de Configuração.</span><span class="sxs-lookup"><span data-stu-id="7a11d-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="7a11d-105">Se a coluna não estiver visível, pode adicioná-la, ao clicar com o botão do rato em qualquer um dos cabeçalhos da coluna e selecioná-la a partir da lista.</span><span class="sxs-lookup"><span data-stu-id="7a11d-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="7a11d-106">O valor cogerido deve ser **Sim**.</span><span class="sxs-lookup"><span data-stu-id="7a11d-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="7a11d-107">Se o valor for **Não**, abra a miniaplicação cliente do Gestor de Configuração no dispositivo cliente e verifique a propriedade **Cogestão** no separador Geral.</span><span class="sxs-lookup"><span data-stu-id="7a11d-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="7a11d-108">Se o valor for **Ativado**, isso significa que existem problemas de comunicação do cliente com o Ponto de Gestão.</span><span class="sxs-lookup"><span data-stu-id="7a11d-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="7a11d-109">Consulte o ficheiro **CcmMessaging.log** no dispositivo para investigar potenciais problemas de conectividade.</span><span class="sxs-lookup"><span data-stu-id="7a11d-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="7a11d-110">Se o valor for **Desativado** e o dispositivo estiver inscrito no Intune, certifique-se de que o dispositivo recebeu a política de cogestão, ao rever o ficheiro **CoManagementHandler.log** no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7a11d-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
