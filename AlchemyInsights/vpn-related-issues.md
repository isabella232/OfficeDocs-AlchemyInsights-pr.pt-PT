---
title: Questões relacionadas com a VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555230"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="95fd1-102">Questões relacionadas com a VPN</span><span class="sxs-lookup"><span data-stu-id="95fd1-102">VPN related issues</span></span>

<span data-ttu-id="95fd1-103">A implementação bem sucedida da conectividade VPN para clientes MDM depende de um perfil implantado que reflita corretamente os requisitos da infraestrutura VPN.</span><span class="sxs-lookup"><span data-stu-id="95fd1-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="95fd1-104">Para as definições apropriadas para as plataformas de clientes que está a investigar, consulte:</span><span class="sxs-lookup"><span data-stu-id="95fd1-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="95fd1-105">Windows 10 e Windows Holographic device configurações para adicionar ligações VPN usando Intune</span><span class="sxs-lookup"><span data-stu-id="95fd1-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="95fd1-106">Adicione definições VPN em dispositivos iOS e iPadOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="95fd1-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="95fd1-107">Configurações de dispositivos Android para configurar VPN em Intune</span><span class="sxs-lookup"><span data-stu-id="95fd1-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="95fd1-108">Adicione definições VPN em dispositivos macOS no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="95fd1-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="95fd1-109">Se o seu perfil VPN utilizar a autenticação baseada em certificados, certifique-se de que os perfis de certificado de base e de certificado de autenticação do cliente ligados ao perfil VPN são implementados com sucesso.</span><span class="sxs-lookup"><span data-stu-id="95fd1-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="95fd1-110">**Questões Comuns**</span><span class="sxs-lookup"><span data-stu-id="95fd1-110">**Common Issues**</span></span>

<span data-ttu-id="95fd1-111">**Desloquei um perfil VPN para um dispositivo. A Intune está a mostrar que foi bem sucedida, mas o dispositivo não está a ligar-se à VPN.**</span><span class="sxs-lookup"><span data-stu-id="95fd1-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="95fd1-112">Um estado de sucesso significa que a Intune implementou o perfil com sucesso como configurado.</span><span class="sxs-lookup"><span data-stu-id="95fd1-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="95fd1-113">No entanto, estas configurações podem não corresponder aos seus requisitos de rede e/ou autenticação.</span><span class="sxs-lookup"><span data-stu-id="95fd1-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="95fd1-114">Reveja os registos no serviço de infraestrutura e autenticação (no servidor VPN e no servidor NPS/Radius) para obter mais detalhes sobre a tentativa de ligação.</span><span class="sxs-lookup"><span data-stu-id="95fd1-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="95fd1-115">Poderá ter de trabalhar com a sua equipa de infraestruturas de rede, ou com o fornecedor de VPN de terceiros, para recolher e rever registos.</span><span class="sxs-lookup"><span data-stu-id="95fd1-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="95fd1-116">**Quando configurar uma VPN personalizada para iOS, a funcionalidade VPN por aplicação não é disponibilizada.**</span><span class="sxs-lookup"><span data-stu-id="95fd1-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="95fd1-117">A VPN por aplicação para dispositivos iOS no Intune está atualmente disponível para uma lista específica de fornecedores e parceiros, que também devem cumprir os pré-requisitos do certificado antes de configurar uma VPN por aplicação.</span><span class="sxs-lookup"><span data-stu-id="95fd1-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="95fd1-118">Para obter mais informações, consulte [Configurar por aplicação Rede Privada Virtual (VPN) para dispositivos iOS/iPadOS no Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="95fd1-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="95fd1-119">Para obter mais informações sobre todos os tipos de conexão VPN no Intune, consulte [criar perfis VPN para ligar aos servidores VPN no Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="95fd1-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="95fd1-120">**IOS On Demand VPN não é desencadeando quando um domínio configurado é acedido**</span><span class="sxs-lookup"><span data-stu-id="95fd1-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="95fd1-121">Para testar as definições automáticas de VPN, defina os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="95fd1-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="95fd1-122">Quero fazer o seguinte: **Avaliar cada tentativa de ligação**</span><span class="sxs-lookup"><span data-stu-id="95fd1-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="95fd1-123">Escolha se deve ligar: **Conecte-se se necessário**</span><span class="sxs-lookup"><span data-stu-id="95fd1-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="95fd1-124">Quando os utilizadores acedem a estes domínios: nome de **domínio-alvo** *domain name*</span><span class="sxs-lookup"><span data-stu-id="95fd1-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="95fd1-125">Se a configuração acima não for bem sucedida, adicione o seguinte elemento:</span><span class="sxs-lookup"><span data-stu-id="95fd1-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="95fd1-126">Quando este URL é inacessível, force a ligação da VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="95fd1-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>