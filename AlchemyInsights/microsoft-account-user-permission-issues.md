---
title: Resolver a questão - o utilizador não encontrado no directório
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249924"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Resolver a questão - o utilizador não encontrado no directório

Se os utilizadores estão a receber erros mensagem "utilizador não é possível localizar" no directório. Tente novamente quando o tipo de problema utilizador não estiver no directório.

Os seguintes passos podem ser concluídos para resolver o problema.

- Certifique-se a conta que aceite que o convite de correio electrónico é a mesma conta que está a ser utilizada para iniciar sessão mais tarde. Certifique-se do que utilizador está a utilizar a mesma conta para a aceitar o convite e iniciar sessão no site. 

Para obter mais informações, consulte [como gerir aliases para sua conta Microsoft</a> para gerir o início de sessão do Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Navegue para cada site em que o utilizador está a receber o erro. 

Adicionar "/ _layouts/15/people.aspx/membershipgroupid=0" (entre as aspas) para o fim do URL do site. 

Exemplo: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Seleccione o utilizador a partir da lista.

- Clique em **remover permissões de utilizador** do Friso. 
-  Voltar a adicionar o utilizador e reenvie o convite para o utilizador.

