---
title: Não está a ser enviado correio electrónico de fluxo de trabalho
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270683"
---
# <a name="workflow-email-is-not-being-sent"></a>Não está a ser enviado correio electrónico de fluxo de trabalho

1. Mensagem de correio electrónico fluxos de trabalho não são enviadas para todos os utilizadores ou apenas utilizadores específicos ou ver que o erro **a mensagem de correio electrónico não pode ser enviado. Certifique-se o correio electrónico tem um destinatário válido**.

    Verifique se o utilizador existir no grupo de permissões de **Todas as pessoas** (lista de informações de utilizador) para essa colecção de sites.  Exemplo de URL directa: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Se o utilizador não existir, certifique-se do que utilizador inicia sessão na página. 
    - Se for um utilizador externo, certifique-se de que o seu convite foi aceite.
    - Se o utilizador existir no grupo de permissões, certificar-se de que o endereço de correio electrónico está correcto.
    - Se o endereço de correio electrónico de utilizadores não estiver definido aqui, em seguida, crie um alerta de exemplo para esse utilizador que obriga a sincronização dessa conta de utilizador de perfis de utilizador do SharePoint para esta colecção de sites.
 
2. Mensagem de correio electrónico fluxos de trabalho são enviados para os administradores de colecção de sites, mas não para outros utilizadores e ver o erro **HTTP proibido a <spam> <spam> ** <spam> <spam>.
 

    Consulte [Acesso negado ao correio electrónico enviado para grupos](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Além disso, certifique-se de que a funcionalidade de colecção de sites de **modo de bloqueio de permissão de utilizador de acesso limitado** não está activa.


## <a name="related-topics"></a>Tópicos relacionados
Pretende tentar Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [Fluxo e do SharePoint](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


