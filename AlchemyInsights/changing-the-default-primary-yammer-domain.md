---
title: Alterar o domínio padrão do Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950127"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Alterar o domínio padrão/primário do Yammer

O URL do Yammer contém o nome de domínio primário atual para a sua rede Yammer. Este nome de domínio não pode coincidir com o nome de domínio primário definido no Office 365 ou no Azure AD. Existem diferenças de comportamento baseadas no número de domínios personalizados adicionados ao inquilino e em se o Yammer está numa configuração suportada (1 Inquilino: 1 Rede ou 1:1). Está disponível documentação sobre [domínios do Yammer e Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

A razão mais comum para que veja um domínio incorreto é que existem várias redes do Yammer e estas precisam de ser consolidadas. [Consolidar para apenas uma rede](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) utilizando a ferramenta de migração de rede é um primeiro passo importante. Complete isto antes de tentar definir o seu domínio primário.

**Sem domínios personalizados**

Para novos inquilinos, o domínio padrão (por exemplo: fabrikam.onmicrosoft.com) do inquilino será usado para o Yammer. O domínio primário está definido como yammer.com/fabrikam.onmicrosoft.com.

**Domínio personalizado único**

O Yammer selecionará automaticamente o domínio personalizado (por exemplo: fabrikam.com) do inquilino como o domínio primário no Yammer. Está definido como yammer.com/fabrikam.com. Esta alteração é feita pelo serviço de sincronização de domínio e pode demorar até 24 horas a ser efetuada.

**Vários domínios personalizados**

O Yammer pode ter um domínio primário que é diferente do domínio predefinido do inquilino. Uma vez que existem vários domínios personalizados, o Yammer não tenta adivinhar qual o domínio correto entre os disponíveis. Vai precisar de abrir um caso de suporte para solicitar que o nome de domínio primário seja alterado para o domínio primário da sua escolha.

**Informações adicionais sobre resolução de problemas**

Em alguns casos, os domínios podem ter sido movidos entre os inquilinos e o serviço de sincronização de domínio não foi capaz de funcionar com sucesso. Poderá experienciar problemas ao iniciar sessão ou outro tipo de problemas, além de um domínio primário incorreto. Para resolver este problema, os domínios poderão ter de ser transferidos para a rede correta com a ajuda do Suporte da Microsoft. Esta situação requer assistência direta e pode levar algum tempo a resolver, especialmente se houver uma lista muito longa de nomes de domínio. Abra um caso de suporte para obter assistência na resolução deste tipo de problemas.

Ao trabalhar com um agente de suporte, verificarão se os domínios estão verificados num inquilino sob o seu controlo. Podem fazer perguntas adicionais de verificação sobre os seus domínios se estes forem adicionados ao seu inquilino, mas não verificados pelo DNS. Certifique-se de que os domínios são verificados pelo DNS para acelerar o processo.
