---
title: Chaves de recuperação bitlocker
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
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505079"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="242aa-102">Aceder às chaves de recuperação bitlocker</span><span class="sxs-lookup"><span data-stu-id="242aa-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="242aa-103">Ao configurar as definições do Bitlocker Intune Endpoint Policy, é possível definir se as informações de recuperação do Bitlocker devem ser armazenadas no Diretório Ativo Azure.</span><span class="sxs-lookup"><span data-stu-id="242aa-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="242aa-104">Se esta definição estiver configurada, os dados de recuperação armazenados devem ser visíveis a um administrador Intune como parte dos dados de registo do dispositivo na lâmina de dispositivos Intune de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="242aa-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="242aa-105">Dispositivos - Azure AD dispositivos -> "Dispositivo" OU Dispositivos -> Todos os Dispositivos -> "Dispositivo" -> Chaves de recuperação</span><span class="sxs-lookup"><span data-stu-id="242aa-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="242aa-106">Alternativamente, se houver acesso administrativo ao próprio dispositivo, a chave de recuperação (Password) pode ser vista executando o seguinte comando a partir de uma solicitação de comando elevada:</span><span class="sxs-lookup"><span data-stu-id="242aa-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="242aa-107">Se o dispositivo foi encriptado antes da inscrição no Intune, a chave de recuperação pode ter sido associada à "Conta Microsoft" (MSA) utilizada para iniciar súpido no dispositivo durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="242aa-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="242aa-108">Se for esse o caso, aceder  https://onedrive.live.com/recoverykey e iniciar sessão com esse MSA deverá mostrar os dispositivos para os quais foram armazenadas as chaves de recuperação.</span><span class="sxs-lookup"><span data-stu-id="242aa-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="242aa-109">Se o dispositivo foi encriptado como resultado da configuração através da política de grupo baseada em domínio, as informações de recuperação podem ser armazenadas no Ative Directory no local.</span><span class="sxs-lookup"><span data-stu-id="242aa-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="242aa-110">Se tiver configurado a política de proteção endpoint para armazenar a chave de recuperação no Diretório Azure Ative, mas a chave para um dispositivo específico não foi carregada, pode ativar o upload rodando a chave de recuperação desse dispositivo a partir da consola MEM.</span><span class="sxs-lookup"><span data-stu-id="242aa-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="242aa-111">Para mais detalhes, consulte [as teclas de recuperação do BitLocker rotativos](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="242aa-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

