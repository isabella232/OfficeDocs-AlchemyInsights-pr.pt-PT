---
title: Registos de palavra-passe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527178"
---
# <a name="password-logs"></a><span data-ttu-id="59365-102">Registos de palavra-passe</span><span class="sxs-lookup"><span data-stu-id="59365-102">Password logs</span></span>

<span data-ttu-id="59365-103">**Estou com problemas em aceder a registos de auditoria de redefinição de passwords**</span><span class="sxs-lookup"><span data-stu-id="59365-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="59365-104">Para resolver problemas no que diz respeito ao acesso aos registos de auditoria de redefinição de passwords, execute o seguinte passo:</span><span class="sxs-lookup"><span data-stu-id="59365-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="59365-105">Certifique-se de que está autorizado a visualizar os registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="59365-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="59365-106">Apenas são autorizadas as seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="59365-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="59365-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="59365-107">Global administrator</span></span>
 - <span data-ttu-id="59365-108">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="59365-108">Security administrator</span></span>
 - <span data-ttu-id="59365-109">Leitor de segurança</span><span class="sxs-lookup"><span data-stu-id="59365-109">Security reader</span></span>

<span data-ttu-id="59365-110">**Quero ver todos os eventos de auditoria de redefinição de passwords a partir do momento em que inicialmente desloquei**</span><span class="sxs-lookup"><span data-stu-id="59365-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="59365-111">Até 120.000 eventos de reset/registo de passwords são armazenados nos relatórios dos últimos 30 dias.</span><span class="sxs-lookup"><span data-stu-id="59365-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="59365-112">Este limite máximo aplica-se à UI ao descarregar o CSV.</span><span class="sxs-lookup"><span data-stu-id="59365-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="59365-113">1 milhão de eventos estão disponíveis através do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="59365-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="59365-114">Para mais informações, consulte os links abaixo:</span><span class="sxs-lookup"><span data-stu-id="59365-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="59365-115">Autosserviço de autosserviço redefinir eventos da AZure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="59365-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="59365-116">Como descarregar eventos de registo de redefinição de password rapidamente com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="59365-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="59365-117">**Quero saber mais sobre as capacidades de reporte de redefinição de passwords**</span><span class="sxs-lookup"><span data-stu-id="59365-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="59365-118">Verifique quem está a registar ou a redefinir palavras-passe com registos de auditoria de redefinição de password AD do Azure no portal Azure sob **Utilizadores e grupos**.</span><span class="sxs-lookup"><span data-stu-id="59365-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="59365-119">Para mais informações, consulte os seguintes links:</span><span class="sxs-lookup"><span data-stu-id="59365-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="59365-120">Relatórios de reset de palavra-passe</span><span class="sxs-lookup"><span data-stu-id="59365-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="59365-121">Como visualizar relatórios de reset de palavra-passe no portal Azure</span><span class="sxs-lookup"><span data-stu-id="59365-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="59365-122">Autosserviço de autosserviço redefinir eventos da AZure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="59365-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="59365-123">Como descarregar eventos de registo de redefinição de password rapidamente com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="59365-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


