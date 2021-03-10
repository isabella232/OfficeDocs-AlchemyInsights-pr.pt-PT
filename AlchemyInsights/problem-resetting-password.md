---
title: Palavra-passe de reposição de problemas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696274"
---
# <a name="problems-resetting-password"></a>Problemas na redefinição da palavra-passe

Seguem-se alguns dos problemas que poderá enfrentar ao redefinir a palavra-passe e as possíveis soluções:

**Estou tendo um problema com a palavra-passe não abrangida nas outras categorias**

- Certifique-se de que está autorizado a redefinir palavras-passe. Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador. Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.
- Certifique-se de que compreende os requisitos de licenciamento:
    - Deve ter pelo menos uma licença atribuída na sua organização
        - Utilizadores da Cloud - Qualquer Office 365 (O365) pagou SKU, ou Azure AD Basic
        - Utilizadores em nuvem e/ou no local - Azure AD Premium P1 ou P2, Mobilidade Empresarial + Segurança (EMS) ou Empresa Produtiva Segura (SPE)
        - Para ler mais sobre os requisitos de licenciamento consulte o artigo [Requisitos de licenciamento para a palavra-passe de autosserviço AZure AD repostos](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Estou com problemas em testar a política de reset da palavra-passe que estabeleci**

- As políticas recentemente aplicadas podem demorar vários minutos a replicar-se em todos os centros de dados e pontos finais. A distância física do centro de dados também afetará a rapidez com que as mudanças são aplicadas.
- Teste com um utilizador final, não um administrador, e piloto com um pequeno conjunto de utilizadores. As políticas configuradas no portal Azure aplicam-se apenas aos utilizadores finais e não aos administradores. A Microsoft aplica uma forte política de reset de senha de dois prazos para qualquer função de administrador do Azure (Exemplo: Administrador Global, Administrador de Ajuda, Administrador de Password, etc.)
    - Saiba mais sobre [políticas para administradores.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Quero implementar o reset da palavra-passe, mas não quero que os meus utilizadores registem informações adicionais de segurança.**

Preencha os dados para os seus utilizadores para que não tenham de o fazer! - Como administrador, pode definir propriedades de telefone e e-mail para os seus utilizadores antes de lançar a palavra-passe para a sua organização. Pode fazê-lo utilizando uma Ligação API, PowerShell ou AZure AD. Mais informações aqui:
- [Implementar a palavra-passe reiniciada sem exigir que os utilizadores se registem](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Que dados são usados por reset de senha](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**O botão de reset da palavra-passe está acinzentado**

Não está autorizado a redefinir as palavras-passe deste utilizador. Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador. Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.

**Não vejo a lâmina de reset da palavra-passe.**

Não está autorizado a redefinir palavras-passe. Apenas administradores globais, de palavra-passe e de utilizadores podem redefinir as palavras-passe do utilizador. Os administradores globais também podem redefinir as palavras-passe de outros administradores privilegiados.

**Não vejo a lâmina de integração no local no reset da palavra-passe**

- A lâmina de integração no local só aparece em ambientes híbridos - o que significa que está a usar a gravação de passwords para manipular as palavras-passe do utilizador no local.
- Não se vê esta lâmina se:
    - Não está a usar o writeback da palavra-passe
    - Há um problema com a sua instalação/conectividade de writeback de palavra-passe
    - Há um problema com a sua instalação/conectividade do Azure AD Connect
    - Para obter mais etapas de resolução de problemas para problemas com a gravação de password, consulte a secção [Descreva a palavra-passe de resolução de problemas](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Não sei como redefinir a senha de um utilizador.**

1. Inscreva-se no portal Azure como um administrador apropriado.
1. Aceda à lâmina dos Utilizadores e grupos, selecione **Todos os Utilizadores**.
1. Selecione um utilizador da lista.
1. Para o utilizador selecionado, selecione **'Visão geral'** e, em seguida, na barra de comando, clique em **Redefinir a palavra-passe**.
1. Siga as instruções no ecrã.
    - Apenas resets realizados através da gravação de senha de suporte do portal Azure.

**Repus a palavra-passe de um utilizador no local a partir do portal de administração do Office 365 ou da aplicação móvel do Office 365, mas o utilizador ainda não consegue iniciar sposição.**

A writeback de palavra-passe não é suportada neste portal. Repor novamente a palavra-passe do utilizador no portal Azure - portal.azure.com

