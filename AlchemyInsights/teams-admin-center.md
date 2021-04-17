---
title: Centro de Administração do Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826390"
---
# <a name="teams-admin-center"></a>Centro de Administração do Teams

Saiba mais sobre a gestão do Teams com o [Centro de Administração do Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Se não conseguir aceder ao Centro de Administração do Teams, verifique os seguintes itens:

- Verifique se autorizou os [endereços de IP e URL”s do Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) apropriados nos dispositivos periféricos (firewall, etc) ou nas regras de firewall do seu computador local.
- Verifique se o login que está a utilizar para aceder ao Portal de Administração do Teams corresponde ao seu nome de utilizador listado no [Portal de Administração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Se os utilizadores não aparecerem no Centro de Administração do Teams, verifique os seguintes itens:

- Criou utilizadores ou atribuiu licenças nas últimas 24 horas? Certifique-se de que esperou pelo menos 24 horas antes de iniciar um pedido de suporte.
- Verificou se atribuiu licenças apropriadas?
- Se tiver um Diretório Ativo no local, verifique se [o valor do msRTCSIP-PrimaryUserAddress ou do endereço SIP no campo ProxyAddresses no seu Diretório Ativo local é único e o formato corresponde](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) a um gole: Nome de **utilizador** do utilizador do centro [de administração Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Se pretende manter um Skype para implementação de Servidor de Negócios e ter utilizadores aloiados no local e online: siga o **"set up hybrid with Teams and Skype for Business Online"** no seu Skype para Business Server Control Panel e mova os utilizadores online.
