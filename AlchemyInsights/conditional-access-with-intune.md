---
title: Acesso condicional com intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505005"
---
# <a name="conditional-access-with-intune"></a>Acesso condicional com intune

O **uso do Acesso Condicional** com o Intune requer 3 etapas: 
  
- Crie uma Política de **Acesso Condicional** que defina quais recursos estão sendo protegidos e quais condições precisam ser atendidas para acessar esses recursos. Por exemplo, um dispositivo deve estar em conformidade antes de acessar o e-mail corporativo. 
    
- Crie uma política de **conformidade** para definir configurações que devem ser atendidas antes que o dispositivo seja considerado compatível. Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado compatível. 
    
- Garantir que as **Políticas** de Conformidade e as **Políticas** de Acesso Condicional sejam direcionadas aos grupos de usuários desejados. Isso pode exigir a criação de grupos específicos de usuários no Diretório Ativo Do Azure. 
    
Leia mais:
  
- [Melhores práticas de acesso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Começar com acesso condicional](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

