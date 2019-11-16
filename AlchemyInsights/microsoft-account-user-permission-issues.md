---
title: Problema de solucionamento de problemas - Usuário não encontrado no diretório
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768812"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problema de solucionamento de problemas - Usuário não encontrado no diretório

Se os usuários estiverem recebendo mensagem de erro "o usuário não pode ser encontrado" no diretório, tente novamente onde o tipo de edição não está no diretório.

As seguintes etapas podem ser concluídas para solucionar o problema.

- Certifique-se de que a conta que aceitou o convite por e-mail é a mesma conta que está sendo usada para entrar mais tarde. Certifique-se de que o usuário está usando a mesma conta para aceitar o convite e entrar no site. 

Para mais informações, veja [como gerenciar pseudônimos para sua conta</a> da Microsoft para gerenciar o login do Office 365.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Navegue para cada site (s) em que o usuário está recebendo o erro. 

Adicione "/_layouts/15/people.aspx/membershipgroupid=0" (dentro das cotações duplas) até o final da URL do site. 

Exemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecione o usuário da lista.

- Clique **em remover as permissões** do usuário da fita. 
-  Adicione de volta o usuário e reenviar o convite para o usuário.

