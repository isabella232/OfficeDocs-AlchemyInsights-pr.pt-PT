---
title: Falha na resolução de problemas oneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826210"
---
# <a name="troubleshoot-onedrive-crashes"></a>Falha na resolução de problemas oneDrive

Se o OneDrive se despenhar repetidamente, experimente estes passos de resolução de problemas:

**Certifique-se de que as chaves de registo não estão definidas:**

1. Utilizando o Editor de Registos, navegue para HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Se o DisableFileSyncNGSC estiver presente e definido para 1, abra a chave e altere o valor para 0.
3. Lançar manualmente o OneDrive indo para iniciar ![Prima a tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), digite OneDrive na caixa de pesquisa e, em seguida, clique na aplicação de ambiente de trabalho OneDrive.

**Reset OneDrive:**

Notas:

- A reposição do OneDrive desliga todas as suas ligações de sincronização existentes (incluindo o seu OneDrive pessoal se estiver configurado).
- Não perderá ficheiros ou dados repondo o OneDrive no seu computador.

**Para redefinir o OneDrive:**

1. Abra um diálogo executar premindo a tecla do Windows e R.
2. Digite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset e prima OK. Uma janela de comando pode aparecer brevemente.
3. Lançar manualmente o OneDrive indo para iniciar ![Prima a tecla Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), digite OneDrive na caixa de pesquisa e, em seguida, clique na aplicação de ambiente de trabalho OneDrive.

Notas:

- Se tivesse optado por sincronizar apenas algumas pastas antes do reset, terá de o fazer novamente uma vez concluída a sincronização. Leia [Escolha quais as pastas OneDrive para sincronizar o computador](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)para obter mais   informações.
- Terá de completar isto para o seu OneDrive pessoal e OneDrive para negócios.