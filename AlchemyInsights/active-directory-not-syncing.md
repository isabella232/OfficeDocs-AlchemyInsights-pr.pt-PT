---
title: O Active Directory não está a ser syncing
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889229"
---
# <a name="active-directory-not-syncing"></a>O Active Directory não está a ser syncing

Se estiver a receber erros de sincronização, como "sem sincronização recente", ou repare que o estado de sincronização de diretórios no portal de administração do Office indica "Última sincronização há mais de 3 dias", pode ser que o AADConnect tem definições incorretas ou permissões insuficientes para efetuar uma sincronização.  

Reinstalar o AADConnect através de definições rápidas pode resolver o problema rapidamente:

1. [Transfira a versão mais recente do AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Siga as instruções de instalação rápida.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

O Azure AD Connect tem de ser instalado no Windows Server 2012 ou posterior. Este servidor deve ser unido ao domínio e pode ser um controlador de domínio ou um servidor membro. Para uma lista completa do Azure AD Ligação requisitos e pré-requisitos, reveja os Pré-requisitos do [Azure AD Ligação.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Para obter mais informações sobre contas de serviço do AADConnect, consulte [O Azure AD Ligação: Contas e permissões.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
