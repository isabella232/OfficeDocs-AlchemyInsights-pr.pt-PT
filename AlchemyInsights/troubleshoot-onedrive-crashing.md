---
title: Remoção de OneDrive falhas
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921018"
---
# <a name="troubleshoot-onedrive-crashes"></a>Remoção de OneDrive falhas

Se OneDrive falha repetidamente, experimente estes passos de remoção de problemas:

**Certifique-se de que as chaves de registo não estão definidas:**

1. Ao utilizar o Editor de Registo, navegue até HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Se DisableFileSyncNGSC estiver presente e estiver definido como 1, abra a chave e altere o valor para 0.
3. Iniciar manualmente o OneDrive ao ir para Iniciar ![Prima a tecla Windows tecla](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), escreva OneDrive na caixa de pesquisa e, em seguida, clique na OneDrive de ambiente de trabalho.

**Repor OneDrive:**

Notas:

- A reposição OneDrive desliga todas as ligações de sincronização existentes (incluindo as suas ligações pessoais OneDrive, se configuradas).
- Não irá perder ficheiros ou dados ao repor OneDrive no seu computador.

**Para repor OneDrive:**

1. Abra uma caixa de diálogo Executar ao premir Windows e R.
2. Escreva %localappdata%\Microsoft\OneDrive\onedrive.exe /reset e prima OK. Poderá ser apresentada uma janela de Comando por breves instantes.
3. Iniciar manualmente o OneDrive ao ir para Iniciar ![Prima a tecla Windows tecla](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), escreva OneDrive na caixa de pesquisa e, em seguida, clique na OneDrive de ambiente de trabalho.

Notas:

- Se tiver optado por sincronar apenas algumas pastas antes da reposição, terá de fazê-lo novamente assim que a sincronização estiver concluída. Leia [Escolha quais as OneDrive sincronização com o seu computador para](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)obter mais   informações.
- Terá de concluir este processo para a sua conta pessoal OneDrive e OneDrive para Empresas.