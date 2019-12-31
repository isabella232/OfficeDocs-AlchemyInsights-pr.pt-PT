---
title: Chaves de recuperação do bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908825"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="ebff5-102">Acesso às chaves de recuperação do Bitlocker</span><span class="sxs-lookup"><span data-stu-id="ebff5-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="ebff5-103">Ao configurar as configurações do Bitlocker intune Endpoint Protection Policy, é possível definir se as informações de recuperação do Bitlocker devem ser armazenadas no Diretório Ativo do Azure.</span><span class="sxs-lookup"><span data-stu-id="ebff5-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="ebff5-104">Se essa configuração for configurada, os dados de recuperação armazenados devem ser visíveis para um administrador intune como parte dos dados de registro do dispositivo na lâmina de dispositivos intune de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="ebff5-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="ebff5-105">Dispositivos - dispositivos AD azuis -> "Dispositivo" ou dispositivos -> todos os dispositivos -> "Dispositivo" -> chaves de recuperação</span><span class="sxs-lookup"><span data-stu-id="ebff5-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="ebff5-106">Alternativamente, se houver acesso administrativo ao próprio dispositivo, a chave de recuperação (Senha) pode ser vista executando o comando a seguir de um alerta de comando elevado:</span><span class="sxs-lookup"><span data-stu-id="ebff5-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="ebff5-107">Se o dispositivo foi criptografado antes da inscrição em Intune, a chave de recuperação pode ter sido associada à "Conta Microsoft" (MSA) usada para entrar no dispositivo durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="ebff5-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="ebff5-108">Se fosse esse o https://onedrive.live.com/recoverykey caso, o acesso e a assinatura com esse MSA devem mostrar os dispositivos para os quais as chaves de recuperação foram armazenadas.</span><span class="sxs-lookup"><span data-stu-id="ebff5-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="ebff5-109">Se o dispositivo foi criptografado como resultado da configuração por meio da política de grupo baseada em domínio, as informações de recuperação podem ser armazenadas no Diretório Ativo local.</span><span class="sxs-lookup"><span data-stu-id="ebff5-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

