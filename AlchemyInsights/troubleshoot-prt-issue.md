---
title: Problema de resolução de problemas prt
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573723"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="b90ea-102">Problema de resolução de problemas prt</span><span class="sxs-lookup"><span data-stu-id="b90ea-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="b90ea-103">Para que qualquer dispositivo complete a autenticação, deve estar totalmente registado e em bom estado e capaz de adquirir um Token Primary Refresh (PRT).</span><span class="sxs-lookup"><span data-stu-id="b90ea-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="b90ea-104">O processo híbrido Azure AD junta-se ao processo de registo requer que os dispositivos estejam numa rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="b90ea-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="b90ea-105">Também funciona sobre a VPN, mas há algumas ressalvas nisso.</span><span class="sxs-lookup"><span data-stu-id="b90ea-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="b90ea-106">Ouvimos clientes que precisam de ajuda para resolver problemas com o híbrido Azure AD aderir ao processo de registo em circunstâncias de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="b90ea-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="b90ea-107">Aqui está uma descrição do que está a acontecer 'debaixo do capot' durante o processo de registo.</span><span class="sxs-lookup"><span data-stu-id="b90ea-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="b90ea-108">**Ambiente de autenticação em nuvem (utilizando a sincronização de haxixe de palavra-passe AZure ou a autenticação de passagem)**</span><span class="sxs-lookup"><span data-stu-id="b90ea-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="b90ea-109">Este fluxo de registo também é conhecido como "Sync Join".</span><span class="sxs-lookup"><span data-stu-id="b90ea-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="b90ea-110">O Windows 10 descobre um registo SCP ao iniciar sessão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b90ea-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="b90ea-111">O dispositivo tenta primeiro obter informações do cliente da SCP do lado do cliente no registo [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="b90ea-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="b90ea-112">Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)</span><span class="sxs-lookup"><span data-stu-id="b90ea-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="b90ea-113">Se falhar, o dispositivo comunica com o Ative Directory (AD) no local para obter informações do inquilino do Ponto de Ligação de Serviço (SCP).</span><span class="sxs-lookup"><span data-stu-id="b90ea-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="b90ea-114">Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="b90ea-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="b90ea-115">Recomendamos que se habilita o SCP no AD e utilize apenas o SCP do lado do cliente para validação inicial.</span><span class="sxs-lookup"><span data-stu-id="b90ea-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="b90ea-116">O Windows 10 tenta comunicar com o Azure AD no contexto do sistema para se autenticar contra o AD Azure.</span><span class="sxs-lookup"><span data-stu-id="b90ea-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="b90ea-117">Pode verificar se o dispositivo pode aceder aos recursos da Microsoft sob a conta do sistema utilizando o script de conectividade de registo do dispositivo de teste.</span><span class="sxs-lookup"><span data-stu-id="b90ea-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="b90ea-118">O Windows 10 gera um certificado auto-assinado e armazena-o sob o objeto do computador no Local AD.</span><span class="sxs-lookup"><span data-stu-id="b90ea-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="b90ea-119">Isto requer uma linha de visão para o Controlador de Domínio.</span><span class="sxs-lookup"><span data-stu-id="b90ea-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="b90ea-120">Um objeto do dispositivo que tenha um certificado é sincronizado com a Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b90ea-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="b90ea-121">O ciclo de sincronização é a cada 30 minutos por defeito, mas depende da configuração do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b90ea-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="b90ea-122">Para mais informações, por favor leia as referências a este [documento.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)</span><span class="sxs-lookup"><span data-stu-id="b90ea-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="b90ea-123">Nesta fase, deverá ser possível ver o dispositivo do sujeito em estado "Pendente" sob a lâmina do Dispositivo do Portal Azure.</span><span class="sxs-lookup"><span data-stu-id="b90ea-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="b90ea-124">No próximo login do utilizador para o Windows 10, o registo será concluído.</span><span class="sxs-lookup"><span data-stu-id="b90ea-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="b90ea-125">Se estiver na VPN e um processo de login de logoff terminar a conectividade do domínio, pode acionar o registo manualmente:</span><span class="sxs-lookup"><span data-stu-id="b90ea-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="b90ea-126">Emita um dsregcmd /junte-se localmente na solicitação de administração ou remotamente através do PSExec para o seu PC.</span><span class="sxs-lookup"><span data-stu-id="b90ea-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="b90ea-127">Por exemplo, PsExec -s \\ win10client01 cmd, dsregcmd /join</span><span class="sxs-lookup"><span data-stu-id="b90ea-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="b90ea-128">Para obter mais detalhes sobre os problemas da Hybrid Join, consulte [a Questão dos dispositivos de resolução de problemas](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="b90ea-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
