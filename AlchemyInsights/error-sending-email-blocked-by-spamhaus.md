---
title: Erro ao enviar correio electrónico bloqueado pelo SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912359"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Erro ao enviar uma mensagem de correio electrónico: bloqueado utilizando Spamhaus de anfitrião de cliente

O endereço IP que enviou a mensagem está numa lista de bloqueio pertencente a [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razões para a ser bloqueado pela Spamhaus incluem contas comprometidas, comprometida computadores a partilhar um endereço IP público e políticas do fornecedor de serviços Internet (ISP). Correcções possíveis são:
  
- Para mensagens de entrada bloqueadas para onde pode controlar o servidor de correio electrónico de origem do Office 365, tem de determinar a causa e remover o bloqueio de Web site da Spamhaus.
    
- Para mensagens de entrada bloqueadas para Office 365, se o endereço IP de origem pertence a outra pessoa, o proprietário do endereço tem de remover o bloqueio de Web site da Spamhaus. Se o endereço IP na lista de bloco de política (PBL), o proprietário pode atribuir um endereço IP estático diferente ou remova o endereço de PBL.
    
- Para mensagens de saída bloqueadas do domínio do Office 365, poderá receber este erro se as mensagens são encaminhadas através de um serviço da parte 3. Pode utilizar uma ferramenta de pesquisa WHOIS para encontrar o proprietário de endereços IP bloqueado.
    

