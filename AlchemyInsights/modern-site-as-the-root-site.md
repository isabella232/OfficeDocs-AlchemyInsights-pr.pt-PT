---
title: Site moderna, tal como o site de raiz
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543864"
---
# <a name="modern-site-as-root-site"></a>Moderno site como site de raiz

Vamos ter começado a fase de instalação uma nova funcionalidade que permite-lhe trocar o site de raiz clássico de site com um site Moderno. Utilize [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) para mudar a localização de um site com outro site ao arquivar o site original. Disponível para o Site de equipa (não ligado a um grupo) e o Site de comunicação. 

>[!Important]
> Não elimine o site de raiz clássico para criar um Site de comunicação modernos. Não é suportada pela Microsoft. Eliminar o site de raiz fará com que todos os sites SharePoint da sua organização inacessíveis a todos os utilizadores, até que restaure o site ou crie um novo site com o mesmo URL. A Microsoft vai estar a comunicar esta funcionalidade através do Centro de mensagem. Deve esperar a funcionalidade para ser activado no seu tenant dentro em breve.

## <a name="known-issues-with-swapping-sites"></a>Problemas conhecidos relacionados com sites de comutação
- O site de destino poderá devolver um erro (HTTP 404) "não foi encontrado" durante um curto período de tempo.
- Conteúdo terá de ser pesquisado novamente para actualizar o índice de procura. Não existe nenhum passo manual necessário aqui, isto será feito automaticamente.
- Tudo depende de ligações "estáticas" (por exemplo, ficheiros de sincronização de ficheiros e o OneNote), terá de ser corrigidas manualmente.
- Sites do Project Server poderão ter de ser validadas para garantir que são ainda associadas correctamente. 
