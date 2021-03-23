---
title: Estou a ser bloqueado pelo Acesso Condicional com dispositivo de adesão ao domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038099"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="8b9f5-102">Estou a ser bloqueado pelo Acesso Condicional com dispositivo de adesão ao domínio</span><span class="sxs-lookup"><span data-stu-id="8b9f5-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="8b9f5-103">**Ferramentas altamente recomendadas**</span><span class="sxs-lookup"><span data-stu-id="8b9f5-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="8b9f5-104">[Ferramenta de resolução de problemas de registo do dispositivo](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A ferramenta que ajuda a resolver problemas de resolução dos problemas de registo do dispositivo mais comuns.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="8b9f5-105">[Script de conectividade de registo do dispositivo](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) de teste - O script que ajuda a garantir que um dispositivo pode aceder aos pontos finais de Registo do Dispositivo na conta do sistema.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="8b9f5-106">[Script de limpeza de dispositivos AD Azure](https://github.com/mzmaili/AzureADDeviceCleanup) - O script que lhe permite procurar e gerir dispositivos antigos no seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="8b9f5-107">Eis algumas razões comuns para que o acesso condicional possa estar a falhar num dispositivo que se juntou a um domínio (Hybrid Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8b9f5-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="8b9f5-108">**Não existe nenhum Azure AD PRT no dispositivo** - É necessário garantir que o dispositivo tem Token de AZure AD Primary Refresh (PRT).</span><span class="sxs-lookup"><span data-stu-id="8b9f5-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="8b9f5-109">Para mais informações sobre o PRT, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="8b9f5-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="8b9f5-110">Para verificar se tem Azure AD PRT, pode executar `dsregcmd/status` o comando no dispositivo e verificar se "AzureAdPrt" é igual a "SIM".</span><span class="sxs-lookup"><span data-stu-id="8b9f5-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="8b9f5-111">Se "AzureAdPrt" for "NO", verifique o seguinte:</span><span class="sxs-lookup"><span data-stu-id="8b9f5-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="8b9f5-112">**Se tem um ambiente federado com FS AD, e é inacessível a partir das redes domésticas dos seus utilizadores**: Neste caso, certifique-se de que os seus pontos finais "usernamemixed" estão acessíveis a partir da extranet.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="8b9f5-113">Se o seu FS AD estiver por detrás de uma VPN, certifique-se de que os utilizadores se ligam à VPN e re-iniciam sessão no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="8b9f5-114">Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)</span><span class="sxs-lookup"><span data-stu-id="8b9f5-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="8b9f5-115">**Se o TPM do dispositivo está defeituoso e, portanto, não pode autenticar o dispositivo**: Verifique "tpm.msc" para ver se o estado do TPM está "Pronto".</span><span class="sxs-lookup"><span data-stu-id="8b9f5-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="8b9f5-116">Caso contrário, corra `dsregcmd/leave` e deixe o dispositivo voltar a juntar-se ao Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="8b9f5-117">Então, tente de novo.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-117">Then, try again.</span></span> <span data-ttu-id="8b9f5-118">Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="8b9f5-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="8b9f5-119">**Está a usar um fornecedor de identidade de terceiros, que não suporta WS-Trust protocolo.**</span><span class="sxs-lookup"><span data-stu-id="8b9f5-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="8b9f5-120">Como descrito nos nossos documentos, os dispositivos híbridos Azure AD-joins não podem funcionar neste caso.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="8b9f5-121">Por favor, trabalhe com o seu fornecedor de identidade para apoio.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="8b9f5-122">**Os utilizadores estão a utilizar o navegador Chrome sem as contas do Windows 10** ou **extensão do Office O Chrome não utiliza automaticamente o PRT em dispositivos ligados a AAD ou híbridos- AAD-AAD-** Isto leva a falhas de quaisquer políticas de acesso condicional baseadas no dispositivo, com mensagem de erro "dispositivo não registado" exibida.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="8b9f5-123">Para utilizar o navegador Chrome corretamente, tem de instalar as "Contas Windows 10" ou "Extensão do Office para o navegador Chrome dos utilizadores" via SCCM ou Intune.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="8b9f5-124">Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="8b9f5-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="8b9f5-125">Se não for possível empurrar a extensão remotamente, notifique os utilizadores para instalarem manualmente uma das extensões acima para acederem a aplicações por trás do Acesso Condicional baseado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="8b9f5-126">Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="8b9f5-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="8b9f5-127">**O dispositivo foi corretamente híbrido Azure AD aderido, mas foi inadvertidamente eliminado ou desativado, quer devido a alterações sincronizadas no Azure AD Connect quer a partir do portal Azure**: Se isso acontecer, o objeto do dispositivo já não é reconhecido como um dispositivo totalmente ligado, mesmo que o estado "AzureAdJoined" e "PRT" apareçam como válidos no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="8b9f5-128">Para corrigir este problema, corra `dsregcmd/leave` nos dispositivos afetados e deixe-os voltar a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="8b9f5-129">Para mais informações, consulte este [documento.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)</span><span class="sxs-lookup"><span data-stu-id="8b9f5-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="8b9f5-130">Se os seus dispositivos estiverem na atualização do Windows 10, 1809, com VPN/Cloud Proxy e vir problemas com o estado "AzureAdPrt" ou qualquer aplicação com problema SSO (outlook que não se liga à caixa de correio, mesmo que tenha PRT), certifique-se de que tem este patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ou atualização cumulativa de abril [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) para evitar falhas de PRT nessas máquinas.</span><span class="sxs-lookup"><span data-stu-id="8b9f5-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















