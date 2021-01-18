---
title: Configure o serviço de domínio
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885691"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Não é possível ativar a AAD-DS ou a implantação está a falhar

Para resolver a questão do serviço de domínio AD AD (AAD-DS) não estar ativado ou não ser implementado, execute os seguintes passos:

1. Se estiver a utilizar uma rede virtual já existente, verifique se o NSG tem regras que bloqueiam as portas necessárias para sincronizar em AAD-DS no portal https://aka.ms/aadds-networking .
2. Verifique se a sua mensagem de erro é respondida neste guia de resolução de problemas que está disponível em  https://aka.ms/aadds-troubleshoot-enable .
3. Tente implementar os Serviços de Domínio AZure numa nova rede virtual.
4. Siga o guia 'Iniciar a partida' sobre como implementar a AAD-DS: [Criar e Configurar serviços de domínio AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Se estiver a ter problemas com a Implementação de Serviços de Domínio Azure AD, consulte [os Serviços de Domínio Ad Ad de resolução](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) de problemas para resolver erros comuns para o ajudar a pôr as coisas a funcionar novamente. 

**Incapaz de desativar a AAD-DS**

AAD-DS não pode ser pausada. Se desejar parar de utilizar o seu domínio gerido, este deve ser eliminado.
Para eliminar o seu domínio Gerido, consulte [eliminar o Serviço de Domínio AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



