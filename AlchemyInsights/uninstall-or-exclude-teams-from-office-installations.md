---
title: Desinstalar ou excluir equipas de instalações do Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658232"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Desinstalar ou excluir equipas de instalações do Escritório novas ou existentes

O Microsoft Teams está incluído como parte das aplicações da Microsoft 365 para empresas, aplicações microsoft 365 para negócios e Office for Mac.

- Utilize a [Ferramenta de Implantação do Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) para excluir equipas de novas instalações do Office.
- Para *desinstalar* equipas a partir de um dispositivo que executa o Windows, consulte [Desinstalar as Equipas da Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Para limpar as Equipas microsoft de várias máquinas-alvo ou utilizadores, consulte a [implementação do Microsoft Teams para limpar](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Utilize a opção [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) para impedir que as Equipas da Microsoft se instalem automaticamente no Office.
- Utilize a opção [PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *antes de as equipas serem instaladas,* para evitar que as Equipas da Microsoft arranquem automaticamente após a instalação.

Se estiver a utilizar o Office for Mac, consulte [as instalações da Microsoft Teams num Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).