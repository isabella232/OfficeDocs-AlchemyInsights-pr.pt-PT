---
title: OneDrive para business Web OneDrive redireciona para Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800000"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Redirecionado para Delve depois de clicar no OneDrive

Consulte o nosso Guia de [Resolução de Problemas](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)detalhado .

Para resolver este problema, o administrador deve conceder aos utilizadores o direito de criar o seu site My Sites. Isto porque a página OneDrive for Business é criada nos Meus Sites.

Para conceder este direito, siga estes passos:

1. No centro de administração SharePoint, clique nos **perfis do utilizador**.

2. Na secção **Pessoas,** clique em **Gerir permissões do utilizador**.

3. Adicione utilizadores que necessitem de permissões para criar o seu site My Sites. Por predefinição, esta definição é definida para **Todos, exceto utilizadores externos.**

4. Depois de ter adicionado o utilizador, utilizadores ou grupo, certifique-se de que o utilizador, utilizadores ou grupo adicionados é selecionado, percorra a secção **de permissões** e, em seguida, selecione a caixa de verificação ao lado **do Site Criar Pessoal (necessário para armazenamento pessoal, newsfeed e conteúdo seguido)**.

5. Clique **em OK** e, em seguida, tenha o utilizador a navegar na página OneDrive para criar o site.
