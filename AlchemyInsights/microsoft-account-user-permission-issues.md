---
title: Remoção de problemas – o utilizador não foi encontrado no diretório
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098181"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Remoção de problemas – o utilizador não foi encontrado no diretório

Se os utilizadores estiverem a receber uma mensagem de erro "Não é possível encontrar o utilizador" no diretório, tente novamente onde o Tipo de Problema é Utilizador e não no diretório.

Os passos seguintes podem ser concluídos para detetar o problema.

- Certifique-se de que a conta que aceitou o convite por e-mail é a mesma conta que está a ser utilizada para entrar mais tarde. Certifique-se de que o utilizador está a utilizar a mesma conta para aceitar o convite e para entrar no site. 

Para mais informações, consulte Como gerir aliases da sua conta Microsoft para gerir o início [ </a> Microsoft 365 início de sessão.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Navegue até cada site(s) em que o utilizador está a receber o erro. 

Adicione "/_layouts/15/people.aspx/membershipgroupid=0" (entre aspas) ao final do URL do site. 

Exemplo: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecione o utilizador a partir da lista.

- Clique **em Remover Permissões de** Utilizador do Fita. 
-  Adicione novamente o Utilizador e Reenviar o convite ao utilizador.

