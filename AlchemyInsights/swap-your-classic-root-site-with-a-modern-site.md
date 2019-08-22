---
title: Trocar o site de raiz Classic com um site Moderno
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
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501090"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Trocar o site de raiz Classic com um site Moderno

Se o ambiente tiver sido configurado antes de Abril de 2019, pode alterar o site de raiz para um site moderno utilizando o Microsoft PowerShell:

- Se tiver um site diferente que pretende utilizar como o site de raiz, pode substituir o site de raiz (comutação) com o mesmo. 
    - Utilize [Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para mudar a localização de um site com outro site ao arquivar o site original. Disponível para o Site de equipa (não ligado a um grupo) e o Site de comunicação. 

- Capacidades adicionais serão introduzidas mais rapidamente que lhe permitirá manter, utilizando o conteúdo no site, mas converter o site existente para um site de comunicação. 
>[!Important]
>Estas capacidades serão efectuadas gradualmente. Continue a verificar o Centro de mensagens do Office 365 para obter actualizações. 

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos relacionados com sites de comutação

- O site de destino poderá devolver um erro (HTTP 404) "não foi encontrado" durante um curto período de tempo.
- Conteúdo terá de ser pesquisado novamente para actualizar o índice de procura. Não existe nenhum manual passo necessário - Isto será feito automaticamente.
- Tudo depende de ligações "estáticas" (por exemplo, ficheiros de sincronização de ficheiros e o OneNote), terá de ser corrigidas manualmente.
- Se o site de origem era um site de notícias sobre a organização, actualize o URL.Obter uma lista de todos os sites de notícias sobre a organização.
- Sites do Project Server poderão ter de ser validadas para garantir que são ainda associadas correctamente.





