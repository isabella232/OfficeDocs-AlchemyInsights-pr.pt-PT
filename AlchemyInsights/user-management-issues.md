---
title: Problemas de gestão de utilizadores
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037505"
---
# <a name="user-management-issues"></a>Problemas de gestão de utilizadores

**O que acontece aos utilizadores atuais atribuídos à aplicação se eu desativar a propriedade 'Atribuição de utilizador necessária' (definir esta propriedade para Nº)?**

A desativação **da atribuição do Utilizador necessária** NÃO afeta os utilizadores atualmente afetados. A desativação desta propriedade só permitirá que todos os utilizadores acedam à aplicação. Todos os utilizadores listados e os utilizadores designados para grupos na aplicação continuarão a ser válidos.

- Para restringir a sua aplicação a um conjunto específico de utilizadores, consulte - [Restringir a aplicação AD do Azure a um conjunto de utilizadores - plataforma de identidade da Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Para atribuir utilizadores e grupos, a aplicações empresariais em Azure Ative Directory (Azure AD), quer dentro do portal Azure, quer através da utilização do PowerShell, consulte [gerir a atribuição do utilizador para uma aplicação no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Para delegar permissões de criação e gestão de aplicações, consulte [permissões de administrador de gestão de aplicações delegados - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Ocultar aplicações empresariais específicas dos utilizadores** - Use os seguintes passos para esconder todas as aplicações da Microsoft 365 do painel **MyApps.** As aplicações ainda estarão visíveis no portal do Office 365.

 1. Inscreva-se no portal Azure como administrador global para o seu diretório. 
 2. Selecione **Azure Ative Directory**. 
 3. Selecione **Utilizadores**. 
 4. Selecione **as definições do Utilizador**. 
 5. Nas **aplicações da Enterprise,** clique **em Gerir como os utilizadores finais lançam e vêem as suas aplicações.** 
 6. Para **os utilizadores só podem ver as aplicações do Office 365 no portal Do Office 365**, clique em **Sim**. 
 7. Clique em **Guardar**. 
 8. Para mais detalhes, consulte [a aplicação Ocultar uma Enterprise a partir da experiência do utilizador em Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Se oferecer um Software como uma aplicação de Serviço (SaaS) a muitas organizações, pode configurar a sua aplicação para aceitar insuflações de qualquer inquilino do Azure Ative Directory (Azure AD). Esta configuração chama-se "tornar a sua aplicação multi-inquilina". Os utilizadores de qualquer inquilino Azure AD poderão iniciar sing-in na sua app depois de consentir em utilizar a sua conta com a sua app. Para obter mais informações, consulte [apps Build que assinam em utilizadores AD Azure - plataforma de identidade da Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Como pode um utilizador final aceder à aplicação uma vez que é atribuído à aplicação?**

Cada aplicação na lâmina de aplicação Enterprise tem um link para os utilizadores finais acederem. Os utilizadores também podem aceder à aplicação através do portal **Myapps** de forma fácil.

- **Pretende saber quais as aplicações e tipo de aplicações que estão a ser utilizadas pelos utilizadores?**

Você pode baixar relatórios de inscrição nos últimos 30 dias a partir de **portal.azure.com > Azure Ative directy> Signins> relatórios de descarregamento**.

- Saiba como conceder o [consentimento administrativo de um inquilino para uma aplicação](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) e [configure como os utilizadores finais concordam com as aplicações.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Entenda [como funciona o consentimento](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) e [Gerencie o consentimento para as aplicações.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


