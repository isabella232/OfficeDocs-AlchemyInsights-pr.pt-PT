---
title: Faltam termos na SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750462"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="ce3cb-102">Habilitar a encriptação bitlocker com Intune</span><span class="sxs-lookup"><span data-stu-id="ce3cb-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="ce3cb-103">A Política de Proteção de Pontos Finais intune pode ser usada para configurar as definições de encriptação do Boitlocker para dispositivos Windows, conforme descrito em : Definições do Windows10 (e posteriormente) para proteger dispositivos que utilizam o Intune</span><span class="sxs-lookup"><span data-stu-id="ce3cb-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="ce3cb-104">Deve estar ciente de que muitos dispositivos mais recentes que executam a encriptação automática do Bitlocker do Windows 10, que é acionada sem a aplicação da política DOM.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="ce3cb-105">Isto pode ter impacto na aplicação da política se as definições não padrão forem configuradas.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="ce3cb-106">Consulte as FAQ para obter mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-106">See FAQ for more detail.</span></span>


<span data-ttu-id="ce3cb-107">FAQ   Q: Que edições de encriptação de dispositivo de suporte do Windows utilizando a Política de Proteção de Pontos Finais?</span><span class="sxs-lookup"><span data-stu-id="ce3cb-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="ce3cb-108"> R: As definições na Política de Proteção do Ponto Final intune são implementadas utilizando o CSP Bitlocker.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="ce3cb-109">Nem todas as edições nem as construções do Windows suportam o Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="ce3cb-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="ce3cb-110">Neste momento Windows Editions: Enterprise; Educação, Mobile, Mobile Enterprise e Professional (a partir da construção 1809) são apoiados.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="ce3cb-111">P: Se um dispositivo já estiver encriptado com o Bitlocker utilizando as definições padrão do SISTEMA para o método de encriptação e a resistência cifra (XTS-AES-128) aplicará uma política com diferentes configurações, desencadeie automaticamente a reencriminação da unidade com as novas definições?</span><span class="sxs-lookup"><span data-stu-id="ce3cb-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="ce3cb-112">R: Não.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-112">A: No.</span></span> <span data-ttu-id="ce3cb-113">Para aplicar as novas definições de cifra, a unidade deve ser desencriptado primeiro.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="ce3cb-114">Nota Para os dispositivos que estão a ser matriculados com o Autopilot, a encriptação automática que ocorreria durante o OOBE não é ativada até que a política do Intune seja avaliada, o que permite que as definições baseadas na política sejam utilizadas em vez dos padrãos de SISTEMA</span><span class="sxs-lookup"><span data-stu-id="ce3cb-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="ce3cb-115">Q Se um dispositivo for encriptado como resultado da aplicação da política Intune será desencriptado quando essa política for removida?</span><span class="sxs-lookup"><span data-stu-id="ce3cb-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="ce3cb-116">R: A remoção da política relacionada com a encriptação NÃO resulta na desencriptação das unidades configuradas.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="ce3cb-117">P: Porque é que a política de conformidade intune mostra que o meu dispositivo não tem "Bitlocker Enabled" mas é?</span><span class="sxs-lookup"><span data-stu-id="ce3cb-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="ce3cb-118">R: A definição "Bitlocker ativada" na política de conformidade intune utiliza o cliente windows Device Health Attestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="ce3cb-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="ce3cb-119">Este cliente só mede o estado do dispositivo na hora do arranque.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="ce3cb-120">Assim, se um dispositivo não tiver sido reiniciado desde que a encriptação bitlocker foi concluída, o serviço de clientes DHA não reportará bitlocker como estando ativo.</span><span class="sxs-lookup"><span data-stu-id="ce3cb-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>