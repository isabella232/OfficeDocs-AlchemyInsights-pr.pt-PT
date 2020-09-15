---
title: Problemas de resolução de problemas com a inscrição de dispositivos Windows no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658889"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="d6458-102">Problemas de resolução de problemas com a inscrição de dispositivos Windows no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d6458-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="d6458-103">Reveja os recursos listados abaixo para resolver o seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="d6458-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d6458-104">Algumas mensagens de erro comuns e etapas de resolução:</span><span class="sxs-lookup"><span data-stu-id="d6458-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="d6458-105">**O software não pode ser instalado, 0x80cf4017:** O seu certificado de conta expirou.</span><span class="sxs-lookup"><span data-stu-id="d6458-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="d6458-106">Re-descarregue o pacote de software do Cliente PC na Consola Intune Admin.</span><span class="sxs-lookup"><span data-stu-id="d6458-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="d6458-107">Reveja esta documentação para mais informações.</span><span class="sxs-lookup"><span data-stu-id="d6458-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="d6458-108">**Código de erro 0x801c0003:** O erro pode ocorrer nos seguintes cenários:</span><span class="sxs-lookup"><span data-stu-id="d6458-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="d6458-109">O utilizador tem mais dispositivos matriculados do que o limite do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6458-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d6458-110">Reveja estes documentos para [remover um dispositivo](https://docs.microsoft.com/intune/devices-wipe) ou alterar o limite do [dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="d6458-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="d6458-111">"Os utilizadores podem juntar-se a dispositivos para Azure AD" está definido para "nenhum".</span><span class="sxs-lookup"><span data-stu-id="d6458-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="d6458-112">Desacione-o a todos ou selecione os utilizadores.</span><span class="sxs-lookup"><span data-stu-id="d6458-112">Set it to all or select users.</span></span> <span data-ttu-id="d6458-113">[Reveja esta documentação](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) para mais informações.</span><span class="sxs-lookup"><span data-stu-id="d6458-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="d6458-114">O dispositivo já está matriculado por outro utilizador.</span><span class="sxs-lookup"><span data-stu-id="d6458-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="d6458-115">Se for esse o caso, retire o dispositivo da consola Azure Intune ou desative manualmente o dispositivo antes de voltar a tentar.</span><span class="sxs-lookup"><span data-stu-id="d6458-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="d6458-116">O dispositivo é o Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="d6458-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="d6458-117">Apenas o Windows 10 Pro, Education and Enterprise SKUs pode juntar-se ao Azure Ative Directory.</span><span class="sxs-lookup"><span data-stu-id="d6458-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="d6458-118">Recursos adicionais para ajudar a resolver o seu problema:</span><span class="sxs-lookup"><span data-stu-id="d6458-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="d6458-119">Utilize [o Portal de Resolução de Problemas Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de inscrição.</span><span class="sxs-lookup"><span data-stu-id="d6458-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d6458-120">[Reveja este documento](https://docs.microsoft.com/intune/help-desk-operators) para mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="d6458-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="d6458-121">Reveja estes documentos para obter uma lista de erros comuns que impeçam a inscrição e as resoluções para cada um: [Guia de resolução de problemas](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [doc de resolução de problemas](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d6458-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="d6458-122">[Saiba como inscrever dispositivos Windows no Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="d6458-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
