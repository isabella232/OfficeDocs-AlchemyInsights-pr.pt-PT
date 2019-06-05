---
title: Criar e utilizar uma caixa de correio partilhada
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717357"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Resolver a questão - o utilizador não encontrado no directório

<p>Se os utilizadores estão a receber a mensagem de erro <strong> &ldquo; &hellip;utilizador pode&rsquo;t ser encontrado no directório. Volte a tentar&hellip; </strong> onde o tipo de problema é <strong> &ldquo;utilizador não no directório.&rdquo;</strong>, podem ser concluídos os passos seguintes para resolver o problema.</p> <ol> <li>Certifique-se a conta que aceite que o convite de correio electrónico é a mesma conta que está a ser utilizada para iniciar sessão mais tarde. Certifique-se do que utilizador está a utilizar a mesma conta para a aceitar o convite e iniciar sessão no site. <br /><br />Para obter mais informações, consulte <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">como gerir aliases para sua conta Microsoft</a> para gerir o início de sessão do Office 365. <br /><br /></li> <li>Navegue para cada site em que o utilizador está a receber o erro. <br /><br />a. Adicionar <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (entre as aspas) para o fim do URL do site. <br /><br />Exemplo: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Seleccione o utilizador a partir da lista. <br /><br />c. Clique em <strong>remover permissões de utilizador do Friso</strong>. <br /><br />d. Voltar a adicionar o utilizador e reenvie o convite para o utilizador.</li> </ol>

