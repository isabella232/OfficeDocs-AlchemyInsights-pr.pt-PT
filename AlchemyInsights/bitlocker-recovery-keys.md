---
title: Chaves de recuperação bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820297"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Aceder às chaves de recuperação bitlocker

Ao configurar as definições do Bitlocker Intune Endpoint Policy, é possível definir se as informações de recuperação do Bitlocker devem ser armazenadas no Diretório Ativo Azure.

Se esta definição estiver configurada, os dados de recuperação armazenados devem ser visíveis a um administrador Intune como parte dos dados de registo do dispositivo na lâmina de dispositivos Intune de duas maneiras:

Dispositivos - Azure AD dispositivos -> "Dispositivo" OU Dispositivos -> Todos os Dispositivos -> "Dispositivo" -> Chaves de recuperação

Alternativamente, se houver acesso administrativo ao próprio dispositivo, a chave de recuperação (Password) pode ser vista executando o seguinte comando a partir de uma solicitação de comando elevada:

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
Se o dispositivo foi encriptado antes da inscrição no Intune, a chave de recuperação pode ter sido associada à "Conta Microsoft" (MSA) utilizada para iniciar súpido no dispositivo durante o processo OOBE. Se for esse o caso, aceder  https://onedrive.live.com/recoverykey e iniciar sessão com esse MSA deverá mostrar os dispositivos para os quais foram armazenadas as chaves de recuperação.
 
Se o dispositivo foi encriptado como resultado da configuração através da política de grupo baseada em domínio, as informações de recuperação podem ser armazenadas no Ative Directory no local.

Se tiver configurado a política de proteção endpoint para armazenar a chave de recuperação no Diretório Azure Ative, mas a chave para um dispositivo específico não foi carregada, pode ativar o upload rodando a chave de recuperação desse dispositivo a partir da consola MEM. Para mais detalhes, consulte [as teclas de recuperação do BitLocker rotativos](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

