---
title: Remoção de problemas de associação do Azure AD
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
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939930"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Remoção de problemas de associação do Azure AD

1. Se estiver a configurar registos de dispositivos pela primeira vez, certifique-se de que reviu a Introdução à gestão de dispositivos no [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) que irá guiá-lo sobre como colocar os Dispositivos sob controlo para o Azure AD. 
1. Se estiver a registar dispositivos diretamente no Azure AD e a inscrever os [dispositivos](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) no Intune, terá de se certificar de que configurou o [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) e de que o licenciamento está em vigor primeiro.
1. Certifique-se de que está autorizado a efetuar operações no Azure AD. Apenas um administrador global no Azure AD pode gerir as definições dos registos de dispositivos.
1. Para implementar a associação do Azure AD, consulte [Planear a associação do Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Para obter mais detalhes sobre Windows 10 Pro como resolver problemas comuns com a associação do Azure AD, consulte as FAQ da [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) e para um dispositivo pro Windows 10, consulte Não é possível associar um computador com o [Azure AD -](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) É necessário atualizar para – Comunidade Microsoft
