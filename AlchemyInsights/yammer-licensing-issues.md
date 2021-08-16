---
title: Yammer de licenciamento
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989746"
---
# <a name="yammer-licensing-issues"></a>Yammer de licenciamento

Todos os utilizadores têm de ter uma licença para utilizar o serviço Yammer Enterprise, mas por predefinição o Yammer não necessita que os utilizadores tenham uma licença para aceder ao serviço. Quando um administrador altera a definição para bloquear Microsoft 365 utilizadores sem licenças Yammer, os utilizadores que não tenham uma licença do Yammer Enterprise não podem aceder ao serviço Yammer. Para mais informações, consulte [Gerir Yammer licenças de utilizador no Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Quando as licenças são removidas dos utilizadores, o m Yammer de Dados já não é apresentado e outros serviços podem utilizar a remoção de licenças para ocultar funcionalidades. Noutros casos, as funcionalidades podem continuar a ser apresentadas, mas a atribuição de licença para funcionar.  

**A licença não está a ser atualizada para o utilizador**  

Ocasionalmente, é atribuída uma licença a um utilizador, mas continua a não conseguir aceder à Yammer. Existe uma maior probabilidade de ocorrerem atrasos quando a atribuição de licenças em massa está em curso. Yammer utilizadores podem não ser atualizados na mesma ordem em que as licenças são alteradas no Azure AD porque o sistema é executado assíncronamente. Aguarde até 24 horas antes de abrir um caso de suporte para comunicar problemas de sincronização de licenças.  

**Atribuição de licenças em massa**  

As licenças podem ser atribuídas através do centro de administração ou de scripts do PowerShell. Para mais informações, consulte Atribuir [licenças](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a utilizadores e Atribuir licenças a contas de utilizador com [o Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

O Suporte da Microsoft não fornece assistência para a criação de scripts, mas a documentação Yammer atribuição de licenças está disponível. Para mais informações, consulte [Gerir Yammer licenças de e-mail utilizando Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).