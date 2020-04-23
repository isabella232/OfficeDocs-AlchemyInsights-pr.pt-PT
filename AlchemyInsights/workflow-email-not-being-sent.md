---
title: O e-mail do workflow não está a ser enviado
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766144"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>O e-mail workflow não está a ser enviado para uma lista de SharePoint ou biblioteca

1. O e-mail dos fluxos de trabalho não é enviado para todos os utilizadores ou apenas utilizadores específicos, ou vê o erro **A mensagem de correio eletrónico não pode ser enviada. Certifique-se de que o e-mail tem um destinatário válido**.

    Verifique se o utilizador existe no grupo de permissões **All People** (lista de informações do utilizador) para essa recolha do site.  URL direto da<tenant>amostra: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0

    - Se o utilizador não existir, certifique-se de que o utilizador está inscrito na página. 
    - Se for um utilizador externo, certifique-se de que o seu convite foi aceite.
    - Se o utilizador existir no grupo de permissões, certifique-se de que o endereço de e-mail está correto.
    - Se o endereço de e-mail dos utilizadores não estiver definido aqui, crie um alerta de amostra para esse utilizador que força a sincronização dessa conta de utilizador desde os Perfis de Utilizador do SharePoint até à recolha do site.
 
2. O e-mail dos fluxos de trabalho é enviado aos administradores de recolha do site, mas não a outros utilizadores e ver o erro **HTTP Proibido de <span>https:</span>//URL/_vti_bin/cliente.xvc.sp.utilities.utility.sendEmail**.
 

    Ver [Acesso Negado quando envia um e-mail para um grupo SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Além disso, verifique se a funcionalidade de recolha do modo de **bloqueio de autorização do utilizador** de acesso limitado não está ativa.


## <a name="related-topics"></a>Tópicos relacionados
Quer experimentar o Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


