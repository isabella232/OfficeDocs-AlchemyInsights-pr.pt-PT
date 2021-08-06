---
title: Não é possível definir ou ver a política AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020203"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Não é possível definir ou ver a política AllowSelfServicePurchase

Ao tentar definir ou ver a política AllowSelfServicePurchase, recebe a seguinte mensagem de erro:

*HandleError: Falha ao obter a política de produto com a PolíticaId 'AllowSelfServicePurchase', ErrorMessage – a ligação subjace foi fechada: ocorreu um erro inesperado num envio.*

Isto pode ser devido a uma versão anterior do Transport Layer Security (TLS). Para ligar o serviço MSCommerce, tem de utilizar o TLS 1.2 ou um número maior.  

Experimente os seguintes passos para ativar/definir o protocolo TLS para 1.2, verificar e tentar novamente.
 1. Na lista de comandos do PowerShell (PS C: introduza o seguinte comando para definir o protocolo \) TLS para a versão 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verifique os protocolos TLS em utilização, com o seguinte comando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Repetir os comandos Obter ou Atualizar conforme necessário.

