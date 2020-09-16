---
title: Não é possível definir ou ver a política AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735210"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Não é possível definir ou ver a política AllowSelfServicePurchase

Ao tentar definir ou ver a política AllowSelfServicePurchase, recebe a seguinte mensagem de erro:

*HandleError : Falhou na recuperação da política do produto com a PolicyId 'AllowSelfServicePurchase', ErrorMessage - A ligação subjacente foi encerrada: Ocorreu um erro inesperado num envio.*

Isto pode ser devido a uma versão mais antiga da Segurança da Camada de Transporte (TLS). Para ligar o serviço MSCommerce, é necessário utilizar o TLS 1.2 ou superior.  

Experimente os seguintes passos para ativar/definir o protocolo TLS para 1.2, verificar e voltar a tentar.
 1. Na tenção de comando PowerShell (PS C: \) insira o seguinte comando para definir o protocolo TLS para a versão 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verifique os protocolos TLS em uso, com o seguinte comando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Revendo os comandos Get ou Update conforme necessário.

