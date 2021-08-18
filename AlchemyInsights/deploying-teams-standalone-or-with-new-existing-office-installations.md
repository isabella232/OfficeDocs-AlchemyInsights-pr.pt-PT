---
title: Implementar o Teams como autarca ou com instalações de dados Office novas ou existentes
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320133"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementar o Teams como autarca ou com instalações de dados Office novas ou existentes

Microsoft Teams está agora incluído como  parte de novas instalações do Microsoft 365 Apps para Grandes Empresas, Microsoft 365 Apps para Pequenas e Médias Empresas e Office para Mac. Para obter mais informações, [consulte Quando é Microsoft Teams começar a ser incluído nas novas instalações do Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Além disso, a partir da Versão 1906 na Via com Atualizações ***Recentes,*** o Teams será adicionado a instalações existentes do Microsoft 365 Apps para Grandes Empresas (e do Microsoft 365 Apps para Pequenas e Médias Empresas) em dispositivos com o Windows quando atualizar a sua instalação existente para a versão mais recente. Para obter mais informações, [consulte e as instalações existentes do Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Nota:** Se não quiser esperar por esta agenda de implementação, pode implementar o Teams como [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) autônomo para os seus utilizadores ao seguir estas instruções ou pode fazer com que os seus utilizadores instalem o Teams para eles próprios a partir de [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Se a sua organização não estiver pronta para implementar o Teams, temos os passos que [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) pode [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) tomar para excluir Teams de instalações novas ou existentes do Office.  Se pretender que o Teams seja instalado, mas não pretender que o Teams seja iniciado automaticamente para o utilizador após a instalação, consulte Impedir que o [Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)seja iniciado automaticamente após a instalação.

Para ***desinstalar Teams*** de um dispositivo a executar o Windows, consulte [Desinstalar Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Para limpar os Microsoft Teams de vários utilizadores ou máquinas de destino, consulte Limpar [Microsoft Teams implementação](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Se estiver a utilizar computadores partilhados, Serviços de Ambiente de Trabalho Remoto (RDS) ou Infraestrutura de Ambiente de Trabalho Virtual (VDI), consulte [Ambientes](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)de trabalho e computadores partilhados com Microsoft Teams .

Se estiver a utilizar o Office para Mac, [consulte Microsoft Teams instalações num Mac.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Nota:** depois Teams instalado, é automaticamente [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) atualizado aproximadamente a cada duas semanas com novas funcionalidades e atualizações de qualidade. 