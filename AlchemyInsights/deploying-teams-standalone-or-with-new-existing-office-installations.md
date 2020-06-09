---
title: Equipas de implantação como autónomas ou com instalações de Escritórios novas ou existentes
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617906"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Equipas de implantação como autónomas ou com instalações de Escritórios novas ou existentes

O Microsoft Teams está agora incluído como parte de ***novas instalações*** de Aplicações Microsoft 365 para empresas, Aplicações Microsoft 365 para negócios e Office for Mac. Para mais informações, veja [quando é que as Equipas da Microsoft vão começar a ser incluídas com novas instalações do Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Além disso, a partir da versão 1906 do Current Channel, as equipas serão ***adicionadas às instalações existentes*** de Aplicações Microsoft 365 para empresas (e Aplicações microsoft 365 para empresas) em dispositivos que executam o Windows quando atualizar a instalação existente para a versão mais recente. Para mais informações, veja [e as instalações existentes do Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Se não quiser esperar por este horário de lançamento, pode implementar equipas como autónomas para os seus utilizadores [seguindo estas instruções](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ou pode ter os seus utilizadores a instalar equipas para si mesmos a partir de  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Se a sua organização não estiver pronta para implementar equipas, temos os passos que pode tomar para ***excluir equipas*** de instalações [novas](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ou [existentes](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) do Office. Se quiser que as Equipas sejam instaladas, mas não quer que as Equipas arranquem automaticamente para o utilizador depois de instaladas, consulte [Prevent Microsoft Teams para iniciar automaticamente após a instalação](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Para ***desinstalar equipas*** a partir de um dispositivo que executa o Windows, consulte [Desinstalar as Equipas da Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Para limpar as Equipas microsoft de várias máquinas-alvo ou utilizadores, consulte a [implementação do Microsoft Teams para limpar](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Se estiver a utilizar computadores partilhados, Serviços remotos de Desktop (RDS) ou Infraestruturas de Ambiente de Trabalho Virtuais (VDI), consulte [ambientes de computador partilhado e VDI com equipas da Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Se estiver a utilizar o Office for Mac, consulte [as instalações da Microsoft Teams num Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Após a instalação das Equipas, é [automaticamente atualizado](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) de duas em duas semanas com novas funcionalidades e atualizações de qualidade. 