---
title: Controle atualizações automáticas para apps do Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439921"
---
# <a name="control-automatic-updates-for-office-apps"></a>Controle atualizações automáticas para apps do Office

Por predefinição, as atualizações para Apps do Office são descarregadas automaticamente e aplicadas em segundo plano sem qualquer intervenção do utilizador. No entanto, os administradores podem controlar a forma como as atualizações são aplicadas utilizando as definições de Atualização do Office. As definições de atualização permitem aos administradores ativar ou desativar atualizações automáticas, mostrar ou ocultar o botão **Update Now** no Office, definir prazos de atualização e muito mais. Para obter informações detalhadas, consulte:

- [Configurar definições de atualização para o Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [A atualização automática do Office não está ativada](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Defina como o Office é atualizado depois de instalado](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Para rever as definições de atualizações existentes aplicadas a uma máquina cliente, siga estes passos:

1. Abra o Editor de Registo saindo para **start**  >  **run**  >  **regedit**.
2. Mude para a seguinte localização e reveja as definições de Atualização do Office:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuração

**Nota**  Se a tecla OfficeMgmtCOM estiver definida, poderá ver a mensagem "Atualizações são geridas pelo administrador **do**seu sistema" nas  >  **Account**  >  **Atualizações do Office**Account Office . Para obter mais informações, consulte [Gerir atualizações para as aplicações da Microsoft 365 com o Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  