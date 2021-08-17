---
title: Single-Sign para dispositivos Azure Active Directory associados
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
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050021"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>O único sinal de ação para Azure Active Directory Associados

Se tiver um ambiente do Active Directory (AD) no local e pretender associar os seus computadores associados ao domínio do Azure AD ao Azure AD, pode fazê-lo através da associação híbrida do Azure AD. [Como: Planear](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) a sua implementação Azure Active Directory associação híbrida fornece-lhe os passos relacionados para implementar uma associação híbrida do Azure AD no seu ambiente.

[Configurar dispositivos associados ao Azure AD para dispositivos Single-Sign No local através do Windows Hello para Empresas](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemas principais do Token de Atualização (PRT)** Um Token de Atualização Principal (PRT) é um artefacto chave da autenticação do Azure AD em Windows 10, Windows Server 2016 e versões posteriores, iOS e dispositivos Android. É um JSON Web Token (JWT) emitido especialmente para interrompidos por tokens de primeiras partes da Microsoft para ativar o início de sessão único (SSO) nas aplicações utilizadas nesses dispositivos. Em O que é um Token de Atualização [Principal?,](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)iremos fornecer detalhes sobre como um PRT é emitido, utilizado e protegido em Windows 10 dispositivos.

**WamDefaultSet: YES e AzureADPrt: YES** Estes campos indicam se o utilizador exigiu com êxito a autenticação no Azure AD ao entrar no dispositivo. Se os valores são **NÃO,** pode ser devido:

- Chave de armazenamento incorreta na TPM associada ao dispositivo após o registo (verifique a chave TesteDe Chave enquanto está a ser executada elevada).
- ID de Início de Sessão Alternativo
- Proxy HTTP não encontrado

Remova dispositivos com o comando dsregcmd – [estado do SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
