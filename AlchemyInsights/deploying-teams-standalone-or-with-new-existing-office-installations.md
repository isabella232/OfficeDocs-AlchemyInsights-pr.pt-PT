---
title: Equipas de implementação como autónoma ou com instalações do Office novas ou existentes
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054241"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Equipas de implementação como autónoma ou com instalações do Office novas ou existentes

Teams da Microsoft está agora incluída como parte das ***novas instalações*** do Office 365 ProPlus, Office 365 Business e Office para Mac. Para mais informações, consulte [Quando Teams da Microsoft começará a ser incluídos nas novas instalações do Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Além disso, a partir da versão 1906 no canal mensal, equipas será ***adicionado às instalações existentes*** do Office 365 ProPlus (e Business do Office 365) em dispositivos com o Windows quando actualizar a instalação existente para a versão mais recente. Para mais informações, consulte [e quanto as instalações existentes do Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Se não pretender esperar para esta agenda de fase de instalação, pode implementar equipas como autónomo para os utilizadores seguindo [estas instruções](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ou pode fazer com que os utilizadores instalar equipas para si próprios de [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Se a organização não estiver preparada para implementar equipas, temos os passos que pode tomar para ***excluir as equipas*** de instalações de [Novo](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) ou [existente](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) do Office. Se pretender que as equipas para ser instalado, mas não pretende equipas para iniciar automaticamente para o utilizador depois de instalado, consulte [Equipas da Microsoft impede que seja iniciado automaticamente após a instalação](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Para ***desinstalar equipas*** a partir de um dispositivo com o Windows, consulte [Desinstalar equipas da Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). A limpeza Microsoft Teams de vários computadores de destino ou utilizadores, consulte a [Limpar a implementação de equipas da Microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Se estiver a utilizar computadores partilhados, serviços de ambiente de trabalho remoto (RDS) ou infra-estrutura de ambiente de Trabalho Virtual (VDI), consulte o [computador partilhado e ambientes de VDI com equipas da Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Se estiver a utilizar o Office para Mac, consulte [Microsoft equipas instalações uma Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Depois de equipas estiver instalado, é [automaticamente actualizada](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) aproximadamente cada duas semanas com novas funcionalidades e actualizações de qualidade. 