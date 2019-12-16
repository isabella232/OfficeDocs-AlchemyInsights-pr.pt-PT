---
title: Troque o seu site de raiz clássico com um site moderno
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042938"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Troque o seu site de raiz clássico com um site moderno

Se seu ambiente foi configurado antes de abril de 2019, você pode mudar seu site raiz para um site moderno usando o Microsoft PowerShell:

- Se você tem um site diferente que você deseja usar como seu site raiz, você pode substituir [(trocar) o site raiz](https://docs.microsoft.com/sharepoint/modern-root-site) com ele. 
    - Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para trocar a localização de um site com outro site enquanto arquiva o site original. Disponível para o Site da Equipe (não conectado a um grupo) e ao Site de Comunicação. 

- Recursos adicionais serão introduzidos em breve que permitirão que você continue usando o conteúdo no site, mas converta o site existente em um site de comunicação. 
>[!Important]
>Estas capacidades serão implementadas gradualmente. Continue a verificar o Centro de Mensagens do Escritório 365 para atualizações. 

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos com a troca de sites

- O site-alvo pode retornar um erro "não encontrado" (HTTP 404) por um curto período de tempo.
- O conteúdo precisará ser rerabiscado para atualizar o índice de pesquisa. Não há nenhuma etapa manual exigida - esta será feita automaticamente.
- Qualquer coisa dependente de links "estáticos" (como arquivos File Sync e OneNote) precisará ser corrigido manualmente.
- Se o site de origem era um site de notícias organizacional, atualize a URL.Receba uma lista de todos os sites de notícias organizacionais.
- Os sites do Servidor do Projeto podem precisar ser validados para garantir que eles ainda estejam associados corretamente.





