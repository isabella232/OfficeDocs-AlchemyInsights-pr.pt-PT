---
title: Adicionar um subdomâneo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506774"
---
# <a name="adding-a-sub-domain"></a>Adicionar um subdomâneo

Os subdomês podem ser adicionados ao mesmo inquilino ou a um inquilino diferente do domínio principal. Em qualquer um dos casos, tem de gerir as suas próprias definições de DNS no site da sua organização de registo. Se deixou que a Microsoft faça a gestão das suas definições de DNS com registos NS ou se comprou o domínio à Microsoft, não pode adicionar subdomínios sem alterar isto primeiro.

Adicione primeiro o domínio principal e, em seguida, adicione o subdomâneo. Se o subdomínio estiver no mesmo inquilino, não é necessária nenhuma verificação adicional. Se adicionar o subdomínio a um inquilino separado, é necessário o registo TXT DNS para a verificação de propriedade antes de adicionar o domínio e os registos DNS adicionais para os serviços selecionados.

- Para adicionar um domínio ou subdomírio, siga o assistente [Adicionar](https://admin.microsoft.com/Adminportal#/Domains/Wizard)Domínio ou adicione o domínio ou subdomírio manualmente ao ir para **Setting**  >  **Domains**  >  **Add domains**.

Se for necessário:

- Para alterar quem gere as suas definições de DNS para um domínio existente, vá para **Definições** Domains , selecione a caixa de verificação junto ao domínio e, em  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)seguida, selecione **Manage DNS**. No assistente, selecione **Adicionar os seus próprios registos DNS e** conclua o assistente.
- Para adicionar subdomínios a um domínio comprado pela Microsoft, primeiro transfira o domínio para outra pessoa de registo de domínios e, em seguida, faça a alteração acima para gerir os seus próprios registos DNS. Para obter instruções, consulte [Transferir um domínio da Microsoft para outro anfitrião.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Se receber uma mensagem de erro a dizer que o seu domínio já está a ser utilizado por outros membros ou pessoas na sua organização, primeiro terá de assumir esta conta não utilizada antes de utilizar o domínio. Para obter instruções, consulte Assumir o lugar de administrador de um diretório não [gerido no Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
