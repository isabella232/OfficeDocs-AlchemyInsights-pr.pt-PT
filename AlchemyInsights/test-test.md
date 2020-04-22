---
title: Termos em falta na SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766864"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="b3b89-102">Habilitar a encriptação bitlocker com Intune</span><span class="sxs-lookup"><span data-stu-id="b3b89-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="b3b89-103">A Intune Endpoint Protection Policy pode ser usada para configurar as definições de encriptação boitlocker para dispositivos Windows, conforme descrito em : Windows10 (e mais tarde) definições para proteger dispositivos que utilizem Intune</span><span class="sxs-lookup"><span data-stu-id="b3b89-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="b3b89-104">Deve estar ciente de que muitos dispositivos mais recentes que executam o Windows 10 suportam encriptação automática de bitlockers que é desencadeada sem a aplicação da política de MDM.</span><span class="sxs-lookup"><span data-stu-id="b3b89-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="b3b89-105">Isto pode ter impacto na aplicação da política se as definições não predefinidas forem configuradas.</span><span class="sxs-lookup"><span data-stu-id="b3b89-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="b3b89-106">Consulte as FAQ para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="b3b89-106">See FAQ for more detail.</span></span>


<span data-ttu-id="b3b89-107">FAQ  Q: Que edições da encriptação do dispositivo de suporte do Windows utilizando a Política de Proteção do Ponto Final?</span><span class="sxs-lookup"><span data-stu-id="b3b89-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="b3b89-108"> R: As definições na Política de Proteção de Pontos Finais intune são implementadas utilizando o Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="b3b89-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="b3b89-109">Nem todas as edições nem as construções do Windows suportam o Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="b3b89-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="b3b89-110">Neste momento, as Edições Windows: Enterprise; Educação, Mobile, Mobile Enterprise e Professional (a partir da construção 1809) são apoiados.</span><span class="sxs-lookup"><span data-stu-id="b3b89-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="b3b89-111">P: Se um dispositivo já estiver encriptado com o Bitlocker utilizando as definições predefinidas do OS para o método de encriptação e a força da cifra (XTS-AES-128) aplicará uma política com diferentes configurações que desencadeiem automaticamente a reencriptação da unidade com as novas definições?</span><span class="sxs-lookup"><span data-stu-id="b3b89-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="b3b89-112">A: Não.</span><span class="sxs-lookup"><span data-stu-id="b3b89-112">A: No.</span></span> <span data-ttu-id="b3b89-113">Para aplicar as novas definições de cifra, a unidade deve primeiro ser desencriptada.</span><span class="sxs-lookup"><span data-stu-id="b3b89-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="b3b89-114">Nota Para dispositivos que estão a ser matriculados com Autopilot a encriptação automática que ocorreria durante o OOBE não é acionada até que a política Intune seja avaliada, o que permite que as definições baseadas na política sejam utilizadas no lugar dos predefinições do SO</span><span class="sxs-lookup"><span data-stu-id="b3b89-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="b3b89-115">Q Se um dispositivo for encriptado como resultado da aplicação da política Intune será desencriptado quando essa política for removida?</span><span class="sxs-lookup"><span data-stu-id="b3b89-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="b3b89-116">R: A remoção da política relacionada com a encriptação NÃO resulta na desencriptação das unidades configuradas.</span><span class="sxs-lookup"><span data-stu-id="b3b89-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="b3b89-117">P: Porque é que a política de conformidade intune mostra que o meu dispositivo não tem "Bitlocker Enabled" mas é?</span><span class="sxs-lookup"><span data-stu-id="b3b89-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="b3b89-118">R: A definição "Bitlocker ativada" na política de conformidade inoportuna utiliza o cliente de Attestation de Saúde do Dispositivo Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="b3b89-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="b3b89-119">Este cliente só mede o estado do dispositivo no momento do arranque.</span><span class="sxs-lookup"><span data-stu-id="b3b89-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="b3b89-120">Portanto, se um dispositivo não tiver sido reiniciado desde que a encriptação bitlocker foi concluída, o serviço de cliente DHA não reportará o bitlocker como estando ativo.</span><span class="sxs-lookup"><span data-stu-id="b3b89-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>