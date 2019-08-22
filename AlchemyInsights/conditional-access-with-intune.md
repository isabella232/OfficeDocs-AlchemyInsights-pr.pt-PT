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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505005"
---
# <a name="conditional-access-with-intune"></a>Acesso condicional com Intune

A utilização de **Acesso condicional** com Intune requer 3 passos: 
  
- Crie uma **Política de acesso condicional** que define quais os recursos que estão a ser protegidos e o que as condições que devem ser cumpridos para aceder aos recursos. Por exemplo, um dispositivo tem de ser compatível com antes de aceder a correio electrónico da empresa. 
    
- Crie uma **Política de conformidade** para definir as definições que devem ser satisfeitas antes do dispositivo é considerado compatível. Por exemplo, um dispositivo tem de ter um pin de pelo menos 6 dígitos antes de ser considerado compatível. 
    
- Assegurar a **Conformidade de políticas** e **Políticas de acesso condicional** são orientados para os grupos de utilizadores pretendidos. Isto pode requerer a criação de grupos específicos de utilizadores do Active Directory Azure. 
    
Ler mais:
  
- [Condicionais procedimentos recomendados de acesso](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Introdução ao acesso condicional](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

