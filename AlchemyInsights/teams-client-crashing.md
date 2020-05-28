---
title: O cliente do Teams está a falhar?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354063"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="d21ba-102">O cliente do Teams está a falhar?</span><span class="sxs-lookup"><span data-stu-id="d21ba-102">Teams client crashing?</span></span>

<span data-ttu-id="d21ba-103">Se o seu cliente do Teams estiver a falhar, tente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d21ba-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="d21ba-104">Se estiver a utilizar a aplicação de ambiente de trabalho do Teams, [certifique-se de que a aplicação está totalmente atualizada](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="d21ba-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="d21ba-105">Certifique-se de que todos os [URLs e endereços microsoft 365 estão acessíveis.](https://docs.microsoft.com/microsoftteams/connectivity-issues)</span><span class="sxs-lookup"><span data-stu-id="d21ba-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="d21ba-106">Inicie sessão com a sua conta de administrador de inquilinos e verifique o seu Dashboard de [Saúde de Serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se não existe qualquer interrupção ou degradação do serviço.</span><span class="sxs-lookup"><span data-stu-id="d21ba-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="d21ba-107">Desinstalar e reinstalar a Aplicação de Equipas (link)</span><span class="sxs-lookup"><span data-stu-id="d21ba-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="d21ba-108">Navegue na pasta %appdata%\Microsoft\teams\ no seu computador e elimine todos os ficheiros desse diretório.</span><span class="sxs-lookup"><span data-stu-id="d21ba-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="d21ba-109">[Descarregue e instale a App equipas](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), e se possível, instale equipas como administrador (clique à direita no instalador de Equipas e selecione "Executar como administrador" se estiver disponível).</span><span class="sxs-lookup"><span data-stu-id="d21ba-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="d21ba-110">Se o cliente da equipa ainda está a falhar, pode reproduzir o problema?</span><span class="sxs-lookup"><span data-stu-id="d21ba-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="d21ba-111">Se assim for:</span><span class="sxs-lookup"><span data-stu-id="d21ba-111">If so:</span></span>

1. <span data-ttu-id="d21ba-112">Use o gravador de passos para capturar os seus passos.</span><span class="sxs-lookup"><span data-stu-id="d21ba-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="d21ba-113">Feche todos os pedidos desnecessários ou confidenciais.</span><span class="sxs-lookup"><span data-stu-id="d21ba-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="d21ba-114">Lance o Gravador de Passos e reproduza o problema enquanto inicia sessão com a conta de utilizador afetada.</span><span class="sxs-lookup"><span data-stu-id="d21ba-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="d21ba-115">[Recolha os registos das equipas que captam os passos repro registados.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="d21ba-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="d21ba-116">**Nota:** Certifique-se de que captura o endereço de entrada do utilizador com impacto.</span><span class="sxs-lookup"><span data-stu-id="d21ba-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="d21ba-117">Recolha a informação do balde de despejo e/ou falha (Windows).</span><span class="sxs-lookup"><span data-stu-id="d21ba-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="d21ba-118">Lance o Windows Powershell na máquina onde o acidente está a ocorrer e execute os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d21ba-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="d21ba-119">Prenda o ficheiro ao seu caso de suporte.</span><span class="sxs-lookup"><span data-stu-id="d21ba-119">Attach the file to your support case.</span></span>
