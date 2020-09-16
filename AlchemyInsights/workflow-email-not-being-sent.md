---
title: O e-mail do workflow não está a ser enviado
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749000"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>O email workflow não está a ser enviado para uma lista ou biblioteca do SharePoint

1. E-mail de fluxos de trabalho não são enviados para todos os utilizadores ou apenas utilizadores específicos, ou vê o erro **A mensagem de e-mail não pode ser enviada. Certifique-se de que o e-mail tem um destinatário válido**.

    Verifique se o utilizador existe no grupo de permissões **All People** (lista de informações do utilizador) para a recolha do site.  URL direto da amostra: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Se o utilizador não existir, certifique-se de que o utilizador está assinado na página. 
    - Se for um utilizador externo, certifique-se de que o seu convite foi aceite.
    - Se o utilizador existir no grupo de permissões, certifique-se de que o endereço de e-mail está correto.
    - Se o endereço de e-mail dos utilizadores não for definido aqui, então crie um alerta de amostra para esse utilizador que force a sincronização dessa conta de utilizador desde os Perfis de Utilizador do SharePoint até à recolha deste site.
 
2. O e-mail dos fluxos de trabalho é enviado aos administradores de recolha do site, mas não para outros utilizadores e ver o erro **HTTP Proibido para <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendEmail**.
 

    Ver [Acesso Negado quando envia um e-mail para um grupo SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Além disso, verifique se a funcionalidade de recolha do site de **bloqueio de acesso limitado** do utilizador não está ativa.


## <a name="related-topics"></a>Tópicos relacionados
Quer experimentar o Microsoft Flow no SharePoint Online?
- [Criar Fluxo](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


