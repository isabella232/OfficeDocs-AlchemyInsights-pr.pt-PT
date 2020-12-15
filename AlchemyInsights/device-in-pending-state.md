---
title: Dispositivo em estado pendente
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679988"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="82600-102">Dispositivo em estado pendente</span><span class="sxs-lookup"><span data-stu-id="82600-102">Device in pending state</span></span>

<span data-ttu-id="82600-103">**Pré-requisitos:**</span><span class="sxs-lookup"><span data-stu-id="82600-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="82600-104">Se estiver a configurar os registos do dispositivo pela primeira vez, certifique-se de que reviu [a Introdução à gestão do dispositivo no Azure Ative Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) que o guiará sobre como obter dispositivos sob o controlo da Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82600-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="82600-105">Se estiver a registar os dispositivos no Azure AD diretamente e a inscrevê-los no Intune, terá de se certificar de que [tem configurado Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) e ter o [licenciamento](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) em primeiro lugar.</span><span class="sxs-lookup"><span data-stu-id="82600-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="82600-106">Certifique-se de que está autorizado a realizar operações em Azure AD e no local AD.</span><span class="sxs-lookup"><span data-stu-id="82600-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="82600-107">Apenas um administrador global em Azure AD pode gerir as definições para registos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="82600-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="82600-108">Além disso, se estiver a configurar registos automáticos no seu Ative Directory no local, terá de ser administrador do Ative Directory e da AD FS (se aplicável).</span><span class="sxs-lookup"><span data-stu-id="82600-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="82600-109">O processo híbrido Azure AD aderir ao processo de registo requer que os dispositivos estejam na rede corporativa.</span><span class="sxs-lookup"><span data-stu-id="82600-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="82600-110">Também funciona sobre a VPN, mas há algumas ressalvas nisso.</span><span class="sxs-lookup"><span data-stu-id="82600-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="82600-111">Ouvimos os clientes precisarem de assistência para resolver problemas com o híbrido Azure AD aderir ao processo de registo em circunstâncias de trabalho remoto.</span><span class="sxs-lookup"><span data-stu-id="82600-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="82600-112">**Ambiente de autenticação em nuvem (utilizando a sincronização de haxixe de palavra-passe AZure ou a autenticação de passagem)**</span><span class="sxs-lookup"><span data-stu-id="82600-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="82600-113">Este fluxo de registo também é conhecido como "Sync Join".</span><span class="sxs-lookup"><span data-stu-id="82600-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="82600-114">Aqui está uma descrição do que acontece durante o processo de registo:</span><span class="sxs-lookup"><span data-stu-id="82600-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="82600-115">O Windows 10 descobre o registo do Ponto de Ligação de Serviço (SCP) quando o utilizador inicia sessão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="82600-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="82600-116">O dispositivo tenta primeiro obter informações do cliente da SCP do lado do cliente no registo [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="82600-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="82600-117">Para mais informações, consulte [o documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)</span><span class="sxs-lookup"><span data-stu-id="82600-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="82600-118">Se falhar, o dispositivo comunica com o Ative Directory no local para obter informações do inquilino da SCP.</span><span class="sxs-lookup"><span data-stu-id="82600-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="82600-119">Para verificar o SCP, consulte este [documento](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="82600-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="82600-120">Recomendamos que se habilita o SCP no Ative Directory e utilize apenas o SCP do lado do cliente para validação inicial.</span><span class="sxs-lookup"><span data-stu-id="82600-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="82600-121">O Windows 10 tenta comunicar com o Azure AD no contexto do sistema para se autenticar contra o AD Azure.</span><span class="sxs-lookup"><span data-stu-id="82600-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="82600-122">Pode verificar se o dispositivo pode aceder aos recursos da Microsoft sob a conta do sistema utilizando o [script de conectividade de registo do dispositivo de teste](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="82600-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="82600-123">O Windows 10 gera certificado auto-assinado e armazena-o sob o objeto do computador no Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="82600-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="82600-124">Isto requer uma linha de visão para o Controlador de Domínio.</span><span class="sxs-lookup"><span data-stu-id="82600-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="82600-125">O objeto do dispositivo que tem certificado é sincronizado com Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="82600-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="82600-126">O ciclo de sincronização é a cada 30 minutos por defeito, mas depende da configuração do Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="82600-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="82600-127">Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)</span><span class="sxs-lookup"><span data-stu-id="82600-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="82600-128">Nesta fase, você deve ser capaz de ver o dispositivo sujeito em estado "**Pendente**" sob a lâmina do dispositivo do Portal Azure.</span><span class="sxs-lookup"><span data-stu-id="82600-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="82600-129">No próximo login do utilizador para o Windows 10, o registo será concluído.</span><span class="sxs-lookup"><span data-stu-id="82600-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="82600-130">Se estiver em VPN e o logoff/login terminar a conectividade do domínio, pode ativar o registo manualmente.</span><span class="sxs-lookup"><span data-stu-id="82600-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="82600-131">Para fazer isto:</span><span class="sxs-lookup"><span data-stu-id="82600-131">To do that:</span></span>
    >
    > <span data-ttu-id="82600-132">Emita um `dsregcmd /join` local local na solicitação de administração ou remotamente via PSExec para o seu PC.</span><span class="sxs-lookup"><span data-stu-id="82600-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="82600-133">Por exemplo: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="82600-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="82600-134">Para questões comuns com o registo do dispositivo Azure Ative Directory, consulte [O FAQ dos Dispositivos](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="82600-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
