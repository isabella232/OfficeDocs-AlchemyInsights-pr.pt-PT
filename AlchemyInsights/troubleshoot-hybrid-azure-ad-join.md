---
title: Resolução de problemas de associação ao Azure AD Híbrido
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401918"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Resolução de problemas de associação ao Azure AD Híbrido

Altamente recomendado certifique-se de que um dispositivo pode aceder aos pontos finais de registo de dispositivos na conta do sistema ao utilizar o [script "Test Device Registration Connectivity"](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Se estiver a configurar registos de dispositivos pela primeira vez, consulte [Introdução à gestão de dispositivos no Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) para saber como colocar dispositivos sob o controlo do Azure AD.
1. Se estiver a registar dispositivos no Azure AD diretamente e a inscrevê-los no Intune, certifique-se primeiro de que [configurou o Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e de que tem [licenças](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) disponíveis.
1. Certifique-se de que tem autorização para executar operações no Azure AD e no AD no local. Apenas um administrador global no Azure AD pode gerir as definições dos registos de dispositivos. Além disso, se estiver a configurar o registo automático no seu Active Directory no local, terá de ser um administrador do Active Directory e do AD FS (se aplicável).

Para obter mais detalhes sobre como resolver potenciais problemas de associação ao Azure AD híbrido, consulte [Resolução de Problemas de Associação ao Azure AD híbrido](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Para configurar a associação ao Azure AD híbrido e Gerir Dispositivos através do portal Azure AD, consulte [Configurar dispositivos associados ao Azure AD híbrido (associados a um domínio no local)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) e [Gerir dispositivos através do portal do Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Para resolver problemas comuns com a associação ao Azure Active Directory Híbrido (AD), consulte [FAQ sobre a associação ao Azure AD híbrido](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
