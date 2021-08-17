---
title: Ativar Cofre anexos para o SharePoint Online, OneDrive e Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894474"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ativar Cofre anexos para o SharePoint Online, OneDrive e Microsoft Teams

1. Utilizando as suas credenciais de administrador global ou administrador de segurança, abra o portal do Microsoft 365 Defender em e, em seguida, vá a Políticas & Políticas de <https://security.microsoft.com>  \>  \> **ameaça Cofre Anexos**  na secção Políticas

   Para ir diretamente para a **Cofre Anexos,** utilize <https://security.microsoft.com/safeattachmentv2> .

2. Na página **Anexos Cofre,** clique em **Definições globais**.
3. Na panfleto que é exibida, selecione Atalho para o Microsoft Defender Office 365 para o **SharePoint, OneDrive e Microsoft Teams e,** em seguida, selecione **Guardar**.

    > [!TIP]
    >
    > Faça os seguintes passos para melhorar a proteção de Cofre Anexos para SharePoint, OneDrive e Microsoft Teams:
    >
    > - Para impedir que os utilizadores transfiram ficheiros maliciosos, utilize o valor do parâmetro `$true` *DisallowInfectedFileDownload* no cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** no PowerShell do SharePoint Online. Para obter mais informações, [consulte Utilizar o PowerShell do SharePoint Online para impedir que os utilizadores transfiram ficheiros maliciosos.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Criar uma política de alerta para ficheiros detetados](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Para obter mais informações, consulte Cofre Anexos Office 365 para [o SharePoint, OneDrive e Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
