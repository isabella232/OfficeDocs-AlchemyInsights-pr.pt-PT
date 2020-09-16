---
title: Problema de resolução de problemas - Utilizador não encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725418"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problema de resolução de problemas - Utilizador não encontrado no diretório

Se os utilizadores estiverem a receber uma mensagem de erro "o utilizador não pode ser encontrado" no diretório, tente novamente onde o Tipo de Problemas está no diretório do Utilizador.

Os seguintes passos podem ser concluídos para resolver problemas.

- Certifique-se de que a conta que aceitou o convite por e-mail é a mesma que está a ser usada para iniciar scontabilidade mais tarde. Certifique-se de que o utilizador está a usar a mesma conta para aceitar o convite e assinar no site. 

Para obter mais informações, consulte [Como gerir os pseudónimos da sua conta Microsoft </a> para gerir o login da Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Navegue por cada site(s) em que o utilizador esteja a receber o erro. 

Adicione "/_layouts/15/people.aspx/membershipgroupid=0" (dentro das cotações duplas) até ao final do URL do site. 

Exemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecione o utilizador da lista.

- Clique **em Remover Permissões** do Utilizador da Fita. 
-  Adicione de volta o Utilizador e reenvimente o convite ao utilizador.

