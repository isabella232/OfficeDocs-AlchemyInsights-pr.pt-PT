---
title: Trocar o site raiz Clássica por um site moderno
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
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316151"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Trocar o site raiz Clássica por um site moderno

Se o seu ambiente foi configurado antes de abril de 2019, pode alterar o site raiz para um site moderno através do Microsoft PowerShell:

- Se tiver um site diferente que pretende utilizar como site raiz, pode substituir [(trocar)](https://docs.microsoft.com/sharepoint/modern-root-site) o site raiz pelo mesmo. 
    - Utilize [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site com outro site enquanto arquiva o site original. Disponível para o Site de Equipa (não ligado a um grupo) e o Site de Comunicação. 

- Serão introduzidas funcionalidades adicionais em breve, o que lhe irá permitir continuar a utilizar os conteúdos no site, mas converter o site existente num site de comunicação. 

**Importante:** estas funcionalidades serão adicionadas gradualmente. Continue a procurar atualizações no Centro de Mensagens. 

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com a troca de sites

- O site de destino poderá devolver um erro "não encontrado" (HTTP 404) durante um curto período de tempo.
- O conteúdo terá de ser recriado para atualizar o índice de pesquisa. Não é necessário seguir passos manuais. Este passo será realizado automaticamente.
- Tudo o que depender de ligações "estáticas" (como a Sincronização de Ficheiros e OneNote ficheiros) terá de ser corrigido manualmente.
- Se o site de origem era um site de notícias organizacional, atualize o URL. Obter uma lista de todos os sites de notícias organizacionais.
- Project Os sites de servidor poderão ter de ser validados para garantir que ainda estão associados corretamente.
