---
title: Problemas problemas - Utilizador não encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702749"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problemas problemas - Utilizador não encontrado no diretório

Se os utilizadores estiverem a receber uma mensagem de erro "o utilizador não pode ser encontrado" no diretório, tente novamente onde o Tipo de Problema está o Utilizador não no diretório.

Os seguintes passos podem ser concluídos para resolver o problema.

- Certifique-se de que a conta que aceitou o convite por e-mail é a mesma conta que está a ser usada para assinar mais tarde. Certifique-se de que o utilizador está a usar a mesma conta para aceitar o convite e assinar no site. 

Para mais informações, consulte como gerir pseudónimos para a [sua conta</a> Microsoft gerir o login Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Navegue por cada site em que o utilizador esteja a receber o erro. 

Adicione "/_layouts/15/people.aspx/membershipgroupid=0" (dentro das cotações duplas) ao final do URL do site. 

Exemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecione o utilizador da lista.

- Clique em **remover permissões** de utilizador da fita. 
-  Adicione de volta o Utilizador e reenvie o convite para o utilizador.

