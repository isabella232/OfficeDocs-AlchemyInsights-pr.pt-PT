---
title: Single-Sign para o Azure Ative Directory juntou-se a dispositivos
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
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405657"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Sinal único para dispositivos de alistação ative aderiu

Se tiver um ambiente de Ative Directory (AD) no local e quiser juntar os seus computadores ligados ao domínio AD ao Azure AD, pode fazê-lo fazendo a ad AD híbrida. [Como: Planeie a sua implementação híbrida Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) fornece-lhe os passos relacionados para implementar um AD híbrido Azure no seu ambiente.

[Configure Ad AD juntou dispositivos para on-ins Single-Sign Na utilização do Windows Hello para negócios](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemas primários de Token (PRT)** Um Token De Atualização Primária (PRT) é um artefacto chave da autenticação AD do Azure no Windows 10, Windows Server 2016 e versões posteriores, iOS e dispositivos Android. Trata-se de um JSON Web Token (JWT) especialmente emitido para os corretores de token da primeira parte da Microsoft para permitir um único sign-on (SSO) em todas as aplicações utilizadas nesses dispositivos. [Em What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: SIM e AzureADPrt: SIM** Estes campos indicam se o utilizador autenticou com sucesso a Azure AD ao iniciar sessão no dispositivo. Se os valores forem **NÃO,** pode ser devido:

- Chave de armazenamento estragada no TPM associado ao dispositivo no momento do registo (verifique o KeySignTest enquanto está em funcionamento elevado).
- ID de login alternativo
- HTTP Proxy não encontrado

Dispositivos de resolução de problemas utilizando o comando dsregcmd - [Estado SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
