---
title: Procurar e eliminar mensagens de e-mail na sua organização
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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948894"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Procurar e eliminar mensagens de e-mail na sua organização

Siga estes passos:

1. Se não for um administrador global, para procurar mensagens, a sua  conta tem de ser adicionada ao grupo de funções do Gestor da Deteção de Dados Técnicos ou à função de gestão **da Pesquisa de Conformidade.** Para eliminar mensagens, terá de aderir ao grupo de funções Gestão da Organização ou à função de Gestão de Pesquisa **e Remoção.**  As permissões para estas funções são atribuídas no Centro [de conformidade & segurança.](https://protection.office.com)
2. [Crie uma pesquisa de](https://docs.microsoft.com/office365/securitycompliance/content-search) conteúdo para encontrar a mensagem a eliminar.
3. [Ligação ao PowerShell do & de Conformidade e Segurança.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Se estiver a utilizar a autenticação multifatores, consulte estas instruções: Ligar para Ligação Centro de Conformidade & PowerShell através da autenticação [multifatores](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Eliminar a mensagem: execute `New-ComplianceSearchAction` o cmdlet para eliminar a mensagem. As mensagens eliminadas são movidas para a pasta Itens Recuperáveis de um utilizador. Para um comando de exemplo, [consulte o Passo 3: eliminar a mensagem.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
