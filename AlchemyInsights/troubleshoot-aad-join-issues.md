---
title: Resolução de problemas Azure AD junta-se a questões
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405757"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Resolução de problemas Azure AD junta-se a questões

1. Se estiver a configurar os registos do dispositivo pela primeira vez, certifique-se de que reviu [a Introdução à gestão do dispositivo no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) que o irá orientar sobre como colocar os Dispositivos sob o controlo da Azure AD. 
1. Se estiver a registar os dispositivos no Azure AD diretamente e a inscrevê-los no Intune, terá de se certificar de que [tem configurado Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) e ter o [licenciamento](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) em primeiro lugar.
1. Certifique-se de que está autorizado a realizar operações no Azure AD. Apenas um administrador global em Azure AD pode gerir as definições para registos de dispositivos.
1. Para fazer a Azure AD aderir à implementação, consulte [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Para obter mais detalhes sobre a resolução de problemas comuns com a Azure AD consulte [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) e para o windows 10 pro device, ver [Incapaz de juntar a máquina do Windows 10 Pro a Azure AD - Necessidade de upgrade para - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
