---
title: Resolução de problemas Único sinal para dispositivos de ad AD Azure
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037329"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Resolução de problemas Único sinal para dispositivos de ad AD Azure

Se tiver um ambiente de Ative Directory (AD) no local e quiser juntar os seus computadores ligados ao domínio AD ao Azure AD, pode fazê-lo fazendo a ad AD híbrida. [Como: Planeie a sua implementação híbrida Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) fornece-lhe os passos relacionados para implementar um AD híbrido Azure no seu ambiente.

Para obter mais informações, consulte [dispositivos de ad Configure Azure Ad para Single-Sign No uso do Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Problemas primários de Token (PRT)**

Um Token De Atualização Primária (PRT) é um artefacto chave da autenticação AD do Azure no Windows 10, Windows Server 2016 e versões posteriores, iOS e dispositivos Android. Trata-se de um JSON Web Token (JWT) especialmente emitido para os corretores de token da primeira parte da Microsoft para permitir um único sign-on (SSO) em todas as aplicações utilizadas nesses dispositivos. Para obter mais informações sobre como um PRT é emitido, usado e protegido em dispositivos Windows 10, veja [o que é um Token de Atualização Primária?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: SIM e AzureADPrt: SIM**

Estes campos indicam se o utilizador autenticou com sucesso a Azure AD ao iniciar sessão no dispositivo. Se os valores forem **NÃO,** pode ser devido a:

- Chave de armazenamento estragada no TPM associado ao dispositivo no momento do registo (verifique o KeySignTest enquanto está em execução elevado)
- ID de login alternativo
- HTTP Proxy não encontrado

Para resolver os problemas utilizando o comando dsregcmd, consulte o [estado SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
