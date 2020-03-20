---
title: 'Teams: problemas comuns de clientes das subscrições para educação'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 81b80d76530327767bc58adf2e06e5b7ae265f18
ms.sourcegitcommit: 7d787b8c5af223e2711b4c2a2ca55ce2bdc25aea
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/19/2020
ms.locfileid: "42856808"
---
# <a name="teams-common-issues-for-education-customers"></a>Teams: problemas comuns de clientes das subscrições para educação

**Para os clientes das subscrições para educação:**

Se precisar de ajuda a implementar o Teams para suportar a aprendizagem remota, visite o [Centro FastTrack](https://www.microsoft.com/fasttrack) para submeter um pedido. Veja os seguintes problemas comuns de clientes das subscrições do Teams para educação:

- Está a ver a mensagem "**Está a perder!**"? Certifique-se de [Ativar o Microsoft Teams para a sua Escola](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Para os inquilinos da EDU, o Microsoft Teams não está ativado por padrão. Terá de ligá-lo primeiro.

- **É novo utilizador do Teams?** Consulte [Ensino e aprendizagem à distância no Office 365 Educação](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) para obter acesso às orientações mais recentes sobre a configuração da sua escola, planeamento de aulas, reuniões virtuais e partilha de conteúdos com os estudantes.

- Uma vez ativado, os utilizadores podem executar o Teams ao instalar o [cliente para ambiente de trabalho](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) e o [cliente para dispositivos móveis](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) ou a partir do browser em https://teams.microsoft.com.

- **Ativar o acesso de convidados ao Teams:** consulte a [lista de verificação de acesso de convidados do Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) e certifique-se de que todos os passos foram concluídos.
    - [Understanding Guest Access in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access) (Compreender o Acesso de Convidados no Microsoft Teams)
    - [Setup – Microsoft Teams Guest Access Checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist) (Configuração – Lista de Verificação de Convidados do Microsoft Teams)
    - [How a guest joins a Team](https://docs.microsoft.com/microsoftteams/guest-joins) (Como é que um convidado adere ao Teams)

- **Acesso Telefónico e Reuniões do Teams**: precisa de ajuda para ligar ou configurar as Conferências de Áudio no Microsoft Teams? Este utilizador foi criado recentemente? Em caso afirmativo, terá de esperar 2 a 24 horas para que as definições entrem em vigor. Para verificar se o utilizador está licenciado para Conferências de Áudio e tem um Número de Serviço Pago Predefinido:
    1. Aceda a Utilizadores Ativos e selecione o utilizador em questão.
    2. Dependendo da versão do centro de administração, selecione **Licenças e Aplicações** ou clique em **Editar** em **Licenças de produtos**.
    3. Confirme que o utilizador tem licenças selecionadas para Conferências de Áudio, o Microsoft Teams e o Skype para Empresas Online (Plano 2).
    4. Em Centros de Administração, clique em **Mostrar tudo** e, em seguida, em **Teams**.
    5. No Centro de administração do Microsoft Teams, clique em **Portal legado**.
    6. No Centro de administração do Skype para Empresas, clique em **conferências áudio** e, em seguida, em **utilizadores**.
    7. Selecione o utilizador em questão e verifique se tem um Número de Serviço Pago Predefinido.

    Para mais informações, consulte [Planos de Chamadas para o Office 365](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) ou ligue para a equipa de faturação da Microsoft Commerce para obter ajuda com questões relacionadas com licenciamento.

    Recursos Adicionais

    - [Reuniões e conferências no Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Conferências de Áudio no Office 365](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Políticas de Reuniões**: as políticas de reuniões são utilizadas para controlar as funcionalidades disponíveis para os participantes das reuniões agendadas pelos utilizadores na sua organização. Depois de criar uma política e fazer alterações, poderá atribuir utilizadores à política.

    - **Alterar ou criar uma política de reunião**: para alterar ou criar uma política de reunião, aceda ao **Centro de administração do Microsoft Teams > Reuniões > Políticas de reuniões**. Selecione uma política a partir da lista ou clique em **Adicionar**. Se estiver a criar uma nova política, adicione um nome e uma descrição. O nome não pode conter carateres especiais nem ter mais de 64 carateres. Selecione as suas definições e, em seguida, clique em **Guardar**. 
    
        Por exemplo, imagine que tem um grupo de utilizadores e quer limitar a largura de banda que a sua reunião exige. Crie uma nova política chamada "Largura de banda limitada" e desative as seguintes definições:

        Em **Áudio e vídeo**:
        - Desative a opção **Permitir gravação na nuvem**.
        - Desative a opção **Permitir vídeo IP**.

        Em **Partilha de conteúdos**:

        - Desative o modo de partilha de ecrã.
        - Desative a opção **Permitir quadro**.
        - Desative a opção **Permitir notas partilhadas**.

        Em seguida, **atribua a política aos utilizadores**:

    1. No menu de navegação esquerdo do centro de administração do Microsoft Teams, aceda a **Utilizadores** e, em seguida, clique no utilizador.
    2. Selecione o utilizador ao clicar à esquerda do nome do utilizador e, em seguida, clique em **Editar definições**.
    3. Em **Política de reunião**, selecione a política que pretende atribuir e, em seguida, clique em **Aplicar**.

    Para atribuir uma política a vários utilizadores de cada vez, consulte [Edit Teams user settings in bulk](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk) (Editar definições de utilizadores do Teams em massa).

    Em alternativa, pode fazer o seguinte:
    1. No menu de navegação esquerdo do centro de administração do Microsoft Teams, aceda a **Reuniões > Políticas de reunião**.
    2. Selecione a política ao clicar à esquerda do nome da política.
    3. Clique em **Gerir utilizadores**.
    4. No painel **Gerir utilizadores**, procure o utilizador por nome a apresentar ou nome de utilizador, selecione o nome e, em seguida, clique em **Adicionar**. Repita este passo para cada utilizador que pretenda adicionar.
    5. Após terminar de adicionar utilizadores, clique em **Guardar**.

- **Resolução de Problemas com o teclado de marcação em falta**:
    - Certifique-se de que o utilizador tem uma [licença do Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses) atribuída.
    - Certifique-se de que o utilizador tem um [Plano de Chamadas](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page) atribuído.
    - Ative a [Voz para Empresas](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail) para os utilizadores.

- **Resolver problemas com o início de sessão do Teams:** primeiro, certifique-se de que o [serviço do Microsoft Teams está a funcionar normalmente](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Em seguida, verifique se há códigos de erro comuns e reveja [Por que razão estou com problemas em iniciar sessão no Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Também poderá ser necessário rever [Identity models and authentication in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication) (Modelos de identidade e autenticação no Microsoft Teams).
