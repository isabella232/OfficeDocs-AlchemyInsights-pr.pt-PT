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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="20a48-102">Diagnósticos para diferentes questões de acesso a portas</span><span class="sxs-lookup"><span data-stu-id="20a48-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="20a48-103">Para resolver os diferentes problemas de acesso à porta, execute os seguintes passos:</span><span class="sxs-lookup"><span data-stu-id="20a48-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="20a48-104">Parar/negociar a máquina virtual (VM) a partir do portal, reiniciar o VM e testar novamente.</span><span class="sxs-lookup"><span data-stu-id="20a48-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="20a48-105">Verifique as definições de rede do seu VM para determinar se tem grupos de segurança de rede (NSGs) bloqueando o tráfego.</span><span class="sxs-lookup"><span data-stu-id="20a48-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="20a48-106">Também pode utilizar a [ferramenta de verificação do fluxo IP do Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) para verificar se os NSGs bloqueiam o tráfego, User-Defined Rotas (UDRs) reencaminhando o seu tráfego de volta para o local ('Rota Padrão' 0.0.0/0), ou para um aparelho de rede.</span><span class="sxs-lookup"><span data-stu-id="20a48-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="20a48-107">Se ainda tiver problemas depois de experimentar os passos acima, por favor forneça o nome VM e a porta TCP que está a tentar enviar por correio para um diagnóstico posterior.</span><span class="sxs-lookup"><span data-stu-id="20a48-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="20a48-108">**Documentos Recomendados**</span><span class="sxs-lookup"><span data-stu-id="20a48-108">**Recommended Documents**</span></span>

[<span data-ttu-id="20a48-109">Limitações e recomendações para envio de e-mail de saída sobre o porto 25</span><span class="sxs-lookup"><span data-stu-id="20a48-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)