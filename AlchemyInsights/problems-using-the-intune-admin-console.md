---
title: Problemas na utilização da consola de administração Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555389"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemas na utilização da consola de administração Intune

**"Acesso negado" ao navegar no portal de administração Intune.**

- Se for membro de uma função personalizada Intune, certifique-se de que uma licença Intune ou Enterprise Mobility Suite (EMS) é atribuída à sua conta.
- Se estiver a utilizar o Gestor de Configuração para gerir dispositivos, verifique se não faz parte da coleção de utilizadores Intune para o Gestor de Configuração MDM.
- Verifique se lhe foi atribuídas as permissões adequadas de controlo de administração (RBAC) na lâmina de funções Intune.
- Verifique se o grupo utilizado não é uma lista de distribuição. Intune no portal Azure apenas suporta contas de utilizadores que pertencem a grupos de segurança do Azure Ative Directory. Reveja os seus grupos no portal Azure > Grupos **Intune**  >  **Groups**, ou no portal Azure > **Azure Ative Directory**.

**O utilizador tem demasiadas permissões para o papel intune atribuído**

Aconselhe o utilizador a ir às funções **Intune**  >  **Intune**  >  **As minhas permissões**  >  **Exportar** para rever permissões concedidas.

**Adicionei um grupo de âmbito a um papel, mas os utilizadores nessa função ainda vêem outros utilizadores ou dispositivos.**

Os grupos de âmbito não filtram os utilizadores ou dispositivos. Grupos de âmbito:

- Limite a quem os utilizadores podem atribuir políticas ou aplicações.
- Permitir que apenas utilizadores específicos executem tarefas remotas em dispositivos.

Para obter mais informações sobre grupos de âmbito, consulte [o controlo de acesso baseado em funções (RBAC) com o Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Adicionei um utilizador a um papel intune, mas eles ainda têm acesso total à consola de administração Intune.**

Navegue para Intune > **Utilizadores** no portal Azure e verifique se o utilizador não está atribuído a nenhuma das seguintes funções no portal Azure:

- Administrador global
- Administrador de serviço intune
- Administrador do SharePoint

Para obter mais informações, consulte [o controlo de acesso baseado em funções (RBAC) com o Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemas de acesso**

Para mais informações, veja [não pode assinar no Office 365, Azure ou Intune.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)