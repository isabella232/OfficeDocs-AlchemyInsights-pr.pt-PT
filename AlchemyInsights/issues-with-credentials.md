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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986830"
---
# <a name="issues-with-credentials"></a>Problemas com credenciais

plataforma de identidades da Microsoft e o fluxo de credenciais de cliente [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) descrevem como programar diretamente com as credenciais de cliente OAuth 2.0 concedem fluxo.

**Como posso gerir a palavra-passe de uma aplicação ou as credenciais de certificado?**

No Azure CLI, pode utilizar as credenciais da [aplicação Az AD](https://docs.microsoft.com/cli/azure/ad/app/credential) para eliminar, listar ou repor as credenciais de certificado ou palavra-passe de uma aplicação.

**Como é que os meus utilizadores repostam as respetivos palavras-passe?**

Os utilizadores têm de [efetuar uma reposição de palavra-passe](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) pessoal antes de poderem repor as palavras-passe. Assim que um utilizador se registar, pode seguir as instruções neste artigo para repor a palavra-passe: Repor a sua palavra-passe [escolar ou pessoal.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Como é que os meus utilizadores alteram as respetivos palavras-passe?**

Os utilizadores podem seguir os passos neste artigo para alterarem as respetivos palavras-passe: [Como alterar a sua palavra-passe](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Também podem Gerir [palavras-passe de aplicação para verificação de dois passos.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**O meu utilizador está a obter um erro ao alterar ou repor a palavra-passe**

Esta ligação irá fornecer informações sobre problemas comuns que podem surgir quando um utilizador está a tentar repor a palavra-passe: [Problemas comuns e respetivas soluções](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Estou a ter um problema ao repor a palavra-passe de um utilizador**

- Certifique-se de que está autorizado a repor palavras-passe. *Apenas os administradores globais, de palavra-passe e de utilizador podem repor palavras-passe de utilizador.* Os administradores globais também podem repor as palavras-passe de outros administradores privilegiados.

- Certifique-se de que compreende os requisitos de licenciamento:

  - Tem de ter, pelo menos, uma licença atribuída na sua organização:
    - **Apenas utilizadores na nuvem** – Office 365 SKU pago (O365) ou Azure AD Basic
    - **Utilizadores da nuvem e/ou** no local : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
    - Para saber mais sobre os requisitos de licenciamento, consulte Requisitos de licenciamento para a reposição de palavra-passe de responsabilidade do [Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Para repor a palavra-passe de um utilizador, procure-o no Azure AD. Em seguida, na guia de visualização geral para esse utilizador, clique no botão "repor palavra-passe".

**O botão de reposição da palavra-passe está a cinzento**

Não está autorizado a repor **as palavras-passe** deste utilizador. *Apenas os administradores globais, de palavra-passe e de utilizador podem repor palavras-passe de utilizador.* Os administradores globais também podem repor as palavras-passe de outros administradores privilegiados.

**Não vejo a chave de reposição de palavra-passe**

Não está autorizado a repor palavras-passe. *Apenas os administradores globais, de palavra-passe e de utilizador podem repor palavras-passe de utilizador.* Os administradores globais também podem repor as palavras-passe de outros administradores privilegiados.

**Não vejo o blade de integração no local na reposição de palavra-passe**

- A guia de integração no local só é mostrada em ambientes híbridos, o que significa que está a utilizar o writeback por palavra-passe para manipular palavras-passe de utilizadores no local.

- Não verá esta patada se:

  - Não está a utilizar o writeback da palavra-passe
  - Existe um problema com a sua instalação/conectividade de escrita de palavra-passe
  - Existe um problema com a sua instalação/conectividade do Azure AD Ligação
  - Para mais passos de remoção de problemas relacionados com a escrita de palavras-passe, consulte o artigo [Remoção de problemas de escrita de palavras-passe](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Não sei como repor a palavra-passe de um utilizador**

1. Inscreva-se no portal do Azure como administrador adequado.
2. Vá para a ponta **Utilizadores e grupos,** selecione **Todos os Utilizadores.**
3. Selecione um utilizador a partir da lista.
4. Para o utilizador selecionado, **selecione Visão Geral e,** em seguida, na barra de comando, selecione **Repor palavra-passe**.
5. **Selecione o botão Repor** palavra-passe e siga as instruções no ecrã.
    - Apenas as reposição efetuadas através do **portal do Azure suportam** o writeback da palavra-passe.

**Repor a palavra-passe de um utilizador no local a partir do portal Administração do Office 365 ou da Office 365 para dispositivos móveis, mas o utilizador continua a não conseguir entrar**

A Escrita de Palavra-passe não é suportada neste portal. Repor a palavra-passe do utilizador novamente no portal do Azure.
