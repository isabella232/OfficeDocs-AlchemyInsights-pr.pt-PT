---
title: Troque o seu site de raiz clássico com um site moderno
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741555"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Troque o seu site de raiz clássico com um site moderno

Se o seu ambiente foi criado antes de abril de 2019, pode mudar o seu site de raiz para um site moderno usando o Microsoft PowerShell:

- Se tiver um site diferente que deseja utilizar como site raiz, pode substituir [(trocar) o site raiz](https://docs.microsoft.com/sharepoint/modern-root-site) por ele. 
    - Utilize o [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site por outro site enquanto arquiva o site original. Disponível tanto para o Site da Equipa (não ligado a um grupo) como para o Site de Comunicação. 

- Em breve serão introduzidas capacidades adicionais que lhe permitirão continuar a utilizar o conteúdo no site, mas converter o site existente num site de comunicação. 
>[!Important]
>Estas capacidades serão lançadas gradualmente. Continue a verificar se o Centro de Mensagens está a ver se há novidades. 

## <a name="known-issues-with-swapping-sites"></a>Questões conhecidas com sites de troca

- O local-alvo pode devolver um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo terá de ser reescrito para atualizar o índice de pesquisa. Não é necessário um passo manual - isto será feito automaticamente.
- Qualquer coisa dependente de links "estáticos" (como ficheiros Sync e OneNote) terá de ser corrigido manualmente.
- Se o site de origem fosse um site de notícias organizacional, atualize o URL.Obtenha uma lista de todos os sites de notícias organizacionais.
- Os sites do Project Server podem ter de ser validados para garantir que ainda estão corretamente associados.
