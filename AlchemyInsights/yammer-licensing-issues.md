---
title: Questões de licenciamento yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657287"
---
# <a name="yammer-licensing-issues"></a>Questões de licenciamento yammer

Todos os utilizadores devem ter uma licença para usar o serviço Yammer Enterprise, mas por padrão a Yammer não requer que os utilizadores tenham uma licença para aceder ao serviço. Quando um administrador altera a definição para bloquear utilizadores da Microsoft 365 sem licenças Yammer, os utilizadores não atribuídos a uma licença Yammer Enterprise não podem aceder ao serviço Yammer. Para mais informações, consulte [as licenças de utilizador da Manage Yammer no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Quando as licenças são removidas dos utilizadores, o azulejo Yammer já não é apresentado, e outros serviços podem usar a remoção da licença para ocultar funcionalidades. Noutros casos, as características ainda podem aparecer, mas requerem a atribuição de licenças para operar.  

**A licença não está a ser atualizada para o utilizador**  

Ocasionalmente, um utilizador é atribuído a uma licença, mas ainda não consegue aceder a Yammer. Os atrasos são mais prováveis de ocorrer quando uma atribuição de licença em massa está em andamento. Os utilizadores de Yammer podem não ser atualizados na mesma ordem que as licenças são alteradas em Azure AD porque o sistema funciona assíncronamente. Aguarde até 24 horas antes de abrir um caso de apoio para reportar problemas de sincronização de licenças.  

**Atribuição de licença a granel**  

As licenças podem ser atribuídas através do centro de administração ou da scripting PowerShell. Para obter mais informações, consulte [atribuir licenças aos utilizadores](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) e [atribuir licenças às contas dos utilizadores com o Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

O Microsoft Support não presta assistência na criação de scripts, mas a documentação sobre a atribuição da licença Yammer está disponível. Para obter mais informações, consulte [as licenças Manage Yammer utilizando o Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).