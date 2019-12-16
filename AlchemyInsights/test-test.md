---
title: Termos ausentes da SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053524"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="6ae1b-102">Habilitando a criptografia bitlocker com intune</span><span class="sxs-lookup"><span data-stu-id="6ae1b-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="6ae1b-103">A política de proteção de ponto final em conjunto pode ser usada para configurar configurações de criptografia Boitlocker para dispositivos Windows, conforme descrito em: configurações do Windows10 (e posteriores) para proteger dispositivos usando O Intune</span><span class="sxs-lookup"><span data-stu-id="6ae1b-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="6ae1b-104">Você deve estar ciente de que muitos dispositivos mais novos que executam o Windows 10 suportam criptografia automática de bitlocker que é acionada sem a aplicação da política mdm.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="6ae1b-105">Isso pode afetar a aplicação da política se as configurações não padrão forem configuradas.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="6ae1b-106">Veja o FAQ para mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-106">See FAQ for more detail.</span></span>


<span data-ttu-id="6ae1b-107">FAQ  Q: Quais edições da criptografia do dispositivo de suporte ao Windows usando a Política de Proteção de Ponto Final?</span><span class="sxs-lookup"><span data-stu-id="6ae1b-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="6ae1b-108"> R: As configurações da Política de Proteção de Pontos Finais Intune são implementadas usando o Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="6ae1b-109">Nem todas as edições nem compilações de Windows suportam o Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="6ae1b-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="6ae1b-110">Neste momento Windows Editions: Enterprise; Educação, Mobile, Mobile Enterprise e Professional (a partir da construção de 1809) são suportados.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="6ae1b-111">P: Se um dispositivo já estiver criptografado com o Bitlocker usando as configurações padrão do SISTEMA OPERACIONAL para método de criptografia e força de cifra (XTS-AES-128) aplicará uma política com configurações diferentes acionando automaticamente a recriptografia da unidade com as novas configurações?</span><span class="sxs-lookup"><span data-stu-id="6ae1b-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="6ae1b-112">R: Não.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-112">A: No.</span></span> <span data-ttu-id="6ae1b-113">A fim de aplicar as novas configurações de cifra, a unidade deve primeiro ser descriptografada.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="6ae1b-114">Nota Para dispositivos que estão sendo registrados com piloto automático a criptografia automática que ocorreria durante o OOBE não é acionada até que a política de intune seja avaliada, o que permite que as configurações baseadas na política sejam usadas no lugar dos padrões do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="6ae1b-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="6ae1b-115">Q Se um dispositivo é criptografado como resultado da aplicação da política Intune será descriptografado quando essa política for removida?</span><span class="sxs-lookup"><span data-stu-id="6ae1b-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="6ae1b-116">R: A remoção da política relacionada à criptografia não resulta na decodificação das unidades que foram configuradas.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="6ae1b-117">P: Por que a política de conformidade intune mostra que meu dispositivo não tem "Bitlocker Habilitado", mas é?</span><span class="sxs-lookup"><span data-stu-id="6ae1b-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="6ae1b-118">R: A configuração "Bitlocker" configurada em intunte a política de conformidade utiliza o cliente de atestado de saúde do dispositivo Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="6ae1b-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="6ae1b-119">Este cliente só mede o estado do dispositivo na hora da inicialização.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="6ae1b-120">Portanto, se um dispositivo não foi reiniciado desde que a criptografia do bitlocker foi concluída, o serviço de cliente DHA não informará o bitlocker como ativo.</span><span class="sxs-lookup"><span data-stu-id="6ae1b-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>