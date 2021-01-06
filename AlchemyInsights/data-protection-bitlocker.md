---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768828"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="1831d-102">Ativar a encriptação bitlocker com Intune</span><span class="sxs-lookup"><span data-stu-id="1831d-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="1831d-103">A Política de Proteção de Pontos Finais intune pode ser utilizada para configurar definições de encriptação bitlocker para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="1831d-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="1831d-104">Para obter mais informações, consulte [as definições do Windows 10 (e posterior) para proteger os dispositivos que utilizam o Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)</span><span class="sxs-lookup"><span data-stu-id="1831d-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="1831d-105">Deve estar ciente de que muitos dispositivos mais recentes que executam a encriptação automática do Bitlocker do Windows 10, que é desencadeada sem a aplicação da política DOM.</span><span class="sxs-lookup"><span data-stu-id="1831d-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="1831d-106">Isto pode ter impacto na aplicação da política se as definições não padrão forem configuradas.</span><span class="sxs-lookup"><span data-stu-id="1831d-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="1831d-107">Consulte as seguintes FAQ para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="1831d-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="1831d-108">Para obter informações sobre problemas de resolução de problemas, consulte [as políticas bitLocker de resolução de problemas no Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="1831d-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="1831d-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="1831d-109">**FAQ**</span></span>

<span data-ttu-id="1831d-110">P: Que edições de encriptação do dispositivo de suporte do Windows utilizando a Política de Proteção de Pontos Finais?</span><span class="sxs-lookup"><span data-stu-id="1831d-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="1831d-111">R: As definições na Política de Proteção do Ponto Final intune são implementadas utilizando o [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="1831d-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="1831d-112">Nem todas as edições ou construções do Windows suportam o Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="1831d-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="1831d-113">P: Como pode o Bitlocker ser ativado em dispositivos sem necessitar de interação do utilizador final?</span><span class="sxs-lookup"><span data-stu-id="1831d-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="1831d-114">R: Enquanto forem cumpridos os pré-requisitos necessários, é possível ativar bitlocker "Silent Encryption" através do Intune.</span><span class="sxs-lookup"><span data-stu-id="1831d-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="1831d-115">Consulte os detalhes dos requisitos do dispositivo e as definições de política de exemplo para permitir a encriptação silenciosa no seguinte doc: [Ativar silenciosamente a encriptação bitlocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="1831d-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="1831d-116">P: Se um dispositivo já estiver encriptado com o Bitlocker utilizando as definições padrão do SISTEMA para o método de encriptação e a resistência cifra (XTS-AES-128), aplicará uma política com diferentes configurações desencadeando automaticamente a reen encriptação da unidade com as novas definições?</span><span class="sxs-lookup"><span data-stu-id="1831d-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="1831d-117">R: Não.</span><span class="sxs-lookup"><span data-stu-id="1831d-117">A: No.</span></span> <span data-ttu-id="1831d-118">Para aplicar as novas definições de cifra, a unidade deve primeiro ser desencriptado.</span><span class="sxs-lookup"><span data-stu-id="1831d-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="1831d-119">**Nota:** Para os dispositivos que estão a ser matriculados com o Autopilot, a encriptação automática que ocorreria durante o OOBE não é ativada até que a política do Intune seja avaliada, o que permite que as definições baseadas em políticas sejam utilizadas em vez dos padrãos de SISTEMA.</span><span class="sxs-lookup"><span data-stu-id="1831d-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="1831d-120">P: Se um dispositivo for encriptado como resultado da aplicação da política Intune, será desencriptado quando essa política for removida?</span><span class="sxs-lookup"><span data-stu-id="1831d-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="1831d-121">R: A remoção da política relacionada com a encriptação NÃO resulta na desencriptação das unidades configuradas.</span><span class="sxs-lookup"><span data-stu-id="1831d-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="1831d-122">P: Porque é que a Intune Compliance Policy mostra que o meu dispositivo não tem o Bitlocker ativado, mesmo que seja?</span><span class="sxs-lookup"><span data-stu-id="1831d-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="1831d-123">R: A definição "Bitlocker ativada" na Política de Conformidade intune utiliza o cliente windows device Health Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="1831d-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="1831d-124">Este cliente só mede o estado do dispositivo na hora do arranque.</span><span class="sxs-lookup"><span data-stu-id="1831d-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="1831d-125">Assim, se um dispositivo não tiver sido reiniciado desde que a encriptação Bitlocker foi concluída, o serviço de clientes DHA não reportará bitlocker como estando ativo.</span><span class="sxs-lookup"><span data-stu-id="1831d-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 