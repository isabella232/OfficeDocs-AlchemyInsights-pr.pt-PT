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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890349"
---
# <a name="teams-client-crashing"></a>Teams cliente falha

Se o seu cliente do Teams estiver a falhar, tente o seguinte:

- Se estiver a utilizar a aplicação de ambiente de trabalho do Teams, [certifique-se de que a aplicação está totalmente atualizada](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Certifique-se de que todos [os Microsoft 365 URLs e intervalos de endereços estão](https://docs.microsoft.com/microsoftteams/connectivity-issues) acessíveis.

- Indique sessão com a conta de administrador do seu inquilino e verifique o [Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) do Estado de Estado de Serviço para verificar se existe qualquer degradação no serviço ou indistionável.

- Desinstalar e reinstalar a Aplicação Teams Aplicação
    - Navegue para a pasta %appdata%\Microsoft\Teams\ no seu computador e elimine todos os ficheiros nesse diretório.
    - Transfira e instale a [Aplicação Teams](https://www.microsoft.com/microsoft-teams/download-app)e, se possível, instale o Teams como administrador  (clique com o botão direito do rato no instalador do Teams e selecione Executar como administrador se disponível).

Se o Teams cliente continuar a falhar, tente reproduzir o problema. Se possível:

1. Utilize o Gravador de Passos para capturar os seus passos.
    - Feche TODAS as aplicações desnecessárias ou confidenciais.
    - Instalar o Gravador de Passos e reproduzir o problema com a sessão iniciada com a conta de utilizador afetada.
    - [Recolha os registos das equipas que capturam os passos de reprovação gravados](https://docs.microsoft.com/microsoftteams/log-files). **Nota:** certifique-se de que captura o endereço de assinatura do utilizador afetado.
    - Recolha as informações do inserção de dados e/ou Do(s) falha (Windows). In execute Windows PowerShell no máquina onde a falha está a ocorrer e execute os seguintes comandos (após cada comando, prima Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Após o ficheiro de texto ser gerado e aparecer no ecrã, guarde o ficheiro e anexe-o ao pedido de serviço. 
