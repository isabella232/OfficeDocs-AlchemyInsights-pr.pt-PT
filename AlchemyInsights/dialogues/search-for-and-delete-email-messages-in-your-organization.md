---
title: Procure e elimine mensagens de e-mail na sua organização
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525438"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Procure e elimine mensagens de e-mail na sua organização

Siga estes passos:

1. Se não for administrador global, procurar mensagens a sua conta deve ser adicionada ao **grupo de funções eDiscovery Manager** ou à **função de gestão de Compliance Search**. Para eliminar mensagens, terá de se juntar ao grupo de **funções de Gestão** da Organização ou à **função de gestão de Pesquisa e Purga.** As permissões a estas funções são atribuídas no [Centro de Conformidade & Segurança.](https://protection.office.com)
2. [Crie uma pesquisa de conteúdo](https://docs.microsoft.com/office365/securitycompliance/content-search) para encontrar a mensagem para eliminar.
3. [Ligue-se ao Centro de Conformidade & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Se estiver a utilizar o MFA, consulte estas instruções: [Ligue-se à Segurança & Compliance Center PowerShell utilizando a autenticação de vários fatores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Eliminar a mensagem: executar o `New-ComplianceSearchAction` cmdlet para apagar a mensagem. As mensagens eliminadas são transferidas para a pasta de Itens Recuperáveis de um utilizador. Para um comando de exemplo, consulte [o passo 3: Eliminar a mensagem.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
