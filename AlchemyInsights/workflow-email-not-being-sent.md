---
title: E-mail de fluxo de trabalho não está sendo enviado
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049384"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail de fluxo de trabalho não está sendo enviado para uma lista ou biblioteca do SharePoint

1. Os e-mails dos fluxos de trabalho não são enviados para todos os usuários ou apenas usuários específicos, ou você vê o erro **A mensagem de e-mail não pode ser enviada. Certifique-se de que o e-mail tem um destinatário válido.**

    Verifique se o usuário existe no grupo de permissões **de todas as pessoas** (lista de informações do usuário) para essa coleção do site.  Url direto da<tenant>amostra: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0

    - Se o usuário não existir, certifique-se de que o usuário está inscrito na página. 
    - Se for um usuário externo, certifique-se de que seu convite tenha sido aceito.
    - Se o usuário existir no grupo de permissões, certifique-se de que o endereço de e-mail esteja correto.
    - Se o endereço de e-mail dos usuários não for definido aqui, crie um alerta de amostra para aquele usuário que força a sincronização dessa conta de usuário, desde perfis de usuário do SharePoint até essa coleção do site.
 
2. E-mail de fluxos de trabalho são enviados para os administradores de coleta do site, mas não para outros usuários e ver o erro **HTTP Proibido para <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.
 

    Veja o [Access Denied quando enviar um e-mail para um grupo SharePoint.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Além disso, verifique se o recurso de coleta do site de bloqueio de **permissão** de usuário de acesso limitado não está ativo.


## <a name="related-topics"></a>Tópicos relacionados
Quer experimentar o Microsoft Flow no SharePoint Online?
- [Criar fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


