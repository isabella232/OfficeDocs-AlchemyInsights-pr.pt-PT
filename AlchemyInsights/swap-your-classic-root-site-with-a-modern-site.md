---
title: Troque o seu site de raiz clássico por um site moderno
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691190"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Troque o seu site de raiz clássico por um site moderno

Se o seu ambiente foi configurado antes de abril de 2019, pode alterar o seu site de raiz para um site moderno utilizando o Microsoft PowerShell:

- Se tiver um site diferente que pretende utilizar como seu site de raiz, pode substituir [(trocar) o site raiz](https://docs.microsoft.com/sharepoint/modern-root-site) por ele. 
    - Utilize [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site por outro site enquanto arquiva o site original. Disponível para o Site de Equipa (não ligado a um grupo) e site de comunicação. 

- Em breve serão introduzidas capacidades adicionais que lhe permitirão continuar a utilizar o conteúdo do site, mas converter o site existente num site de comunicação. 
>[!Important]
>Estas capacidades serão lançadas gradualmente. Continue a verificar as atualizações do Centro de Mensagens. 

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com sites de troca

- O local alvo pode devolver um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo terá de ser recrawlado para atualizar o índice de pesquisa. Não é necessário um passo manual - isto será feito automaticamente.
- Qualquer coisa dependente de ligações "estáticas" (como ficheiros File Sync e OneNote) terá de ser corrigida manualmente.
- Se o site de origem foi um site de notícias organizacional, atualize o URL.Obtenha uma lista de todos os sites de notícias organizacionais.
- Os sites do Project Server podem ter de ser validados para garantir que ainda estão corretamente associados.
