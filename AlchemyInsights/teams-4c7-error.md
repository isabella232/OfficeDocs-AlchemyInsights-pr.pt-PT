---
title: Equipes 4c7 erro
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796296"
---
# <a name="4c7-error-in-microsoft-teams"></a>Erro de 4c7 em equipes de Microsoft

Esse erro ocorre porque o Microsoft Teams requer autenticação de formulários. Quando você implanta serviços da Federação de Direção Ativa (AD FS), a autenticação de formulários não é ativada para a intranet por padrão. Se a autenticação integrada do Windows falhar, você será solicitado a entrar usando a autenticação de formulários.

Para resolver esse problema, habilite a autenticação de formulários usando o snap-in do AD FS Microsoft Management Console (MMC) no computador que tem a cópia local do Diretório Ativo. To do this, follow these steps: 

1. No painel de navegação, procure as Políticas de **Autenticação.**
2. **ações** no painel de detalhes, selecione **Eitie Autenticação Primária Global**.
3. Na guia **Intranet,** selecione **Autenticação de Formulários**.
4. Selecione **OK** (ou **Inscreva-se).**