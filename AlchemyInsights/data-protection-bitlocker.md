---
title: Proteção de dados - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908720"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="78f68-102">Habilitando a criptografia bitlocker com Intune</span><span class="sxs-lookup"><span data-stu-id="78f68-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="78f68-103">A Política de Proteção de Ponto Final insumo pode ser usada para configurar configurações de criptografia bitlocker para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="78f68-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="78f68-104">Para obter mais informações, consulte as configurações do [Windows 10 (e posteriores) para proteger os dispositivos que usam o Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)</span><span class="sxs-lookup"><span data-stu-id="78f68-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="78f68-105">Você deve estar ciente de que muitos dispositivos mais novos que executam o Windows 10 suportam criptografia bitlocker automática, que é ativada sem a aplicação da política mdm.</span><span class="sxs-lookup"><span data-stu-id="78f68-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="78f68-106">Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas.</span><span class="sxs-lookup"><span data-stu-id="78f68-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="78f68-107">Veja o SEGUINTE FAQ para mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="78f68-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="78f68-108">Para obter informações sobre problemas de solução de problemas, consulte [as políticas troubleshoot BitLocker no Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="78f68-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="78f68-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="78f68-109">**FAQ**</span></span>

 <span data-ttu-id="78f68-110">P: Quais edições da criptografia do dispositivo de suporte ao Windows usando a Política de Proteção de Ponto Final?</span><span class="sxs-lookup"><span data-stu-id="78f68-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="78f68-111">R: As configurações da Política de Proteção de Ponto Final Intune são implementadas usando o [Bitlocker CSP.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)</span><span class="sxs-lookup"><span data-stu-id="78f68-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="78f68-112">Nem todas as edições ou compilações de Windows suportam o Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="78f68-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="78f68-113">Neste momento, as seguintes edições do Windows são suportadas: Enterprise, Education, Mobile, Mobile Enterprise e Professional (build 1809 and later).</span><span class="sxs-lookup"><span data-stu-id="78f68-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="78f68-114">P: Se um dispositivo já estiver criptografado com o Bitlocker usando as configurações padrão do SISTEMA OPERACIONAL para método de criptografia e força de cifra (XTS-AES-128), aplicará uma política com configurações diferentes acionando automaticamente a recriptografia da unidade com as novas configurações?</span><span class="sxs-lookup"><span data-stu-id="78f68-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="78f68-115">R: Não.</span><span class="sxs-lookup"><span data-stu-id="78f68-115">A: No.</span></span> <span data-ttu-id="78f68-116">Para aplicar as novas configurações de cifra, a unidade deve primeiro ser descriptografada.</span><span class="sxs-lookup"><span data-stu-id="78f68-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="78f68-117">**Nota:** Para dispositivos que estão sendo registrados com piloto automático, a criptografia automática que ocorreria durante o OOBE não é ativada até que a política de intune seja avaliada, o que permite que as configurações baseadas em políticas sejam usadas no lugar dos padrões do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="78f68-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="78f68-118">P: Se um dispositivo for criptografado como resultado da aplicação da política de Intune, ele será descriptografado quando essa política for removida?</span><span class="sxs-lookup"><span data-stu-id="78f68-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="78f68-119">R: A remoção da política relacionada à criptografia não resulta na decodificação das unidades configuradas.</span><span class="sxs-lookup"><span data-stu-id="78f68-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="78f68-120">P: Por que a Política de Conformidade Intune mostra que meu dispositivo não tem o Bitlocker habilitado, mesmo que seja?</span><span class="sxs-lookup"><span data-stu-id="78f68-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="78f68-121">R: A configuração "Bitlocker habilitado" na Política de Conformidade Intune utiliza o cliente de Atestado de Saúde do Dispositivo Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="78f68-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="78f68-122">Este cliente só mede o estado do dispositivo na hora da inicialização.</span><span class="sxs-lookup"><span data-stu-id="78f68-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="78f68-123">Portanto, se um dispositivo não foi reiniciado desde que a criptografia bitlocker foi concluída, o serviço de cliente DHA não informará o Bitlocker como ativo.</span><span class="sxs-lookup"><span data-stu-id="78f68-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 