---
title: Alterar canais de atualização para aplicações do Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440017"
---
# <a name="change-update-channels-for-office-apps"></a>Alterar canais de atualização para aplicações do Office

Para novas instalações do Office, utilize definições de descarregamento de software do Office para selecionar o canal de atualização pretendido e, em seguida, instale (ou reintefira) aplicações do Office. Para obter mais informações, consulte [As definições de descarregamento de software no Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Nota** O canal de atualização selecionado através das Definições de Descarregamento do Software do Office aplica-se a todos os utilizadores que realizem novas instalações utilizando o portal O365. Para obter mais informações, consulte [Download e instale ou reinstale o Microsoft 365 ou o Office 2019 num PC ou Mac.](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)   

Para as instalações existentes do Office, utilize a Ferramenta de Implementação do Office (ODT) para mudar para um canal de atualização diferente:  

1. Descarregue a versão mais recente da Ferramenta de Implementação do Office (setup.exe) a partir do [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identifique o nome do canal para o qual pretende mudar. Para obter mais informações, consulte [as opções de Configuração para a Ferramenta de Implementação do Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Crie um ficheiro XML de configuração especificando o nome do canal apropriado, por exemplo, update.xml.  
    a. <Configuration>  
    b. <Atualizações **Channel="Mensal"** />  
    c. </Configuration>
4. A partir de um pedido de comando elevado, mude para o local da pasta onde reside setup.exe e executar o seguinte comando:  
    a. update.xml de setup.exe /configuração
5. Inicie uma aplicação do Office (como o Excel) e, em seguida, selecione **Conta de Ficheiros**  >  **Account**. Na secção informações sobre o produto, selecione **Update Options**  >  **Update Now**.

Para obter mais informações, consulte [Como mudar os canais de atualização para as aplicações do Office existentes.](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel) 

Para mudar os canais de atualização para um grupo selecionado de utilizadores ou utilizando o Gestor de Configuração (SCCM), configufique a definição do 'Update Channel' utilizando o GPO. Para mais informações, consulte [a visão geral dos canais de atualização para aplicações microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Para mais detalhes, consulte [como gerir os canais ProPlus do Office 365 para IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) e [Gerir atualizações para as aplicações da Microsoft 365 com o Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).