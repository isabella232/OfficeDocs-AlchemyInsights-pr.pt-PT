---
title: Incapaz de definir ou ver a política de Compra allowSelfService
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158572"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Incapaz de definir ou ver a política de Compra allowSelfService

Ao tentar definir ou visualizar a política AllowSelfServicePurchase, recebe a seguinte mensagem de erro:

*HandleError : Falha na recuperação da política do produto com o PolicyId 'AllowSelfServicePurchase', ErrorMessage - A ligação subjacente foi fechada: Ocorreu um erro inesperado num envio.*

Isto pode ser devido a uma versão mais antiga da Transport Layer Security (TLS). Para ligar o serviço MSCommerce, precisa de utilizar o TLS 1.2 ou superior.  

Tente os seguintes passos para ativar/definir o protocolo TLS para 1.2, verificar e voltar a tentar.
 1. No pedido de comando PowerShell\) (PS C: insira o seguinte comando para definir o protocolo TLS na versão 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verifique os protocolos TLS em uso, com o seguinte comando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Tente novamente os comandos Get ou Update, conforme necessário.

