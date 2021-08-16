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
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049355"
---
# <a name="teams-admin-center"></a>Centro de Administração do Teams

Saiba mais sobre a gestão do Teams com o [Centro de Administração do Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Se não conseguir aceder ao Centro de Administração do Teams, verifique os seguintes itens:

- Verifique se autorizou os [endereços de IP e URL”s do Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) apropriados nos dispositivos periféricos (firewall, etc) ou nas regras de firewall do seu computador local.
- Verifique se o login que está a utilizar para aceder ao Portal de Administração do Teams corresponde ao seu nome de utilizador listado no [Portal de Administração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Se os utilizadores não aparecerem no Centro de Administração do Teams, verifique os seguintes itens:

- Criou utilizadores ou atribuiu licenças nas últimas 24 horas? Certifique-se de que esperou pelo menos 24 horas antes de iniciar um pedido de suporte.
- Verificou se atribuiu licenças apropriadas?
- Se tiver um Active Directory no local, verifique se o valor [de msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) ou do endereço SIP no campo ProxyAddresses no seu Active Directory local é exclusivo e o formato corresponde a sip: Nome de utilizador do utilizador do [centro de administração do Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Se quiser manter uma implementação do Skype para Empresas Server e permitir que os utilizadores se aloguem no local e online: siga a "Configuração híbrida com **o Teams e o Skype para Empresas Online"** no seu Painel de Controlo do Skype para Empresas Server e mova utilizadores Online.
