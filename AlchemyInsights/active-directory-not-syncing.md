---
title: Diretório Ativo não sincronização
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697640"
---
# <a name="active-directory-not-syncing"></a>Diretório Ativo não sincronização

Se estiver a receber erros de sincronização, como "nenhuma sincronização recente", ou notar o estado de sincronização do diretório no portal de administração do Office diz: "A última sincronização foi há mais de 3 dias", pode ser que a AADConnect tenha configurações incorretas ou permissões insuficientes para realizar uma sincronização.  

Reinstalar o AADConnect utilizando definições expressas pode resolver o problema rapidamente:

1. [Descarregue a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Siga as instruções de instalação expressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Para obter mais informações sobre as contas do serviço AADConnect, consulte [Azure AD Connect: Contas e permissões](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
