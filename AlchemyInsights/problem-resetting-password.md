---
title: Problema ao repor palavra-passe
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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039977"
---
# <a name="problems-resetting-password"></a>Problemas ao repor palavra-passe

Seguem-se alguns dos problemas que poderá ter ao repor a palavra-passe e as possíveis soluções:

**Estou a ter um problema com a reposição da palavra-passe não abrangida nas outras categorias**

- Certifique-se de que está autorizado a repor palavras-passe. Apenas os administradores globais, de palavra-passe e de utilizador podem repor palavras-passe de utilizador. Os administradores globais também podem repor as palavras-passe de outros administradores privilegiados.
- Certifique-se de que compreende os requisitos de licenciamento:
    - Tem de ter pelo menos uma licença atribuída na sua organização
        - Apenas utilizadores na nuvem – Office 365 SKU pago (O365) ou Azure AD Basic
        - Utilizadores da nuvem e/ou no local: Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
        - Para ler mais sobre os requisitos de licenciamento, consulte o artigo Requisitos de licenciamento para a reposição de [palavra-passe do Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Estou a ter problemas em testar a política de reposição de palavras-passe que definai**

- As políticas aplicadas recentemente podem demorar vários minutos a replicar em todos os centros de dados e pontos finais. A distância física do centro de dados também afetará a velocidade com que as alterações são aplicadas.
- Teste com um utilizador final, não com um administrador e piloto com um pequeno conjunto de utilizadores. As políticas configuradas no portal do Azure aplicam-se APENAS aos utilizadores finais e não aos administradores. A Microsoft impõe uma política de reposição de palavra-passe predefinida predefinida para qualquer função de administrador do Azure (Exemplo: Administrador Global, Administrador de Sistema de Ajuda, Administrador de Palavras-passe, etc.)
    - Saiba mais sobre [políticas para administradores.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Quero implementar a reposição de palavra-passe, mas não quero que os meus utilizadores registem informações de segurança adicionais**

Preenchidos dados para os seus utilizadores, para que não tenham de o fazer! - Enquanto administrador, pode definir as propriedades de telefone e e-mail para os seus utilizadores antes de reiniciar a palavra-passe na sua organização. Pode fazê-lo com uma API, PowerShell ou Azure AD Ligação. Mais informações aqui:
- [Implementar a reposição de palavra-passe sem que os utilizadores se registe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Que dados são utilizados pela reposição de palavra-passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**O botão de reposição da palavra-passe está a cinzento**

Não está autorizado a repor as palavras-passe deste utilizador. Apenas os administradores globais, de palavra-passe e de utilizador podem repor palavras-passe de utilizador. Os administradores globais também podem repor as palavras-passe de outros administradores privilegiados.

**Não vejo a chave de reposição de palavra-passe**

Não está autorizado a repor palavras-passe. Apenas os administradores globais, de palavra-passe e de utilizador podem repor palavras-passe de utilizador. Os administradores globais também podem repor as palavras-passe de outros administradores privilegiados.

**Não vejo o blade de integração no local na reposição de palavra-passe**

- A guia de integração no local só é mostrada em ambientes híbridos, o que significa que está a utilizar o writeback por palavra-passe para manipular palavras-passe de utilizadores no local.
- Não verá esta patada se:
    - Não está a utilizar o writeback da palavra-passe
    - Existe um problema com a sua instalação/conectividade de escrita de palavra-passe
    - Existe um problema com a sua instalação/conectividade do Azure AD Ligação
    - Para mais passos de remoção de problemas relacionados com a escrita de palavras-passe, consulte a secção Remoção de problemas de escrita [de palavra-passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Não sei como repor a palavra-passe de um utilizador**

1. Inscreva-se no portal do Azure como administrador adequado.
1. Vá para a ponta Utilizadores e grupos, selecione **Todos os Utilizadores.**
1. Selecione um utilizador a partir da lista.
1. Para o utilizador selecionado, **selecione Visão Geral e,** em seguida, na barra de comando, clique em **Repor palavra-passe**.
1. Siga as instruções no ecrã.
    - Apenas as reposição efetuadas através do portal do Azure suportam o writeback da palavra-passe.

**Repor a palavra-passe de um utilizador no local a partir do portal Administração do Office 365 ou da Office 365 para dispositivos móveis, mas o utilizador continua a não conseguir entrar**

A Escrita de Palavra-passe não é suportada neste portal. Repor a palavra-passe do utilizador novamente no portal do Azure – portal.azure.com

