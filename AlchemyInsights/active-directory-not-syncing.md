---
title: Diretório ativo não sincronizando
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265267"
---
# <a name="active-directory-not-syncing"></a>Diretório ativo não sincronizando

Se estiver a receber erros de sincronização, tais como "nenhuma sincronização recente", ou notar o estado de sincronização do diretório no portal de administração do Office diz: "Última sincronizada há mais de 3 dias", pode ser que o AADConnect tenha configurações incorretas ou insuficientes permissões para realizar uma sincronização.  

Reinstalar o AADConnect utilizando definições expressas pode resolver o problema rapidamente:

1. [Descarregue a versão mais recente do AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Siga as instruções de instalação expressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Para obter mais informações sobre as contas de serviço AADConnect, consulte [o Azure AD Connect: Contas e permissões](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
