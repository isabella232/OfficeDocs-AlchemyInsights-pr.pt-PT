---
title: Read-Only para Manutenção ao tentar utilizar o SharePoint ou o OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910557"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only para Manutenção ao tentar utilizar o SharePoint ou o OneDrive

Os utilizadores poderão receber uma mensagem **Só** de Leitura para Manutenção ao tentarem utilizar o SharePoint ou OneDrive um dos seguintes cenários. 

-   Uma atividade de manutenção planeada ou ativa.  Procure-os ao navegar para o Centro [de Mensagens.](https://portal.office.com/adminportal/home#/messagecenter)
-   Um incidente de serviço ativo de alta prioridade que poderá estar a ocorrer. Verifique se há avisos/incidentes ao navegar para Estado [de Saúde do Serviço.](https://portal.office.com/adminportal/home#/servicehealth)
-   Um cenário de recuperação secundária que poderia ocorrer devido a eventos inesperados nos servidores que poderia durar menos de 30 min. 
    
    Não existem mensagens no Centro de Mensagens ou Estado de Funcionamento do Serviço para estas recuperações secundárias, mas deverá voltar ao normal brevemente.

Em poucas ocasiões, observamos que um dos três cenários indicados acima foi a causa e o serviço foi restaurado, mas a cache do browser dos utilizadores não foi limpa.

Tente limpar a cache do browser antes de navegar para o site.

1. No seu browser Microsoft Edge, selecione Definições **e,** em seguida, **selecione Privacidade e Segurança.**
2. Em **Limpar navegação, selecione** **Escolher o que limpar**.
3. **Selecione Cookies e dados do site guardados e** selecione **Limpar**.

>[!Note] 
> Estes passos poderão ser diferentes ao utilizar outros browsers como o Mozilla Firefox ou o Google Chrome.

>[!Note] 
> Outra opção seria abrir o seu site do SharePoint ou OneDrive numa nova janela InPrivate.