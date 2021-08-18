---
title: Ativar a repetição de escrita de palavras-passe do Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118215"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Ativar a repetição de escrita de palavras-passe do Azure AD Connect

Para ativar a repetição de escrita de reposição personalizada de palavra-passe, ative primeiro a opção repetição de escrita no Azure AD Connect. A partir do seu servidor do Azure AD Connect, efetue os seguintes passos:

1. Inicie sessão no seu servidor do Azure AD Connect e inicie o assistente de configuração do **Azure AD Connect**.
2. Na página de **Boas-vindas**, clique em **Configurar**.
3. Na página **Tarefas adicionais**, selecione **Personalizar opções de sincronização** e, em seguida, clique em **Seguinte**.
4. Na página **Ligar ao Azure AD**, introduza uma credencial de administrador global para o seu inquilino do Azure e, em seguida, clique em **Seguinte**.
5. Nas páginas de filtragem de **Ligar diretórios** e de **Domínio/UO**, clique em **Seguinte**.
6. Na página **Funcionalidades opcionais**, selecione a caixa junto a **Repetição de escrita da palavra-passe** e clique em **Seguinte**.
7. Na página **Preparado para configurar**, clique em **Configurar** e aguarde até que o processo seja concluído.
8. Assim que a configuração estiver terminada, clique em **Sair**.

Com a repetição de escrita de palavra-passe ativada no Azure AD Connect, configure o Azure AD SSPR para a repetição de escrita.  Para ativar a repetição de escrita de uma palavra-passe no SSPR, efetue os seguintes passos:

1. Inicie sessão no portal do Azure através de uma conta de administrador global.
2. Procure e selecione o **Azure Active Directory**, clique em **Reposição de palavra-passe** e, em seguida, clique em **Integração no local**.
3. Defina a opção **Repetir a escrita de palavras-passe no diretório no local?** como **Sim**.
4. Defina a opção **Permitir que os utilizadores desbloqueiem as contas sem repor a palavra-passe?** como **Sim**.
5. Quando estiver pronto, clique em **Guardar**.

Para obter mais informações, consulte [Ativar a repetição de escrita de reposição personalizada de palavra-passe do Azure Active Directory num ambiente no local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Se um administrador redefinir a palavra-passe de um utilizador no portal do Azure, se esse utilizador estiver federado ou tiver sincronização de hash de palavra-passe, a escrita da palavra-passe será repetida no local. Esta funcionalidade necessita da licença do Azure Premium (P1 ou P2) e não é atualmente suportada no portal de Administração do Office.
