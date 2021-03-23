---
title: Diagnósticos para diferentes questões de acesso a portas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036812"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnósticos para diferentes questões de acesso a portas

Para resolver os diferentes problemas de acesso à porta, execute os seguintes passos:

1. Parar/negociar a máquina virtual (VM) a partir do portal, reiniciar o VM e testar novamente. 
2. Verifique as definições de rede do seu VM para determinar se tem grupos de segurança de rede (NSGs) bloqueando o tráfego. Também pode utilizar a [ferramenta de verificação do fluxo IP do Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) para verificar se os NSGs bloqueiam o tráfego, User-Defined Rotas (UDRs) reencaminhando o seu tráfego de volta para o local ('Rota Padrão' 0.0.0/0), ou para um aparelho de rede.
Se ainda tiver problemas depois de experimentar os passos acima, por favor forneça o nome VM e a porta TCP que está a tentar enviar por correio para um diagnóstico posterior.

**Documentos Recomendados**

[Limitações e recomendações para envio de e-mail de saída sobre o porto 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)