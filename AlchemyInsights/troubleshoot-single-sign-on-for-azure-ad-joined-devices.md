---
title: Remoção de Um Só-sinal nos Dispositivos Associados ao Azure AD
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
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039257"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Remoção de Um Só-sinal nos Dispositivos Associados ao Azure AD

Se tiver um ambiente do Active Directory (AD) no local e pretender associar os seus computadores associados ao domínio do Azure AD ao Azure AD, pode fazê-lo através da associação híbrida do Azure AD. [Como: Planear](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) a sua implementação Azure Active Directory associação híbrida fornece-lhe os passos relacionados para implementar uma associação híbrida do Azure AD no seu ambiente.

Para obter mais informações, consulte [Configurar dispositivos associados ao Azure AD para dispositivos associados ao Azure AD Single-Sign No Windows Hello para Empresas.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Problemas principais do Token de Atualização (PRT)**

Um Token de Atualização Principal (PRT) é um artefacto chave da autenticação do Azure AD em Windows 10, Windows Server 2016 e versões posteriores, iOS e dispositivos Android. É um JSON Web Token (JWT) emitido especialmente para interrompidos por tokens de primeiras partes da Microsoft para ativar o início de sessão único (SSO) nas aplicações utilizadas nesses dispositivos. Para obter detalhes sobre como um PRT é emitido, utilizado e protegido em dispositivos Windows 10, consulte O que é um Token de [Atualização Principal?.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES e AzureADPrt: YES**

Estes campos indicam se o utilizador exigiu com êxito a autenticação no Azure AD ao entrar no dispositivo. Se os valores são **NÃO,** pode ser devido a:

- Chave de armazenamento incorreta na TPM associada ao dispositivo após o registo (verifique a chave TesteTesteDa Chave enquanto está a ser executada)
- ID de Início de Sessão Alternativo
- Proxy HTTP não encontrado

Para remoção de problemas de dispositivos com o comando dsregcmd, consulte [Estado do SSO.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
