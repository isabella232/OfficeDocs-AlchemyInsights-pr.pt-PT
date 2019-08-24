---
title: Só de leitura para mensagens de manutenção ao tentar utilizar o SharePoint ou OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620734"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Só de leitura para mensagens de manutenção ao tentar utilizar o SharePoint ou OneDrive

Os utilizadores poderão receber uma mensagem **Só de leitura para manutenção** , quando tenta utilizar o SharePoint ou OneDrive para um dos seguintes cenários. 

-   Uma actividade de manutenção planeada ou activa.  Verifique os navegando para o [Centro de mensagens](https://portal.office.com/adminportal/home#/messagecenter).
-   Incidentes de serviço activo de elevada prioridade, que podem estar a ocorrer. Verificar a existência de quaisquer avisos de incidentes navegando para a [Saúde do serviço](https://portal.office.com/adminportal/home#/servicehealth).
-   Um pequena reparação automática cenário de recuperação que poderia ser acontecer devido a quaisquer acontecimentos imprevistos nos servidores que podem durar menos de 30 min., mais ou menos. 
    
    Não existem nenhum Centro de mensagens ou serviço de saúde regista estes pequenas recuperações mas deverá ser normal muito mais rapidamente.

Em ocasiões muito poucos Vamos observar que um dos três cenários listados acima ter sido a causa e serviço foi restaurado, mas ainda não foram eliminada da cache do browser os utilizadores.

Tente limpar a cache do browser antes de navegar para o site.

1. No browser do Microsoft Edge, seleccione **Definições**e, em seguida, seleccione a **privacidade e segurança**.
2. Em **Navegação clara**, seleccione **Escolher o que para a desmarcar**.
3. Seleccione **Cookies e dados dos Web sites guardada**e, seleccione **Limpar**.

>[!Note] 
> Estes passos podem ser diferentes quando utiliza outros browsers, tais como o Mozilla Firefox ou o Google Chrome.

>[!Note] 
> Outra opção seria abrir o SharePoint site ou OneDrive numa nova janela InPrivate.