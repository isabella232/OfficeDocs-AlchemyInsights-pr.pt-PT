---
title: Outlook Recolha do ambiente de trabalho ou substitua uma mensagem de e-mail
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918406"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Ressarte ou substitua uma mensagem Outlook-mail

- Enquanto administrador, pode ressartar **mensagens em nome dos utilizadores através do PowerShell.** Não é possível ressaltar mensagens a partir do centro de administração.
- Só pode **ressaltar mensagens enviadas para pessoas na sua organização.** Se a mensagem tiver sido enviada para um endereço do Gmail, por exemplo, não se consegue ressaltar.
- Só pode **ressartar mensagens enviadas a partir Outlook 2016 no PC.** Se um utilizador enviar uma mensagem através do Outlook para Mac ou Outlook na Web, não é possível ressambrar a mensagem.

Para ressartar ou substituir uma mensagem de e-mail:

1. No painel de pastas à esquerda da janela de Outlook, selecione a pasta Itens Enviados.
1. Faça duplo clique na mensagem que pretende ressartar para a abrir.
1. Selecione o **separador** Mensagem e, em seguida, **selecione**  >  **Ações Ressartar Esta Mensagem**.
1. **Selecione Eliminar as cópias** não lidas desta mensagem ou Eliminar as cópias não lidas e substituí-as por uma nova mensagem **e,** em seguida, selecione **OK.**
1. Se estiver a enviar uma mensagem de substituição, componha a mensagem e, em seguida, selecione **Enviar**.
1. O sucesso ou a falha do ressarcemento de uma mensagem depende das definições do destinatário Outlook. Para ver os passos para verificar o ressarto, [consulte este artigo.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Procurar e eliminar mensagens de e-mail na sua organização

- Se não for um administrador global, a sua conta tem de ser adicionada à função gestor de Deteção de Dados Técnicos ou à função de gestão da Pesquisa de Conformidade para procurar mensagens. Para eliminar mensagens, terá de aderir ao grupo de funções Gestão da Organização ou à função de Gestão de Pesquisa e Remoção. As permissões para estas funções são atribuídas no Centro [de Conformidade e Segurança.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Crie uma pesquisa de](https://docs.microsoft.com/microsoft-365/compliance/content-search) conteúdo para encontrar a mensagem a eliminar.
- [Ligação ao PowerShell do Centro de Conformidade e Segurança.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Se estiver a utilizar a autenticação multifatores, consulte o Ligação o PowerShell do Centro de Conformidade e Microsoft 365 utilização da autenticação [multifatores.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)