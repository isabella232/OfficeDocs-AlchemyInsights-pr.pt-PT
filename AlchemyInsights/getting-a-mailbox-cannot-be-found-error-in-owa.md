---
title: 126 Não foi possível encontrar o erro Obter uma Caixa de Correio no OWA?
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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056501"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Está a obter um erro de caixa de correio que não foi encontrado Outlook na Web?

Se estiver **a** utilizar o Outlook na Web e receber uma Caixa de Correio não poderá ser encontrada por erro, significa que a conta que usou para se ligar ao Outlook na Web não tem uma licença do Exchange Online e, portanto, não existe uma caixa de correio associada à conta. O seu administrador pode atribuir uma licença à sua conta ao seguir estes passos:

1. Abra o [centro de administração do Microsoft 365](https://portal.office.com/adminportal/home#/homepage) e vá para  **Utilizadores ativos** na secção Utilizadores e selecione o utilizador que está a ver o erro.

2. Na página de utilizador que é aberta, vá para a  secção **Licenças** e Aplicações, selecione o valor de Localização adequado e atribuir uma licença que contenha Exchange Online (expanda a licença para ver os detalhes). Quando terminar, clique em **Guardar alterações.**

Em alguns casos, se a licença já estiver atribuída a uma conta de utilizador, remover e reatribir a licença ajuda a resolver o problema e a aprovisioná-la corretamente no sistema: 

- Verifique se as suas subscrições Exchange Online M365 (e outras, se tiver alguma) estão atuais e não expiraram recentemente.

Depois de se certificar de que a sua subscrição não expirou e de que foi atribuída uma licença válida à conta de utilizador, pode demorar até 24 horas para que a licença seja aprovisionada, pelo que poderá ter de aguardar até que o seu problema seja resolvido. Para mais informações, consulte [Atribuir e gerir licenças.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)