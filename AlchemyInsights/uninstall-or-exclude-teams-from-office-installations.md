---
title: Desinstalar ou excluir Teams de Office instalação
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: a960c96abf6215e3a34908ce8669a0c61298daac829343b3673dbfef0c4cbfc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007729"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Desinstalar ou excluir Teams de instalações de sistema Office novas ou existentes

Microsoft Teams incluído como parte de Microsoft 365 Apps para Grandes Empresas, Microsoft 365 Apps para Pequenas e Médias Empresas e Office para Mac.

- Utilize [a Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) para excluir Teams de novas instalações do Office.
- Para *desinstalar* Teams de um dispositivo a executar o Windows, consulte [Desinstalar Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Para limpar o Microsoft Teams de vários utilizadores ou máquinas de destino, consulte Limpar [Microsoft Teams implementação .](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)
- Utilize a [opção PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) para impedir Microsoft Teams ser instalado automaticamente com o Office.
- Utilize a opção [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *antes* Teams ser instalado, para impedir que o Microsoft Teams seja iniciado automaticamente após a instalação.

Se estiver a utilizar o Office para Mac, [consulte Microsoft Teams instalação do Mesmo num Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)