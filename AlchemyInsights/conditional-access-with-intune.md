---
title: Acesso condicional com Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393552"
---
# <a name="conditional-access-with-intune"></a>Acesso condicional com Intune

A utilização de **Acesso condicional** com Intune requer 3 passos: 
  
- Crie uma **Política de acesso condicional** que define quais os recursos que estão a ser protegidos e o que as condições que devem ser cumpridos para aceder aos recursos. Por exemplo, um dispositivo tem de ser compatível com antes de aceder a correio electrónico da empresa. 
    
- Crie uma **Política de conformidade** para definir as definições que devem ser satisfeitas antes do dispositivo é considerado compatível. Por exemplo, um dispositivo tem de ter um pin de pelo menos 6 dígitos antes de ser considerado compatível. 
    
- Assegurar a **Conformidade de políticas** e **Políticas de acesso condicional** são orientados para os grupos de utilizadores pretendidos. Isto pode requerer a criação de grupos específicos de utilizadores do Active Directory Azure. 
    
Ler mais:
  
- [Condicionais procedimentos recomendados de acesso](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introdução ao acesso condicional](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

