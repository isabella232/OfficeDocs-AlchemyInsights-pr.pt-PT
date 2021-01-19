---
title: Controlador de domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901310"
---
# <a name="domain-controller"></a>Controlador de domínio

**Não é possível ativar a AAD-DS ou a implantação está a falhar**

Para resolver a questão do serviço de domínio AD AD (AAD-DS) não estar ativado ou não ser implementado, execute os seguintes passos:

1. Se estiver a utilizar uma rede virtual já existente, verifique se o NSG tem regras que bloqueiam as portas necessárias para sincronizar em AAD-DS no portal https://aka.ms/aadds-networking .
2. Verifique se a sua mensagem de erro é respondida neste guia de resolução de problemas que está disponível em  https://aka.ms/aadds-troubleshoot-enable .
3. Tente implementar os Serviços de Domínio AZure numa nova rede virtual.
4. Siga o guia 'Iniciar a ção' sobre como implementar o AAD-DS, que está disponível no [Tutorial para criar serviços de domínio AD AD Azure](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Se estiver a ter problemas com a Implementação de Serviços de Domínio Azure AD, consulte [os Serviços de Domínio Ad Ad de resolução](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) de problemas para resolver erros comuns para o ajudar a pôr as coisas a funcionar novamente. 

**Incapaz de desativar a AAD-DS**

AAD-DS não pode ser pausada. Se desejar parar de utilizar o seu domínio gerido, este deve ser eliminado.

Se encontrar problemas, para resolver mensagens de erro comuns e para medidas de resolução de problemas associadas para ajudá-lo a pôr as coisas a funcionar novamente, consulte [os Serviços de Domínio do Diretório Ativo troubleshoot Azure](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
