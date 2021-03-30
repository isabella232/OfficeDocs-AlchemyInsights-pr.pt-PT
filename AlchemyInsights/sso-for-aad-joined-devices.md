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
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="10028-102">Sinal único para dispositivos de alistação ative aderiu</span><span class="sxs-lookup"><span data-stu-id="10028-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="10028-103">Se tiver um ambiente de Ative Directory (AD) no local e quiser juntar os seus computadores ligados ao domínio AD ao Azure AD, pode fazê-lo fazendo a ad AD híbrida.</span><span class="sxs-lookup"><span data-stu-id="10028-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="10028-104">[Como: Planeie a sua implementação híbrida Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) fornece-lhe os passos relacionados para implementar um AD híbrido Azure no seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="10028-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="10028-105">Configure Ad AD juntou dispositivos para on-ins Single-Sign Na utilização do Windows Hello para negócios</span><span class="sxs-lookup"><span data-stu-id="10028-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="10028-106">**Problemas primários de Token (PRT)** Um Token De Atualização Primária (PRT) é um artefacto chave da autenticação AD do Azure no Windows 10, Windows Server 2016 e versões posteriores, iOS e dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="10028-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="10028-107">Trata-se de um JSON Web Token (JWT) especialmente emitido para os corretores de token da primeira parte da Microsoft para permitir um único sign-on (SSO) em todas as aplicações utilizadas nesses dispositivos.</span><span class="sxs-lookup"><span data-stu-id="10028-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="10028-108">[Em What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="10028-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="10028-109">**WamDefaultSet: SIM e AzureADPrt: SIM** Estes campos indicam se o utilizador autenticou com sucesso a Azure AD ao iniciar sessão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="10028-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="10028-110">Se os valores forem **NÃO,** pode ser devido:</span><span class="sxs-lookup"><span data-stu-id="10028-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="10028-111">Chave de armazenamento estragada no TPM associado ao dispositivo no momento do registo (verifique o KeySignTest enquanto está em funcionamento elevado).</span><span class="sxs-lookup"><span data-stu-id="10028-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="10028-112">ID de login alternativo</span><span class="sxs-lookup"><span data-stu-id="10028-112">Alternate Login ID</span></span>
- <span data-ttu-id="10028-113">HTTP Proxy não encontrado</span><span class="sxs-lookup"><span data-stu-id="10028-113">HTTP Proxy not found</span></span>

<span data-ttu-id="10028-114">Dispositivos de resolução de problemas utilizando o comando dsregcmd - [Estado SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="10028-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
