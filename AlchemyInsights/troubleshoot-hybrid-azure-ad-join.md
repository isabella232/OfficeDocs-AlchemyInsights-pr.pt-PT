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
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939282"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Resolução de problemas de associação ao Azure AD Híbrido

Altamente recomendado certifique-se de que um dispositivo pode aceder aos pontos finais de registo de dispositivos na conta do sistema ao utilizar o [script "Test Device Registration Connectivity"](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Se estiver a configurar registos de dispositivos pela primeira vez, consulte [Introdução à gestão de dispositivos no Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) para saber como colocar dispositivos sob o controlo do Azure AD.
1. Se estiver a registar dispositivos no Azure AD diretamente e a inscrevê-los no Intune, certifique-se primeiro de que [configurou o Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e de que tem [licenças](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) disponíveis.
1. Certifique-se de que tem autorização para executar operações no Azure AD e no AD no local. Apenas um administrador global no Azure AD pode gerir as definições dos registos de dispositivos. Além disso, se estiver a configurar o registo automático no seu Active Directory no local, terá de ser um administrador do Active Directory e do AD FS (se aplicável).

Para obter mais detalhes sobre como resolver potenciais problemas de associação ao Azure AD híbrido, consulte [Resolução de Problemas de Associação ao Azure AD híbrido](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Para configurar a associação ao Azure AD híbrido e Gerir Dispositivos através do portal Azure AD, consulte [Configurar dispositivos associados ao Azure AD híbrido (associados a um domínio no local)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) e [Gerir dispositivos através do portal do Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Para resolver problemas comuns com a associação ao Azure Active Directory Híbrido (AD), consulte [FAQ sobre a associação ao Azure AD híbrido](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
