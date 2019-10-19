---
title: Troque seu site raiz clássico com um site moderno
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749271"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Troque seu site raiz clássico com um site moderno

Se seu ambiente foi configurado antes de abril de 2019, você pode alterar seu site raiz para um site moderno usando o Microsoft PowerShell:

- Se você tiver um site diferente que você deseja usar como seu site raiz, você pode substituir [(swap) o site raiz](https://docs.microsoft.com/sharepoint/modern-root-site) com ele. 
    - Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar o local de um site com outro site ao arquivar o site original. Disponível para o site de equipe (não conectado a um grupo) e o site de comunicação. 

- Recursos adicionais serão introduzidos em breve que permitirão que você continue usando o conteúdo no site, mas converta o site existente em um site de comunicação. 
>[!Important]
>Esses recursos serão lançados gradualmente. Continue a verificar o Office 365 Message Center para obter atualizações. 

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com a troca de sites

- O site de destino pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo precisará ser rastreado para atualizar o índice de pesquisa. Não há nenhuma etapa manual exigida-isto será feito automaticamente.
- Qualquer coisa dependente de links "estáticos" (como arquivos de sincronização de arquivo e OneNote) precisará ser corrigido manualmente.
- Se o site de origem for um site de notícias organizacionais, atualize a URL.Obtenha uma lista de todos os sites de notícias organizacionais.
- Sites do Project Server talvez precise ser validado para garantir que eles ainda estão associados corretamente.





