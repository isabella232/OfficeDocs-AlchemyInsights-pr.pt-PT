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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030677"
---
# <a name="teams-client-crashing"></a>O cliente do Teams está a falhar?

Se o seu cliente do Teams estiver a falhar, tente o seguinte:

- Se estiver a utilizar a aplicação de ambiente de trabalho do Teams, [certifique-se de que a aplicação está totalmente atualizada](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Certifique-se de que todos os [URLs e intervalos de endereços do Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) estão acessíveis.

- Inicie sessão com a sua conta de administração e verifique o seu [Dashboard do Estado de Funcionamento do Serviço](https://docs.microsoft.com/office365/enterprise/view-service-health) para verificar se não existe qualquer interrupção ou degradação do serviço.

 - Como último passo, pode tentar limpar a cache do seu cliente do Teams:

    1.  Saia completamente do cliente de ambiente de trabalho do Microsoft Teams. Pode clicar com o botão direito do rato em **Teams** na área do tabuleiro de sistema e clique em **Sair**, ou execute o Gestor de Tarefas e termine totalmente o processo.

    2.  Aceda ao Explorador de Ficheiros e escreva %appdata%\Microsoft\teams.

    3.  Uma vez no diretório, verá algumas das seguintes pastas:

         - Em **Cache de Aplicação**, aceda a Cache e elimine qualquer um dos ficheiros na localização da Cache:  %appdata%\Microsoft\teams\application cache\cache.

        - Em **Blob_storage**, elimine todos os ficheiros: %appdata%\Microsoft\teams\blob_storage.

        - Em **Cache**, elimine todos os ficheiros: %appdata%\Microsoft\teams\Cache.

        - Em **databases**, elimine todos os ficheiros: %appdata%\Microsoft\teams\databases.

        - Em **GPUCache**, elimine todos os ficheiros: %appdata%\Microsoft\teams\GPUcache.

        - Em **IndexedDB**, elimine o ficheiro .db: %appdata%\Microsoft\teams\IndexedDB.

        - Em **Local Storage**, elimine todos os ficheiros: %appdata%\Microsoft\teams\Local Storage.

        - Por último, em **tmp**, elimine qualquer ficheiro: %appdata%\Microsoft\teams\tmp.

    4. Reinicie o seu cliente do Teams.
