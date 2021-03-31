---
title: 126 A obtenção de uma caixa de correio não pode ser encontrada erro na OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426673"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Receber uma caixa de correio não encontrou erro no Outlook na web?

Se estiver a usar o Outlook na web e receber uma **Caixa de Correio não foi encontrada por** erro, a conta que usou para ligar ao Outlook na web não tem uma licença Exchange Online e, portanto, nenhuma caixa de correio está associada à conta. O seu administrador pode atribuir uma licença à sua conta seguindo estes passos:

1. Abra o [centro de administração Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e vá para **utilizadores Ativos** sob a secção **Utilizadores** e selecione o utilizador que está a ver o erro.

2. Na página de utilizador que abre, aceda à secção **licenças e aplicações,** selecione o valor de **Localização** apropriado e atribua uma licença que contenha Exchange Online (expanda a licença para ver os seus dados). Quando terminar, clique em **Guardar as alterações.**

Em alguns casos, se a licença já estiver atribuída a uma conta de utilizador, remover e reatribuir a licença ajuda a resolver o problema e a obtê-la adequadamente a provisionada no sistema: 

- Verifique se as suas subscrições M365 Exchange Online (e outras, caso tenha alguma) estão em vigor e não expiraram recentemente.

Uma vez que tenha assegurado que a sua subscrição não expirou e que foi atribuída uma licença válida à conta de utilizador, pode demorar até 24 horas para que a licença seja antesetada, pelo que poderá ter de esperar que o seu problema seja resolvido. Para mais informações, consulte [Atribuir e gerir licenças.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)