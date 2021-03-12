---
title: Problemas de grupo de resolução de problemas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714049"
---
# <a name="troubleshoot-group-issues"></a>Problemas de grupo de resolução de problemas

**Preciso atribuir um grupo a um papel de AD Azure**

Para atribuir um grupo Azure Ative Directory (AD) a uma função AD Azure, execute os seguintes passos:

1. Criar um novo grupo - Criar um novo grupo:

    a. Inscreva-se no centro de administração Azure AD com funções privilegiadas de administrador ou permissões globais de administrador. 
    b. Selecione Azure Ative Directory > Groups > Todos os grupos > Novo grupo. 
    c. Criar o grupo.

2. Atribua o papel ao grupo durante a criação do grupo ou após a criação do grupo.

    a. Para atribuir um papel ao grupo no momento da criação do grupo, ligue as funções de AD Azure pode ser atribuída ao grupo e criar o grupo.
    b. Para atribuir um papel ao grupo depois de criado, navegue no separador de funções atribuído para o grupo recém-criado e atribua o papel ao grupo.

**Preciso de gerir a adesão a um grupo que é atribuído ao papel de AD Azure**

1. Para evitar a elevação de privilégios, por defeito, apenas o administrador privilegiado e administrador global pode modificar a adesão de um grupo que é atribuído a um papel. Podem, no entanto, optar por designar um proprietário para tal grupo e delegar esta tarefa. Para obter mais informações, [utilize grupos de nuvem para gerir atribuições de funções no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Para questões comuns e dicas de resolução de problemas para atribuir funções a grupos em Azure AD, consulte [as funções de resolução de problemas atribuídas a grupos de nuvem](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Grupos dinâmicos**

1. Se não conseguir encontrar os atributos do utilizador incorporados, certifique-se de que o atributo está na lista de propriedades suportadas.
2. Se estiver à procura de atributos de dispositivo incorporados, certifique-se de que o atributo está na lista de atributos do dispositivo 
3. Além dos atributos do utilizador e do dispositivo incorporados, também pode utilizar [atributos de extensão.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Após sincronizar os atributos de extensão a partir de AD do Windows Server ou de uma aplicação SaaS conectada, os atributos devem ser visíveis na lista de down-down do construtor de regras. O nome de atributo personalizado pode ser encontrado no diretório consultando o atributo de um utilizador usando PowerShell e procurando o nome do atributo. Estes poderiam também ser utilizados na construção de regras na sintaxe de regras.
4. Certifique-se de que o seu inquilino tem a licença adequada. Grupos dinâmicos exigem que o inquilino tenha uma licença Azure AD P1 Premium. A lista de planos de licença AD Azure pode ser acedida [aqui.](https://azure.microsoft.com/pricing/details/active-directory/) Os planos de licenciamento de Mobilidade Empresarial + Segurança podem ser acedidos [aqui.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Certifique-se de que o papel do utilizador que cria o grupo dinâmico é um administrador global, administrador intune, administrador de grupo ou administrador de utilizador.
6. Por favor, dê tempo para que o grupo povoe. Dependendo do tamanho do seu inquilino, o grupo pode demorar até 24 horas para a povoagem pela primeira vez ou após uma mudança de regras.
7. Para obter mais informações, consulte [Criar regras baseadas em atributos para a adesão dinâmica ao grupo](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Preciso apagar um grupo.**

1. Os grupos podem ser eliminados do diretório utilizando o Remove-AzureADGroup cmdlet no módulo Azure AD Powershell.
2. Antes de tentar eliminar um grupo sincronizado em Azure AD, certifique-se de que apagou todas as licenças atribuídas para evitar erros.
3. Para obter mais informações sobre a eliminação de grupos, consulte [a Eliminação de um grupo com uma licença atribuída.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Preciso restaurar um grupo apagado.**

1. Se um grupo do Office 365 for eliminado, só pode ser restaurado até 30 dias antes da eliminação permanente. Uma vez eliminado permanentemente, o grupo já não pode ser restaurado. Saiba mais sobre a restauração de grupos [aqui.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Esta funcionalidade não é suportada por grupos de segurança e grupos de distribuição.
3. Certifique-se de que está autorizado a restaurar um grupo office 365. Os administradores globais, os administradores de grupos, os administradores de contas de utilizador, os administradores de serviços intune, o suporte de nível 1 ou de nível 2, e o proprietário do grupo podem ser capazes de restaurar um grupo.
4. Quando um grupo dinâmico é eliminado e restaurado, é visto como um novo grupo e repovoado de acordo com a regra. Este processo pode demorar até 24 horas.
5. Para obter mais informações sobre a restauração de um grupo eliminado, consulte [Restaurar um grupo eliminado do Office 365 no Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Configuração da política de expiração do grupo**

1. Esta funcionalidade é suportada apenas para grupos do Office 365, e não para grupos de segurança e grupos de distribuição não são suportados.
2. Configurar e utilizar a política de caducidade para grupos office 365 requer uma licença Azure AD Premium.
3. Atualmente, apenas uma política de caducidade pode ser configurada para grupos do Office 365 num inquilino.
4. Apenas administradores globais, administradores de grupos, administradores de utilizadores e o proprietário do grupo podem renovar um grupo.
5. Se um grupo do Office 365 expirar, este é eliminado e só pode ser restaurado até 30 dias antes da eliminação permanente. Uma vez eliminado permanentemente, o grupo já não pode ser restaurado. Saiba mais sobre a restauração de grupos [aqui.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Renovação automática baseada na atividade**

As atividades do utilizador do SharePoint, Outlook e Teams podem desencadear a renovação automática do grupo. As atividades são verificadas em 35 dias antes de um grupo expirar. Se houver atividade durante o ciclo de vida do grupo atual, o grupo será renovado automaticamente e a notificação por e-mail não será enviada para os proprietários do grupo.

**Tempo de notificação para grupos caducados**

1. As notificações por e-mail são enviadas ao Office 365 proprietários do grupo 30 dias, 15 dias e 1 dia antes da expiração do grupo.
2. Quando configurar a expiração pela primeira vez, os grupos mais velhos do que o intervalo de validade são definidos para 35 dias até ao termo.
3. A data de validade do grupo é calculada com base na data de renovação do grupo, não com base na data atualizada da apólice. Se a política de validade for atualizada, a data de validade não será alterada.
4. Para mais informações consulte, [política de expiração do Grupo e e-mails de renovação](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) e [Restaurar um grupo eliminado do Office 365 em Azure Ative Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Permissão para criar um grupo**

Certifique-se de que está autorizado a criar um novo grupo. Os administradores globais podem desativar a criação de grupos no portal Azure ou no Painel de Acesso. Pode precisar de um administrador para criar o novo grupo para si, ou para lhe dar permissões apropriadas.

1. [Criar um novo grupo e adicionar membros no portal Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Criar grupos em Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Criação de grupos desativação em Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Gerir quem pode criar grupos no Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Notificação de boas-vindas do Gabinete 365 via Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Funções administrativas da AD AZure](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Gerir permissões de criação de grupo**

1. Os administradores globais podem gerir permissões de criação de grupos para grupos de segurança ou do Office 365 criados no portal Azure ou painel de acesso, definindo **os Utilizadores podem criar grupos de segurança em portais Azure** ou **os utilizadores podem criar grupos office 365 em configurações de portais Azure** em **todos os grupos > Geral (Definições)**.
2. Também pode restringir a criação de grupo para selecionar um grupo de utilizadores se tiver uma licença Azure AD P1 Premium.

**Notificação de boas-vindas incapacitante para novos membros de um grupo do Office 365**

A notificação de boas-vindas enviada aos utilizadores adicionados aos grupos Office 365 pode ser desativada por definição `UnifiedGroupWelcomeMessageEnabled` de **False** in Powershell. Saiba mais sobre este cenário [aqui.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













