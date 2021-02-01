---
title: Problemas com credenciais
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063684"
---
# <a name="issues-with-credentials"></a>Problemas com credenciais

[A plataforma de identidade da Microsoft e o fluxo de credenciais de cliente OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrevem como programar diretamente contra o fluxo de concessão de credenciais de cliente OAuth 2.0.

**Como posso gerir as credenciais de senha ou certificado de uma aplicação?**

No CLI Azure, pode utilizar [a credencial de aplicação ad az](https://docs.microsoft.com/cli/azure/ad/app/credential) para eliminar, listar ou redefinir as credenciais de senha ou certificado de uma aplicação.

**Como é que os meus utilizadores repõei as suas palavras-passe?**

Os utilizadores precisam de [se registar para redefinição da palavra-passe de autosserviço](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) antes de poderem redefinir as suas palavras-passe. Uma vez registado um utilizador, podem seguir as instruções deste artigo para redefinir a sua palavra-passe: [Redefinir o seu trabalho ou a palavra-passe da escola](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Como é que os meus utilizadores mudam as suas palavras-passe?**

Os utilizadores podem seguir os passos deste artigo para alterar as suas palavras-passe: [Como alterar a sua palavra-passe](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Também podem [Gerir palavras-passe de aplicações para verificação em duas etapas.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**O meu utilizador está a ter um erro ao alterar ou redefinir a sua palavra-passe**

Este link fornecerá informações sobre problemas comuns que podem surgir quando um utilizador está a tentar redefinir a sua palavra-passe: [Problemas comuns e suas soluções](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Estou a ter problemas em redefinir a senha de um utilizador.**

- Certifique-se de que está autorizado a redefinir palavras-passe. *Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.* Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.

- Certifique-se de compreender os requisitos de licenciamento:

  - Deve ter pelo menos uma licença atribuída na sua organização:
    - **Utilizadores da Cloud -** Qualquer Office 365 (O365) pagou SKU, ou Azure AD Basic
    - **Utilizadores em nuvem e/ou no local** - Azure AD Premium P1 ou P2, Mobilidade Empresarial + Segurança (EMS) ou Empresa Produtiva Segura (SPE)
    - Para saber mais sobre os requisitos de licenciamento, consulte [os requisitos de licenciamento para a Azure AD autosserviço de autosserviço reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Para redefinir a palavra-passe de um utilizador, encontre o utilizador no Azure AD. Em seguida, na lâmina de visão geral para esse utilizador, clique no botão "redefinir a palavra-passe".

**O botão de reset da palavra-passe está acinzentado**

Não está autorizado a redefinir as palavras-passe **deste** utilizador. *Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.* Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.

**Não vejo a lâmina de reset da palavra-passe.**

Não está autorizado a redefinir palavras-passe. *Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador.* Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.

**Não vejo a lâmina de integração no local no reset da palavra-passe**

- A lâmina de integração no local só aparece em ambientes híbridos - o que significa que está a usar a gravação de passwords para manipular as palavras-passe do utilizador no local.

- Não se vê esta lâmina se:

  - Não está a usar o writeback da palavra-passe
  - Há um problema com a sua instalação/conectividade de writeback de palavra-passe
  - Há um problema com a sua instalação/conectividade do Azure AD Connect
  - Para obter mais etapas de resolução de problemas para problemas com a writeback de password, consulte [o writeback da palavra-passe de Resolução de Problemas](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Não sei como redefinir a senha de um utilizador.**

1. Inscreva-se no portal Azure como um administrador apropriado.
2. Aceda à lâmina **dos Utilizadores e grupos,** selecione **Todos os Utilizadores**.
3. Selecione um utilizador da lista.
4. Para o utilizador selecionado, selecione **'Visão geral'** e, em seguida, na barra de comando, **selecione Redefinir a palavra-passe**.
5. Selecione o botão **de palavra-passe Reset** e siga as instruções no ecrã.
    - Apenas resets realizados através da gravação de senha de suporte do **portal Azure.**

**Repus a palavra-passe de um utilizador no local a partir do portal de administração do Office 365 ou da aplicação móvel do Office 365, mas o utilizador ainda não consegue iniciar sposição.**

A writeback de palavra-passe não é suportada neste portal. Repor novamente a palavra-passe do utilizador no portal Azure.
