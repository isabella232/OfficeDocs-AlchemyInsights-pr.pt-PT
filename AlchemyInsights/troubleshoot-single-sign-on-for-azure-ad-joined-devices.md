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
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="b105a-102">Resolução de problemas Único sinal para dispositivos de ad AD Azure</span><span class="sxs-lookup"><span data-stu-id="b105a-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="b105a-103">Se tiver um ambiente de Ative Directory (AD) no local e quiser juntar os seus computadores ligados ao domínio AD ao Azure AD, pode fazê-lo fazendo a ad AD híbrida.</span><span class="sxs-lookup"><span data-stu-id="b105a-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="b105a-104">[Como: Planeie a sua implementação híbrida Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) fornece-lhe os passos relacionados para implementar um AD híbrido Azure no seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="b105a-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="b105a-105">Para obter mais informações, consulte [dispositivos de ad Configure Azure Ad para Single-Sign No uso do Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="b105a-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="b105a-106">**Problemas primários de Token (PRT)**</span><span class="sxs-lookup"><span data-stu-id="b105a-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="b105a-107">Um Token De Atualização Primária (PRT) é um artefacto chave da autenticação AD do Azure no Windows 10, Windows Server 2016 e versões posteriores, iOS e dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="b105a-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="b105a-108">Trata-se de um JSON Web Token (JWT) especialmente emitido para os corretores de token da primeira parte da Microsoft para permitir um único sign-on (SSO) em todas as aplicações utilizadas nesses dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b105a-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="b105a-109">Para obter mais informações sobre como um PRT é emitido, usado e protegido em dispositivos Windows 10, veja [o que é um Token de Atualização Primária?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="b105a-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="b105a-110">**WamDefaultSet: SIM e AzureADPrt: SIM**</span><span class="sxs-lookup"><span data-stu-id="b105a-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="b105a-111">Estes campos indicam se o utilizador autenticou com sucesso a Azure AD ao iniciar sessão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b105a-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="b105a-112">Se os valores forem **NÃO,** pode ser devido a:</span><span class="sxs-lookup"><span data-stu-id="b105a-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="b105a-113">Chave de armazenamento estragada no TPM associado ao dispositivo no momento do registo (verifique o KeySignTest enquanto está em execução elevado)</span><span class="sxs-lookup"><span data-stu-id="b105a-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="b105a-114">ID de login alternativo</span><span class="sxs-lookup"><span data-stu-id="b105a-114">Alternate Login ID</span></span>
- <span data-ttu-id="b105a-115">HTTP Proxy não encontrado</span><span class="sxs-lookup"><span data-stu-id="b105a-115">HTTP Proxy not found</span></span>

<span data-ttu-id="b105a-116">Para resolver os problemas utilizando o comando dsregcmd, consulte o [estado SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="b105a-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
