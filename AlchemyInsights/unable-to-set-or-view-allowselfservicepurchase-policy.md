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
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826102"
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

