---
title: Termos em falta do arquivo de termos de Online do SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762081"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="5112c-102">Activar a encriptação de Bitlocker com Intune</span><span class="sxs-lookup"><span data-stu-id="5112c-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="5112c-103">Política de protecção de ponto final de Intune pode ser utilizada para configurar definições de encriptação de Boitlocker para os dispositivos Windows conforme descrito em: Windows10 (e posterior) as definições para proteger dispositivos que utilizem Intune</span><span class="sxs-lookup"><span data-stu-id="5112c-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="5112c-104">Deverá ter em atenção que muitos dispositivos mais recentes com o Windows 10 suportam a encriptação de bitlocker automático que é accionada sem a aplicação da política do MDM.</span><span class="sxs-lookup"><span data-stu-id="5112c-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="5112c-105">Se as definições predefinidas não forem configuradas, isto pode afectar a aplicação da política.</span><span class="sxs-lookup"><span data-stu-id="5112c-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="5112c-106">Consulte as perguntas mais frequentes para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="5112c-106">See FAQ for more detail.</span></span>


<span data-ttu-id="5112c-107">Perguntas mais frequentes  p: quais as edições do Windows suportam a encriptação de dispositivo utilizando a política de protecção de ponto final?</span><span class="sxs-lookup"><span data-stu-id="5112c-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="5112c-108"> R: as definições de política de protecção de ponto final de Intune são implementadas utilizando o CSP do Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="5112c-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="5112c-109">Nem todas as edições nem versões do Windows que suportam o CSP do Bitlocker. 
     </span><span class="sxs-lookup"><span data-stu-id="5112c-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="5112c-110">Neste momento tempo as edições do Windows: empresa; Educação, portáteis, móveis Enterprise e Professional (de compilação 1809 e posteriores) são suportados.</span><span class="sxs-lookup"><span data-stu-id="5112c-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="5112c-111">Q: se um dispositivo já está encriptado com Bitlocker utilizando as predefinições do sistema operativo para o método de encriptação e intensidade da cifra (XTS-AES-128) irá aplicar uma política com diferentes definições de accionam automaticamente reencriptação da unidade com as novas definições?</span><span class="sxs-lookup"><span data-stu-id="5112c-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="5112c-112">R: ' não '.</span><span class="sxs-lookup"><span data-stu-id="5112c-112">A: No.</span></span> <span data-ttu-id="5112c-113">Para aplicar as novas definições de cifra que a unidade deve, primeiro, ser desencriptada.</span><span class="sxs-lookup"><span data-stu-id="5112c-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="5112c-114">Nota para dispositivos que está a ser inscritos com Autopilot a encriptação automática que ocorreria durante a OOBE, não é activada até que é avaliada a política de Intune, que permite que a política com base em definições para ser utilizado em vez das predefinições de SO</span><span class="sxs-lookup"><span data-stu-id="5112c-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="5112c-115">Q se um dispositivo é encriptado na sequência da aplicação da política de Intune será-desencriptado quando é removida dessa política?</span><span class="sxs-lookup"><span data-stu-id="5112c-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="5112c-116">R: remoção de encriptação relacionados com a política não resulta na desencriptação das unidades que foram configuradas.</span><span class="sxs-lookup"><span data-stu-id="5112c-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="5112c-117">P: por que razão intune política conformidade mostrar que o dispositivo não tem "Bitlocker activado", mas é?</span><span class="sxs-lookup"><span data-stu-id="5112c-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="5112c-118">R: o "Bitlocker activado" na política de conformidade intune utiliza o cliente de atestado de saúde de dispositivo do Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="5112c-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="5112c-119">Este cliente medidas apenas o estado do dispositivo no momento do arranque.</span><span class="sxs-lookup"><span data-stu-id="5112c-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="5112c-120">Por isso, se um dispositivo não ter sido reiniciado desde a encriptação de bitlocker foi concluída o serviço de cliente DHA não reportará bitlocker como estando activo.</span><span class="sxs-lookup"><span data-stu-id="5112c-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>