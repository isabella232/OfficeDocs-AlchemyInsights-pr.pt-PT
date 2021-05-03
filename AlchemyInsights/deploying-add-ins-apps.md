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
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="6b2f4-102">Implementar os add-ins para Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="6b2f4-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="6b2f4-103">A Implementação Centralizada é a forma recomendada de implementar Office para utilizadores e grupos na sua organização.</span><span class="sxs-lookup"><span data-stu-id="6b2f4-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="6b2f4-104">Para implementar os add-ins, siga os passos abaixo:</span><span class="sxs-lookup"><span data-stu-id="6b2f4-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="6b2f4-105">**Nota:** Para instalar os seus Office como um utilizador individual, consulte [Ver,](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)gerir e instalar os seus Office programas .</span><span class="sxs-lookup"><span data-stu-id="6b2f4-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="6b2f4-106">Além disso, certifique-se de que a aquisição individual Office da Store está ativada.</span><span class="sxs-lookup"><span data-stu-id="6b2f4-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="6b2f4-107">Certifique-se de que o seu ambiente cumpre os requisitos para a implementação de add-ins através da Implementação Centralizada.</span><span class="sxs-lookup"><span data-stu-id="6b2f4-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="6b2f4-108">Para obter detalhes, consulte [Requisitos.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="6b2f4-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="6b2f4-109">Vá para **Definições**  >  **Aplicações Integradas** Obter aplicações no Microsoft 365 de administração para implementar  >   os add-ins.</span><span class="sxs-lookup"><span data-stu-id="6b2f4-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="6b2f4-110">Notas:</span><span class="sxs-lookup"><span data-stu-id="6b2f4-110">Notes:</span></span> 

- <span data-ttu-id="6b2f4-111">As Aplicações Integradas requerem que o administrador tenha permissões de Administrador Exchange Globais.</span><span class="sxs-lookup"><span data-stu-id="6b2f4-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="6b2f4-112">Ao implementar os add-ins para múltiplos utilizadores, recomendamos que faça atribuições ao utilizar grupos em vez de utilizadores individuais.</span><span class="sxs-lookup"><span data-stu-id="6b2f4-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="6b2f4-113">Para obter detalhes, [consulte Considerações a ter ao atribuir um add-in a utilizadores e grupos.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="6b2f4-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="6b2f4-114">A Implementação Centralizada não suporta utilizadores em grupos aninhados ou grupos que tenham grupos principal.</span><span class="sxs-lookup"><span data-stu-id="6b2f4-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="6b2f4-115">Para obter detalhes, consulte [Atribuições de utilizador e de grupo.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="6b2f4-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="6b2f4-116">Certifique-se de que o Serviço Microsoft 365 de Gestão de Aplicações (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') está ativado para que os utilizadores inscreva-se.</span><span class="sxs-lookup"><span data-stu-id="6b2f4-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="6b2f4-117">Para obter detalhes, consulte [Configurar propriedades da aplicação.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="6b2f4-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="6b2f4-118">Caso se depare com problemas ao implementar os add-ins através das Aplicações Integradas, experimente implementar com [os Add-Ins.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="6b2f4-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="6b2f4-119">Para mais informações, consulte:</span><span class="sxs-lookup"><span data-stu-id="6b2f4-119">For more information, see:</span></span>

<span data-ttu-id="6b2f4-120">[Implementar os add-ins no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Gerir os add-ins no centro de administração](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Utilizar os cmdlets do PowerShell de Implementação Centralizada para gerir os add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Publicar Office com](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) a Implementação Centralizada através do Microsoft 365 de administração 
 [Remoção de problemas: o utilizador não está a ver os seus add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Remova erros de utilizadores com Office com os Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="6b2f4-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>