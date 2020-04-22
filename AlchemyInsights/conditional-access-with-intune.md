---
title: Acesso Condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706032"
---
# <a name="conditional-access-with-intune"></a>Acesso Condicional com Intune

Utilizar **o Acesso Condicional** com Intune requer 3 passos: 
  
- Criar uma Política de **Acesso Condicional** que defina quais os recursos que estão a ser protegidos e quais as condições a cumprir para aceder a esses recursos. Por exemplo, um dispositivo deve ser compatível antes de aceder a e-mails corporativos. 
    
- Crie uma Política de **Conformidade** para definir as definições que devem ser satisfeitas antes de o dispositivo ser considerado conforme. Por exemplo, um dispositivo deve ter um pino de pelo menos 6 dígitos antes de ser considerado compatível. 
    
- Garantir que tanto as Políticas de **Conformidade** como as Políticas de **Acesso Condicional** são direcionadas aos grupos de utilizadores pretendidos. Isto pode exigir a criação de grupos específicos de utilizadores no Diretório Ativo Do Azure. 
    
Leia mais:
  
- [Acesso Condicional às melhores práticas](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Começar com acesso condicional](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

