---
title: Tema genérico do Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2605"
- "9000701"
ms.openlocfilehash: e1d5f07a10fc014ac8b983bd6dd426c13fc7b807
ms.sourcegitcommit: 7d787b8c5af223e2711b4c2a2ca55ce2bdc25aea
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2020
ms.locfileid: "42856478"
---
# <a name="teams-common-issues-and-resolutions"></a>Problemas conhecidos do Teams e resoluções

Para obter uma resposta mais específica, tente reformular a sua pergunta para incluir quaisquer erros que esteja a ver ou as funcionalidades do Teams que está a usar.

Se precisar de ajuda para implementar o Teams no suporte de Trabalhadores Remotos (WFH) devido ao COVID-19, consulte [Suporte a trabalhadores remotos usando o Microsoft Teams](https://docs.microsoft.com/microsoftteams/support-remote-work-with-teams). Além disso, poderá ser elegível para a assistência de implementação do Programa Microsoft 365 FastTrack: visite o [Centro FastTrack](https://www.microsoft.com/fasttrack) para submeter um pedido.

Para todos os clientes do Teams:

- **Novo no Teams?** Consulte [Introdução ao Microsoft Teams](https://docs.microsoft.com/microsoftteams/get-started-with-teams-quick-start).
- **Ativar o acesso de convidados ao Teams:** consulte a [lista de verificação de acesso de convidados do Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) e certifique-se de que todos os passos foram concluídos. Recursos adicionais:
    - [Understanding Guest Access in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access) (Compreender o Acesso de Convidados no Microsoft Teams)
    - [Setup – Microsoft Teams Guest Access Checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist) (Configuração – Lista de Verificação de Convidados do Microsoft Teams)
    - [How a guest joins a Team](https://docs.microsoft.com/microsoftteams/guest-joins) (Como é que um convidado adere ao Teams)

- **Acesso Telefónico e Reuniões do Teams**: precisa de ajuda para ligar ou configurar as Conferências de Áudio no Microsoft Teams? Este utilizador foi criado recentemente? Em caso afirmativo, terá de esperar entre 2 a 24 horas **para que as definições entrem em vigor**. 

    Para verificar se o utilizador está licenciado para Conferências de Áudio e tem um Número de Serviço Pago Predefinido:
    1.    Aceda a Utilizadores Ativos e, em seguida, selecione o utilizador em questão.
    2.    Dependendo da versão do centro de administração, selecione **Licenças e Aplicações** ou clique em **Editar** em **Licenças de produtos**.
    3.    Confirme que o utilizador tem licenças selecionadas para Conferências de Áudio, o Microsoft Teams e o Skype para Empresas Online (Plano 2).
    4.    Em Centros de Administração, clique em **Mostrar tudo** e, em seguida, em **Teams**.
    5.    No Centro de administração do Microsoft Teams, clique em **Portal legado**.
    6.    No Centro de administração do Skype para Empresas, clique em **conferências áudio** e, em seguida, em **utilizadores**.
    7.    Selecione o utilizador em questão e verifique se tem um Número de Serviço Pago Predefinido.
    
    Para mais informações, consulte [Planos de Chamadas para o Office 365](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) ou ligue para a equipa de faturação da Microsoft Commerce para obter ajuda com questões relacionadas com licenciamento.

    Recursos Adicionais:

    - [Reuniões e conferências no Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Conferências de Áudio no Office 365](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Licença de Preparação do Teams**: A experiência Preparação para o Microsoft Teams permite que os utilizadores na sua organização que têm o Azure Active Directory (AAD) e que não têm uma licença do Teams iniciem uma experiência Preparação para o Teams. Os administradores podem ativar ou desativar esta funcionalidade para os utilizadores na sua organização. A versão de avaliação do [Microsoft Commercial Cloud](https://docs.microsoft.com/microsoftteams/iw-trial-teams) anterior foi agora substituída pela experiência Preparação para o Teams.

    Recursos Adicionais:

    - [How users sign up for the Teams Exploratory experience](https://docs.microsoft.com/microsoftteams/teams-exploratory#how-users-sign-up-for-the-teams-exploratory-experience) (Como é que os utilizadores se inscrevem na experiência de Preparação para o Teams)
    - [Manage the Teams Exploratory experience](https://docs.microsoft.com/microsoftteams/teams-exploratory#manage-the-teams-exploratory-experience) (Gerir a experiência de Preparação para o Teams)

- **Canais Privados**: os canais privados no Microsoft Teams criam espaços focados para a colaboração entre equipas. Apenas os utilizadores da equipa que sejam proprietários ou membros do canal privado podem aceder ao canal. Qualquer pessoa, incluindo convidados, podem ser adicionados como membros de um canal privado, desde que já sejam membros da equipa.

    Recomendamos que utilize um canal privado se quiser limitar a colaboração às pessoas que têm de obter as informações ou se quiser facilitar a comunicação entre um grupo de pessoas atribuídas a um projeto específico, sem ter de criar uma equipa adicional para gerir.

    Recursos Adicionais:
    - [Private channel creation and membership](https://docs.microsoft.com/microsoftteams/private-channels#private-channel-creation-and-membership) (Criação e adesão a canais privados)
    - [Manage private channel membership and settings](https://docs.microsoft.com/microsoftteams/private-channels#manage-private-channel-membership-and-settings) (Gerir a associação e as definições de canais privados)

- **Políticas de Reuniões**: as políticas de reuniões são utilizadas para controlar as funcionalidades que estão disponíveis para os participantes das reuniões agendadas pelos utilizadores na sua organização. Depois de criar uma política e fazer alterações, poderá então atribuir utilizadores à política. 
    - **Alterar ou criar uma política de reunião**: para alterar ou criar uma política de reunião, aceda ao **Centro de administração do Microsoft Teams > Reuniões > Políticas de reuniões**. Selecione uma política a partir da lista ou selecione Adicionar. Se estiver a criar uma nova política, adicione um nome e uma descrição. O nome não pode conter carateres especiais nem ter mais de 64 carateres. Escolha as suas definições e, em seguida, clique em **Guardar**.

        Por exemplo, imagine que tem um grupo de utilizadores e quer limitar a quantidade de largura de banda que a sua reunião exige. Crie uma nova política chamada "Largura de banda limitada" e desative as seguintes definições:

        Em **Áudio e vídeo**:
        - Desative a opção Permitir gravação na nuvem.
        - Desative a opção Permitir vídeo IP.

        Em **Partilha de conteúdos**:
        - Desative o modo de partilha de ecrã.
        - Desative a opção Permitir quadro.
        - Desative a opção Permitir notas partilhadas.

        Em seguida, atribua a política aos utilizadores.

- **Atribuir uma política de reunião aos utilizadores**

    1. No menu de navegação esquerdo do centro de administração do Microsoft Teams, aceda a **Utilizadores** e, em seguida, clique no utilizador.
    2. Selecione o utilizador ao clicar à esquerda do nome do utilizador e, em seguida, clique em **Editar definições**.
    3. Em **Política de reunião**, selecione a política que pretende atribuir e, em seguida, clique em **Aplicar**.

    Para atribuir uma política a vários utilizadores de cada vez, consulte [Edit Teams user settings in bulk](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk) (Editar definições de utilizador do Teams em massa). Em alternativa, pode fazer o seguinte:

    1. No menu de navegação esquerdo do centro de administração do Microsoft Teams, aceda a **Reuniões > Políticas de reunião**.
    2. Selecione a política ao clicar à esquerda do nome da política.
    3. Selecione **Gerir utilizadores**.
    4. No painel **Gerir utilizadores**, procure o utilizador por nome a apresentar ou nome de utilizador, selecione o nome e, em seguida, clique em **Adicionar**. Repita este passo para cada utilizador que pretenda adicionar.
    5. Após terminar de adicionar utilizadores, clique em **Guardar**.

- **Resolução de Problemas com o teclado de marcação ausente**  

    - Certifique-se de que o utilizador tem uma [licença do Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses) atribuída.
    - Certifique-se de que o utilizador tem um [Plano de Chamadas](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) atribuído.
    - Ative a [Voz para Empresas](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail) para os utilizadores.

- **Resolva problemas com o início de sessão do Teams:** primeiro, certifique-se de que o [serviço do Microsoft Teams está a funcionar normalmente](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Em seguida, verifique se há códigos de erro comuns e reveja [Por que razão estou com problemas em iniciar sessão no Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)  Também poderá ser necessário rever [modelos de identidade e autenticação no Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).

**Para os clientes da Educação:**

Se os seus utilizadores estiverem a ver a mensagem "Está a perder!" Certifique-se de [Ativar o Microsoft Teams para a sua Escola](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Para os inquilinos da EDU, o Microsoft Teams não está ativado por padrão. Terá de ligá-lo primeiro.

Em seguida, consulte [Ensino e aprendizagem à distância no Office 365 Educação](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) para obter acesso às orientações mais recentes sobre a configuração da sua escola, planeamento de aulas, reuniões virtuais e partilha de conteúdos com os estudantes.

Por fim, consulte Vídeos e Apresentações de Formação para Administradores de TI do Microsoft Teams e muito mais aqui: https://docs.microsoft.com/MicrosoftTeams/itadmin-readiness#technical-training. 
