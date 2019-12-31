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
# <a name="accessing-bitlocker-recovery-keys"></a>Acesso às chaves de recuperação do Bitlocker

Ao configurar as configurações do Bitlocker intune Endpoint Protection Policy, é possível definir se as informações de recuperação do Bitlocker devem ser armazenadas no Diretório Ativo do Azure.

Se essa configuração for configurada, os dados de recuperação armazenados devem ser visíveis para um administrador intune como parte dos dados de registro do dispositivo na lâmina de dispositivos intune de duas maneiras:

Dispositivos - dispositivos AD azuis -> "Dispositivo" ou dispositivos -> todos os dispositivos -> "Dispositivo" -> chaves de recuperação

Alternativamente, se houver acesso administrativo ao próprio dispositivo, a chave de recuperação (Senha) pode ser vista executando o comando a seguir de um alerta de comando elevado:

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
Se o dispositivo foi criptografado antes da inscrição em Intune, a chave de recuperação pode ter sido associada à "Conta Microsoft" (MSA) usada para entrar no dispositivo durante o processo OOBE. Se fosse esse o https://onedrive.live.com/recoverykey caso, o acesso e a assinatura com esse MSA devem mostrar os dispositivos para os quais as chaves de recuperação foram armazenadas.
 
Se o dispositivo foi criptografado como resultado da configuração por meio da política de grupo baseada em domínio, as informações de recuperação podem ser armazenadas no Diretório Ativo local.
 

