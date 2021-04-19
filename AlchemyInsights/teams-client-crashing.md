---
title: O cliente do Teams está a falhar?
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
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826282"
---
# <a name="teams-client-crashing"></a>O cliente do Teams está a falhar?

Se o seu cliente do Teams estiver a falhar, tente o seguinte:

- Se estiver a utilizar a aplicação de ambiente de trabalho do Teams, [certifique-se de que a aplicação está totalmente atualizada](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Certifique-se de que todos os [URLs e intervalos de endereços Microsoft 365 estão acessíveis.](https://docs.microsoft.com/microsoftteams/connectivity-issues)

- Faça login com a sua conta de administração do inquilino e verifique o seu [Painel de Saúde de Serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se não existe nenhuma falha ou degradação do serviço.

- Desinstalar e reinstalar a Aplicação de Equipas (link)
    - Navegue na pasta %appdata%\Microsoft\teams\ no seu computador e elimine todos os ficheiros desse diretório.
    - [Descarregue e instale a App Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), e, se possível, instale equipas como administrador (clique no instalador de Equipas e selecione "Executar como administrador" se disponível).

Se o cliente das Equipas ainda estiver em queda, pode reproduzir o problema? Em caso afirmativo:

1. Utilize o gravador de passos para capturar os seus passos.
    - Feche todas as aplicações desnecessárias ou confidenciais.
    - Lance o Gravador de Passos e reproduza o problema enquanto inicia sessão com a conta de utilizador afetada.
    - [Recolher os registos das equipas que captam os passos de repro registados.](https://docs.microsoft.com/microsoftteams/log-files) **Nota:** Certifique-se de que captura o endereço de inscrição do utilizador afetado.
    - Recolher a informação do balde de despejo e/ou fault (Windows). Lançar o Windows Powershell na máquina onde está a ocorrer a falha e executar os seguintes comandos:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Anexe o ficheiro ao seu caso de suporte.
