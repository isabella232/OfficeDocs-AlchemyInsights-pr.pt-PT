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
# <a name="teams-client-crashing"></a>O cliente do Teams está a falhar?

Se o seu cliente do Teams estiver a falhar, tente o seguinte:

- Se estiver a utilizar a aplicação de ambiente de trabalho do Teams, [certifique-se de que a aplicação está totalmente atualizada](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Certifique-se de que todos os [URLs e endereços microsoft 365 estão acessíveis.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- Inicie sessão com a sua conta de administrador de inquilinos e verifique o seu Dashboard de [Saúde de Serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se não existe qualquer interrupção ou degradação do serviço.

- Desinstalar e reinstalar a Aplicação de Equipas (link)
    - Navegue na pasta %appdata%\Microsoft\teams\ no seu computador e elimine todos os ficheiros desse diretório.
    - [Descarregue e instale a App equipas](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), e se possível, instale equipas como administrador (clique à direita no instalador de Equipas e selecione "Executar como administrador" se estiver disponível).

Se o cliente da equipa ainda está a falhar, pode reproduzir o problema? Se assim for:

1. Use o gravador de passos para capturar os seus passos.
    - Feche todos os pedidos desnecessários ou confidenciais.
    - Lance o Gravador de Passos e reproduza o problema enquanto inicia sessão com a conta de utilizador afetada.
    - [Recolha os registos das equipas que captam os passos repro registados.](https://docs.microsoft.com/microsoftteams/log-files) **Nota:** Certifique-se de que captura o endereço de entrada do utilizador com impacto.
    - Recolha a informação do balde de despejo e/ou falha (Windows). Lance o Windows Powershell na máquina onde o acidente está a ocorrer e execute os seguintes comandos:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Prenda o ficheiro ao seu caso de suporte.
