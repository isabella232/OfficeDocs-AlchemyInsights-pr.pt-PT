---
title: Diagnóstico de problemas de acesso a portas diferentes
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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030913"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnóstico de problemas de acesso a portas diferentes

Para resolver os diferentes problemas de acesso a portas, efetue os seguintes passos:

1. Pare/esgote a máquina virtual (VM) a partir do portal, reinicie a VM e teste novamente. 
2. Verifique as definições de rede da sua VM para determinar se tem Grupos de Segurança de Rede (NSGs) a bloquear tráfego. Também pode utilizar a ferramenta de verificação de fluxo de IP do [Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) para verificar se os NSGs estão a bloquear o tráfego, as Rotas do User-Defined (UDRs) a reencaminhar o tráfego para o local ("Rota Predefinida" 0.0.0.0/0) ou para um aparelho de rede.
Se continuar a ter problemas após tentar os passos acima, forneça o nome da VM e a porta TCP que está a tentar enviar e-mails para fazer um diagnóstico adicional.

**Documentos recomendados**

[Limitações e recomendações para o envio de e-mails através da porta 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)