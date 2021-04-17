---
title: Problemas na resolução de problemas com a inscrição de dispositivos Android no Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830953"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ecf7f-102">Problemas na resolução de problemas com a inscrição de dispositivos Android no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ecf7f-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ecf7f-103">Reveja os recursos listados abaixo para resolver o seu problema agora.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ecf7f-104">Algumas questões comuns e passos de resolução:</span><span class="sxs-lookup"><span data-stu-id="ecf7f-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ecf7f-105">**Dispositivo não erro encriptado no Portal da Empresa:** As versões mais recentes do Android, nomeadamente a começar pelo v7.0, requerem uma senha de arranque para garantir que o seu dispositivo está totalmente encriptado.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="ecf7f-106">As soluções comuns são para permitir um pin de arranque ou encriptar totalmente o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="ecf7f-107">[Reveja este documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) para mais informações.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="ecf7f-108">**Os dispositivos não conseguem fazer o check-in com o serviço Intune ou exibir como "In unhealthy" na consola de administração Intune:** Alguns dispositivos Samsung 4.4 e 5.5 podem não entrar no serviço.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="ecf7f-109">Existem 3 soluções possíveis para esta questão:</span><span class="sxs-lookup"><span data-stu-id="ecf7f-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="ecf7f-110">Abra manualmente a aplicação Portal da Empresa Intune, que iniciará automaticamente uma sincronização do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="ecf7f-111">Atualize o dispositivo para o Android 6.0 ou superior.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="ecf7f-112">Desativar o Smart Manager da Samsung na gestão do Portal da Empresa Intune.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="ecf7f-113">[Reveja este documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) para mais informações sobre estas questões e resoluções.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="ecf7f-114">Tipo de licença de **utilizador Inválido** ou **Nome de Utilizador Não Reconhecido:** O utilizador precisa de ser atribuído a uma licença Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ecf7f-115">Reveja estes documentos para atribuir uma licença através de: Office Admin Center ou portal Azure.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="ecf7f-116">Recursos adicionais para ajudar a resolver o seu problema:</span><span class="sxs-lookup"><span data-stu-id="ecf7f-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ecf7f-117">Utilize [o Portal de Resolução de Problemas Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) para diagnosticar e resolver falhas comuns de inscrição.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ecf7f-118">[Reveja este documento](https://docs.microsoft.com/intune/help-desk-operators) para mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="ecf7f-119">[Reveja este documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) para obter uma lista de erros comuns que impeçam a inscrição e as resoluções para cada um.</span><span class="sxs-lookup"><span data-stu-id="ecf7f-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="ecf7f-120">[Saiba como inscrever dispositivos Android no Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="ecf7f-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
