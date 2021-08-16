---
title: O e-mail do fluxo de trabalho não está a ser enviado
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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072531"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>O e-mail do fluxo de trabalho não está a ser enviado para uma lista ou biblioteca do SharePoint

1. Os e-mails dos fluxos de trabalho não são enviados para todos os utilizadores ou apenas para utilizadores específicos ou o utilizador vê o erro A mensagem de e-mail não pode ser **enviada. Certifique-se** de que o e-mail tem um destinatário válido.

    Verifique se o utilizador existe no grupo de **permissões** Todas as Pessoas (lista de informações de utilizador) para essa coleção de site.  URL direto de exemplo: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Se o utilizador não existir, certifique-se de que o utilizador tem a conta de entrada na página. 
    - Se for um utilizador externo, certifique-se de que o convite foi aceite.
    - Se o utilizador existir no grupo de permissões, certifique-se de que o endereço de e-mail está correto.
    - Se o endereço de e-mail dos utilizadores não estiver definido aqui, crie um alerta de exemplo para esse utilizador que força a sincronização da conta de utilizador dos Perfis de Utilizador do SharePoint para esta coleção de site.
 
2. Os e-mails dos fluxos de trabalho são enviados para os administradores da coleção de site mas não para outros utilizadores e o erro HTTP Proibido a **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Consulte [Acesso Negado quando envia um e-mail para um grupo do SharePoint.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Verifique também se a funcionalidade de coleção **de site do** modo de bloqueio de permissões de acesso limitado dos utilizadores não está ativa.


## <a name="related-topics"></a>Tópicos relacionados
Pretende experimentar o Microsoft Flow SharePoint Online?
- [Criar Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint e Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


