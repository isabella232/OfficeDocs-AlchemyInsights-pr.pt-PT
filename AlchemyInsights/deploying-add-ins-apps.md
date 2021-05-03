---
title: Implementar os add-ins para Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125682"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Implementar os add-ins para Microsoft 365 Apps

A Implementação Centralizada é a forma recomendada de implementar Office para utilizadores e grupos na sua organização. Para implementar os add-ins, siga os passos abaixo:

**Nota:** Para instalar os seus Office como um utilizador individual, consulte [Ver,](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)gerir e instalar os seus Office programas . Além disso, certifique-se de que a aquisição individual Office da Store está ativada. 

1. Certifique-se de que o seu ambiente cumpre os requisitos para a implementação de add-ins através da Implementação Centralizada. Para obter detalhes, consulte [Requisitos.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Vá para **Definições**  >  **Aplicações Integradas** Obter aplicações no Microsoft 365 de administração para implementar  >   os add-ins. 

Notas: 

- As Aplicações Integradas requerem que o administrador tenha permissões de Administrador Exchange Globais.

- Ao implementar os add-ins para múltiplos utilizadores, recomendamos que faça atribuições ao utilizar grupos em vez de utilizadores individuais. Para obter detalhes, [consulte Considerações a ter ao atribuir um add-in a utilizadores e grupos.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- A Implementação Centralizada não suporta utilizadores em grupos aninhados ou grupos que tenham grupos principal. Para obter detalhes, consulte [Atribuições de utilizador e de grupo.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Certifique-se de que o Serviço Microsoft 365 de Gestão de Aplicações (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') está ativado para que os utilizadores inscreva-se. Para obter detalhes, consulte [Configurar propriedades da aplicação.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Caso se depare com problemas ao implementar os add-ins através das Aplicações Integradas, experimente implementar com [os Add-Ins.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Para mais informações, consulte:

[Implementar os add-ins no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gerir os add-ins no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Utilizar os cmdlets do PowerShell de Implementação Centralizada para gerir os add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicar Office com](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) a Implementação Centralizada através do Microsoft 365 de administração 
 [Remoção de problemas: o utilizador não está a ver os seus add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Remova erros de utilizadores com Office com os Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)