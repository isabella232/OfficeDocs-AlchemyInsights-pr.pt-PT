---
title: Teams cliente falha
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187732"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="fd789-102">Teams cliente falha</span><span class="sxs-lookup"><span data-stu-id="fd789-102">Teams client crashing</span></span>

<span data-ttu-id="fd789-103">Se o seu cliente do Teams estiver a falhar, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="fd789-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="fd789-104">Se estiver a utilizar a aplicação de ambiente de trabalho do Teams, [certifique-se de que a aplicação está totalmente atualizada](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="fd789-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="fd789-105">Certifique-se de que todos [os Microsoft 365 URLs e intervalos de endereços são](/microsoftteams/connectivity-issues) acessíveis.</span><span class="sxs-lookup"><span data-stu-id="fd789-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="fd789-106">Indique sessão com a conta de administrador do seu inquilino e verifique o [Dashboard](/office365/enterprise/view-service-health) do Estado de Estado de Serviço para verificar se existe qualquer degradação no serviço ou indistionável.</span><span class="sxs-lookup"><span data-stu-id="fd789-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="fd789-107">Desinstalar e reinstalar a aplicação Teams Aplicação</span><span class="sxs-lookup"><span data-stu-id="fd789-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="fd789-108">Navegue para a pasta %appdata%\Microsoft\Teams\ no seu computador e elimine todos os ficheiros nesse diretório.</span><span class="sxs-lookup"><span data-stu-id="fd789-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="fd789-109">Transfira e instale a [Aplicação Teams](https://www.microsoft.com/microsoft-teams/download-app)e, se possível, instale o Teams como administrador  (clique com o botão direito do rato no instalador do Teams e selecione Executar como administrador se disponível).</span><span class="sxs-lookup"><span data-stu-id="fd789-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="fd789-110">Se o Teams cliente continuar a falhar, tente reproduzir o problema.</span><span class="sxs-lookup"><span data-stu-id="fd789-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="fd789-111">Se possível:</span><span class="sxs-lookup"><span data-stu-id="fd789-111">If you can:</span></span>

1. <span data-ttu-id="fd789-112">Utilize o Gravador de Passos para capturar os seus passos.</span><span class="sxs-lookup"><span data-stu-id="fd789-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="fd789-113">Feche TODAS as aplicações desnecessárias ou confidenciais.</span><span class="sxs-lookup"><span data-stu-id="fd789-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="fd789-114">Instalar o Gravador de Passos e reproduzir o problema com a sessão iniciada com a conta de utilizador afetada.</span><span class="sxs-lookup"><span data-stu-id="fd789-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="fd789-115">[Recolha os registos das equipas que capturam os passos de reprovação gravados](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="fd789-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="fd789-116">**Nota:** certifique-se de que captura o endereço de assinatura do utilizador afetado.</span><span class="sxs-lookup"><span data-stu-id="fd789-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="fd789-117">Recolha as informações do inserção de informações e/ou Falha do Windows).</span><span class="sxs-lookup"><span data-stu-id="fd789-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="fd789-118">Incorra Windows PowerShell no máquina onde a falha está a ocorrer e execute os seguintes comandos (após cada comando, prima Enter):</span><span class="sxs-lookup"><span data-stu-id="fd789-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="fd789-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="fd789-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="fd789-120">Após o ficheiro de texto ser gerado e aparecer no ecrã, guarde o ficheiro e anexe-o ao pedido de serviço.</span><span class="sxs-lookup"><span data-stu-id="fd789-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
