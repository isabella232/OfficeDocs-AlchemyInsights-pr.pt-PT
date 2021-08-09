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
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060075"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Aceder a chaves de recuperação Bitlocker

Ao configurar a Política de Proteção de Pontos Finais do Intune, é possível definir se as informações de recuperação do Bitlocker devem ser armazenadas na Azure Active Directory.

Se essa definição estiver configurada, os dados de recuperação armazenados deverão ser visíveis para um administrador do Intune como parte do registo de dados do dispositivo na folha de dispositivos do Intune:

Dispositivos - dispositivos Azure AD -> "Dispositivo" OU Dispositivos -> Todos os Dispositivos -> "Dispositivo" -> Chaves de Recuperação

Em alternativa, se houver acesso administrativo ao dispositivo, a chave de recuperação (Palavra-passe) pode ser vista ao executar o seguinte comando a partir de uma lista de comandos elevada:

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
Se o dispositivo foi encriptado antes da inscrição no Intune, a chave de recuperação poderá ter sido associada à "Conta Microsoft" (MSA) utilizada para entrar no dispositivo durante o processo OOBE. Se fosse esse o caso, aceder e entrar com essa MSA devia mostrar os dispositivos para os quais as chaves de recuperação  https://onedrive.live.com/recoverykey estavam armazenadas.
 
Se o dispositivo tiver sido encriptado como resultado da configuração através da política de grupo baseada no domínio, as informações de recuperação poderão ser armazenadas no Active Directory no local.

Se tiver configurado a política de proteção do Ponto Final para armazenar a chave de recuperação no Azure Active Directory mas a chave de um dispositivo específico não tiver sido carregada, pode ativar o carregamento ao rodar a chave de recuperação do dispositivo a partir da consola MEM. Para obter detalhes, consulte [Rodar chaves de recuperação BitLocker.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

