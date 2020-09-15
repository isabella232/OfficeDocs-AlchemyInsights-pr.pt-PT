---
title: Erro das equipas 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700214"
---
# <a name="4c7-error-in-microsoft-teams"></a>Erro 4c7 nas Equipas da Microsoft

Este erro ocorre porque as equipas da Microsoft requerem autenticação de formulários. Quando implementa serviços da Federação de Diretórios Ativos (AD FS), a autenticação de formulários não está ativada para a intranet por predefinição. Se a autenticação integrada do Windows falhar, é-lhe pedido que faça sedutação utilizando a Autenticação de Formulários.

Para resolver este problema, ative a autenticação de formulários utilizando o encaixe da Consola de Gestão da Microsoft (MMC) AD FS no computador que tem a cópia local do Ative Directory. Para tal, siga estes passos: 

1. No painel de navegação, procure políticas **de autenticação.**
2. Em **Ações** no painel de detalhes, **selecione Editar Autenticação Primária Global.**
3. No separador **Intranet,** selecione **Autenticação de Formulários.**
4. Selecione **OK** (ou **Aplique).**